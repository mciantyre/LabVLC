# LabVLC
Programmatic video control in LabVIEW, version 1.0

![demo](https://raw.githubusercontent.com/mciantyre/LabVLC/master/demo.PNG)

![blockdemo](https://raw.githubusercontent.com/mciantyre/LabVLC/master/blockdemo.PNG)

### Features
LabVLC provides a high-level library for adding video playback to your LabVIEW projects
- Play, pause, mute, stop video
- Manipulate video volume
- Manipulate video playback speed (affects sound pitch)

### Dependencies
- LabVIEW
- VLC

### Workflow
1. Initialize a VLC controller  in your VI using ```LabVLC - InitControl.vi```. Requires a pointer to the ```libvlc.dll``` of the VLC installation directory, a path to your video, and a PictureBox handle (.NET).
2. Pass the output cluster to the Play VI (```LabVLC - PlayControl.vi```)
3. Perform other playback controls, make some popcorn, watch a movie...
4. Stop the video when desired (```LabVLC - StopControl.vi```)
5. Release the VLC media player using ```LabVLC - TerminateControl.vi```

See ```LabVLC - Example.vi``` to try out a simple video player

### Future work
1. Rewrite documentation to correspond with version 1.0 changes
2. Rewind and fast-forward capabilities
3. Chapter skipping and video bookmarking

