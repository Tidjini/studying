SETTINGS
**************
- **DRY PRINCIPAL** use multi settings files in your project:
    - base, development, production, staging ...
- Use **Environment Variables** to store secret information like SECRET_KEY, or to **switch** between settings in different envirnments.
- Define your STATIC_ROOT folder.
- In production when you set **DEBUG = False** you should always define your ALLOWED_HOSTS in your settings.
