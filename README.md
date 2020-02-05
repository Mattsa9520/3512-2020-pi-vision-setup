# 3512-2020-pi-vision-setup
FRC Team 3512's setup for raspberry pi for vision processing and driver view

This is the setup we used for our vision processer, Chameleon Vision, and our driver view, 
Potential engine. 

WHAT YOU NEED:
A raspberry pi with chameleon vision and potential engine. 

WHAT TO DO: 
copy both files, you can change the names if you want, obviously.

both files need to be in /lib/systemd/system
 you can do this by running the command:

 "sudo nano /lib/systemd/system/<filename>"

 after that you need to run:
 
 "sudo chmod 644 /lib/systemd/system/<filename>"

 then:

 "sudo systemctl daemon-reload" and after that, "sudo systemctl enable <filename>" 

 after that you can reboot. This process needs to be done for both service files. After that
 chameleon vision and potential engine will be running in the background, and you'll be able to also
 use your pi console at that same time. 

 NOTES:
 To configure your potential engine server you'll need to edit the service file and change the server ip, port, etc.
 You can configure chameleon vision in the 
