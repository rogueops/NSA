# NSA About
NSA Style Plymouth Boot Splash Updated in 09/2020

The original NSA Plymouth theme by skd1993 in 2015 has been updated
to reflect any changes to Plymouth as well as new backround
and other tweaks.

Continous updates to follow as new changes are implemented

# Install
Run the following to download to current folder:

sudo git clone https://github.com/rogueops/nsa-plymouth.git

Then unzip the file either to the same folder you have the zip
in or better yet straight to the Plymouth themes folder:

sudo unzip /path/to/nsaPlymouth.zip -d /usr/share/plymouth/themes

Then add the NSA Theme to Plymouth:

sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/nsa/nsa.plymouth 60

Now time to select the new NSA Theme:

sudo update-alternatives --config default.plymouth

Lastly update your kernel so it uses the NSA Plymouth boot theme:

sudo update-initramfs -u

Then reboot to see new bootscreen!
