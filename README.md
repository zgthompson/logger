# Toy Ubuntu keylogger

This is just a simple bash script that logs alphabetic keystrokes into LOGGED_KEYS.txt. The format is one line per letter.
It can be run without superuser privileges and will capture keys from any application on the machine.

I haven't tested this on other Linux environments, but it should work whenever the xinput utility is available.
Running "xinput" will show the id of all devices available, while "xinput test NUM" will test the device with the corresponding id.
In my case "AT Translated Set 2 keyboard" was mapped to id 10. I'm not sure if this number is different on different machines. If so,
just change the KEYBOARD_ID at the beginning of the bash script to the appropriate id.

