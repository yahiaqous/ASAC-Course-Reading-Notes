# Django Custom User

The official Django documentation highly recommends using a custom user model instead. This provides far more flexibility down the line so, as a general rule, always use a custom user model for all new Django projects.

&nbsp;

## AbstractUser vs AbstractBaseUser

There are two modern ways to create a custom user model in Django:

- **AbstractUser**
- **AbstractBaseUser**

In both cases, we can subclass them to extend existing functionality however AbstractBaseUser requires much, much more work.

Creating an initial custom user model requires four steps:

- Update project settings
- Create a new CustomUser model
- Create new UserCreation and UserChangeForm
- Update the admin

        from django.contrib.auth.models import AbstractUser
        class User(AbstractUser):
            pass
