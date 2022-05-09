# WinAppRegistryRebuild
WinAppRegistry attempts to rebuild some of the registry of programs that lost their registry info when they were copied into Windows installation without a proper installation, or after a modification to the registry.

The most important part is that it will rebuild the path of programs in HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\App Paths. It will check shortcuts and paths of files in C:\ProgramData\Microsoft\Windows\Start Menu, HKEY_CLASSES_ROOT\Applications and from other sources. It will also automatically rebuild app paths from popular programs by checking if their default installation directories are present. There will be a feature to individually approve every program that WinAppRegistry tries to rebuild, and to view and undo changes that it made to the registry.

Other plans include rebuilding file associations and icons. More stuff may be added.

I am not very knowledgeable on Windows' registry and I'm new to programming in general so please use this at your own risk. That being said, the software is to my knowledge currently not configured to modify any registry values that have already been created, and only seeks to add values. This may change in the future, and I will do my best to change this info accordingly.

Programs that lack registry entries may need more registry entries than what this application seeks to rebuild. I am not aware of all the things programs may need. If you have an idea for something to implement into WinAppRegistry for rebuilding missing parts of an applications registry information, please let me know.
