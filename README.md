# Smart-Blinds
Make normal string Blinds smart using an ESP32 and a Servo Motor

### This config is for Homeassistant currently, but you could probably use arduino code or similar as well to control this.

### The Build instructions are below, The code for an ESP32 and an ESP8266 are yaml files for ESPHome.

## Build Instructions:
- Buy an esp32 or esp8266, and a servo. Here are the links (non-affiliate):

[ESP32 - Amazon](https://www.amazon.com/ESP-WROOM-32-Development-Microcontroller-Integrated-Compatible/dp/B08D5ZD528/ref=sr_1_3?crid=2Q4D8H26THTUZ&dib=eyJ2IjoiMSJ9.XBINg-sjhfF_gUtnMiKGjiaUVHZzlth3MSG3HA94qR_-kqokqweLRBdfmyBPh-86Mt8noI2L5vTV1s1tN4sPNIG1cyDPkht7ifMeDQ1IDXo79iIS77LZtZbpMFcHsMQKDa6FOHn1xN28rNfC_hrJ4gBdUQEnwVngkVqyhTGaoDY8bz1oqBjB9momXC--vevjJiNF33y2S8AFlE30iIb7cGJ2DQsiVh4ujhhrqXIxA4g.PlpdDZ1oZ9Nf8q1NzM3jKrD_1hRGygzUFIaNNKXwc0o&dib_tag=se&keywords=esp32&qid=1766063752&sprefix=esp3%2Caps%2C159&sr=8-3)

[ESP8266 - Amazon](https://www.amazon.com/Hosyond-Wireless-Development-Compatible-Micropython/dp/B09SPWYS4B/ref=sr_1_5?crid=279RRF20TOKRX&dib=eyJ2IjoiMSJ9.gJShu3rQeKD8EK_mYUdf6X_pH-K5K_92i8HvzqK1FLfFdVL7VG5uZKo7qls8mvAKpXfuRwAT7t4CUjPP9FVe4g5YJ1QEEvuTtAwUl-Pv1QmUeqK-brL16z6dzfhnw-bnPmizaDch9_bE1EPuRG5cgaNiAYmAgvzz6SNYHTJ3bZC5lkyu9BSs7U2-SaLc_UNrzECpFzldrcFbK4Z9PFY5CaSu3MGvt8rGwbf3kA9SYOY.UEdLThGfA2mXoLH83AEBReHlo8Yzah_lKXgrk_qspu0&dib_tag=se&keywords=esp8266&qid=1766063849&sprefix=esp8266%2Caps%2C147&sr=8-5&th=1)

[Servo Motor - Amazon](https://www.amazon.com/KOOKYE-360-Continuous-Rotation-Helicopter/dp/B01HSX1IDE/ref=sr_1_6?crid=2UTA7T34HESQB&dib=eyJ2IjoiMSJ9.BIphb0xR3DJDSX1mn8BPEaa9Xnp5qxxcUTred9Ogz0VjYLMMelYVI8qqNbHHT_i1z7hhg5CNVze5cQSK7lTb0MnvDYdql5dFCi7akkG02leU5sLlfdtgwfPPNR_A1HJ0parpTVSb4ANDQehD-JaG02AoeXjbicmWtw-yJEGHz96sH1tDjTx-N3vG5smJOszNKf9RE9rQ1iA3FyCtNw5zeApX_s6h3bT3v6L7ZPArdKU2u6JiEAjcaVwFdGRCfdgm6BwdZZbiOuCOpyu4FX1JtoLcgCcu1gwnNz3MHdHyH8Y.kQJC6yFKMwZQ5vKQDB7crR4T56kqcF4QEe3sBnOrXeI&dib_tag=se&keywords=mini%2Bservo%2Bmotor%2Bmetal%2Bgear%2Bkookye&qid=1766063963&sprefix=mini%2Bservo%2Bmotor%2Bmetal%2Bgear%2Bkookye%2Caps%2C109&sr=8-6&th=1)

- You will also need some wires, depending on how you plan to wire this (solder or pin connectors)

# Step 1:
- Connect the red wire from the servo to the VIN (5v) pin on the ESP
- Connect the white wire to pin D1 on the ESP8266 or pin D22 on the ESP32 (These can be changed if you are willing to edit the code)
- Connect the black wire to the GND (Ground) pin on the ESP

# Step 2
- Flash the ESP with ESPhome using Homeassistant or https://web.esphome.io/
- Use the file I have provided based on your board, you should only need the code after the line "captive_portal:", everything else should already be there, with your credentials

# Step 3
- 3D print the spool.stl file, and attach it to the motor using hotglue or any other method you prefer
- Use the reference image if confused
- Attach everything close to your window, and spool the strings as shown in the final.png image.
