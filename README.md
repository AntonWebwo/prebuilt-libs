# LIBZ 1.2.13
[http://www.zlib.net/](http://www.zlib.net/)   
  
**TARGETS**    
* linux-armhf (gcc-4.9)   
   
**BUILD LIBZ (linux-armhf)**   
Open "Ubuntu 18.04 LTS"   
```
git clone https://github.com/madler/zlib.git -b v1.2.13 --depth=1
export CROSS_COMPILE=arm-linux-gnueabihf-
export CC=arm-linux-gnueabihf-gcc-4.9
export AR=arm-linux-gnueabihf-gcc-ar-4.9
export RANLIB=arm-linux-gnueabihf-gcc-ranlib-4.9
cd zlib
CFLAGS="-fPIC" ./configure --static --prefix=$(pwd)/out
make && make install
```
   
Get files from zlib/out 
   
## ADDITIONAL LICENSE INFORMATION
   
**XCODE AND APPLE SDKS AGREEMENT**   
The instructions provided above indirectly reference the use of intellectual material that is the property of Apple, Inc.  This intellectual material is not FOSS (Free and Open Source Software) and by using it you agree to be bound by the terms and conditions set forth by Apple, Inc. in the [Xcode and Apple SDKs Agreement](https://www.apple.com/legal/sla/docs/xcode.pdf).
