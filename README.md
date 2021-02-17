# PiSafe  -  Raspberry Pi imaging app

Backup or Restore Raspberry Pi devices (SD-cards, USB sticks, SSD...) to/from a compressed image-file right on your Pi!

 - Backup an SD card to an image-file.

 - Restore an image-file to an SD card.

 - Works entirely on a Raspberry Pi.  No Windows or Mac needed. 
 
 - Creates a compressed image-file that will resize to fill the new card it is restored to (thanks to PiShrink!).
 
 - Supports .img .zip .xz and .gz file formats.
 
 - Supports all USB storage (I think).
 
 - Supports USB boot 
 
 - Seems to support backing up the live boot SD-card.  You have to enable "allow root backup".  
    CAUTION: Reboot first, close everything and don't use the system while it is backing up!  Send your backup image to a different drive!
    
 - Compatible with RPI Imager that comes with the pi.

 - Create a library of your own pi images, then restore them to whatever device you want, whenever you want.  
 
 - This adds a graphical front-end to my 'sd' project which is a command-line version.
 
 - See Leepspvideo review on youtube:  https://www.youtube.com/watch?v=XP6ycUR9Ih0&t=2s
 
 .
 
# SETUP
 
   1) Install Raspberry PI OS on an SD card that is large enough to hold some SD image-files.  32GB or 64GB will do.  This is your Master SD-card.
   
   2) Install Pi-Safe as described below.
   
   3) You will need a USB-SD reader for your source SD-card.
   
   4) You will need some SD cards.  Use as small of an SD-card as you can because the entire card has to be read in before it is shrunk and compressed.  I have been using Sandisk Industrial 8GB cards.
   
.   

   
# TO MAKE AN IMAGE FILE  
   
   1) Remove your source SD card (8GB) and Boot your Pi with your Master SD-card as above.
   
   2) Put your source SD-card (8GB) in the USB SD reader and insert it in a Pi USB port.
   
   3) Startup Pi-Safe from the menu.  Or in a terminal, type in 'pisafe'
        
   5) Use the menu to select BACKUP, select your SD-card and the image-file a name.
   
   6) Watch your image-file get created, shrunk and compressed automatically.
   
   7) Note: At this point, I have left several safeties in place.  I may add an option to remove them in the future.  For example you have to type in "YES"
 before it will RESTORE an image file to an SD card.   
 .
   

# INSTALL

In a terminal window, type in

    wget https://raw.githubusercontent.com/RichardMidnight/pi-safe/main/pisafe
    bash pisafe
    
    Then you can select 'install' from the menu to install it in your Raspberry Pi menu
    
   
   
 # REFERENCES
 
Thanks to Raspberry Pi for how to read and write an image file.

Thanks to https://github.com/Drewsif/PiShrink for the PiShrink engine.

Thanks to all the people who posted code snipets on the web.

    
