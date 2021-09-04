# Django REST Framework & Docker

**Docker**: a way to isolate and run entire applications.

If you rent space on a cloud provider like **AWS** they are typically not providing you with a dedicated piece of hardware. Instead, you are probably sharing a physical server with hundreds or even thousands of other clients.

&nbsp;

## Images and containers

Images and containers are the two fundamental concepts to grasp when you start with Docker. An image is a snapshot in time of what a project contains. A container is a running instance of the image.

Every image is made up of one or more image layers. The base layer is often a flavor of Linux, like alpine.

&nbsp;

## Library Website and API

**Django REST Framework works** alongside the **Django web framework** to create web APIs. We cannot build a web API with only Django Rest Framework; it always must be added to a project after Django itself has been installed and configured.

### How to install Django REST Framework

    pipenv install djangorestframework~=3.11.0

### Serializers

A serializer translates data into a format that is easy to consume over the internet, typically **JSON**, and is displayed at an **API endpoint**.
