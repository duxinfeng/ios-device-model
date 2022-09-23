# ios-device-model

```objective-c
#import <sys/utsname.h>

// https://www.theiphonewiki.com/wiki/Models

+ (NSString *)devicePlatform
{
  
  struct utsname systemInfo;
  uname(&systemInfo);
  NSString *platform = [NSString stringWithCString:systemInfo.machine encoding:NSUTF8StringEncoding];
    
  //iPhone
  if ([platform isEqualToString:@"iPhone1,1"])    return @"iPhone 1G";
  if ([platform isEqualToString:@"iPhone1,2"])    return @"iPhone 3G";
  if ([platform isEqualToString:@"iPhone2,1"])    return @"iPhone 3GS";
  if ([platform isEqualToString:@"iPhone3,1"])    return @"iPhone 4";
  if ([platform isEqualToString:@"iPhone3,2"])    return @"iPhone 4";
  if ([platform isEqualToString:@"iPhone4,1"])    return @"iPhone 4S";
  if ([platform isEqualToString:@"iPhone5,1"])    return @"iPhone 5";
  if ([platform isEqualToString:@"iPhone5,2"])    return @"iPhone 5";
  if ([platform isEqualToString:@"iPhone5,3"])    return @"iPhone 5C";
  if ([platform isEqualToString:@"iPhone5,4"])    return @"iPhone 5C";
  if ([platform isEqualToString:@"iPhone6,1"])    return @"iPhone 5S";
  if ([platform isEqualToString:@"iPhone6,2"])    return @"iPhone 5S";
  if ([platform isEqualToString:@"iPhone7,1"])    return @"iPhone 6 Plus";
  if ([platform isEqualToString:@"iPhone7,2"])    return @"iPhone 6";
  if ([platform isEqualToString:@"iPhone8,1"])    return @"iPhone 6S";
  if ([platform isEqualToString:@"iPhone8,2"])    return @"iPhone 6S Plus";
  if ([platform isEqualToString:@"iPhone8,4"])    return @"iPhone SE";
  if ([platform isEqualToString:@"iPhone9,1"])    return @"iPhone 7";
  if ([platform isEqualToString:@"iPhone9,3"])    return @"iPhone 7";
  if ([platform isEqualToString:@"iPhone9,2"])    return @"iPhone 7 Plus";
  if ([platform isEqualToString:@"iPhone9,4"])    return @"iPhone 7 Plus";
  if ([platform isEqualToString:@"iPhone10,1"])   return @"iPhone 8";
  if ([platform isEqualToString:@"iPhone10.4"])   return @"iPhone 8";
  if ([platform isEqualToString:@"iPhone10,2"])   return @"iPhone 8 Plus";
  if ([platform isEqualToString:@"iPhone10,5"])   return @"iPhone 8 Plus";
  if ([platform isEqualToString:@"iPhone10,3"])   return @"iPhone X";
  if ([platform isEqualToString:@"iPhone10,6"])   return @"iPhone X";
  if ([platform isEqualToString:@"iPhone11,2"])   return @"iPhone XS";
  if ([platform isEqualToString:@"iPhone11,4"])   return @"iPhone XS Max";
  if ([platform isEqualToString:@"iPhone11,6"])   return @"iPhone XS Max";
  if ([platform isEqualToString:@"iPhone11,8"])   return @"iPhone XR";
	if ([platform isEqualToString:@"iPhone12,1"])   return @"iPhone 11";
	if ([platform isEqualToString:@"iPhone12,3"])   return @"iPhone 11 Pro";
	if ([platform isEqualToString:@"iPhone12,5"])   return @"iPhone 11 Pro Max";
	if ([platform isEqualToString:@"iPhone12,8"])   return @"iPhone SE 2";
	if ([platform isEqualToString:@"iPhone13,1"])   return @"iPhone 12 mini";
	if ([platform isEqualToString:@"iPhone13,2"])   return @"iPhone 12";
  if ([platform isEqualToString:@"iPhone13,3"])   return @"iPhone 12 Pro";
	if ([platform isEqualToString:@"iPhone13,4"])   return @"iPhone 12 Pro Max";
	if ([platform isEqualToString:@"iPhone14,4"])   return @"iPhone 13 mini";
  if ([platform isEqualToString:@"iPhone14,5"])   return @"iPhone 13";
	if ([platform isEqualToString:@"iPhone14,2"])   return @"iPhone 13 Pro";
	if ([platform isEqualToString:@"iPhone14,3"])   return @"iPhone 13 Pro Max";
  if ([platform isEqualToString:@"iPhone14,7"])   return @"iPhone 14";
	if ([platform isEqualToString:@"iPhone14,7"])   return @"iPhone 14 Plus";
	if ([platform isEqualToString:@"iPhone15,2"])   return @"iPhone 14 Pro";
	if ([platform isEqualToString:@"iPhone15,2"])   return @"iPhone 14 Pro Max";


  // iPod
  if ([platform isEqualToString:@"iPod1,1"])      return @"iPod Touch 1G";
  if ([platform isEqualToString:@"iPod2,1"])      return @"iPod Touch 2G";
  if ([platform isEqualToString:@"iPod3,1"])      return @"iPod Touch 3G";
  if ([platform isEqualToString:@"iPod4,1"])      return @"iPod Touch 4G";
  if ([platform isEqualToString:@"iPod5,1"])      return @"iPod Touch 5G";
  if ([platform isEqualToString:@"iPod7,1"])      return @"iPod Touch 6G";
	if ([platform isEqualToString:@"iPod9,1"])      return @"iPod Touch 7";

	
  // iPad
  if ([platform isEqualToString:@"iPad1,1"])      return @"iPad 1";
  if ([platform isEqualToString:@"iPad2,1"])      return @"iPad 2 (WiFi)";
  if ([platform isEqualToString:@"iPad2,2"])      return @"iPad 2 (GSM)";
  if ([platform isEqualToString:@"iPad2,3"])      return @"iPad 2 (CDMA)";
  if ([platform isEqualToString:@"iPad2,4"])      return @"iPad 2 (32nm)";
  if ([platform isEqualToString:@"iPad2,5"])      return @"iPad mini (WiFi)";
	if ([platform isEqualToString:@"iPad2,6"])      return @"iPad mini (GSM)";
	if ([platform isEqualToString:@"iPad2,7"])      return @"iPad mini (CDMA)";
  if ([platform isEqualToString:@"iPad3,1"])      return @"iPad 3 (WiFi)";
  if ([platform isEqualToString:@"iPad3,2"])      return @"iPad 3 (CDMA)";
  if ([platform isEqualToString:@"iPad3,3"])      return @"iPad 3 (GSM)";
  if ([platform isEqualToString:@"iPad3,4"])      return @"iPad 4 (WiFi)";
  if ([platform isEqualToString:@"iPad3,5"])      return @"iPad 4 (GSM)";
  if ([platform isEqualToString:@"iPad3,6"])      return @"iPad 4 (CDMA)";
  if ([platform isEqualToString:@"iPad4,1"])      return @"iPad Air (WiFi)";
  if ([platform isEqualToString:@"iPad4,2"])      return @"iPad Air (Cellular)";
  if ([platform isEqualToString:@"iPad4,3"])      return @"iPad Air (China)";
	if ([platform isEqualToString:@"iPad4,4"])      return @"iPad mini 2 (WiFi)";
	if ([platform isEqualToString:@"iPad4,5"])      return @"iPad mini 2 (Cellular)";
	if ([platform isEqualToString:@"iPad4,6"])      return @"iPad mini 2 (China)";
	if ([platform isEqualToString:@"iPad4,7"])      return @"iPad mini 3 (WiFi)";
	if ([platform isEqualToString:@"iPad4,8"])      return @"iPad mini 3 (Cellular)";
	if ([platform isEqualToString:@"iPad4,9"])      return @"iPad mini 3 (China)";
	if ([platform isEqualToString:@"iPad5,1"])      return @"iPad mini 4 (WiFi)";
	if ([platform isEqualToString:@"iPad5,2"])      return @"iPad mini 4 (Cellular)";
  if ([platform isEqualToString:@"iPad5,3"])      return @"iPad Air 2 (WiFi)";
  if ([platform isEqualToString:@"iPad5,4"])      return @"iPad Air 2 (Cellular)";
	if ([platform isEqualToString:@"iPad6,3"])      return @"iPad Pro 9.7 (WiFi)";
	if ([platform isEqualToString:@"iPad6,4"])      return @"iPad Pro 9.7 (Cellular)";
	if ([platform isEqualToString:@"iPad6,7"])      return @"iPad Pro 12.9 (WiFi)";
	if ([platform isEqualToString:@"iPad6,8"])      return @"iPad Pro 12.9 (Cellular)";
	if ([platform isEqualToString:@"iPad6,11"])     return @"iPad (5th generation)";
	if ([platform isEqualToString:@"iPad6,12"])     return @"iPad (5th generation)";
	if ([platform isEqualToString:@"iPad7,1"])      return @"iPad Pro (12.9-inch, 2nd generation)";
	if ([platform isEqualToString:@"iPad7,2"])      return @"iPad Pro (12.9-inch, 2nd generation)";
	if ([platform isEqualToString:@"iPad7,3"])      return @"iPad Pro (10.5-inch)";
	if ([platform isEqualToString:@"iPad7,4"])      return @"iPad Pro (10.5-inch)";
	if ([platform isEqualToString:@"iPad7,5"])      return @"iPad 6 (WiFi)";
	if ([platform isEqualToString:@"iPad7,6"])      return @"iPad 6 (Cellular)";
	if ([platform isEqualToString:@"iPad7,11"])     return @"iPad 7";
	if ([platform isEqualToString:@"iPad7,12"])     return @"iPad 7";
	if ([platform isEqualToString:@"iPad8,1"])      return @"iPad Pro 11-inch (WiFi)";
	if ([platform isEqualToString:@"iPad8,2"])      return @"iPad Pro 11-inch (WiFi, 1TB)";
	if ([platform isEqualToString:@"iPad8,3"])      return @"iPad Pro 11-inch (Cellular)";
	if ([platform isEqualToString:@"iPad8,4"])      return @"iPad Pro 11-inch (Cellular, 1TB)";
	if ([platform isEqualToString:@"iPad8,5"])      return @"iPad Pro 12.9-inch 3 (WiFi)";
	if ([platform isEqualToString:@"iPad8,6"])      return @"iPad Pro 12.9-inch 3 (WiFi, 1TB)";
	if ([platform isEqualToString:@"iPad8,7"])      return @"iPad Pro 12.9-inch 3 (Cellular)";
	if ([platform isEqualToString:@"iPad8,8"])      return @"iPad Pro 12.9-inch 3 (Cellular, 1TB)";
	if ([platform isEqualToString:@"iPad8,9"])      return @"iPad Pro 2 (11-inch) ";
	if ([platform isEqualToString:@"iPad8,10"])     return @"iPad Pro 2 (11-inch) ";
	if ([platform isEqualToString:@"iPad8,11"])     return @"iPad Pro 4 (12.9-inch) ";
	if ([platform isEqualToString:@"iPad8,12"])     return @"iPad Pro 4 (12.9-inch) ";
	if ([platform isEqualToString:@"iPad11,1"])     return @"iPad mini 5";
	if ([platform isEqualToString:@"iPad11,2"])     return @"iPad mini 5";
	if ([platform isEqualToString:@"iPad11,3"])     return @"iPad Air 3";
	if ([platform isEqualToString:@"iPad11,4"])     return @"iPad Air 3";
	if ([platform isEqualToString:@"iPad11,6"])     return @"iPad 8";
	if ([platform isEqualToString:@"iPad11,7"])     return @"iPad 8";
	if ([platform isEqualToString:@"iPad12,1"])     return @"iPad 9";
	if ([platform isEqualToString:@"iPad12,2"])     return @"iPad 9";
	if ([platform isEqualToString:@"iPad13,1"])     return @"iPad Air 4";
	if ([platform isEqualToString:@"iPad13,2"])     return @"iPad Air 4";
	if ([platform isEqualToString:@"iPad13,4"])     return @"iPad Pro 4 (11-inch) ";
	if ([platform isEqualToString:@"iPad13,5"])     return @"iPad Pro 4 (11-inch) ";
	if ([platform isEqualToString:@"iPad13,6"])     return @"iPad Pro 4 (11-inch) ";
	if ([platform isEqualToString:@"iPad13,7"])     return @"iPad Pro 4 (11-inch) ";
	if ([platform isEqualToString:@"iPad13,8"])     return @"iPad Pro 5 (12.9-inch) ";
	if ([platform isEqualToString:@"iPad13,9"])     return @"iPad Pro 5 (12.9-inch) ";
	if ([platform isEqualToString:@"iPad13,10"])    return @"iPad Pro 5 (12.9-inch) ";
	if ([platform isEqualToString:@"iPad13,11"])    return @"iPad Pro 5 (12.9-inch) ";
	if ([platform isEqualToString:@"iPad14,1"])     return @"iPad mini 6";
	if ([platform isEqualToString:@"iPad14,2"])     return @"iPad mini 6";
	
	
  // Simulator
  if ([platform isEqualToString:@"i386"])         return @"iPhone Simulator";
  if ([platform isEqualToString:@"x86_64"])       return @"iPhone Simulator";
    
  return platform;
}

```

