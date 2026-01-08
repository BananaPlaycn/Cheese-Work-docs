Settings
========

PyQt-Fluent-Widgets provides a set of components for creating settings interfaces.

Settings Card
-------------

The `SettingsCard` component is used to group related settings:

.. code-block:: python

    from qfluentwidgets import SettingsCard, SwitchButton, Label

    class ExampleCard(SettingsCard):
        def __init__(self, parent=None):
            super().__init__("Example", "This is an example setting", parent)
            self.switch = SwitchButton(self)
            self.hBoxLayout.addWidget(self.switch, 0, Qt.AlignRight)

Settings Group
--------------

The `SettingsGroup` component is used to group multiple settings cards:

.. code-block:: python

    from qfluentwidgets import SettingsGroup

    group = SettingsGroup("General", self)
    group.addWidget(ExampleCard())
    group.addWidget(AnotherCard())

Settings Panel
--------------

The `SettingsPanel` component provides a complete settings interface:

.. code-block:: python

    from qfluentwidgets import SettingsPanel

    panel = SettingsPanel(self)
    panel.addGroup(group)