Device Security
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Data sent to ELMO should be set up securely using HTTPS
(**Administrators take note!**). In addition, each physical device
should also be secured. Here are some security methods you might
consider:

1. Use a Screen Lock
2. Encrypt Device with SD Card Encryption
3. Turn off Developer Options
4. Protect Device from Harmful Applications
5. Delete forms automatically after being sent in ODK Collect

These suggestions are covered in more detail below. They are just here
for your consideration; you should refer to the Android Quick Start
Guide for more information. If your device is on Android version 5.x,
`click
here <https://play.google.com/books/reader?id=dnzVBAAAQBAJ&printsec=frontcover&output=reader&hl=en&pg=GBS.PR1>`__;
if it is on 6.x, `click
here <https://play.google.com/books/reader?id=tu6bCgAAQBAJ&printsec=frontcover&output=reader&hl=en&pg=GBS.PP1>`__.

Use a Screen Lock
^^^^^^^^^^^^^^^^^^^^^^^^

Think of a screen lock as a password to unlock a phone. Using a screen
lock is important for security. If someone is in physical possession of
a device, to access the device’s information, they will need to know how
to unlock the device.

Android has several options for screen locks. These include drawing a
pattern, a numerical keyphrase, and a text passphrase. On newer devices,
fingerprint scanning is also possible as a screen lock.

A screen lock should allow the user of the device easy access to the
device and their data, but should be difficult for someone else to guess
or access.

**Opening the Screen Lock Menu**

To change screen lock settings, go to the main settings menu and look
for a Lock Screen, Screen Lock, or Security or something similar.

**Android 6.0 and up**

*Settings > Security > Screen Lock*

Open the device’s Settings application. Look for Security and select it.
Then select Screen Lock.

**Android 5.0**

*Settings > Lock screen*

From the Home screen, pull down the main menu by swiping down. The gear
menu in the right corner opens Settings. Inside Settings, find and
select Lock Screen.

**Changing The Screen Lock**

Once inside the screen lock menu, select the screen lock you wish to
use. You will be guided through how to change the screen lock. The
screen lock options available depend on each device, its operating
system (OS), and the version of the OS on the device.

Encrypt Device with SD Card Encryption
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

If a device is lost, stolen, or in someone else’s possession, they may
be able to gain access to the data on the device by physically accessing
the data card. Encryption stores data in a scrambled state. Encryption
ensures that only those with credentials can unscramble or unencrypt the
data and read it.

According to Android documentation: “Encryption stores… data in a form
that can only be read if you have the right credentials. This can
provide additional protection in case [a] device is stolen.” (1) Types
of data that can be encrypted include “account data, app data, music and
other media, and downloaded information.”
`(source) <https://support.google.com/nexus/answer/2844831>`__

**To Access Encryption Settings**

In the main settings menu, look for *Security* or similar. Inside the
security screen, look for *Encryption*, *Encrypt phone*, *Encrypt
tablet*, or similar.

**Android (5.0, 4.4 and lower)**

*Settings > Security > Encrypt [device]*

**Encrypting Your Device**

Inside the Encryption menu, follow the instructions on the screen to
encrypt the device. You will need to have access to a charger and set
aside an hour or more for the encryption process.

**Use Encryption with a screen lock**

It is recommended to use a screen lock if encryption is used on a
device. Without a screen lock, encryption’s security protection is
reduced.

Some devices require a screen lock if encryption is enabled. Some
devices only allow certain types of screen locks to be used, such as a
pin or password, when encryption is enabled.

Turn off Developer Options
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Developer options are settings within the Android system that allow a
device to be used to develop and debug an application. If you are not
actively testing an application, you do not need to keep developer
options on.

**Determine If You Have Ever Activated Developer Options**

By default, developer options are completely hidden in Settings. Look in
the main settings menu. Is there an option listed for *Developer
Options* or something similar?

If not, developer options have not been activated on the device. You can
skip the remaining steps in this section.

If *Developer Options* or something similar is listed, you should follow
the next steps to secure the device.

**Open Developer Options**

*Settings > Developer Options*

**Turn Off Developer Options**

Once *Developer Options* is open, turn off *Developer Options*.

Inside *Developer Options*, if you see that *Developer Options* are
already turned off on this device, this device is protected. You can
skip the remaining steps in this section.

Turning off *Developer Options* may involve moving a toggle from the
“\ *on*\ ” to “\ *off*\ ” position. Or it may involve deselecting all
options so that no checkboxes remain checked.

**Android 5.0**

On the top bar inside *Developer Options*, switch the toggle from *On*
to *Off*. You will know *Developer Options* are turned off when the
options on the screen are grayed out.

Protection from Harmful Applications
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Each time an application is installed, it has the potential to access
data and media, information about other apps, geolocation, and a great
deal of information about each device. It is important to install only
trusted applications and to remove any applications that are not
trusted.

After the initial install of necessary programs on the device, such as
ELMO software, device preparers can add security measures to protect
against harmful applications.

**Use the Approved Application Store**

It is recommended to install applications through the operating system’s
approved application store. For Android devices, this means most
applications should be installed through *Google Play Store*. The
applications found in the operating system’s approved application store
have been vetted to ensure the application does not contain malware.
Despite this, it is possible for an application from the approved
application store to be rouge in some way, including asking for
permissions to information on your device that it does not need. It is
good practice for election observers and device preparers to only
install programs that are needed and trusted.

**Turn Off Unknown Sources**

To ensure only applications from the approved application store can be
used, device prepares can turn off the *Unknown Sources* setting.

Inside the device’s settings, look for a setting related to types of
applications that can be installed. On some devices, this may mean
making sure the box marked next to *Unknown Sources* is not checked or
to uncheck it, if needed. On other devices, there may be a different way
to turn off *Unknown Sources*.

**Android 5.0**

*Settings > Security > Phone Administration > Unknown Sources*

**Turn on App Verification**

App verification ensures that an application undergoes a security check
on install and periodically. Look for a setting inside the main settings
security menu related to “\ *app verification*,” “\ *verify apps*,” or
something similar. Ensure that application verification is enabled.

**Android 5.0**

*Settings > Security > Phone Administration > Verify Apps*

Make sure the box next to Verify apps is checked.

**Android 6.0**

1. Access *Google Settings*. You can use one of these methods:

   1. Open the *Settings* Touch *Google*.
   2. Open the *Google Settings*

2. Inside *Google Settings*, touch *Security*.
3. Under *Verify Apps*, ensure that *Verify Apps* is turned on and turn
   on *Scan device for security threats*.

**Uninstall questionable applications**

If questionable apps have been installed on a device or there are
applications that are no longer needed on the device, it is recommended
that these applications be uninstalled for added security.

ODK Collect: Delete After Sending Forms
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

In case you are worried about sensitive information you’ve collected and
“what if I lose my device,” you may want to also consider removing any
filled out forms on the ODK Collect app after they have been submitted
and received by ELMO.

The “Delete After Send” option is available through ODK Collect
settings. For more information, please visit https://opendatakit.org/.
