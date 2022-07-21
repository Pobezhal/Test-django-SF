# Test-django-SF

Не могу понять почему не работает голая ссылка http://127.0.0.1:8000/. Пишет page not found.
Захожу только если после слеша указать конкретную страницу например /admin, или /about/ или /third_page

/third_page доступна только авторизованному пользователю. Если заходить на нее без логина то появляется сообщение  - 
Page not found (404)
Request Method:	GET
Request URL:	http://127.0.0.1:8000/accounts/login/?next=/third_page/
Using the URLconf defined in project33.urls, Django tried these URL patterns, in this order:

admin/
pages/
The current path, accounts/login/, didn’t match any of these.

You’re seeing this error because you have DEBUG = True in your Django settings file. Change that to False, and Django will display a standard 404 page.

Так и должно быть? Это нормальная реакция страницы на неавторизованный вход?
