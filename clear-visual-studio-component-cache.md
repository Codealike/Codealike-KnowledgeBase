# Clear Visual Studio Component Cache

It is a well known fact that the Component Cache may corrupt on extensions installations. It happens randomly and without any warning. 

While there are many ways to ask Visual Studio "politely" to rebuild it, this is the rudest but guaranteed way to do it.

On Visual Studio 2015

	1. Close Visual Studio (ensure devenv.exe is not present in the Task Manager)
	2. Delete the %USERPROFILE%\AppData\Local\Microsoft\VisualStudio\14.0\ComponentModelCache directory
	3. Restart Visual Studio.

On Visual Studio 2013

	1. Close Visual Studio (ensure devenv.exe is not present in the Task Manager)
	2. Delete the %USERPROFILE%\AppData\Local\Microsoft\VisualStudio\12.0\ComponentModelCache directory
	3. Restart Visual Studio.

On Visual Studio 2012

	1. Close Visual Studio (ensure devenv.exe is not present in the Task Manager)
	2. Delete the %USERPROFILE%\AppData\Local\Microsoft\VisualStudio\11.0\ComponentModelCache directory
	3. Restart Visual Studio. 


On Visual Studio 2010

	1. Close Visual Studio (ensure devenv.exe is not present in the Task Manager)
	2. Delete the %USERPROFILE%\AppData\Local\Microsoft\VisualStudio\10.0\ComponentModelCache directory
	3. Restart Visual Studio.






