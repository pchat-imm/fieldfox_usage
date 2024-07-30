# fieldfox_usage
**date:** 30/07/2024 \
**purpose:** note down how to use the [Fieldfox N9950B](https://www.keysight.com/us/en/product/N9950B/fieldfox-b-handheld-microwave-analyzer-32-ghz.html) \

## Connect LAN between notebook and FieldFox N9950B 
open the `control panel` and set IPV4 information as below
```
IP address: 192.168.0.54
Subnet mask: 255.255.255.0
default GW: 157.56.104.1
```

https://github.com/user-attachments/assets/b3b2bdb0-9cfb-4886-9579-7a024ba983d1

then to display on the notebook, open the application `Keysight Fieldfox Remote Display` to connect to the equipment. You can choose `front panel` and `front panel click` to interact with the equipment directly from the notebook.

https://github.com/user-attachments/assets/c5deb68b-42aa-447f-8d81-fcf7deba2713

## Mechanical Calibration of the Equipment
we used two calibration kit
- **Anritsu Calibration Kit TOSLKF50A-20** Type K(f) DC to 20 GHz, 50 ohm
- **Keysight Cal Kit 85561A 2.92 mm (f)** DC to 40 GHz \
<img src="https://github.com/user-attachments/assets/0c624a26-e56e-4f4e-a71d-0cc1663c34f6" width="50%" height="auto">
### for S11
- set start and stop frequency
- go to calibrate, select `mechanical calibrate' and choose `2.92 mm, female, 85561A` for `1 port OSL`\
<img src="https://github.com/user-attachments/assets/67c194c4-85f8-4f06-8bd1-dfe09f3298b6" width="50%" height="auto">

https://github.com/user-attachments/assets/2e666ab5-0949-46f3-9aad-2c744720c755

https://github.com/user-attachments/assets/1e4d8da5-94c7-4b52-9488-e4257f6c8010



### for S21
- set start and stop frequency
- go to calibrate, select `mechanical calibrate' and for both port choose `2.92 mm, female, 85561A` for `2 port SOLT`\
<img src="https://github.com/user-attachments/assets/f8985a41-77ed-4ad0-8d39-cec1fe30c87c" width="50%" height="auto">


