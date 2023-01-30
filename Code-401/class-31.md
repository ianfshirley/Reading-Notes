## Django REST Framework & Docker

### Beginner's Guide to Docker

- Docker is a way to isolate and run entire applications. With this it doesn't matter if you're using Mac, Windows or Linux, the development environment is isolated: programming language, software packages, databases and more. This removes the need for virtual environments, and Docker can be shared among team members so everyone is working with the same setup. The downside is that it's very complex under the hood.

**Linux Containers**
- Docker is really just Linux containers, which are a type of virtualization.
- In recent years, containerization has become increasingly popular. For most applications, a virtual machine provides far more resources than are needed and a container is more than sufficient.
- Virtual machines are like homes: stand-alone building with their own infrastructure (plumbing, heating, bed/bath/kitchen etc.). Docker containers are like apartments: they share most, if not all, of the common infrastructure like plumbing & heating, but come in various sizes that match the exact needs of the owner.

**Containers vs. Virtual Environments**
- Virtual environments are used to isolate Python software packages locally. This allows you to install different frameworks/packages & use different versions of the same language/framework/program in multiple environments on the same computer. They can only isolate Python packages however. 
- Virtual environments can't run production databases or other services, so they're far more limited compared to Docker.

**Images and Containers**
- An image is a snapshot in time of what a project contains.
- A container is running an instance of the image.
- We will typically create custom images and we do so using a `Dockerfile`. We will also use `docker-compose.yml` files to run the containers.
- A baking analogy:
  - a `Dockerfile` is the recipe for a cake
  - an *image* is a snapshot of the recipe at a given time
  - a `docker-compose.yml` says how to make the cake
  - the container is the actual, baked cake

**Images**
- To create an 'image' for the Python programming language:
  - create a local directory on computer, cd into that directory, and then make another directory inside of that one for python:
    ```
    $ cd ~/Desktop
    $ mkdir code
    $ cd code
    $ mkdir python3.7
    $ cd python3.7
    ```
  - Now we need to define the image with a `Dockerfile`. This is similar to a pipenv or a requirements.txt file. It is a list of all the requirements needed to build our image. It is simpler to have them all in one place rather than install each manually line-by-line.
  - (on a mac) create a new `Dockerfile` on the command line with the 'touch' command:
    `$ touch Dockerfile`
  - open text editor, and add the following line to the `Dockerfile`:
    `FROM python:3.7-alpine`
    - Dockerfiles are read top-to-bottom. The first instruction **must** be the `FROM` command which lets us import a base image to use for our image. This base image could be a Docker image or one we create from scratch. In this case we'll use the official Docker image for Python 3.7, specifically the alpine version which only includes the bare minimum needed to run Python. (78md compared to 923mb for the full version)

**Image Builds**
- In the terminal:
  `$ docker image build .` (don't forget the space & period)
  *(this did not give me the expected return from the tutorial)*

**Image Layers**
- Every image is made of up one or more image layers. The base layer is often a flavor of Linux, like `alpine`. The image for `python:3.7-alpine` *should* have the id `b2c276538711`, but that image depended on five other images which were visible while building it:
  ```
  c9b1b535fdd9: Pull complete
  2cc5ad85d9ab: Pull complete
  53a2fca3c2ea: Pull complete
  30fce49de8b1: Pull complete
  49bcb9571cc7: Pull complete
  ```
  - This is called image layering, and it exists for two main reasons:
    - Each image layer is immutable, like a git commit. This helps ensure consistency when two developers build the same image
    - Performance: Docker catches the steps in a `Dockerfile` to speed up subsequent builds. When a change is made to a step, all steps following it will be executed from scratch. For this reason, order matters in a `Dockerfile`. Typically you want to put code that won't change often at the top and code that *will* change at the end.

**Containers**
- Just as `Dockerfile` is a list of image instructions, a `docker-compose.yml` file is a list of container instructions.
*(got all kinds of warnings when installing pipenv so I'll have to try that again I guess)*

- to create a Django project from scratch:
  - go up one directory to the docker-image-tutorial folder'
  ```
  $ mkdir djangoapp && cd djangoapp
  $ pipenv install django==3.0
  $ pipenv shell
  ```
  - this creates a `pipfile` and a `pipfile.lock`. 


### Django for APIs - Library Website

- APIs must always be added to a project *after* Django has been installed and configured.



### Sources

[Beginner's Guide to Docker](https://wsvincent.com/beginners-guide-to-docker/)<br>
[Django for APIs - Library Website](https://djangoforapis.com/library-website-and-api/)<br>
[Official Django REST Framework Tutorial - A Beginners Guide](https://learndjango.com/tutorials/official-django-rest-framework-tutorial-beginners)<br>
[REST, Hypermedia & HATEOAS](https://www.django-rest-framework.org/topics/rest-hypermedia-hateoas/)<br>
[Django APIs - Serializers](https://www.django-rest-framework.org/api-guide/serializers/)<br>