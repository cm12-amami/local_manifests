# CM12.1

## How launch a cm-12.1 build:
```Shell session
make clean  
repo sync  
source build/envsetup.sh  
brunch amami  
```

## How to initially set up your build tree:
```Shell session
repo init -u https://github.com/cm12-amami/android.git -b cm-12.1 
cd .repo
git clone https://github.com/cm12-amami/local_manifests 
cd local_manifests 
git checkout cm-12.1-sepol
cd ../.. 
repo sync
```

## About this variant
Enhanced SELinux policy to prevent nosy apps from spying and recording, which sites each app is connecting to.
You need to add the following line to you local mainfest in addition:
```  
<project name="MSe1969/privacy-friendly-netmonitor-prebuilt" 
           path="external/secuso/privacy-friendly-netmonitor-prebuilt" 
           revision="master" clone-depth="1" />
```
