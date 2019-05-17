Beginner Pillow Tutorial 
=====

Flask is a lightweight `WSGI`_ web application framework. It is designed
to make getting started quick and easy, with the ability to scale up to
complex applications. It began as a simple wrapper around `Werkzeug`_
and `Jinja`_ and has become one of the most popular Python web
application frameworks.

Flask offers suggestions, but doesn't enforce any dependencies or
project layout. It is up to the developer to choose the tools and
libraries they want to use. There are many extensions provided by the
community that make adding new functionality easy.


Installing
----------

Install and update using `pip`_:

.. code-block:: text

    pip install -U pillow


Some Concepts with Examples
----------------

Loading a picture
.. code-block:: python

    from PIL import Image

    img = Image.open('.pics/handsome.jpg')

    img.show()
    .. image:: ./pics/handsome.jpg
       :width: 40pt

Pasting a logo on an image
.. code-block:: python

    from PIL import Image

    img = Image.open('.pics/handsome.jpg')
    img_copy = img.copy()
    location = (525, 1109)
    img_copy.paste(logo, position,logo)
    img_copy.show()
    .. image:: ./logoed/handsome.jpg
       :width: 40pt

Donate
------

.. _please donate today: https://venmo.com/LOVER


Works Cited
-----
* Pillow Documentation: https://pillow.readthedocs.io/en/stable/
* auth0 image processing with Pillow: https://auth0.com/blog/image-processing-in-python-with-pillow/
* Python for beginners Tutorial on Pillow: https://www.pythonforbeginners.com/gui/how-to-use-pillow
* Intro to Pillow: https://www.blog.pythonlibrary.org/2016/10/07/an-intro-to-the-python-imaging-library-pillow/

.. me: https://lokinario.github.io
