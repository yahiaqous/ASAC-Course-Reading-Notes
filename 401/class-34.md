# API Deployment

## Configuring Django Settings

### Managing Django Settings: Issues

- **Different environments** - each one can have its own specific settings

- **Sensitive data** - like SECRET_KEY in each Django project, passwords, and tokens for third-party APIs

- **Sharing settings between team members** - approach to eliminate human error when working with the settings

- **Django settings are a Python code** - gives a lot of flexibility, but can also be a problem

### Setting Configuration: Different Approaches

- **settings_local.py** - extend all environment-specific settings in the settings_local.py file, which is ignored by VCS

- **Separate settings file for each environment** - keep all configurations in VCS and share default settings between developers.

- **Environment variables** - solve the issue with sensitive data

- **12 Factors** -

  - Codebase
  - Dependencies
  - Config
  - Backing services
  - Build, release, run
  - Processes
  - Port binding
  - Concurrency
  - Disposability
  - Dev/prod parity
  - Logs
  - Admin processes

- **django-environ** - it’s a merge of:

  - envparse
  - honcho
  - dj-database-url
  - dj-search-url
  - dj-config-url
  - django-cache-url

- **Setting Structure** - splitting settings by the source: Django, third- party apps (Celery, DRF, etc.)

&nbsp;

### Django Settings: Best practices

- Keep settings in environment variables.

- Write default values for production configuration (excluding secret keys and tokens).

- Don’t hardcode sensitive settings, and don’t put them in VCS.

- Split settings into groups: Django, third-party, project.

- Follow naming conventions for custom (project) settings.

&nbsp;

## How Does SSH Work

SSH, or Secure Shell, is a remote administration protocol that allows users to control and modify their remote servers over the Internet. The service was created as a secure replacement for the unencrypted Telnet and uses cryptographic techniques to ensure that all communication to and from the remote server happens in an encrypted manner

Encryption technologies used by SSH:

- **Symmetrical encryption** - the secret key is used for both encryption and decryption of a message by both the client and the host

- **Asymmetrical encryption** - uses two separate keys for encryption and decryption

- **Hashing** - generate a unique value of a fixed length for each input that shows no clear trend which can be exploited

&nbsp;

## Infrastructure as a service (IaaS)

Infrastructure as a service (IaaS) are online services that provide high-level APIs used to dereference various low-level details of underlying network infrastructure like physical computing resources, location, data partitioning, scaling, security, backup, etc

&nbsp;

## Platform as a service (PaaS)

Platform as a service (PaaS) or application platform as a service (aPaaS) or platform-based service is a category of cloud computing services that allows customers to provision, instantiate, run, and manage a modular bundle comprising a computing platform and one or more applications, without the complexity of building and maintaining the infrastructure typically associated with developing and launching the application(s); and to allow developers to create, develop, and package such software bundles

&nbsp;

## Cross-origin resource sharing

Cross-origin resource sharing (CORS) is a mechanism that allows restricted resources on a web page to be requested from another domain outside the domain from which the first resource was served.
