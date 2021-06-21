
# Environments

OS:  
1.macOS Big Sur(11.5 Beta)  
2.Parallels(16.1.2)  
3.Ubuntu(18.04.01)  
  
Xilinx Tools:  
1.Vivado 2020.1  
2.Vitis:2020.1  
3.Petalinux:2020.3(I tried to use 2020.1, but there will be error about yocto when executing "petalinux-build", but 2020.3 can avoid that error)
  
Xilinx Hardware:  
1.xczu15eg
  
# Petalinux Installation  
1.Create Petalinux installation direction:  
```
sudo mkdir -p /tools/Xilinx/PetaLinux/2020.3/
```
2.Give this direction 755 permissions(making the folder globally read-execute):  
```
sudo chmod -R 755 /tools/Xilinx/PetaLinux/2020.3/
```
3.Give the Petalinux installer 777 permission:  
```
sudo chmod 777 ./Downloads/petalinux-v2020.3-final-installer.run
```
4.Change wonership of the directory you're installing Petalinux in to the user:  
```
sudo chown -R <user>:<user> /tools/Xilinx/PetaLinux/2020.3/
```
5.Run the PetaLinux installer(donot run the Petalinux installer as root(sudo) and donot move/copy any of Petalinux source file after installation):  
```
./Downloads/petalinux-v2020.3-final-installer.run /tools/Xilinx/PetaLinux/2020.3/
```
6.If there are some package missing, using following cmd to install it and redo step-5:  
```
sudo apt-get install <pkg-name>
```
7.Access the license of Xilinx during the installation
8.Open /home/<user_name>/.bashrc and append the following cmd in the end
```
source /tools/Xilinx/PetaLinux/2020.3/settings.sh
```

