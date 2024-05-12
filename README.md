# KLV-BspwmCE

![Screenshot](https://github.com/sofijacom/KLV-BspwmCE/assets/107557749/10b99097-9983-4832-acb9-e09236b3c9fc)


# Assembly of KLV-BspwmCE

1) Create a folder `KLV-BspwmCE` typing in the terminal `mkdir -p KLV-BspwmCE`

2) Open a terminal in the created folder `KLV-BspwmCE` or go to the folder by typing in the terminal

   - `cd KLV-BspwmCE`

3) Place the build script  `FR_minimal_void_bspwm_rc5.sh` in the created folder.
   
4) Make it executable.`chmod +x FR_minimal_void_bspwm_rc5.sh`

5) Enter in terminal `./FR_minimal_void_bspwm_rc5.sh`

6) Wait for the build to finish.

7) After the build is complete to package `07firstrib_rootfs` into `07KLV-BspwmCE-x.x.sfs` where x.x is your build number.

8) Type in terminal.

```
mksquashfs 07firstrib_rootfs 07 KLV-Spectrwm-CE-x.x.sfs -noappend -comp xz -b 512k
```
  - where x.x is your build number.

9) Delete the `07firstrib_rootfs` folder.

##

FirstRib-KLV build script. 

```
./FR_minimal_void_bspwm_rc5.sh
```
FirstRib-KLV build script PLUG file.

Example of using a .plug file:

```
./build_firstrib_rootfs.sh void default amd64 f_00_Void_amd64_noXsimple00_sofiya-120rc5.plug
```

***f_00_Void_amd64_noXsimple00_sofiya-120rc5.plug***  builds a  ***(root filesystem)***  for the Void Linux-based Bspwm desktop operating system, similar to **KLV-BspwmCE**.

To create a complete distribution, all other utilities, tools and configurations are downloaded from a centralized repository and installed as a .tar.gz file.
