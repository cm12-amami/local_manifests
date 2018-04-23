# CM-14.1

## This is work in progress

build 
cd ~/where/you want
repo init -u https://github.com/LineageOS/android.git -b cm-14.1
cd .repo
git clone https://github.com/cm12-amami/local_manifests 
cd local_manifests 
git checkout cm-14.1 
cd ../.. 
repo sync
source build/envsetup.sh
export USE_CCACHE=1
ccache -M 50G
export CCACHE_COMPRESS=1
export ANDROID_JACK_VM_ARGS="-Dfile.encoding=UTF-8 -XX:+TieredCompilation -Xmx4G"
croot
brunch amami






