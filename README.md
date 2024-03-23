# Termux Api

```
_____                                   _          _
|_   _|__ _ __ _ __ ___  _   ___  __    / \   _ __ (_)
  | |/ _ \ '__| '_ ` _ \| | | \ \/ /   / _ \ | '_ \| |
  | |  __/ |  | | | | | | |_| |>  <   / ___ \| |_) | |
  |_|\___|_|  |_| |_| |_|\__,_/_/\_\ /_/   \_\ .__/|_|
                                             |_|
```


<ol>
 <li><b>termux-wake-lock</li></b> 

```
usage: termux-wake-lock
Acquire the Termux wake lock to prevent the CPU from sleeping.
```

<li><b>termux-fix-shebang</li></b> 


```
usage: termux-fix-shebang <files>
Rewrite shebangs in specified files for running under Termux,
which is done by rewriting #!*/bin/binary to #!$PREFIX/bin/binary.
```

<li><b>termux-reload-settings</li></b> 


```
usage: termux-reload-settings
Use without arguments to reload settings after modifying any of:
  ~/.termux/colors.properties
  ~/.termux/font.ttf 
  ~/.termux/termux.properties
```

<li><b>termux-wake-unlock</li></b> 


```
usage: termux-wake-unlock
Release the Termux wake lock to allow the CPU to sleep.
```

<li><b>termux-fix-shebang</li></b> 


```
usage: termux-setup-storage
Use without arguments to ensure storage permission granted
and symlinks to storage available in $HOME/storage
```

<li><b>termux-open-url</li></b> 


```
usage: termux-open-url <url>
open a URL for viewing.
```

<li><b>termux-info</li></b> 


```
usage: termux-info
Provides information about Termux, and the current system. Helpful for debugging.
```

<li><b>termux-open</li></b> 


```
Usage: termux-open [options] path-or-url
Open a file or URL in an external app.
  --send               if the file should be shared for sending
  --view               if the file should be shared for viewing (default)
  --chooser            if an app chooser should always be shown
  --content-type type  specify the content type to use
```

<li><b>termux-job-scheduler</li></b> 


```
Usage: termux-job-scheduler [options]
Schedule a script to run at specificied time(s).
  --script                   path to the script to be called
  --job-id int               job id (will overwrite any previous job with the same id)
  --pending boolean          list pending jobs only (default false)
  --period-ms int            schedule job approximately every period-ms milliseconds (default 0 means once)
  --network                  run only when this type of network available, default none (any|unmetered|cellular|not_roaming|none)
  --battery-not-low boolean  run only when battery is not low, default true (at least Androi O)
  --storage-not-low boolean  run only when storage is not low, default false (at least Androi O)
  --charging boolean         run only when charging, default false
  --trigger-content-uri text (at least Android N)
  --trigger-content-flag int default 1, (at least Android N)
```

<li><b>termux-wallpaper</li></b> 


```
Change wallpaper on your device

Usage: termux-wallpaper cmd [args]
-h         show this help
-f <file>  set wallpaper from file
-u <url>   set wallpaper from url resource
-l         set wallpaper for lockscreen (Nougat and later)
```

<li><b>termux-sensor</li></b> 


```
Usage: termux-sensor
Get information about types of sensors as well as live data
  -h, help           Show this help
  -a, all            Listen to all sensors (WARNING! may have battery impact)
  -c, cleanup        Perform cleanup (release sensor resources)
  -l, list           Show list of available sensors
  -s, sensors [,,,]  Sensors to listen to (can contain just partial name)
  -d, delay [ms]     Delay time in milliseconds before receiving new sensor update
  -n, limit [num]    Number of times to read sensor(s) (default: continuous) (min: 1)
```

<li><b>termux-notification</li></b> 


```
Usage: termux-notification [options]
Display a system notification. Content text is read from stdin or specified using --content.
  --action action          action to execute when pressing the notification
  --button1 text           text to show on the first notification button
  --button1-action action  action to execute on the first notification button
  --button2 text           text to show on the second notification button
  --button2-action action  action to execute on the second notification button
  --button3 text           text to show on the third notification button
  --button3-action action  action to execute on the third notification button
  --content content        content to show in the notification. Will take precedence over stdin.
  --id id                  notification id (will overwrite any previous notification with the same id)
  --led-color rrggbb       color of the blinking led as RRGGBB (default: none)
  --led-on milliseconds    number of milliseconds for the LED to be on while it's flashing (default: 800)
  --led-off milliseconds   number of milliseconds for the LED to be off while it's flashing (default: 800)
  --on-delete action       action to execute when the the notification is cleared
  --priority prio          notification priority (high/low/max/min/default)
  --sound                  play a sound with the notification
  --title title            notification title to show
  --vibrate pattern        vibrate pattern, comma separated as in 500,1000,200
```

<li><b>termux-media-scan</li></b> 


```
Usage: termux-media-scan [-v] [-r] file [file...]
Scan the specified file(s) and add it to the media content provider.
  -r  scan directories recursively
  -v  verbose mode
```

<li><b>termux-infrared-frequencies</li></b> 


```
Usage: termux-infrared-frequencies
Query the infrared transmitter's supported carrier frequencies.
```

<li><b>termux-wifi-connectioninfo</li></b> 


```
Usage: termux-wifi-connectioninfo
Get information about the current wifi connection.
```

<li><b>termux-telephony-deviceinfo</li></b> 


```
Usage: termux-telephony-deviceinfo
Get information about the telephony device.
```

<li><b>termux-camera-photo</li></b> 


```
Usage: termux-camera-photo [-c camera-id] output-file
Take a photo and save it to a file in JPEG format.
  -c camera-id  ID of the camera to use (see termux-camera-info), default: 0
```

<li><b>termux-fingerprint</li></b> 


```
Usage: termux-fingerprint
Use fingerprint sensor on device to check for authentication
NOTE: Only available on Marshmallow and later
```

<li><b>termux-torch</li></b> 


```
Illegal parameter: -h
Usage: termux-torch [on | off]
Toggle LED Torch on device
```

<li><b>termux-call-log</li></b> 


```
Usage: termux-call-log [-l limit] [-o offset]
List call log history
  -l limit   offset in call log list (default: 10)
  -o offset  offset in call log list (default: 0)
```

<li><b>termux-tts-speak</li></b> 


```
Usage: termux-tts-speak [-e engine] [-l language] [-n region] [-v variant] [-p pitch] [-r rate] [-s stream] [text-to-speak]
Speak text with a system text-to-speech (TTS) engine. The text to speak is either supplied as arguments or read from stdin if no arguments are given.
  -e engine    TTS engine to use (see termux-tts-engines)
  -l language  language to speak in (may be unsupported by the engine)
  -n region    region of language to speak in
  -v variant   variant of the language to speak in
  -p pitch     pitch to use in speech. 1.0 is the normal pitch,
                 lower values lower the tone of the synthesized voice,
                 greater values increase it.
  -r rate      speech rate to use. 1.0 is the normal speech rate,
                 lower values slow down the speech
                 (0.5 is half the normal speech rate)
                 while greater values accelerates it
                 (2.0 is twice the normal speech rate).
  -s stream    audio stream to use (default:NOTIFICATION), one of:
                 ALARM, MUSIC, NOTIFICATION, RING, SYSTEM, VOICE_CALL
```

<li><b>termux-toast</li></b> 


```
Usage: termux-toast [-b bgcolor] [-c color] [-g gravity] [-s] [text]
Show text in a Toast (a transient popup). The text to show is either supplied as arguments or read from stdin if no arguments are given.
 -h  show this help
 -b  set background color (default: gray)
 -c  set text color (default: white)
 -g  set position of toast: [top, middle, or bottom] (default: middle)
 -s  only show the toast for a short while
NOTE: color can be a standard name (i.e. red) or 6 / 8 digit hex value (i.e. "#FF0000" or "#FFFF0000") where order is (AA)RRGGBB. Invalid color will revert to default value
```

<li><b>termux-tts-engines</li></b> 


```
Usage: termux-tts-engines
Get information about the available text-to-speech (TTS) engines. The name of an engine may be given to the termux-tts-speak command using the -e option.
```

<li><b>termux-clipboard-get</li></b> 


```
Usage: termux-clipboard-get
Get the system clipboard text.
```

<li><b>termux-battery-status</li></b> 


```
Usage: termux-battery-status
Get the status of the device battery.
```

<li><b>termux-notification-remove</li></b> 


```
Usage: termux-notification-remove notification-id
Remove a notification previously shown with termux-notification --id.
```

<li><b>termux-vibrate</li></b> 


```
Usage: termux-vibrate [-d duration] [-f]
Vibrate the device.
  -d duration  the duration to vibrate in ms (default:1000)
  -f           force vibration even in silent mode
```

<li><b>termux-camera-info</li></b> 


```
Usage: termux-camera-info
Get information about device camera(s).
```

<li><b>termux-location</li></b> 


```
usage: termux-location [-p provider] [-r request]
Get the device location.
  -p provider  location provider [gps/network/passive] (default: gps)
  -r request   kind of request to make [once/last/updates] (default: once)
```

<li><b>termux-wifi-enable</li></b> 


```
Usage: termux-wifi-enable [true | false]
Toggle Wi-Fi On/Off
```

<li><b>termux-infrared-transmit</li></b> 


```
Usage: termux-infrared-transmit -f frequency pattern
Transmit an infrared pattern. The pattern is specified in comma-separated on/off intervals, such as '20,50,20,30'. Only patterns shorter than 2 seconds will be transmitted.
  -f frequency  IR carrier frequency in Hertz
```

<li><b>termux-storage-get</li></b> 


```
Usage: termux-storage-get output-file
Request a file from the system and output it to the specified file.
```

<li><b>termux-audio-info</li></b> 


```
Usage: termux-audio-info
Get information about audio capabilities.
```

<li><b>termux-keystore</li></b> 


```
Usage: termux-keystore command
These commands are supported:
  list [-d]
  delete <alias>********
  generate <alias> [-a alg] [-s size] [-u validity]
  sign <alias> <algorithm>
  verify <alias> <algorithm> <signature>

list: List the keys stored inside the keystore.
  -d           Detailed results (includes key parameters).

delete: Permanently delete a given key from the keystore.
  alias        Alias of the key to delete.

generate: Create a new key inside the hardware keystore.
  alias        Alias of the key.
  -a alg       Algorithm to use (either 'RSA' or 'EC'). Defaults to RSA.
  -s size      Key size to use. For RSA, the options are 2048, 3072
               and 4096. For EC, the options are 256, 384 and 521.
  -u validity  User validity duration in seconds. Omit to disable.
               When enabled, the key can only be used for the
               duration specified after the device unlocks. After
               the duration has passed, the user needs to re-lock
               and unlock the device again to be able to use this key.

sign: Sign using the given key, the data is read from stdin and the
signature is output to stdout.
  alias        Alias of the key to use for signing.
  algorithm    Algorithm to use, e.g. 'SHA256withRSA'. This should
               match the algorithm of the key.

verify: Verify a signature. The data (original file) is read from stdin.
  alias        Alias of the key to use for verify.
  algorithm    Algorithm that was used to sign this data.
  signature    Signature file to use in verification.
```

<li><b>termux-share</li></b> 


```
Usage: termux-share [-a action] [-c content-type] [-d] [-t title] [file]
Share a file specified as argument or the text received on stdin if no file argument is given.
  -a action        which action to performed on the shared content:
                     edit/send/view (default:view)
  -c content-type  content-type to use (default: guessed from file extension,
                     text/plain for stdin)
  -d               share to the default receiver if one is selected
                     instead of showing a chooser
  -t title         title to use for shared content (default: shared file name)
```

<li><b>termux-clipboard-set</li></b> 


```
Usage: termux-clipboard-set [text]
Set the system clipboard text. The text to set is either supplied as arguments or read from stdin if no arguments are given.
```

<li><b>termux-telephony-cellinfo</li></b> 


```
Usage: termux-telephony-cellinfo
Get information about all observed cell information from all radios on the device including the primary and neighboring cells.
```

<li><b>termux-dialog</li></b> 


```
Usage: termux-dialog widget [options]
Get user input w/ different widgets! Default: text
   -h, help   Show this help
   -l, list   List all widgets and their options
   -t, title  Set title of input dialog (optional)
```

<li><b>termux-speech-to-text</li></b> 


```
Usage: termux-speech-to-text
Converts speech to text, sending partial matches to stdout.
```

<li><b>termux-download</li></b> 


```
Usage: termux-download [-d description] [-t title] url-to-download
Download a resource using the system download manager.
  -d description  description for the download request notification
  -t title        title for the download request notification
```

<li><b>termux-telephony-call</li></b> 


```
Usage: termux-telephony-call <number>
Call a telephony number.
```

<li><b>termux-media-player</li></b> 


```
termux-media-player: Invalid cmd: '-h'
Usage: termux-media-player cmd [args]

help        Shows this help
info        Displays current playback information
play        Resumes playback if paused
play <file> Plays specified media file
pause       Pauses playback
stop        Quits playback
```

<li><b>termux-wifi-scaninfo</li></b> 


```
Usage: termux-wifi-scaninfo
Get information about the last wifi scan.
```

<li><b>termux-microphone-record</li></b> 


```
Usage: termux-microphone-record [args]
Record using microphone on your device

-h           Shows this help
-d           Start recording w/ defaults
-f <file>    Start recording to specific file
-l <limit>   Start recording w/ specified limit (in seconds, unlimited for 0)
-e <encoder> Start recording w/ specified encoder (aac, amr_wb, amr_nb)
-b <bitrate> Start recording w/ specified bitrate (in kbps)
-r <rate>    Start recording w/ specified sampling rate (in Hz)
-c <count>   Start recording w/ specified channel count (1, 2, ...)
-i           Get info about current recording
-q           Quits recording
```

<li><b>termux-volume</li></b> 


```
Usage: termux-volume stream volume
Change volume of audio stream
Valid audio streams are: alarm, music, notification, ring, system, call
Call w/o arguments to show information about each audio stream
```

<li><b>termux-contact-list</li></b> 


```
Usage: termux-contact-list
List all contacts.
```

<li><b>termux-sms-list</li></b> 


```
Usage: termux-sms-list [-d] [-l limit] [-n] [-o offset] [-t type]
List SMS messages.
  -d         show dates when messages were created
  -l limit   offset in sms list (default: 10)
  -n         show phone numbers
  -o offset  offset in sms list (default: 0)
  -t type    the type of messages to list (default: inbox):
             all|inbox|sent|draft|outbox
```

<li><b>termux-sms-send</li></b> 


```
Usage: termux-sms-send -n number[,number2,number3,...] [text]
Send a SMS message to the specified recipient number(s). The text to send is either supplied as arguments or read from stdin if no arguments are given.
  -n number(s)  recipient number(s) - separate multiple numbers by commas
```

<li><b>termux-brightness</li></b> 


```
Usage: termux-brightness brightness
Set the screen brightness between 0 and 255 or auto
```
</ol> 
