SETTINGS
**************
- for Token Authentication:
    - INSTALLED_APPS += 'rest_framework.authtoken' # application
    - REST_FRAMEWORK['DEFAULT_AUTHENTICATION_CLASSES'] = "rest_framework.authentication.TokenAuthentication"
    

- serve decimal and date with no coerce to string:
    - REST_FRAMEWORK['COERCE_DECIMAL_TO_STRING'] = False
    - REST_FRAMEWORK['COERCE_DATE_TO_STRING'] = False

