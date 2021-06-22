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






