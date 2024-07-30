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

## Mechanical Calibration for NA
we used two calibration kits to calibrate for mode `Network Analyzer (NA)`
- **Anritsu Calibration Kit TOSLKF50A-20** Type K(f) DC to 20 GHz, 50 ohm
- **Keysight Cal Kit 85561A 2.92 mm (f)** DC to 40 GHz \
<img src="https://github.com/user-attachments/assets/0c624a26-e56e-4f4e-a71d-0cc1663c34f6" width="50%" height="auto">
### for S11
- select mode `NA`
- select `measurement` as `S11`
- set start and stop frequency
- go to calibrate, select `mechanical calibrate' and choose `2.92 mm, female, 85561A` for `1 port OSL`\
<img src="https://github.com/user-attachments/assets/67c194c4-85f8-4f06-8bd1-dfe09f3298b6" width="50%" height="auto">

https://github.com/user-attachments/assets/2e666ab5-0949-46f3-9aad-2c744720c755

https://github.com/user-attachments/assets/1e4d8da5-94c7-4b52-9488-e4257f6c8010

### for S21
- select mode `NA`
- select `measurement` as `S21`
- set start and stop frequency
- go to calibrate, select `mechanical calibrate' and for both port choose `2.92 mm, female, 85561A` for `2 port SOLT`\
<img src="https://github.com/user-attachments/assets/f8985a41-77ed-4ad0-8d39-cec1fe30c87c" width="50%" height="auto">

## example use case
### 0. benchmark 
- **good S11 should be below -20 dB**
- **good S21 should be below 0 dB**
- example of correct S11
<img src="https://github.com/user-attachments/assets/77e9ae14-9868-4198-9b4c-3cb8543c857c" width="50%" height="auto">

- wrong S11 setup, require repeat of calibration
<img src="https://github.com/user-attachments/assets/a2639f6a-cad2-456f-a778-0a73477d96d8" width="50%" height="auto">


### 1. Measure S21 and S11 of 4 cables to see if the cables are working or not
- test setup 
<img src="https://github.com/user-attachments/assets/10d44e02-5fd9-4873-90fb-fb2fb0aabe92" width="30%" height="auto">

- result S21 
<img src="https://github.com/user-attachments/assets/b90fa60a-673d-49ae-95dc-6ff855316532" width="50%" height="auto">

- result S11 
<img src="https://github.com/user-attachments/assets/3f6ebcb8-2fac-4735-8de5-a0482ed08d20" width="50%" height="auto">

- weird S11 result 
<img src="https://github.com/user-attachments/assets/7fb1a55f-db1b-4dcd-b76a-d73d23bad345" width="50%" height="auto">


