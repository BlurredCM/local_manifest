CyanogenMod local_manifest for BlurredCM
===========

Getting Started
---------------

To get started with Android/CyanogenMod, you'll need to get
familiar with [Git and Repo](http://source.android.com/source/using-repo.html).

First, make a build directory:

	mkdir Andoid (or whatever name you choose)
	cd Android (or the name  you chose)
	mkdir .repo/local_manifests

To initialize your local repository using the CyanogenMod trees, use a command like this:

    repo init -u git://github.com/CyanogenMod/android.git -b cm-11.0

Then download additional repo's for unofficial devices:

    curl -L -o .repo/local_manifests/BlurredCM.xml -O -L https://raw.github.com/BlurredCM/local_manifest/cm-11.0/BlurredCM.xml
 
    	( or Download: https://github.com/BlurredCM/local_manifest/blob/cm-11.0/BlurredCM.xml
		and place it in your ~/Android/.repo/local_manifest.xml (or ~/'name you choose'/.repo)

Then to sync up:

    repo sync [-J#] (# = of your choosing based on your building machine) <-- Read up on this if you care to speed up your suff!
