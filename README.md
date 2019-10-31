# Building JW Boot Logo

JW Boot Logo uses 'stb' which is included as a git submodule in the
project.


```
# Clone JW Boot Logo
git clone https://github.com/jwatte/jw_boot_logo.git

# Pull in dependencies:
git submodule update --init

# Generate the configure script
./bootstrap

# Run the configure script
./configure

# Build the app:
make

# Optionally install
sudo make install
```

# Installing the Logo

A simple way to install the new logo is to copy it to the Jetson
device and then use `dd` to update the BMP partition.

```
scp bmp.blob nvidia@192.168.55.1:
ssh nvidia@192.168.55.1
sudo dd if=bmp.blob of=/dev/disk/by-partlabel/BMP
```
