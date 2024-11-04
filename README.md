# Building-a-real-time-clock
I have create a real time clock using mint linux terminal. Here's code for this mini project:
i
#!/bin/bash
Red=$'/e[1.31m'
Green=$'/e[1.32m'
Blue=$'/e[1.34m'   

while true
do
   clear
   echo $ green $(date +%T)
   sleep 1s
done

                                              EXPLATION OF CODE:
These lines define three color variables: Red, Green, and Blue. Each variable is set to an escape sequence that changes the text color. However, the escape sequences are written incorrectly as $'/e[1.31m', and should be '\e[1;31m' (note the corrected slash and semicolon).
1;31m changes text to bright red.
1;32m changes text to bright green.
1;34m changes text to bright blue.
while true: Creates an infinite loop, so the script will run until it’s manually stopped.
clear: Clears the terminal screen before each time update, creating a refreshing effect.
echo $ green $(date +%T): Attempts to display the current time in green. However, echo $ green should be corrected to echo $Green (with proper variable referencing).
date +%T: Displays the current time in HH:MM:SS format.
sleep 1s: Pauses for 1 second to create a delay, updating the time once per second.
