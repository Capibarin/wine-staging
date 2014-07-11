wine-compholio
==============

The Wine "Compholio" Edition repository includes a variety of patches for Wine to run common Windows applications under Linux.

These patches fix the following Wine bugs:

* ([Wine Bug #32328](http://bugs.winehq.org/show_bug.cgi?id=32328)) Many .NET and Silverlight applications require SIO_ADDRESS_LIST_CHANGE for interface change notifications
* ([Wine Bug #31858](http://bugs.winehq.org/show_bug.cgi?id=31858)) Netflix on Firefox fails with Internet Connection Problem when loading bar is at 99%
* ([Wine Bug #34406](http://bugs.winehq.org/show_bug.cgi?id=34406)) Finale Notepad 2012 doesn't copy/create user files on program start
* ([Wine Bug #17273](http://bugs.winehq.org/show_bug.cgi?id=17273)) Many apps and games need SetNamedPipeHandleState implementation (support for named pipe message mode)(FireFox+Flash, Win8/NET 4.x SDK/vcrun2012, WiX installers)
* ([Wine Bug #12401](http://bugs.winehq.org/show_bug.cgi?id=12401)) Support junction points, i.e. DeviceIoCtl(FSCTL_SET_REPARSE_POINT/FSCTL_GET_REPARSE_POINT)
* ([Wine Bug #5048](http://bugs.winehq.org/show_bug.cgi?id=5048)) Multiple applications and games need support for ws2_32 SIO_GET_EXTENSION_FUNCTION_POINTER TransmitFile (WSAID_TRANSMITFILE)
* ([Wine Bug #32323](http://bugs.winehq.org/show_bug.cgi?id=32323)) Netflix (Silverlight 4.x) and several .NET Framework 3.x/4.0 WPF apps require either Arial or Verdana to be installed
* ([Wine Bug #15980](http://bugs.winehq.org/show_bug.cgi?id=15980)) Rhapsody 2 crashes on startup (GetSecurityInfo returns NULL DACL for process object)
* ([Wine Bug #29903](http://bugs.winehq.org/show_bug.cgi?id=29903)) Some Microsoft debuggers fail to enumerate processes due to wtsapi32.WTSEnumerateProcessesW() being a stub (Microsoft Visual Studio 2005, DbgCLR from .NET 2.0 SDK)


Besides that the following additional changes are included:

* XEMBED support for embedding Wine windows inside Linux applications
* Support for PulseAudio backend for audio
* Support for GetVolumePathName
* Lockfree algorithm for filedescriptor cache (improves file access speed)
* Workaround for shlwapi URLs with relative paths
* Reduced SetTimer minimum value from 15 ms to 5 ms (improves Silverlight framerates)
* Other Pipelight specific enhancements

