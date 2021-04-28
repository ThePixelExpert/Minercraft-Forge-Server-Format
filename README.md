install java :
	extract the tar.gz to the dir

1.Change to the directory in which you want to install. Type:
cd directory_path_name
For example, to install the software in the /usr/java/ directory, Type:
cd /usr/java/

2.Move the .tar.gz archive binary to the current directory.
Unpack the tarball and install Java
tar zxvf jre-8u73-linux-x64.tar.gz

3.The Java files are installed in a directory called jre1.8.0_73 in the current directory. In this example, it is installed in the /usr/java/jre1.8.0_73 directory. When the installation has completed, you will see the word Done.
Delete the .tar.gz file if you want to save disk space.

CONFIGURE : 

1. Exit Firefox browser if it is already running.

2.Uninstall any previous installations of Java Plugin.
Only one Java Plugin can be used at a time. When you want to use a different plugin, or version of a plugin, remove the symbolic links to any other versions and create a fresh symbolic link to the new one.

Remove the symbolic links (or move them to another directory) to javaplugin-oji.so and libnpjp2.so from the Firefox plugins directory.

3.Create a symbolic link to the Java Plugin in the Firefox plugins directory
Go to the Firefox plugins directory
cd ~/.mozilla/plugins
Create the plugins directory if it does not exist.
Create the symbolic link
32-bit plugin:
ln -s Java installation directory/lib/i386/libnpjp2.so .
64-bit plugin:
ln -s Java installation directory/lib/amd64/libnpjp2.so .

Example
If the Java is installed at this directory:
/usr/java/Java installation directory
Then type in the terminal window to go to the browser plug-in directory:
cd ~/.mozilla/plugins/
Enter the following command to create a symbolic link to the Java Plug-in for Firefox:
ln -s /usr/java/Java installation directory/lib/i386/libnpjp2.so .

4.Start the Firefox browser or restart it if it is already up.

In Firefox, type about:plugins in the Location bar to confirm that the Java Plugin is loaded. You can also click the Tools menu to confirm that Java Console is there.

go to https://www.linuxnorth.org/minecraft/modded_linux.html#Step%203%20-%20Download%20Minecraft%20and%20Forge for help


