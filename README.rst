========
SnapPass-Heroku
========

|build|

.. |build| image:: https://travis-ci.org/samteezy/snappass-heroku.svg
    :target: http://travis-ci.org/samteezy/snappass-heroku
    :alt: Build status

It's like SnapChat... for Passwords... (for Heroku).

If you want to read more about how it works, go check out `the original`__ from the great folks at Pinterest: they detail security as well as available configuration options. We are simply modifying it for Heroku, plus maybe a couple more additional features ;)

I'm not a programmer by trade, so I know there's some Docker-related items and more in here that can be removed - just haven't gotten to testing that yet. Also, rather than running on Flask, this uses Gunicorn. I haven't determined if I can remove the Flask dependency yet.

.. __: https://github.com/pinterest/snappass

Requirements
------------

* Redis: just add the Heroku Redis add-on to your app prior to deploying this code.
* Python 2.6, 2.7 or 3.3+.

Installation
------------

1. Create app.
2. Add Heroku Redis add-on. Make sure it populates a config variable for REDIS_URL.
3. Deploy code from this branch.

That's it!
