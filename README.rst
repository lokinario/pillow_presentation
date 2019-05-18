Beginner Pillow Tutorial 
=====

Introduction
*************
A lot of applications use digital images, and with this there is usually a need to process the images used. If you are building your application with Python and need to add image processing features to it, there are various libraries you could use. Some popular ones are OpenCV, scikit-image, Python Imaging Library and Pillow.

This tutorial will focus on Pillow, a library that is powerful, provides a wide array of image processing features, and is simple to use.

Goals
*******
Through this tutorial I hope to take my audience on a journey of self discovery of the wonderous world of Pillow -kidding- I hope to instill the knowledge of Pillow's use cases for image manipulation. 


Installing
----------

Install and update using `pip`_:

.. code-block:: text

    pip install -U pillow

Concepts
----------------
- Bands 
- Modes
- Size
- Data 
- Cordinate System 
- Filters

Examples
----------------

Loading a picture

.. code-block:: python

    from PIL import Image

    img = Image.open('.pics/me_top_left.jpg')

    img.show()
    
.. image:: ./pics/me_top_left.jpg
   :height: 3024 px
   :width:  4032 px
   :scale: 50 %
   
Pasting a logo on an image  

.. code-block:: python

    from PIL import Image

    img = Image.open('.pics/me_top_left.jpg')
    img_copy = img.copy()
    location = (525, 1109)
    img_copy.paste(logo, position,logo)
    img_copy.show()
    
.. image:: ./logoed/me_top_left_logo.jpg
   :height: 1512 px
   :width:  2016 px
   :scale: 50 %
   
Donate
------
`don't donate`_.


Works Cited
************

* Pillow Documentation: https://pillow.readthedocs.io/en/stable/
* auth0 image processing with Pillow: https://auth0.com/blog/image-processing-in-python-with-pillow/
* Python for beginners Tutorial on Pillow: https://www.pythonforbeginners.com/gui/how-to-use-pillow
* Intro to Pillow: https://www.blog.pythonlibrary.org/2016/10/07/an-intro-to-the-python-imaging-library-pillow/


.. _pip: https://pip.pypa.io/en/stable/quickstart/
.. _don't donate: https://venmo.com/LOVER
