==============================
Installation of docs_template
==============================


Docs
=====

To build the documentation, you need to install the following packages:

* sphinx
* sphinx_rtd_theme
* sphinx-autodocgen
* sphinxcontrib-napoleon

Then, you can build the documentation by running the following command:

.. code:: bash

    sphinx-build -b html docs/source/ docs/build/html
    docker run -it --rm -d -p 9999:80 --name docs_template -v /path/to/docs/html/:/usr/share/nginx/html nginx
