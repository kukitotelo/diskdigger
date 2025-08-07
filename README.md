# diskdigger
Are you aware of creating ISO imagÑes by using DISKDIGGER, Aren’t you?  Then have a glimpse at our article. The article is all about creating an ISO file from any CD or DVD. An ISO file is a copy content of an optical disk like a CD or DVD. If you want to back up the disk’s contents simple you can make ISO images of a disk. After a while, you can burn the ISO file you created onto a new disk, which will become a facsimile of the original one. 
comandos de instalacion para linux:
1.-wget https://diskdigger.org/diskdigger_linux_x64.zip
2.-cd diskdigger
3.-cd tmp
4.-chmod +x ./diskdigger
5.-sudo ./diskdigger
disponible kali linux 
Nota: esta herramienta recupera efectivanebte los archivos desde dispositivos de almacenamiento externo en linux en esta distro no se escanea el equipo por si mismo

EN MAC OS 
Running DiskDigger in macOS

This brief guide explains how to run DiskDigger in macOS.

Although support for macOS is still experimental, DiskDigger should provide all the same powerful recovery functionality as it does on Windows. The current Beta version of DiskDigger is built using Avalonia UI, which is a cross-platform toolkit that allows DiskDigger to run on various platforms including Windows, Linux, and macOS.

To run DiskDigger on macOS, download and unzip the appropriate version for your Mac's architecture:

    DiskDigger (beta) for Apple silicon macOS
    DiskDigger (beta) for Intel silicon macOS

Then, open a console window and execute DiskDigger with sudo:

$ cd ~/Downloads
$ sudo ./diskdigger

Here is DiskDigger running in macOS:

 

You must run DiskDigger as a superuser (sudo) because it requires low-level access to your disk(s). If you don't run it with sudo, it will not be able to detect or read any of the physical disks in your system, but you would still be able to read and scan disk images, if you like.
Considerations

Here are a few things to keep in mind when running DiskDigger in macOS:

    Since this is still an experimental version of the application, it is not yet distributed as a self-contained .app file. When you download and extract the Zip file, it will extract the diskdigger executable plus a few native runtime libraries necessary for DiskDigger to function.
    It is generally discouraged to run GUI applications with sudo, but this is simply how DiskDigger works for the moment. I am actively working towards refactoring the business logic into a self-contained lightweight background process that will request its own elevated permissions, independently of the GUI.
    DiskDigger tries to automatically detect the disks in your system by searching for devices of the form "/dev/rdiskn", and so on. If your disk has a different device name, you'll need to manually enter it in the "Advanced" tab on the main screen of DiskDigger.
    When you save any recoverable files, they are saved under the same permissions as the user who launched DiskDigger. In other words, if you launched it with sudo, the recovered files will be owned by the root user. This means that you may need to chmod the permissions on the recovered files to make them accessible to non-sudo users.

Have fun!
Media Coverage

Here's an abridged list of reviews of DiskDigger on other websites:

 

    PCWorld review of the original and updated version
    CNET review
    Lifehacker story
    TechRepublic review
    MajorGeeks review
    dotTech.org review
    ...and many moreDiskDigger for Android!

DiskDigger is now available as an app for Android devices! You can find it on the Google Play Store by searching for "DiskDigger".

Although DiskDigger does not require your device to be rooted, it is more likely to recover more photos and files if your device is rooted. Need help rooting your device?

The app is compatible with any device (tablet or phone) that uses Android 2.2 (Froyo) or higher.
Free or Pro — Which is right for me?

    The free version of DiskDigger can recover photos and videos only (recovering videos requires your device to be rooted).
    The Pro version can recover other types of files besides photos and videos, and also allows uploading recovered files over FTP (again, recovering any types of files besides photos requires your device to be rooted). It also allows more efficient deleting and wiping of unwanted files and free space.

Starting the App

Using DiskDigger for Android is very simple. After launching the app, it will display two options: "Basic scan" and "Full scan." The "full" scan functionality is available only on rooted devices, whereas the "basic" functionality is available regardless of whether your device is rooted.

If your device is rooted, the app should allow you to select the memory partition to scan. Your device's internal memory usually appears as "/data", and the device's SD card usually appears as "/mnt/sdcard" or something similar.

  

If your device is not rooted, tap the "Start basic photo scan" button to continue, and continue to the "Scanning for files" section below.

When you use the app on a rooted device, you may see a Superuser request window. Make sure to press "Allow" in order to grant DiskDigger root access.

After you select the memory device to scan, you will select the types of files that you'd like to recover. For better performance, please select only the file types that you actually need.

Scanning for files

When the app starts scanning for deleted files, you will see the main DiskDigger screen, which will start populating with recoverable files:

You may tap on any of the files to select its checkbox, which will select it for recovery. You may also tap on the overflow menu (three dots) on each of the files, to see recovery options for each individual file.

 
Filtering files

Pressing the "Options" button (gear icon) will allow you to filter the recoverable files based on file size, and file type. If you want to impose a minimum size on the files shown, press the checkbox next to "Minimum file size", and enter the minimum number of bytes below. By default, a minimum size is enabled when recovering photos, to filter out most other (non-photo) images that may be on your device's memory (from browser cache, bitmaps from other apps, etc).

 
Saving files

DiskDigger provides three different ways for you to save the recoverable files: Save to an app, Save to device, and FTP upload, each which are discussed below. To recover one or more files, tap the check mark next to the recoverable files you want to recover, then tap the "Recover" button in the top toolbar.

 
Saving to an app

The first and most recommended method allows you to send the recoverable files to another app on your device. For example, you can send the files to your Email app, so that you could email the files to yourself. You can also send the files to a cloud storage app such as Dropbox or Google Drive. Your device will automatically let you select the app to which the files will be sent:

Saving locally

The second option allows you to save the recoverable files back to the local device (to the internal memory or SD card of the same device from which the files are being recovered).
Saving on Android 5 (Lollipop) and above

This will take you to the standard Android folder picker that you can use to select the folder into which the files will be saved. Unfortunately the standard picker can be a bit difficult to use for the first time. If you see an empty screen with an "Open from" title like in the screenshots below, then follow these steps:

    Swipe away the "Open from" panel to the left.
    Tap the overflow menu (three dots) in the top right corner, and select "Show SD card" or "Show internal memory".
    Tap the navigation menu (three lines in the top left corner, and you should now be able to pick the SD card or Internal memory, and navigate to the exact location where you want to save the files.

Saving on Android 4.4 (Kitkat) and below

You will be prompted to select the directory where the file(s) will be saved. The directory defaults to the location of the memory card on your device (most commonly "/mnt/sdcard"). The directory picker allows you to navigate through the directory structure of your device:

Important note: You should use this method only if you can save the files onto a different partition than the one from which the files are recovered. For example, if you're recovering files from internal memory, you should save the files onto an external SD card (not internal memory).  It is not recommended to save the files onto the same partition from which they were recovered, because that would risk permanently overwriting the very same files that are being recovered!  You should attempt to use one of the other methods of saving the files (save to another app or FTP upload) before resorting to saving locally.
Saving by FTP uploading

The last method allows you to upload the recoverable files to an FTP server. In order to do this, you need to have access to an FTP server that is online, with the correct credentials for accessing and uploading to the server. DiskDigger will display a dialog for you to enter the FTP server's host name, and your user name and password for logging on to the server:

You can also enter an optional subdirectory on the server where the files will be uploaded.

Tap "OK" to begin the uploading process. If the login to the server is successful, you will see status updates at the bottom of the screen, until all files have been uploaded. The files will be named based on the location where they were found.
Cleaning up

Along with recovering your files, DiskDigger gives you the ability to delete them permanently, so that they will no longer be recoverable. Next to the "Recover" button you'll find the "Clean up" button, which will take you to Clean Up mode:

    

The Cleanup screen is divided into two tabs: "Thumbnail caches" and "Photos."  This is because a thumbnail cache (a file that contains multiple thumbnails) must be deleted as a whole, which would delete all the thumbnails contained in it.  Therefore the app allows you to examine these thumbnail caches, as well as individual photos, and select which ones you want to delete.

Cleanup Mode is currently available only in the Basic Scan. Making it available in the Full (rooted) scan is quite a bit more complex, and will be available in a future version.

Note: Since the deletion is done at the filesystem level, the contents of the deleted files are not physically wiped from the device's memory, and may still be recoverable if the device is rooted. In fact, even physical wiping of the files' contents is unreliable with flash memory, which employs wear-leveling that might redirect the overwritten data to a different physical location.

Wiping free space

Another powerful feature provided by DiskDigger is the ability to wipe the free space on your device's memory. This is useful for ensuring that your deleted files (which are now considered free space in your device's memory) will no longer be recoverable, even using tools like DiskDigger.

The "Wipe free space" feature can be accessed directly from the main screen of the DiskDigger app (underneath the selections of Basic Scan and Full Scan). It can also be accessed while performing a Full Scan by tapping the Cleanup button.

    

Like the "Clean up" feature, the "Wipe free space" feature is still a bit experimental, so you should be aware of some of its caveats and limitations:

    Wiping of free space is done by creating a temporary file and filling it with random data, until it consumes the entire amount of free space on your device. When the temporary file begins to reach the limit of free space, the Android system will usually display a notification that your available space is running out. You should ignore this notification until the wipe process is complete. When it finishes, it will delete the temporary file and free up the remaining space again.
    It is possible that the Android system will stop DiskDigger from being able to write to the temporary file before the memory is completely full. This means that there is a possibility that not all of the free space will be wiped, and some deleted data might still be recoverable. You can always re-run DiskDigger and scan your device's memory to ensure whether the wipe was successful.
    The wiping is done only on the internal memory of the device. The ability to wipe an external SD card will be added in a future version.
    It's important to note that because the wiping is done by overwriting all the free space, it means that the process inflicts a significant amount of wear on the device's memory. This can potentially shorten the life span of the memory, and should be performed sparingly, and only when necessary.

Additional notes

The app will likely recover files that haven't been deleted, in addition to files that have.  Because of this, you may have to look through a large number of files before seeing the file(s) you're looking for. This is something that is under continuing development, and will be improved in the future.

If using the app with a non-rooted device, the app will likely recover lower-resolution versions of your photos. This is a limitation that cannot be avoided. To recover the original full-resolution photos, your device must be rooted.
Enjoy!

Of course, all constructive feedback and requests for features are appreciated!

© Dmitry Brant, 2012-2018

 



...and let me know if you encounter any issues!

