URLS
***********
- in debug mode to use static files, add static url to urlpatterns:
    .. code-block :: python
        from django.conf import settings
        form django.conf.urls.static import static

        if settings.DEBUG:
            urlpatterns += static(settings.STATIC_URL, document_root=settings.STATIC_ROOT)
        
        
        
