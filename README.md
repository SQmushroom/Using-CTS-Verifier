## Using-CTS-Verifier
-Ubuntu 16.04
-Android 5.1

Install OpenJDK on Ubuntu 16.04

>sudo add-apt-repository ppa:openjdk-r/ppa  
>sudo apt-get update   
>sudo apt-get install openjdk-7-jre  

If the java version is not correct, you can change the default java version.

>sudo update-alternatives --config java

# Install Android SDK on Ubuntu

Use command line to install the latest Android SDK.

>wget http://dl.google.com/android/android-sdk_r22.0.5-linux.tgz

Go to the location where you set to download the file and select "Extract Here." 

Open the terminal and open the file. For example:

> cd /home/casper/Downloads/android-sdk-linux/tools
> ./android

Now the Android SDK Manager will show up and you can continue to install packages.

Oen a new terminal and type

>gedit ~/.bashrc

Add path to the top of the text and save it.

> export PATH=${PATH}:~/android-sdk-linux/tools
> export PATH=${PATH}:~/android-sdk-linux/platform-tools


# Install CTS verifier

Go to https://source.android.com/compatibility/cts/downloads and download correct version of CTS Verifier.

Then install apk file on test device.

>adb install <path_to_apk>

Finally the icon will show up on the test device.
