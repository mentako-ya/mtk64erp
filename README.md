# mtk64erp

mtk64erp is homebrew keyboard with thumb operated trackball & rotary encoder.

<img src="image/mtk64erp_top.jpg" width="80%" style="border: 1px solid;"/>

<img src="image/mtk64erp_front.jpg" width="80%" style="border: 1px solid;"/>

<img src="image/mtk64erp_left.jpg" width="80%" style="border: 1px solid;"/>

<img src="image/mtk64erp_right.jpg" width="80%" style="border: 1px solid;"/>

<img src="image/mtk64erp_back.jpg" width="80%" style="border: 1px solid;"/><br>
undergrow LED

<img src="image/mtk64erp_thumb.jpg" width="80%" style="border: 1px solid;"/><br>
Extra thumb keyswitches are offset lower

<img src="image/mtk64erp_oled.jpg" width="80%" style="border: 1px solid;"/><br>
OLED 128X64, Leyer indicator LED, Reset button

<img src="image/mtk64erp_encoder.jpg" width="80%" style="border: 1px solid;"/><br>
Alps alpine low hight encoder, 30 click with push switch

<img src="image/mtk64erp_ballcase.jpg" width="80%" style="border: 1px solid;"/><br>
PMW3389 trackball sensor, Offset low to avoid interfering with keystrokes

<img src="image/mtk64erp_switches.jpg" width="80%" style="border: 1px solid;"/><br>
<a href="https://ja.aliexpress.com/item/1005007361067887.html"><img src="image/kailh_v2_deepsea.png" width="40%" style="border: 1px solid;"/></a>
<a href="https://ja.aliexpress.com/item/1005007404357477.html"><img src="image/kailh_v2_shadow.png" width="40%" style="border: 1px solid;"/></a><br>
Chock V1/ [V2 (with out fixed pin model)](https://ja.aliexpress.com/item/1005007361067887.html) / MX compatible key switch can be installed on all keys

<img src="image/cpi_test.png" width="80%" style="border: 1px solid;"/><br>
Higher polling rates with new qmk_firmware and RP2040 MCU

* Keyboard Maintainer: [mentako-ya](https://github.com/mentako-ya)
* Hardware Supported: 
    MCU     : RP2040
    OLED    : SSD1306 128X64 
    Trackball sensor : PMW3389
    Encoder : EC12D
* Hardware Availability: https://jp.mercari.com/search?keyword=mentako-ya

## Firmware
[mtk_mtk64erp_via.uf2](firmware/mtk_mtk64erp_via.uf2)

## via.json
[mtk64erp_via.json](firmware/mtk64erp_via.json)

### Source code
https://github.com/mentako-ya/qmk_firmware/tree/master/keyboards/mtk/mtk64erp

Make example for this keyboard (after setting up your build environment):

    qmk compile -kb mtk/mtk64erp -km via

Flashing example for this keyboard:

    qmk flash -kb mtk/mtk64erp -km via

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. 
Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

### Bootloader

Enter the bootloader in 2 ways:

* **Physical reset button**: Press the reset button twice briefly
* **Keycode in layout**: Press the key mapped to `QK_BOOT`

## Key mapping
You can change the key mapping using https://remap-keys.app/configure

 1. connect keyboard

    <img src="image/remap/remap_1.png" width="60%" style="border: 1px solid;"/>

    <img src="image/remap/remap_2.png" width="60%" style="border: 1px solid;"/>

 1. Upload [mtk64erp_via.json](firmware/mtk64erp_via.json)   

    <img src="image/remap/remap_3.png" width="60%" style="border: 1px solid;"/>

    <img src="image/remap/remap_4.png" width="60%" style="border: 1px solid;"/>
 
 1. Map any key to layers 0~7
* Layer 0       Normal key

    <img src="image/remap/remap_layer0.png" width="60%" style="border: 1px solid;"/>

* Layer 1       Equivalent to input with Shift key

    <img src="image/remap/remap_layer1.png" width="60%" style="border: 1px solid;"/>

* Layer 2       Mouse buttons, cursor keys

    <img src="image/remap/remap_layer2.png" width="60%" style="border: 1px solid;"/>

* Layer 3       Trackball settings(see cusom keycord), LED setting, Trackball is in scroll mode

    <img src="image/remap/remap_layer3.png" width="60%" style="border: 1px solid;"/>

* Layer 4..6    unused, any key code can be set

    <img src="image/remap/remap_layer4to6.png" width="60%" style="border: 1px solid;"/>

* Layer 7       Auto mouse layer

    <img src="image/remap/remap_layer7.png" width="60%" style="border: 1px solid;"/>

 ## Cusom keycode
    KBC_LOAD,       // Configuration load from EEPROM
    KBC_SAVE,       // Configuration save to EEPROM
    CPI_I100,       // CPI +100 CPI
    CPI_D100,       // CPI -100 CPI
    CPI_I1K,        // CPI +1000 CPI
    CPI_D1K,        // CPI -1000 CPI
    SCRL_TO,        // Toggle scroll mode ON/OFF
    SCRL_MO,        // Momentary scroll mode
    SCRL_INV,       // Invert scroll direction
    SCRL_DVI,       // Increment scroll divider
    SCRL_DVD,       // Decrement scroll divider
    AM_TG,          // Toggle auto mouse layer ON/OFF
    AM_TOUT_INC,    // Increment AUTO_MOUSE_TIME_OUT
    AM_TOUT_DEC,    // Decrement AUTO_MOUSE_TIME_OUT

## Case data
<img src="image/mtk64erp_render_enc1.png" width="40%" style="border: 1px solid;"/>
<img src="image/mtk64erp_render_ball1.png" width="40%" style="border: 1px solid;"/><br>
<img src="image/mtk64erp_render_enc2.png" width="40%" style="border: 1px solid;"/>
<img src="image/mtk64erp_render_ball2.png" width="40%" style="border: 1px solid;"/><br>

Case data download from [here](casedata/mtk64erp_STL)
