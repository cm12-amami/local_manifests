# CM12.1

## How to build TWRP using cm-12.1-twrp branches:
```
make clean  
repo sync  
source build/envsetup.sh  
lunch cm_$device-eng  
make -jx recoveryimage  
```
Where $device is amami or z3c and x the number of CPU's
