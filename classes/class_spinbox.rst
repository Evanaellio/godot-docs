:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/SpinBox.xml.

.. _class_SpinBox:

SpinBox
=======

**Inherits:** :ref:`Range<class_Range>` **<** :ref:`Control<class_Control>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

Numerical input text field.

Description
-----------

SpinBox is a numerical input text field. It allows entering integers and floats.

\ **Example:**\ 


.. tabs::

 .. code-tab:: gdscript

    var spin_box = SpinBox.new()
    add_child(spin_box)
    var line_edit = spin_box.get_line_edit()
    line_edit.context_menu_enabled = false
    spin_box.horizontal_alignment = LineEdit.HORIZONTAL_ALIGNMENT_RIGHT

 .. code-tab:: csharp

    var spinBox = new SpinBox();
    AddChild(spinBox);
    var lineEdit = spinBox.GetLineEdit();
    lineEdit.ContextMenuEnabled = false;
    spinBox.AlignHorizontal = LineEdit.HorizontalAlignEnum.Right;



The above code will create a ``SpinBox``, disable context menu on it and set the text alignment to right.

See :ref:`Range<class_Range>` class for more options over the ``SpinBox``.

\ **Note:** ``SpinBox`` relies on an underlying :ref:`LineEdit<class_LineEdit>` node. To theme a ``SpinBox``'s background, add theme items for :ref:`LineEdit<class_LineEdit>` and customize them.

\ **Note:** If you want to implement drag and drop for the underlying :ref:`LineEdit<class_LineEdit>`, you can use :ref:`Control.set_drag_forwarding<class_Control_method_set_drag_forwarding>` on the node returned by :ref:`get_line_edit<class_SpinBox_method_get_line_edit>`.

Properties
----------

+-------------------------------------------------------------------+------------------------------------------------------------------------------+-----------+
| :ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` | :ref:`alignment<class_SpinBox_property_alignment>`                           | ``0``     |
+-------------------------------------------------------------------+------------------------------------------------------------------------------+-----------+
| :ref:`float<class_float>`                                         | :ref:`custom_arrow_step<class_SpinBox_property_custom_arrow_step>`           | ``0.0``   |
+-------------------------------------------------------------------+------------------------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>`                                           | :ref:`editable<class_SpinBox_property_editable>`                             | ``true``  |
+-------------------------------------------------------------------+------------------------------------------------------------------------------+-----------+
| :ref:`String<class_String>`                                       | :ref:`prefix<class_SpinBox_property_prefix>`                                 | ``""``    |
+-------------------------------------------------------------------+------------------------------------------------------------------------------+-----------+
| :ref:`String<class_String>`                                       | :ref:`suffix<class_SpinBox_property_suffix>`                                 | ``""``    |
+-------------------------------------------------------------------+------------------------------------------------------------------------------+-----------+
| :ref:`bool<class_bool>`                                           | :ref:`update_on_text_changed<class_SpinBox_property_update_on_text_changed>` | ``false`` |
+-------------------------------------------------------------------+------------------------------------------------------------------------------+-----------+

Methods
-------

+---------------------------------+----------------------------------------------------------------------+
| void                            | :ref:`apply<class_SpinBox_method_apply>` **(** **)**                 |
+---------------------------------+----------------------------------------------------------------------+
| :ref:`LineEdit<class_LineEdit>` | :ref:`get_line_edit<class_SpinBox_method_get_line_edit>` **(** **)** |
+---------------------------------+----------------------------------------------------------------------+

Theme Properties
----------------

+-----------------------------------+------------------------------------------------+
| :ref:`Texture2D<class_Texture2D>` | :ref:`updown<class_SpinBox_theme_icon_updown>` |
+-----------------------------------+------------------------------------------------+

Property Descriptions
---------------------

.. _class_SpinBox_property_alignment:

- :ref:`HorizontalAlignment<enum_@GlobalScope_HorizontalAlignment>` **alignment**

+-----------+---------------------------------+
| *Default* | ``0``                           |
+-----------+---------------------------------+
| *Setter*  | set_horizontal_alignment(value) |
+-----------+---------------------------------+
| *Getter*  | get_horizontal_alignment()      |
+-----------+---------------------------------+

----

.. _class_SpinBox_property_custom_arrow_step:

- :ref:`float<class_float>` **custom_arrow_step**

+-----------+------------------------------+
| *Default* | ``0.0``                      |
+-----------+------------------------------+
| *Setter*  | set_custom_arrow_step(value) |
+-----------+------------------------------+
| *Getter*  | get_custom_arrow_step()      |
+-----------+------------------------------+

If not ``0``, ``value`` will always be rounded to a multiple of ``custom_arrow_step`` when interacting with the arrow buttons of the ``SpinBox``.

----

.. _class_SpinBox_property_editable:

- :ref:`bool<class_bool>` **editable**

+-----------+---------------------+
| *Default* | ``true``            |
+-----------+---------------------+
| *Setter*  | set_editable(value) |
+-----------+---------------------+
| *Getter*  | is_editable()       |
+-----------+---------------------+

If ``true``, the ``SpinBox`` will be editable. Otherwise, it will be read only.

----

.. _class_SpinBox_property_prefix:

- :ref:`String<class_String>` **prefix**

+-----------+-------------------+
| *Default* | ``""``            |
+-----------+-------------------+
| *Setter*  | set_prefix(value) |
+-----------+-------------------+
| *Getter*  | get_prefix()      |
+-----------+-------------------+

Adds the specified ``prefix`` string before the numerical value of the ``SpinBox``.

----

.. _class_SpinBox_property_suffix:

- :ref:`String<class_String>` **suffix**

+-----------+-------------------+
| *Default* | ``""``            |
+-----------+-------------------+
| *Setter*  | set_suffix(value) |
+-----------+-------------------+
| *Getter*  | get_suffix()      |
+-----------+-------------------+

Adds the specified ``suffix`` string after the numerical value of the ``SpinBox``.

----

.. _class_SpinBox_property_update_on_text_changed:

- :ref:`bool<class_bool>` **update_on_text_changed**

+-----------+-----------------------------------+
| *Default* | ``false``                         |
+-----------+-----------------------------------+
| *Setter*  | set_update_on_text_changed(value) |
+-----------+-----------------------------------+
| *Getter*  | get_update_on_text_changed()      |
+-----------+-----------------------------------+

Sets the value of the :ref:`Range<class_Range>` for this ``SpinBox`` when the :ref:`LineEdit<class_LineEdit>` text is *changed* instead of *submitted*. See :ref:`LineEdit.text_changed<class_LineEdit_signal_text_changed>` and :ref:`LineEdit.text_submitted<class_LineEdit_signal_text_submitted>`.

Method Descriptions
-------------------

.. _class_SpinBox_method_apply:

- void **apply** **(** **)**

Applies the current value of this ``SpinBox``.

----

.. _class_SpinBox_method_get_line_edit:

- :ref:`LineEdit<class_LineEdit>` **get_line_edit** **(** **)**

Returns the :ref:`LineEdit<class_LineEdit>` instance from this ``SpinBox``. You can use it to access properties and methods of :ref:`LineEdit<class_LineEdit>`.

\ **Warning:** This is a required internal node, removing and freeing it may cause a crash. If you wish to hide it or any of its children, use their :ref:`CanvasItem.visible<class_CanvasItem_property_visible>` property.

Theme Property Descriptions
---------------------------

.. _class_SpinBox_theme_icon_updown:

- :ref:`Texture2D<class_Texture2D>` **updown**

Sets a custom :ref:`Texture2D<class_Texture2D>` for up and down arrows of the ``SpinBox``.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
