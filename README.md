UIDeviceHardware
================

Get the type of device your program is running on.

Code taken from: https://gist.github.com/Jaybles/1323251 (and some other unknown location, I forgot...)

Re-made my Sassoty to implement into your projects. I also added on some more devices

Usage
=====

```objc
#import "UIDeviceHardware.h"

NSString *platform = [UIDeviceHardware platform];
NSString *platformString = [UIDeviceHardware platformString];

// Device is iPad
if([platform rangeOfString:@"iPad"].location != NSNoutFound) {
	NSLog([NSString stringWithFormat:@"Device is: %@", platformString]);
}else {
	NSLog(@"Device is not an iPad");
}
```
