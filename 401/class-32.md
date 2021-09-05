# Permissions & Postgresql

## DRF Permissions

Together with **authentication** and **throttling**, permissions determine whether a request should be granted or denied access.

Permission checks are always run at the very start of the view before any other code is allowed to proceed. Permission checks will typically use the authentication information in the request.user and request.auth properties to determine if the incoming request should be permitted.

### How permissions are determined

Permissions in REST framework are always defined as a list of permission classes.

When the permissions checks fail either a **"403 Forbidden"** or a \*\*"401 Unauthorized"v response will be returned, according to the following rules:

- The request was successfully authenticated, but permission was denied. — An HTTP **403 Forbidden** response will be returned.

- The request was not successfully authenticated, and the highest priority authentication class does not use WWW-Authenticate headers. — An HTTP **403 Forbidden** response will be returned.

- The request was not successfully authenticated, and the highest priority authentication class does use WWW-Authenticate headers. — An HTTP **401 Unauthorized response**, with an appropriate WWW-Authenticate header will be returned.

### Object level permissions

REST framework permissions support **object-level permissioning**. Object-level permissions are used to **determine if a user should be allowed to act on a particular object**.

### API Reference

- **_AllowAny_** - allow unrestricted access, regardless of if the request was authenticated or unauthenticated

- **_IsAuthenticated_** - deny permission to any unauthenticated user, and allow permission otherwise

- **_IsAdminUser_** - deny permission to any user, unless user.is_staff is True in which case permission will be allowed

- **_IsAuthenticatedOrReadOnly_** - allow authenticated users to perform any request. Requests for unauthorized users will only be permitted if the request method is one of the "safe" methods; GET, HEAD or OPTIONS

- **_DjangoModelPermissions_** - granted if the user is authenticated and has the relevant model permissions assigned

- **_DjangoModelPermissionsOrAnonReadOnly_** - allows unauthenticated users to have read-only access to the API

- **_DjangoObjectPermissions_** - allows per-object permissions on models

## DRF Generic Views

Django’s generic views... were developed as a shortcut for common usage patterns... They take certain common idioms and patterns found in view development and abstract them so that you can quickly write common views of data without having to repeat yourself
