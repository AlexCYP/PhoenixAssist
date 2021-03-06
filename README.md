# Phoenix Assist
 This app simplifies the process of using Phoenix Miner, by dividing it into pieces. This app is a command-line and gui application which works on Linux and Windows.
 
 
 
 
### Dependencies
 [Python 3](https://www.python.org/downloads/) (and add it to PATH)
 
 [Phoenix Miner](https://phoenixminer.org/) (and add it to PATH)
 
 *Nix based Dependenies (Linux, Mac)
 
 [GNU Nano](https://www.nano-editor.org/)
 
 ## Install Script
 
 Download the install script from [here](https://github.com/MadRoadStudio/Phoenix-Assist/releases/latest/download/install.sh).
 
 ## Manual Installation
 
 > On Debian (and Debian-based systems), Read [this](https://github.com/ubden/Miner-Phoenixminer/blob/main/Linux-Ubuntu.md) (Note, this guide also includes installing propiatery amdgpu-pro drivers) 
 
 > On Arch (and Arch-based systems), download from [Pacman](https://aur.archlinux.org/packages/phoenixminer/) ([Binary](https://aur.archlinux.org/packages/phoenixminer-bin/))

### Drivers
**MAKE SURE THAT YOU HAVE THE RIGHT DRIVERS INSTALLED, OR IT WILL NOT WORK**

Linux
|GPU Maker|Driver Software|Does it work?|
|---|---|---|
|Neutral|[opengl-mesa](https://archlinux.org/packages/extra/x86_64/opencl-mesa/) |Untested, unlikely to work|
|NVIDIA|[opencl-nvidia](https://archlinux.org/packages/extra/x86_64/opencl-nvidia/)|Yes, under Cuda**|
|AMD|[opengl-amd](https://aur.archlinux.org/packages/opencl-amd/) |Yes, under OpenGL**|
|Intel|[beignet](https://aur.archlinux.org/packages/beignet/) |Untested, unlikely to work|
|Intel|[intel-compute-runtime](https://archlinux.org/packages/?name=intel-compute-runtime) |Untested, could work|
|Intel|[intel-opencl](https://aur.archlinux.org/packages/intel-opencl/) |Untested, unlikely to work|
|Intel|[intel-opencl-runtime](https://aur.archlinux.org/packages/intel-opencl-runtime/) |Untested, unlikely to work|

*note, these names are based off arch linux's packages and the data is based off [DaVinci Resolve's](https://wiki.archlinux.org/title/DaVinci_Resolve#Installation) OpenGL / Cuda compatibillity*
 
 ** Under propiatery drivers

 * AMD: [xf86-video-amdgpu](https://archlinux.org/packages/extra/x86_64/xf86-video-amdgpu/) and ([amdpro-gpu-libgl](https://aur.archlinux.org/packages/amdgpu-pro-libgl/) or [amdgpu-pro](https://aur.archlinux.org/pkgbase/amdgpu-pro-installer))

 * NVIDIA: [nvidia](https://archlinux.org/packages/extra/x86_64/nvidia/) and [nvidia-utils](https://archlinux.org/packages/extra/x86_64/nvidia-utils/)

 ### Add Phoenix Miner to PATH or locate the file
 
 #### PATH:
 Locate Phoenix Miner and get it's path.
 
 * [Linux](https://linuxize.com/post/how-to-add-directory-to-path-in-linux/#adding-a-directory-to-your-path) 
 
 (note: add the file, not the whole directory)
 
 #### LOCATE:

 Open settings.json and change pm_path to the directory of PhoenixMiner (not the file, only the directory holding the file).

 ### Installation of Phoenix Assist
 Clone the Git repository, and open the mine.py file.

 #### Optional
 Add the "bin" folder to [Path](https://linuxize.com/post/how-to-add-directory-to-path-in-linux/#adding-a-directory-to-your-path) 

 ## Why?
 I made a similar program a while ago, but accidentally deleted it off of my computer. So, i rewrote it in Python and made it open source.

 ## Fees
 We do not have fees, but Phoenix Miner takes a 0.65% fee.
 
 ## TO DO
* GUI App (inside here, but unfinished)
* Inplement issetup
