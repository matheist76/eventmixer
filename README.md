eventmixer
==========

Dvswitch replacement, EventMixer:

* Display in real time
* Store changes in text file.
* Gtk or qt, Python module. Nice and simple.
* Stick to a single format over the wire.
evr_device: Have devices which EventRecorderMixer connects to. They must follow the same output standard: 25 fps, mjpeg, 720p or 1080p resolutions, have ip and port numbers. It shouldn’t save the video as that would be the job of the evr_mixer.
evr_device2dv: Because the evr_devices have the same output a simple gstreamer command should be able to convert the mjpeg stream into dv for use with dvswitch. If using the evr_mixer then we don’t use the conversion script.
evr_mixer files: take stream from evr_device and every 10min/600sec create new file. So open new file with stream name and timestamp. Append for 600 secs. Open new file. Maybe get stream name from Eventstreamr. Has to be uuid of some sort. Maybe room_name.stream_no.timestamp.mjpeg
evr_mixer Record/Cut: As Kim says we shouldn’t have any option to record or cut files. It is viewed that once the mixer starts then recording has began. However space button for timestamp on when the talk begins.
evr_mixer PnP: On the left had side have a radio button with one of four corners to select. A slide will adjust size and a simple on off button to apply. On the left side drop down menu for primary and secondary sources with apply button and current selection.
evr_mixer Audio: Should live feed to headphones. Have a selector button set like the primary and secondary video sources but just with the one drop down menu. Should have vu.
Standby loop: Something that we need resolve. Should we allow the volunteers to start? Should it just begin at the breaks etc. One thing that shouldn’t happen is for it to be on during the talk change over.  
 evr_mixer Advance: 
Communication with Eventstramr to obtain start, end and basic schedule information.
Place for notes.
IM inbuilt client.
