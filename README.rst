Kytos Sphinx Theme
##################


Kytos Sphinx theme is a sphinx theme build to be used into the kytos
documentations.


Installation
************

Installation from `PyPI` is fairly straightforward:

1. Install the package::

      $ pip install kytos_sphinx_theme

2. Edit the "conf.py" configuration file to point to the kytos theme::

      # At the top.
      import kytos_sphinx_theme

      # ...

      # Activate the theme.
      html_theme = 'kytos'
      html_theme_path = kytos_sphinx_theme.get_html_theme_path()

      html_sidebars = {'**': ['globaltoc_sidebar.html'] }
      html_show_sourcelink = False
      
      

Details of Kytos Sphinx Theme 
*****************************

Here you'll find some directions and tips about the Kytos Sphinx Theme
customization. It can all be done right after cloning or forking this
repository.

First of all, your local `sphinx-theme` repository must be the source for
building the documentation. To install it, run `python setup.py develop` in the
root of this repository.

**CSS Style**

To add some new CSS code, the file that should be edited is
`kytos-sphinx.css_t`, and it can be found in this repository in
`../kytos_sphinx_theme/kytos/static/` path. 

Now the updates can be seen by using`make` in `../kytos/kytos/docs` path.
