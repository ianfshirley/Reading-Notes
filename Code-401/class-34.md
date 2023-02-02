## API Deployment

### Django Setting Best Practices

- **Potential Issues when Managing Django Settings:**
  - different environments (local, development, staging, production, etc.)
  - sensitive data
  - sharing settings between team members
  - django settings are a python code

- **Different Approaches:**
  - settings_local.py
    - Pros: 
      - secrets not in VCS/Github
    - Cons: 
      - the file is no in VCS/Github, so you can lose some environment settings
      - it can have some non-obvious logic since it's a python file
  - separate settings file for each environment
    - Pros:
      - all environments are in VCS
    - Cons:
      - need to find a way to handle secret passwords and tokens
      - inheritance of settings can be hard to trace and maintain
  - environment variables
    - Pros:
      - django config separated from code
      - environment parity - same code for all environments
      - no inheritance in settings, cleaner and more consistent code
      - there is a theoretical grounding for this approach
    - Cons:
      - need to handle sharing the config between developers

- **12 Factors**
  - This is a collection of recommendations on how to build distributed web-apps that will be easy to deploy and scale in the cloud. (created by Heroku)
  1. Codebase
  2. Dependencies
  3. Config
  4. Backing services
  5. Build, release, run
  6. Processes
  7. Port binding
  8. Concurrency
  9. Disposability
  10. Dev/prod parity
  11. Logs
  12. Admin Processes

- **django-environ**
  - this is a merge of envparse, honcho, dj-database-url, dj-search-url, dj-config-url, and django-cache-url
  - better than using os.environ
  - gives a well functioning API for reading values from env variables or text files
  - instead of splitting settings by environments, you can split them by the source: django, 3rd party apps, and custom settings

- **Django Settings: Best Practices**
  - Keep settings in environment variables.
  - Write default values for production configuration (excluding secret keys and tokens).
  - Don’t hardcode sensitive settings, and don’t put them in VCS.
  - Split settings into groups: Django, third-party, project.
  - Follow naming conventions for custom (project) settings.

  
### Sources

[Configuring Django Setting Best Practices](https://djangostars.com/blog/configuring-django-settings-best-practices/)<br>
[WhiteNoise](http://whitenoise.evans.io/en/stable/)<br>
[Cross-origin resource sharing](https://en.m.wikipedia.org/wiki/Cross-origin_resource_sharing)<br>