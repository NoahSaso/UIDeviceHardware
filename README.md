UIDeviceHardware
================

Get the type of device your program is running on.

Code taken from: https://gist.github.com/Jaybles/1323251 (and some other unknown location which I forgot but I'm sure is great)

Modified to ease the process of incorporating into projects (git submodule, etc.).

I also added some more devices.

Usage
=====

```objc
#import "UIDeviceHardware.h"

NSString *platform = [UIDeviceHardware platform];
NSString *platformString = [UIDeviceHardware platformString];

// Device is iPad
if([platform rangeOfString:@"iPad"].location != NSNotFound) {
	NSLog([NSString stringWithFormat:@"Device is: %@", platformString]);
}else {
	NSLog(@"Device is not an iPad");
}
```
