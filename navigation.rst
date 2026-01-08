Navigation
==========

PyQt-Fluent-Widgets provides a set of navigation components to help you create intuitive navigation interfaces.

Navigation Bar
--------------

The `NavigationBar` component is used to create a navigation bar at the top of the window:

.. code-block:: python

    from qfluentwidgets import NavigationBar, NavigationItemPosition

    navBar = NavigationBar(self)
    navBar.addItem("Home", "Home.svg", self.homeInterface)
    navBar.addItem("Settings", "Settings.svg", self.settingsInterface)
    navBar.addItem("About", "About.svg", self.aboutInterface, NavigationItemPosition.RIGHT)

Navigation Panel
----------------

The `NavigationPanel` component is used to create a navigation panel on the left side of the window:

.. code-block:: python

    from qfluentwidgets import NavigationPanel

    panel = NavigationPanel(self)
    panel.addItem("Home", "Home.svg", self.homeInterface)
    panel.addItem("Settings", "Settings.svg", self.settingsInterface)

Fluent Window
-------------

The `FluentWindow` component provides a complete window with navigation bar and content area:

.. code-block:: python

    from qfluentwidgets import FluentWindow

    class Window(FluentWindow):
        def __init__(self):
            super().__init__()
            self.addSubInterface(self.homeInterface, "Home", "Home.svg")
            self.addSubInterface(self.settingsInterface, "Settings", "Settings.svg")