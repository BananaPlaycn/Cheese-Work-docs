Theme
=====

PyQt-Fluent-Widgets supports both light and dark themes, and provides a set of APIs to manage themes.

Theme modes
-----------

PyQt-Fluent-Widgets supports three theme modes:

- Light theme
- Dark theme
- System theme (follows the system's theme setting)

Setting theme mode
------------------

You can set the theme mode using the `Theme` class:

.. code-block:: python

    from qfluentwidgets import Theme, setTheme

    # Set light theme
    setTheme(Theme.LIGHT)

    # Set dark theme
    setTheme(Theme.DARK)

    # Set system theme
    setTheme(Theme.AUTO)

Customizing colors
------------------

You can customize the theme colors using the `ThemeColor` class:

.. code-block:: python

    from qfluentwidgets import ThemeColor, setThemeColor

    # Set theme color to blue
    setThemeColor("#0078d4")

    # Set theme color to green
    setThemeColor("#00b42a")