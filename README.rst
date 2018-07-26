======================
diazoframework.amazium
======================


Introduction
============

``diazoframework.amazium`` package provides the diazo framework implementation of the 
`Amazium CSS framework`_ using the **theming** and **packaging** features available in the 
`diazoframework.plone`_ core package for create `Diazo`_ theme using `plone.app.theming`_.

They are useful for creating themes based on `Amazium CSS framework`_. For documentation 
on the framework itself, check the website.

A Diazo framework should provide the framework resources and diazo rules to reuse 
and add to in a Diazo theme.


Requirements
============

- From the Plone 4.1.x To the Plone 4.3 latest version (https://plone.org/download)
- The ``plone.app.theming`` package (*You will need enable it via "Add-ons" control 
  panel to use this package*)
- The ``diazoframework.plone`` package (*You will need enable it via "buildout" 
  configuration to use this package*)


Features
========

- Provides the *Amazium CSS framework* v1.3 resources.
- Included Diazo rules for the **head** that contains ``base`` and ``js`` CSS styles.
- Included Diazo rules for the **body** that contains ``columns`` CSS styles.


Installation
============

This add-on can be installed has any other add-ons. It's doesn't have any profile, so 
just add it to your Zope instance, for doing that please the follow steps: 


Buildout
--------

If you are a developer, you might enjoy installing it via buildout.

For install ``diazoframework.amazium`` package add it to your ``buildout`` section's 
*eggs* parameter e.g.: ::

   [buildout]
    ...
    eggs =
        ...
        diazoframework.amazium


and then running ``bin/buildout``.

Or, you can add it as a dependency on your own product ``setup.py`` file: ::

    install_requires=[
        ...
        'diazoframework.amazium',
    ],


Resources
=========

The resources of this framework can be reached through 
``/++framework++amazium`` and there are placed at 
``diazoframework.amazium/diazoframework/amazium/framework/`` 
directory with following resources files:

::

    _ images
      _ amazium.jpg
      _ apple-touch-icon-114x114.png
      _ apple-touch-icon-72x72.png
      _ apple-touch-icon.png
      _ blank.jpg
      _ btn-arrow.png
      _ bullet.png
      _ favicon.ico
      _ ui.totop.png
    _ includes
      _ amazium.css
      _ base.css
      _ jquery.easing.1.3.js
      _ jquery.ui.totop.js
      _ layout.css
      _ smoothscroll.js
    _ index.html
    _ preview.png
    _ rules
      _ body
        _ columns.xml
      _ head
        _ base.xml
        _ js.xml


Current themes
==============

The `diazoframework.amazium`_ package have the following themes:

`diazotheme.amazium`_
    which contains themes that can both be used as starters for your 
    own *Amazium CSS* based theme.


For more frameworks see: the `diazoframework.plone`_ package.


Contribute
==========

- Issue Tracker: https://github.com/TH-code/diazoframework.amazium/issues
- Source Code: https://github.com/TH-code/diazoframework.amazium


License
=======

The project is licensed under the GPLv2.


Credits
-------

- Thijs Jonkman (t.jonkman at gmail dot com).


Amazing contributions
---------------------

- Leonardo J. Caballero G. aka macagua (leonardocaballero at gmail dot com).

You can find an updated list of package contributors on https://github.com/TH-code/diazoframework.amazium/contributors


.. _`Amazium CSS framework`: http://www.amazium.co.uk/
.. _`diazoframework.plone`: https://github.com/collective/diazoframework.plone#current-frameworks
.. _`Diazo`: http://diazo.org
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
.. _`diazoframework.amazium`: https://github.com/TH-code/diazoframework.amazium
.. _`diazotheme.amazium`: https://github.com/TH-code/diazotheme.amazium
