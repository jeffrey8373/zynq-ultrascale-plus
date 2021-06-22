# Vivado Project Setup

1.Create a project in Vivdao  
2.Click "Create Block Design" to create a new block design.  

<img width="500" height="300" src="https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_09-10-32.jpeg" align="center">  

3.Enter the "Design name" and click "ok" button  
<img width="250" height="200" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_09-24-42.jpeg>  

4.Click the "Add IP" button in the Diagram, then search "zynq", and select "Zynq UltraScale+ MPSoC"  

<img width="500" height="300" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_09-30-03.jpeg>  

5.Double click the ZYNQ IP in the block and start to configure parameters. The ZYNQ hardware architecture will show, ug1085 has detailed introductions for each part.  

<img width="500" height="300" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_09-31-54.jpeg>  

6.Low Speed Configuration(Please refer to your hardware design)  
6.1 Select "I/O Configuration" in the left side, configure the BANK0~BANK2's voltage according to your hardware design. Besides, configure the QSPI as the following picture shows  

<img width="500" height="400" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-07-41.jpeg>  

6.2 Configure SD0  
<img width="500" height="400" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_09-55-27.jpeg>  

6.3 Configure SD1  

<img width="250" height="200" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-11-16.jpeg>  

6.3 Configure CAN 0  

<img width="250" height="200" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-11-50.jpeg>  

6.4 Configure I2C 1, which is used fot EEPROM control  

<img width="250" height="200" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-12-16.jpeg>  

6.5 Configure UART 0  

<img width="250" height="200" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-13-09.jpeg>  

6.6 Select TTC 0 ~ TTC 3  

<img width="250" height="200" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-13-41.jpeg>  

7 High Speed Configuration  
7.1 Enternet Configuration  
<img width="250" height="200" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-14-11.jpeg>  

7.2 USB Configuration  
<img width="250" height="200" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-15-01.jpeg>  

7.3 PCIe Configuration  
<img width="250" height="200" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-16-25.jpeg>  

7.4 Click "Switch To Advanced Mode" and configure PCIe parameters as followling  
<img width="500" height="500" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-17-19.jpeg>  

7.5 Go back to "I/O Configuration", configure PCIe and Display Port  

<img width="300" height="300" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-18-05.jpeg>  

8 Clock configuration  
8.1 Select "Clock Configuration" in the left side, and configure "GT Lane Reference frequency"  

<img width="600" height="300" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-18-28.jpeg>  

8.2 Configure "Output Clocks"  
<img width="600" height="500" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-19-06.jpeg>  

8.3 Configure "PL Fabric Clocks"  
<img width="600" height="200" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-19-33.jpeg>  

8.4 Configure "Full Power Domain Clocks"  
<img width="600" height="300" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-20-08.jpeg>  

8.5 Interconnection configuration  
<img width="600" height="300" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-21-05.jpeg>  

9.DDR Configuration  

9.1 Select ”DDR4_MICRON_MT40A256M16GE_083E” in Load DDR Presets.  
<img width="500" height="400" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-22-38.jpeg>  

9.2 Change some parameters  
<img width="500" height="400" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-23-06.jpeg>  

10. The ZYNQ UltraScale+ IP configuration has finished  

11. Connect "pl_clk0" to "maxlhpm0_ldp_aclk"  
<img width="600" height="200" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_10-23-29.jpeg>  

12.Select Block design, right click "Create HDL Wrapper..." to create a wrapper for block design using verilog/VHDL  
<img width="250" height="250" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_11-27-35.jpeg>  

13.Keep default selection and click "OK"  
<img width="400" height="200" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_11-28-01.jpeg>  

14. Select block design, right click "Generate Output Products", which will generate a output file for block, it includs IP, instance model, RTL source file, XDC constraint, etc.  Then Click "Generate" button in the next setp  
<img width="300" height="300" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_11-28-38.jpeg>  

15. "File->export->Export Hardware" to expert hardware information, which include the PS configuration parameters.  

<img width="600" height="300" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_11-29-20.jpeg>  

16.There will be a .xsa file in your project  

<img width="250" height="200" src=https://github.com/jeffrey8373/zynq-ultrascale-plus/blob/main/petalinux/pictures/Xnip2021-06-22_11-38-32.jpeg>  



# Petalinux Setup

1.Create a petalinux project, named as "petalinux", which type is "project" and using "zynqMP" template  
`petalinux-create -t project -n petalinux --template zynqMP`

2.Using the following cmd to enter the petalinux dirextion  
`cd ./petalinux`

3.Configure the Petalinux hardware parameters, make sure there is only on .xsa file 
`petalinux-config --get-hw-description = ./../`

4.The configuration UI will show, configure it as the follwing picture shows and save the change, exit the UI and waiting for configureation finish


