##Permanently Remove Codealike Extension

Rarely Visual Studio crashes before its even possible to open the "Extensions Manager", in those cases you may need to remove the extension physically.

On Visual Studio 2015

	1. Close Visual Studio (ensure devenv.exe is not present on the Task Manager).
	2. Go to: %USERPROFILE%\AppData\Local\Microsoft\VisualStudio\14.0\Extensions
	3. Visual Studio generate random directories, look for the directory that has Codealike.Client.dll ( you will spot it pretty fast :) )
	4. Delete the whole folder.
	5. Restart Visual Studio.

On Visual Studio 2013

	1. Close Visual Studio (ensure devenv.exe is not present on the Task Manager).
	2. Go to: %USERPROFILE%\AppData\Local\Microsoft\VisualStudio\12.0\Extensions
	3. Visual Studio generate random directories, look for the directory that has Codealike.Client.dll ( you will spot it pretty fast :) )
	4. Delete the whole folder.
	5. Restart Visual Studio.

On Visual Studio 2012

	1. Close Visual Studio (ensure devenv.exe is not present on the Task Manager).
	2. Go to: %USERPROFILE%\AppData\Local\Microsoft\VisualStudio\11.0\Extensions
	3. Visual Studio generate random directories, look for the directory that has Codealike.Client.dll ( you will spot it pretty fast :) )
	4. Delete the whole folder.
	5. Restart Visual Studio.

On Visual Studio 2010

	1. Close Visual Studio (ensure devenv.exe is not present on the Task Manager).
	2. Go to: %USERPROFILE%\AppData\Local\Microsoft\VisualStudio\10.0\Extensions
	3. Visual Studio generate random directories, look for the directory that has Codealike.Client.dll ( you will spot it pretty fast :) )
	4. Delete the whole folder.
	5. Restart Visual Studio.


