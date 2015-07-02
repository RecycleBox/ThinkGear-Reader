# ThinkGear-Reader

Read the data from ThinkGear devices.

# Installation

git clone https://github.com/MakiseKurisu/ThinkGear-Reader.git
cd ThinkGear-Reader/
gcc -std=c99 bs.c -o bs

# Usage

hcitool scan
sdptool records HEADSET_MAC_ADDR
sudo rfcomm bind 0 HEADSET_MAC_ADDR 1
./bs /dev/rfcomm0 OUTPUT_FILE
