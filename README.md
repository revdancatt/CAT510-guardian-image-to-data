![Screen Shot](http://cattopus23.com/img/panel-CAT510.png)

CAT510 Guardian Image to Data
=============================

Because the Guardian doesn't have CORS enabled images, which means you can access the pixel data when
you throw them onto a canvas element, I needed a quick proxy to convert the image to BASE64.

This way, javascript can go grab the BASE64 data and throw that at an image src, now because
the image to within "scope" of the domain the image can be thrown over to a canvas element and
the pixel data accessed.

The PATH to the image is passed over as a ?img= param, the code prepends the guardian domain
onto the front to prevent the proxy from being used to any old images anywhere.

+ Example: http://guardianimagetodata.appspot.com/img_to_json?img=BOOKS/Pix/pictures/2013/7/26/1374850874749/Margaret-Atwood-005.jpg&callback=?

TODO
====

1. Look back at my code to see if there's something I've forgotten about as it's been so very long.

