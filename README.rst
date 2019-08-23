django-simple-polls
========================

Polls is a simple and reusable Django app to conduct Web-based polls.
For each question, visitors can choose between a fixed number of answers.


Key features
-----------

* basic poll handling (poll, choices, votes)
* easy to extend


Installation
-----------

If you want to install the latest stable release from PyPi:
    ```
    $ pip install django-simple-polls
    ```
Or install the latest development version from GitHub:
    ```
    pip3 install -e git://github.com/MisterLenivec/django-simple-polls#egg=django-simple-polls
    ```

Quick start
-----------

1. Add "polls" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'polls',
    ]

2. Include the polls URLconf in your project urls.py like this::

    path('polls/', include('polls.urls')),

3. Run `python manage.py migrate` to create the polls models.

4. Start the development server and visit http://127.0.0.1:8000/admin/
   to create a poll (you'll need the Admin app enabled).

5. Visit http://127.0.0.1:8000/polls/ to participate in the poll.
