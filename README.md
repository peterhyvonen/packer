# packer

New Packer Windows 
Git clone
Create a new branch
Move to branch
Create a new appropriate Autounattend.xml under Windows/floppy/answer_files/yourosname
Copy contents from another Autounattend.xml
In the XML change the following
	Product Key (KMS)
	Image Name (dism /get-wiminfo /wimfile:sources/install.wim)
Add any drivers needed to the floppy/drivers
Create a json file under windows
Copy another json file
	Note that Win10/2016 have different KVM info than previous windows versions
	Under floppy files change the path to the drivers
Create a new json.example file in the vars folder by copying a previous one
	Update packer output directory
	Update checksum (md5sum)
	Update packer iso url
Update build.sh
Logon to the cron box
Go to /usr/local/packer
Change your branch
Copy your json.example file to just .json
Run build.sh with appropriate parameters
Open vnc to the port of the building vm

New Packer Linux
