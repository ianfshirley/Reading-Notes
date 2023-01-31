## DRF Permissions & PostgreSQL

### DRF Permissions

- Permissions (and authentication and throttling) determine whether a request should be granted or denied access.
- Permissions checks are always run before any other code is allowed to proceed. They will typically use the authentication info in the `request.user` and `request.auth` properties to determine if the request should be permitted
- grant or deny access for differe classes of users to different parts of the API
- `IsAuthenticated` - allow authenticated users, deny acess to unauthenticated users
- `IsAuthenticatedOrReadOnly` - allow full access to authenticated users, but allow read-only access to unauthenticated users

- **How permissions are determined**
  - Permissions in the REST framework are always defined as a list of permission classes
  - Each permission in the list is checked before running the main body of the view. If any check fails, the main body will not run, and one of these exceptions will be raised: `exceptions.PermissionDenied` or `exceptions.NotAuthenticated`.

- **Object level permissions**
  - object level permissions are used to determine if a user should be allowed to act on a particular object, which will typically be a model instance.
  - they are run by REST framework's generic views when `.get_object()` is called.
  - if writing your own views and you want to enforce object level permissions, you ust explicitly call the `.check_object_permissions(request, obj)` method on the view at the point at which you've retrieved the object

- **Setting the permission policy**
  - the default permission policy may be set globally, using `DEFAULT_PERMISSION_CLASSES` setting.
  ```
  REST_FRAMEWORK = {
    'DEFAULT_PERMISSION_CLASSES': [
      'rest_framework.permissions.IsAuthenticated',
    ]
  }
  ```

- **Access Restriction Methods**
  - `queryset`/`get_queryset()` - limits the general visibility of existing objects from the database. The queryset limits which objects will be listed and which objects can be modified or deleted. 
  - `permission_classes`/`get_permissions()` - general permissions checks based on current action, request and targeted object. object level permissions can only be applied to retrieve, modify and deletion actions.
  - `serializer_class`/`get_serializer()` - instance level restrictions that apply to all objects on input or output

  | method: | `queryset` | `permissions_classes` | `serializer_class` |
  | ------- | ---------- | --------------------- | ------------------ |
  | Action: list | global | global | object-level* |
  | Action: create | no | global | object-level |
  | Action: retrieve | global | object-level | object-level |
  | Action: update | global | object-level | object-level |
  | Action: partial_update | global | object-level | object-level |
  | Action: destroy | global | object-level | no |
  | Can reference action in decision | no** | yes | no** |
  | Can reference request in decision | no** | yes | yes |
  
  \* A Serializer class should not raise PermissionDenied in a list action, or the entire list would not be returned.
  \* The `get_*()` methods have access to the current view and can return different Serializer or QuerySet instances based on the request or action.




### Sources

[DRF Permissions](https://www.django-rest-framework.org/api-guide/permissions/)<br>
[Classy Django REST Framework](https://www.cdrf.co/)<br>
[DRF Generic Views](https://www.django-rest-framework.org/api-guide/generic-views/)
