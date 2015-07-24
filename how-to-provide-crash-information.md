##How to provide Visual Studio crash information

Crashes are pretty rare, because usually Visual Studio is able to detect issues and stop the loading process. 
If Visual Studio crashes, the odds are something in your configuration is wildly different to anything we have tested before. We would need your help to fix it.

If you have only Visual Studio 2010 installed. 

- Make sure you have .Net 4.5 Installed. You can run the .Net 4.5 installer and it will check for it. 

>This is the most common case of crashes and there is nothing we can do about it. Visual Studio fails to load the assemblies and crash itself. *Installing .NET Framework 4.5 should solve the issue*.


Since the crashes usually happen before the extension can even be loaded by Visual Studio (it they would be able to load, Visual Studio would not crash). The best way to find out why it is not failing on assembly binding time is to enable [Fusion Logging](http://msdn.microsoft.com/en-us/library/e74a18c4%28v=vs.71%29.aspx) and send us the log.

>If you are lazy like us just go to the bottom for the quick way to do it ;)

To enable Fusion add the following values to

	HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Fusion
	Add:
		DWORD ForceLog set value to 1
		DWORD LogFailures set value to 1
		DWORD LogResourceBinds set value to 1
	String LogPath set value to folder for logs (e.g. C:\FusionLog\)
	Make sure you include the backslash after the folder name and that the Folder exists.

You need to restart the program that you're running to force it to read those registry settings

To disable just set all those to 0. 

### Fusion Logging (the quick way)

We have those scripts prepared for you. 

1. Create the directory C:\Fusion or change the directory in the script to a directory that already exists.
2. Enable Fusion with the [Fusion-Enabled.reg](https://github.com/Codealike/Codealike-KnowledgeBase/blob/master/scripts/Fusion-Enabled.reg) script.
3. Start Visual Studio with Codealike enabled
4. Disable Fusion with the [Fusion-Disable.reg](https://github.com/Codealike/Codealike-KnowledgeBase/blob/master/scripts/Fusion-Disable.reg) script.
5. Zip the whole fusion directory and send it to us.

