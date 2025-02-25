:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/AudioStreamPlaybackResampled.xml.

.. _class_AudioStreamPlaybackResampled:

AudioStreamPlaybackResampled
============================

**Inherits:** :ref:`AudioStreamPlayback<class_AudioStreamPlayback>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

**Inherited By:** :ref:`AudioStreamGeneratorPlayback<class_AudioStreamGeneratorPlayback>`, :ref:`AudioStreamPlaybackOggVorbis<class_AudioStreamPlaybackOggVorbis>`



Methods
-------

+---------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`float<class_float>` | :ref:`_get_stream_sampling_rate<class_AudioStreamPlaybackResampled_method__get_stream_sampling_rate>` **(** **)** |virtual| |const|                             |
+---------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`     | :ref:`_mix_resampled<class_AudioStreamPlaybackResampled_method__mix_resampled>` **(** AudioFrame* dst_buffer, :ref:`int<class_int>` frame_count **)** |virtual| |
+---------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                      | :ref:`begin_resample<class_AudioStreamPlaybackResampled_method_begin_resample>` **(** **)**                                                                     |
+---------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------------------------+

Method Descriptions
-------------------

.. _class_AudioStreamPlaybackResampled_method__get_stream_sampling_rate:

- :ref:`float<class_float>` **_get_stream_sampling_rate** **(** **)** |virtual| |const|

----

.. _class_AudioStreamPlaybackResampled_method__mix_resampled:

- :ref:`int<class_int>` **_mix_resampled** **(** AudioFrame* dst_buffer, :ref:`int<class_int>` frame_count **)** |virtual|

----

.. _class_AudioStreamPlaybackResampled_method_begin_resample:

- void **begin_resample** **(** **)**

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
