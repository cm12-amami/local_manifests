# CM12.1

## How launch a cm-12.1 build:
```
make clean  
repo sync  
source build/envsetup.sh  
brunch $device  
```
Where $device is amami or z3c

## How to initially set up your build tree:
```
repo init -u https://github.com/LineageOS/android.git -b cm-12.1 
cd .repo
git clone https://github.com/derfelot/local_manifests 
cd local_manifests 
git checkout cm-12.1 
cd ../../ 
repo sync
```
