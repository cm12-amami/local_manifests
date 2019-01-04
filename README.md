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
repo init -u https://github.com/cm12-amami/android.git -b cm-12.1 --groups=all,-notdefault,-darwin,-x86,-mips
cd .repo
git clone https://github.com/cm12-amami/local_manifests 
cd local_manifests 
git checkout cm-12.1 
cd ../.. 
repo sync --no-tags
```
Note: If you use a MAC to build, omit the `-darwin` in above `repo init` statement.
