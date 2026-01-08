Install
=======

To install lite version (AcrylicLabel is not available) use pip:

.. code-block:: bash

    pip install PyQt-Fluent-Widgets -i https://pypi.org/simple/

Or install full-featured version use pip:

.. code-block:: bash

    pip install "PyQt-Fluent-Widgets[full]" -i https://pypi.org/simple/

If you are using PySide2, PySide6 or PyQt6, you can download the code in PySide2, PySide6 or PyQt6 branch.

.. warning::
    Don't install PyQt-Fluent-Widgets, PyQt6-Fluent-Widgets, PySide2-Fluent-Widgets and PySide6-Fluent-Widgets at the same time, because their package names are all ``qfluentwidgets``.

Run example
-----------

After installing PyQt-Fluent-Widgets package using pip, you can run any demo in the examples directory, for example:

.. code-block:: bash

    cd examples/gallery
    python demo.py

.. note::
    If you encounter ``ImportError: cannot import name 'xxx' from 'qfluentwidgets'``, it indicates that the package version you installed is too low. You can replace the mirror source with https://pypi.org/simple and reinstall again.