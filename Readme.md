FFmpeg Wrapper

Actualized version, corrected some API problems to work on F21

This GitHub repo is a clone/fork of the official drupal module, who seems not supported anymore.

This is a helper model that provides access to the FFmpeg application. It provides some basic functionality for developers who need to process media files. In addition to transcoding media, FFmpeg Wrapper provides a way to extract specifc data from a media file- duration, dimentions, codec, etc. It is intended to help build a community supported interface to FFmpeg instead of having multiple modules reinventing the wheel every time they want to process rich media.

FFmpeg Wrapper provides an ajax enabled form for applications wishing to build conversion settings, as well as an ability to write configuration files which have specific configuration needs.

The 6.2.x version of this module moves the interface to the ffmpeg_wrapper_ui module and does some significant under the hood improvements. Modules which implemented ffmpeg_wrapper functions only need to update a few function calls to get the new behavior. Conversion from 6.1.x requires
renaming ffmpeg_wrapper_frame_sizes() to ffmpeg_wrapper_ui_frame_sizes().
renaming ffmpeg_wrapper_file_duration() to ffmpeg_wrapper_get_file_duration()


