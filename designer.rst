Designer
========

PyQt-Fluent-Widgets provides a set of Qt Designer plugins to help you design UI interfaces visually.

Installation
------------

To use the Qt Designer plugins, you need to install the full version of PyQt-Fluent-Widgets:

.. code-block:: bash

    pip install "PyQt-Fluent-Widgets[full]" -i https://pypi.org/simple/

Using in Qt Designer
--------------------

After installation, you can find the PyQt-Fluent-Widgets components in Qt Designer's widget box. Simply drag and drop them onto your form.

.. note::
    If you can't find the components in Qt Designer, please check if the plugins are installed correctly. You may need to restart Qt Designer after installation.

Customizing components
---------------------

Most components support customization through Qt Designer's property editor. You can adjust properties like:

- Style (light/dark)
- Size
- Color
- Text
- Icon

Previewing
----------

You can use Qt Designer's preview功能 to see how your UI will look with PyQt-Fluent-Widgets components.

Generating code
---------------

Once you've designed your UI, you can use Qt Designer's "Form" > "View Code" menu to generate Python code for your interface.