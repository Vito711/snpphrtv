========
SnapPass-Heroku
========

|build|

.. |build| image:: https://travis-ci.org/samteezy/snappass-heroku.svg
    :target: http://travis-ci.org/samteezy/snappass-heroku
    :alt: Build status

It's like SnapChat... for Passwords... (for Heroku).

If you want to read more about how it works, go check out [the original](https://github.com/pinterest/snappass/) from the great folks at Pinterest: they detail security as well as available configuration options. We are simply modifying it for Heroku, plus maybe a couple more additional features ;)

I'm not a programmer by trade, so I know there's some unnecessary code cleanup to do that I likely haven't covered. Also, rather than running on Flask, this uses Gunicorn. I haven't determined if I can remove the Flask dependency yet. (That's how little I know...)

See it in action and use it yourself at https://snappass.heroku.com.

[test](http://google.com)

Requirements
------------

* Redis: just add the Heroku Redis add-on to your app prior to deploying this code.
* Python: you don't need to specify a version, this is compatible with 2.7+ and 3.4+. As of this writing Heroku defaults to 3.6.2.

Installation
------------


1. Create app.
2. Add Heroku Redis add-on. Make sure it populates a config variable for REDIS_URL.
3. Deploy code from this fork.

That's it!
