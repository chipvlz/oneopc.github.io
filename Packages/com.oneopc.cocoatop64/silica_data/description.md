CocoaTop: Process Viewer for iOS GUI

I'm releasing the source code for everyone to improve. The license is GPL-3, except for the include files in kern, net, netinet, sys, and xpc folders. These are taken from public Mach kernel code and put here to simplify building. You are free to modify the About text (a.k.a. The Story) any way you want, but I will appreciate if you leave a few honorable mentions with links:

Jonathan Levin (http://newosxbook.com/) who gave a deep insight into iOS internals.
@DylanDuff3 (http://twitter.com/dylanduff3) who created the icon.
Domo (https://github.com/D0m0/), who is the original author.
The main challenge is porting the code to modern iOS SDKs by replacing deprecated methods with new ones. This is actually a lot of work, and I don't have the time to do it on my own.

If you are willing to port CocoaTop to iOS 10, 11, 12, etc., please bear in mind the following:

It would be a good idea to build for arm64 platform. The code is already adapted, you need to set "ARCHS = arm64" in the Makefile.
Feel free to remove support for old iOSes (5, 6, 7, 8, etc...)
http://twitter.com/dylanduff3