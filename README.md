Based on the cm11 source code to compile

cd cm

. build/envsetup.sh

make -j4 otatools

./build/tools/device/mkvendor.sh device_manufacturer_name device_name /your/path/to/the/boot.img
（such as
./build/tools/device/mkvendor.sh nubia NX507J ~/cm11/android/recovery.img
）

lunch cm_NX507J-eng

make -j4 recoveryimage

#build cwm_v6.0.5.1_cn for NUBIA NX507J ONLY
