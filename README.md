# obs-arm64

OBS ARM64 is a project that allows you to install OBS v32.1.1 on an ARM SBC (Raspberry Pi, Orange Pi, etc.), an ARM laptop with Linux, or any other ARM device running Linux.

PS: If you are using Windows on ARM, an official OBS build already exists; you can download it [here](https://github.com/obsproject/obs-studio/releases/download/32.1.1/OBS-Studio-32.1.1-Windows-arm64.zip).

⚠️ WARNING: If you want to use this tool on a Raspberry Pi, make sure you have a cooling fan and/or a heatsink, and make sure you have enough space on your drive (~10-15GB) and make sure you're using a 64-bit version of Raspberry Pi OS! This tool is NOT made to run on 32-bit OSes.

This build also works with Raspberry Pi OS (Debian) Trixie (13)

Here's a short, simple tutorial on how to use my build:

1. Go to the releases section of this project.

2. Download the file "obs-v**version number**-install.sh".

3. Open a terminal and run the following commands:
`cd *file location*`
`chmod +x obs-v*version number*-install.sh`
`./obs-v*version number*-install.sh`

Then, the project will begin compiling everything necessary.

This build is specifically optimized for Raspberry Pi OS (Debian) Bookworm and the Raspberry Pi 5.

Here's what the .sh file does in detail:

1. It installs all the necessary libraries for compilation.

2. It compiles CMake 3.28.3 (required to compile OBS).

3. It compiles FFmpeg 7.0 (required for OBS to function correctly).

4. It compiles GLib 2.78 (required for PipeWire to work) in /opt without modifying system files.

5. Finally, it performs the last compilation: OBS Studio ARM64.

6. It creates a small, automatic launcher, which is handy for beginners.

To launch OBS, you will need to use this command: obs-run.

If you want to compile OBS yourself without using my project, you can find a tutorial online that explains how to do it, or ask on the official OBS Discord server.
