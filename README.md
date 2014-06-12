[TITANIUM] Android Audio Recorder
=================================
Records audio using the native android AudioRecord API

# Methods
- startRecording(properties)

### Properties
property | values | default
-------- | ------ | -------
filename | ```string``` | Current timestamp
directoryName | ```string``` | 'audio_recorder'
fileLocation | Storage_EXTERNAL or Storage_INTERAL | Storage_EXTERNAL
success | function | no default
error | function | no default

# Events

## Success event
Sent out when the audio file has recorded, calls the successCallback function supplied in the startRecording method.

Passes the following:
* outputFile => The full path to the output file

## Error event
Sent out when an error occurs during recording, calls the errorCallback function supplied in the startRecording method

Passes the following:
* message => The message containing what went wrong