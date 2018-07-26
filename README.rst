=========================
diazoframework.goldilocks
=========================


Introduction
============

``diazoframework.goldilocks`` package provides the diazo framework implementation of the 
`Goldilocks Approach CSS framework`_ using the **theming** and **packaging** features available in the 
`diazoframework.plone`_ core package for create `Diazo`_ theme using `plone.app.theming`_.

They are useful for creating themes based on `Goldilocks Approach CSS framework`_. For documentation 
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

- This support the *Goldilocks Approach CSS* v0.1 resources.
- Included Diazo rules for ``base`` and ``theme`` *Goldilocks Approach* CSS styles.


Installation
============

This add-on can be installed has any other add-ons. It's doesn't have any profile, so 
just add it to your Zope instance, for doing that please the follow steps: 


Buildout
--------

If you are a developer, you might enjoy installing it via buildout.

For install ``diazoframework.goldilocks`` package add it to your ``buildout`` section's 
*eggs* parameter e.g.: ::

   [buildout]
    ...
    eggs =
        ...
        diazoframework.goldilocks


and then running ``bin/buildout``.

Or, you can add it as a dependency on your own product ``setup.py`` file: ::

    install_requires=[
        ...
        'diazoframework.goldilocks',
    ],


Resources
=========

The resources of this framework can be reached through 
``/++framework++goldilocks`` and there are placed at 
``diazoframework.goldilocks/diazoframework/goldilocks/framework/`` 
directory with following resources files:

::

    _ css
      _ example
        _ global.css
        _ layout.css
      _ global.css
      _ layout.css
    _ example.html
    _ images
      _ example
        _ footer-logo.png
        _ header-logo.png
        _ responsive2.jpg
        _ responsive3.jpg
        _ responsive4.jpg
        _ responsive.jpg
    _ index.html
    _ js
      _ libs
        _ modernizr-1.7.min.js
    _ preview.png
    _ rules
      _ head.xml
        _ base.xml
        _ theme.xml


Current themes
==============

The `diazoframework.goldilocks`_ package have the following themes:

`diazotheme.goldilocks`_
    which contains themes that can both be used as starters for your 
    own *Goldilocks Approach* based theme.


For more frameworks see: the `diazoframework.plone`_ package.


Contribute
==========

- Issue Tracker: https://github.com/TH-code/diazoframework.goldilocks/issues
- Source Code: https://github.com/TH-code/diazoframework.goldilocks


License
=======

The project is licensed under the GPLv2.


Credits
-------

- Thijs Jonkman (t.jonkman at gmail dot com).


Amazing contributions
---------------------

- Leonardo J. Caballero G. aka macagua (leonardocaballero at gmail dot com).

You can find an updated list of package contributors on https://github.com/TH-code/diazoframework.goldilocks/contributors


.. _`Goldilocks Approach CSS framework`: http://goldilocksapproach.com/
.. _`diazoframework.plone`: https://github.com/collective/diazoframework.plone#current-frameworks
.. _`Diazo`: http://diazo.org
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
.. _`diazoframework.goldilocks`: https://github.com/TH-code/diazoframework.goldilocks
.. _`diazotheme.goldilocks`: https://github.com/TH-code/diazotheme.goldilocks
