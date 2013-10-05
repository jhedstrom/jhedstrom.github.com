Install Sphinx and dependencies:
  http://sphinx-doc.org/latest/install.html

Install Hieroglyph:
  https://hieroglyph.readthedocs.org/en/hieroglyph-0.5.5/getting-started.html

conf.py is already configured to load hieroglyph.

To build the slides, run the following in the root of the project:
 ``sphinx-build -b slides . slides`` 

Slides will be located in the slides folder.

To make an HTML version, from the root of the project use:
 ``make html``

You'll find the output in the ``_build`` folder.

The reStructuredText Primer at http://sphinx-doc.org/rest.html is helpful.
