Quick start
===========

This section will help you quickly get started with PyQt-Fluent-Widgets.

Installation
------------

First, you need to install PyQt-Fluent-Widgets using pip:

.. code-block:: bash

    pip install PyQt-Fluent-Widgets -i https://pypi.org/simple/

For full-featured version:

.. code-block:: bash

    pip install "PyQt-Fluent-Widgets[full]" -i https://pypi.org/simple/

Basic usage
-----------

Here's a simple example to get you started:

.. code-block:: python

    from PyQt5.QtWidgets import QApplication
    from qfluentwidgets import FluentWindow, NavigationItemPosition

    class Window(FluentWindow):
        def __init__(self):
            super().__init__()
            # Add navigation items
            self.addSubInterface(self.createHomeInterface(), "Home", "Home.svg")
            self.addSubInterface(self.createSettingsInterface(), "Settings", "Settings.svg")
            
        def createHomeInterface(self):
            from PyQt5.QtWidgets import QWidget, QVBoxLayout, QLabel
            widget = QWidget()
            layout = QVBoxLayout(widget)
            layout.addWidget(QLabel("Welcome to PyQt-Fluent-Widgets!"))
            return widget
            
        def createSettingsInterface(self):
            from PyQt5.QtWidgets import QWidget, QVBoxLayout, QLabel
            widget = QWidget()
            layout = QVBoxLayout(widget)
            layout.addWidget(QLabel("Settings page"))
            return widget

    if __name__ == "__main__":
        app = QApplication([])
        window = Window()
        window.show()
        app.exec_()

Running examples
----------------

You can run the built-in examples to see what PyQt-Fluent-Widgets can do:

.. code-block:: bash

    # Clone the repository
    git clone https://github.com/zhiyiYo/PyQt-Fluent-Widgets.git
    cd PyQt-Fluent-Widgets
    
    # Install dependencies
    pip install -r requirements.txt
    
    # Run gallery example
    cd examples/gallery
    python demo.py