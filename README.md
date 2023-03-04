# Waveshare-DSI-LCD

#Step 1: Download and enter the Waveshare-DSI-LCD driver folder

```html
git clone https://github.com/waveshare/Waveshare-DSI-LCD
```

```html
cd Waveshare-DSI-LCD
```

#Step 2: Enter uname -a in the terminal to view the kernel version and cd to the corresponding file directory

#5.10.103 then run the following command

```html
cd 5.10.103
```

#Step 3: Please check the bits of your system, enter the 32 directory for 32-bit systems, and enter the 64 directory for 64-bit systems

```html
cd 32
```
#cd 64

#Step 4: Enter your corresponding model command to install the driver, pay attention to the selection of the I2C DIP switch

#2.8inch DSI LCD 480×640:

```html
sudo bash ./WS_xinchDSI_MAIN.sh 2_8INCH I2C0
```
#4inch DSI LCD 480×800:

```html
sudo bash ./WS_xinchDSI_MAIN.sh 4INCH I2C0
```
#7inch DSI LCD (C) 1024×600: 

```html
sudo bash ./WS_xinchDSI_MAIN.sh 7INCH I2C0
```
  ## Note to Use I2C0 you must solder two resistors in the figure below with 0 ohm resistance
  
  ![Solder Jumpers](https://github.com/Musicislife6984/Waveshare-DSI-LCD/blob/main/7inch_DSI_LCD_C_FAQ_1.png)
  
#7.9ich DSI LCD 400×1280:

```html
sudo bash ./WS_xinchDSI_MAIN.sh 7_9_INCH I2C0
```
#11.9inch DSI LCD 320×1480:

```html
sudo bash ./WS_xinchDSI_MAIN.sh 11_9_INCH I2C0
```

#Step 5: Wait for a few seconds, when the driver installation is complete and no error is prompted, restart and load the DSI driver and it can be used normally
sudo reboot

Note: The above steps need to ensure that the Raspberry Pi can be connected to the Internet normally.
