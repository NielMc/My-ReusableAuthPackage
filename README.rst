===== Auth =====
Auth is a reusable authorization app for Django
Detailed documentation is in the "docs" directory.
To install:
pip install git+https://github.com/NielMc/My-ReusableAuthPackage
To update:
pip install git+https://github.com/NielMc/My-ReusableAuthPackage --upgrade
Add the following line to your requirements.txt file:
git+https://github.com/NielMc/My-ReusableAuthPackage


Quick start -----------
1. Add "reusable_auth" to your INSTALLED_APPS setting like this::
    INSTALLED_APPS = (         ...         'reusable_auth',  'django_forms_bootstrap',   )


2. Add these two settings to your projects settings.py:
    AUTH_USER_MODEL = 'reusable_auth.User'
    AUTHENTICATION_BACKENDS = ('django.contrib.auth.backends.ModelBackend', 'reusable_auth.backends.EmailAuth',)


3. Run `python manage.py makemigrations and migrate`.

4. Add url(r'', include('reusable_auth.urls')), to your urls.py file.


