Icon
====

PyQt-Fluent-Widgets provides a set of icons that follow the Fluent Design System.

Using built-in icons
--------------------

You can use the built-in icons through the `QIcon` class:

.. code-block:: python

    from qfluentwidgets import FluentIcon

    # Get home icon
    icon = FluentIcon.HOME.icon()

    # Get settings icon
    icon = FluentIcon.SETTING.icon()

Custom icons
------------

You can also use custom icons with PyQt-Fluent-Widgets:

.. code-block:: python

    from PyQt5.QtGui import QIcon

    # Create custom icon
    icon = QIcon("path/to/icon.svg")