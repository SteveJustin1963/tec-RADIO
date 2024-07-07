# tec-RADIO

## AM RX
* https://easyeda.com/editor#id=b322a52f432c4eeeb62464f889dc4683
* http://tinyurl.com/y7llys4e

![](https://github.com/SteveJustin1963/tec-RADIO/blob/master/AM%20RX/am%20regen%20tec1%20hack.png)

![image](https://github.com/SteveJustin1963/tec-RADIO/assets/58069246/0319494f-4f6e-4f2a-b9cc-01d123fc666f)



## parts
* https://www.google.com/search?q=ferrite+antenna
* https://www.aliexpress.com/item/4000666271308.html

## AM TX
* http://tinyurl.com/yamgnxn2

![](https://github.com/SteveJustin1963/tec-RADIO/blob/master/AM%20TX/et-fone-home.png)

## SPARK TX

"Scott Gregory So where does the spark gap and Morse key fit into all this? 😂 
Will we also need a rotary converter to power the TEC? 😂
" Ken Stone Rotary converter? Sure, I have a couple of those. http://fav.me/d2bh811

* https://easyeda.com/editor#id=2cb44aecf83f4266a0655c89954175fc


## Pixie
- https://www.qsl.net/vu2awc/ham_radio_india_p/Pixie/iitckt.JPG
- frog
- 2W
- 

![image](https://github.com/SteveJustin1963/tec-RADIO/assets/58069246/e10f939f-c27b-4454-b8e1-4222af0579db)

## PWM to Sine
- https://en.wikipedia.org/wiki/Pulse-width_modulation
- class E PA
- 

## DDS
### AD9850 DDS Signal Generator Module
![image](https://github.com/SteveJustin1963/tec-RADIO/assets/58069246/2de4c1d4-d60e-4c46-8252-35680b54d5eb)

![image](https://github.com/SteveJustin1963/tec-RADIO/assets/58069246/264ad808-bcbd-4021-a949-a04bd0da0a37)

https://telecnatron.com/articles/Variable-Gain-Amplifier-For-AD9850-DDS/index.html
 

![image](https://github.com/SteveJustin1963/tec-RADIO/assets/58069246/3348f0d2-9439-44dc-8f3e-dfa1475aad72)




To set the frequency of the AD9850 to 7.023 MHz, you need to calculate the 32-bit frequency tuning word using the following formula:

![image](https://github.com/SteveJustin1963/tec-RADIO/assets/58069246/68fa6300-6c53-4fc4-bfbd-4cfb4b5e41fd)


So, the frequency word in bytes is: 0x80, 0xE9, 0x60, 0x0E (little-endian format).

code with the frequency word set for 7.023 MHz `ad9850_1.z80`

In this example:

0x80, 0xE9, 0x60, 0x0E are the 4 bytes representing the 32-bit frequency tuning word for 7.023 MHz.
0x00 is the control byte.
Make sure to adjust the DATA_PORT, W_CLK_PORT, FU_UD_PORT, and RESET_PORT to match the actual ports used in your hardware setup.
 
