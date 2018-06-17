=========================
diazoframework.goldilocks
=========================

This package provides the diazo framework implementation of the 
`Goldilocks Approach CSS framework`_. For documentation on the 
framework itself, check the website.


Introduction
============

``diazoframework.goldilocks`` package using the **theming** and 
**packaging** features available in the `diazoframework.plone`_ core 
package for create Diazo_ theme using `plone.app.theming`_.


Requirements
============

- From the Plone 4.1.x To the Plone 4.3 latest versión (https://plone.org/download)
- The ``plone.app.theming`` package (*will be installed as a dependency of this package*)


Features
========

- This support the *Goldilocks Approach CSS* resources for version 0.1.
- Included Diazo rules for ``base`` and ``theme`` *Goldilocks Approach* CSS styles.


Installation
============


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


..
    Enabling the theme
    ^^^^^^^^^^^^^^^^^^

    Select and enable the theme from the Diazo control panel. That's it!


Themes that use it
==================

This framework is used by:

`diazotheme.goldilocks`_
    which contains themes that can both be used as starters for your 
    own *Goldilocks Approach* based theme.

For more frameworks see: the `diazoframework.plone`_ package.


Goldilocks Resources
====================

The resources of this framework can be reached through 
``/++framework++goldilocks`` and there are placed at 
``diazoframework.goldilocks/diazoframework/goldilocks/framework/`` 
directory with following resources files:

::

    framework/
    ├── css
    ├── example.html
    ├── images
    ├── index.html
    ├── js
    ├── preview.png
    └── rules
        └── head
            ├── base.xml
            └── theme.xml


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
- Leonardo Caballero (leonardocaballero at gmail dot com).

.. _`Goldilocks Approach CSS framework`: http://goldilocksapproach.com/
.. _`diazotheme.goldilocks`: https://github.com/TH-code/diazotheme.goldilocks
.. _`diazoframework.plone`: https://github.com/TH-code/diazoframework.plone#current-frameworks
.. _`Diazo`: http://diazo.org
.. _`plone.app.theming`: https://pypi.org/project/plone.app.theming/
