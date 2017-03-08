#IOS操作系统的层次结构

![](http://img0.tuicool.com/qEN7VnZ.jpg!web)

#1 - Cocoa Touch:
>Cocoa Touch层的框架提供了应用程序的基础架构。这些基础架构提供了集合、文件管理、网络操作等的面向对象支持。Cocoa Touch中最核心的部分是UIKit.Framework(UIKit框架)，它为呈现应用程序界面上的各种组件提供了支持。除此之外，该框架还负责处理屏幕上的多点触摸事件、文字的输出、图片和网页的显示、相机或文件的存取、加速感应的部分等。

#2 - Media
> Media(媒体)层提供了图片、音乐、影片、动画等多媒体功能。图像分为2D图像和3D图像，前者由Quartz2D来支持，后者则是由OpenGLES来支持；音乐是由Core Audio和OpenAL来支持；影片用Media Player来播放；动画由Core Animation来支持。

#3 - Core Services
>Core Services层在Core OS的基础上提供了更加丰富的功能，它包含了Foundation.Framework和Core Foundation.Framework(也就是一些基础的框架)。Core Services和Core OS一起，提供了苹果移动设备(如iPhone和iPad等)的基础接口，包括：用来访问文件的接口、底层数据类型的接口、Bonjour服务接口、网络接口等。值得一提的是，这些接口大多都是用C语言编写的。

#4 - Core OS (核心OS层) 
>Core OS层是用FreeBSD和Mach所改写的Darwin, 是开源、符合POSIX标准的一个Unix核心。
这一层提供了整个iOS的一些基础功能
包括：硬件驱动、内存管理、程序管理、线程管理(POSIX)、文件系统、网络(BSD Socket)，以及标准输入输出等。
此外，Core OS层的驱动也提供了硬件和系统框架之间的接口。


#1 - Cocoa Touch 触摸层： 基本都是基于 Objective-c的接口

**Address Book UI Framework**

**Event Kit UI Framework**

**Game Kit Framework**

**iAd Framework**

**Map Kit Framework**

**Message UI Framework**

**UIKit Framework**

-

###功能:
- multi-Touch
- Core Motion
- View Hierarchy
- Localization
- Controls
- Alerts
- Web View
- Map Kit
- Image Picker
- Camera

-
 
# 2 - Media
**Core Graphics**

**Core Animation**

**OpenGL ES**

**Core Text**

**Image I/O**

**Assets Library Framework**

**Media Player Framework**

**AV Foundation**

**OpenAL**

**Core Audio Frameworks**

**Core Media**

-

###功能:
- Core Audio
- OpenAL
- Audio Mixing
- Audio Recording
- Video Playback
- JPEG,PNG,TIFF
- PDF
- Quartz(2D)
- Core Animation
- OpenGL ES

-

#3 - Core Services 基于c语言的接口

**Address Book Framework**

**CFNetwork Framework**

**Core Data Framework**

**Core Foundation Framework**

**ore Location Framework**

**Core Media Framework**

**Core Telephony Framework**

**Event Kit Framework**

**Foundation Framework**

**Mobile Core Services Framework**

**Quick Look Framework**

**Store Kit Framework**

**System Configuration Framework**

**Block Objects**

**Grand Central Dispatch**

**In App Purchase**

**Location Services**

**SQLite**

**XML Support**

-

###功能:
- Collections
- Core Location
- Address Book
- Net Services
- Networking 
- Threading
- File Access
- Preferences
- SQLite
- URL Utilities

-

#4 - Core OS 基于c语言的接口
**Accelerate Framework**

**External Accessory Framework**

**Security Framewor**

**System**

-

###功能:
- OSX Kernel 
- Mach 3.0
- BSD 		
- Sockets 	    
- Security 		
- Power Management
- keychain Access
- Certificates
- File System 
- Bonjour 