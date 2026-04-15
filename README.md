# obs-arm64

Run OBS on an ARM device running Linux.

⚠️ If you're using Windows on your device, an official build already exists: https://github.com/obsproject/obs-studio/releases .

How to use this project:

1. Open a terminal and type all these commands in the correct order:

`sudo apt update && sudo apt upgrade`
`sudo apt install wget`
`wget https://github.com/Nb1X/obs-arm64/releases/download/v32.1.1/install.sh`
`chmod +x install.sh`
`./install.sh`

Then, the script will do everything for you.

2. To run OBS, run `obs`. If you get an error "Failed to initialize video. Your GPU may not be supported, or your graphics drivers may need to be updated." it's because your GPU doesn't support OpenGL 3.3 or more. Try running OBS with this command instead: `MESA_GL_VERSION_OVERRIDE=3.3 obs`.

If you get errors or issues, you can open an issue, or go in Discussions and open a discussion.
