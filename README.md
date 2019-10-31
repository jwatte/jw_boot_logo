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
