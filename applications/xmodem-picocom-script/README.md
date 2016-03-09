This application demonstrates how to establish communication between a shell script and 
Java application to send/receive a file using Xmodem file transfer protocol.

#####Running this application
   
Run the script as picocom.sh giving ports and file names as shown below.

./picocom.sh RECEIVE_PORT RECEIVE_FILE SEND_PORT SEND_FILE
   
#####What this application does and how it does
- Extract and validate parameters supplied to picocom.sh script.
- Compile Java source files and create app.jar representing Java application that will 
receive the file.
- Schedule this java application to be runned after 4 seconds.
- Schedule simulating keypress and typing file name with the help of xdotool.
- Launch picocom which will receive keyevents and file name and launch sx utility to 
actually do the file transfer.
- Exit after 12 seconds.
     
#####Going further
- The shell script will self terminate after 12 seconds. This can be made interactive.
