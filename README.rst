===== Auth =====
Auth is a reusable authorization app for Django
Detailed documentation is in the "docs" directory.
Quick start -----------
1. Add "reusable_auth" to your INSTALLED_APPS setting like this::
    INSTALLED_APPS = (         ...         'reusable_auth',     )


2. Add these two settings to your projects settings.py:
    AUTH_USER_MODEL = 'reuseable_auth.User'
    AUTHENTICATION_BACKENDS = ('django.contrib.auth.backends.ModelBackend', 'reusable_auth.backends.EmailAuth',)


3. Run `python manage.py makemigrations and migrate`.
