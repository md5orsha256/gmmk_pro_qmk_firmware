# [GMMK Pro][gmmk-pro] firmware by [@md5orsha256](https://github.com/md5orsha256/)

My repository for containing keymap for my GMMK pro keyboard and building in [actions pipelines](https://github.com/md5orsha256/gmmk_pro_qmk_firmware/actions)

## Current Keymap
### Layout 0
<img width="839" alt="image" src="https://user-images.githubusercontent.com/17884471/145017257-a8f3665a-4922-46f3-9d94-ff351132804e.png">

### Layout 1
<img width="844" alt="image" src="https://user-images.githubusercontent.com/17884471/145017403-1b7b7bc7-a66c-4244-ace0-f43267d2edb9.png">

## Update keymap

Afrer clonning this repository do follow steps:

 1. Go to [qmk configurator][qmk-config] page

 2. Click to upload JSON icon
    <img width="1893" alt="image" src="https://user-images.githubusercontent.com/17884471/143854093-3f997432-7219-4251-ad1a-d34c35ab94d5.png">

 3. Select [gmmk_pro_ansi_layout_mine.json][keymap-json-file] frile from this repository

 4. Change keymap configurations

 5. Exporting keymap as JSON file with [gmmk_pro_ansi_layout_mine.json][keymap-json-file] (with overriding file in repository)
    <img width="1840" alt="image" src="https://user-images.githubusercontent.com/17884471/143856877-20dc6990-ba31-4740-9ca1-ccc991a2ca96.png">

 6. Create commit and push changes to repo

 7. Download artifact file from actions build

 8. Launch [qmk-toolbox][qmk-toolbox]

 9. Select dowloaded in 7 step file
    <img width="1089" alt="image" src="https://user-images.githubusercontent.com/17884471/143860028-0e9835ff-537c-4d38-a74a-fcd1ceb17994.png">

 10. Unplug keyboard and and plug in bootloader mode
        > The first time you flash the firmware, stock reset combination on your keyboard is `<Space> + B` but after the first time, it is potentially changed. If you have no idea what did you remap the reset command to, it would by default be `fn + \` (See `reset` key).

 11. When in log window you will see yellow record that the device has been connected
    <img width="997" alt="image" src="https://user-images.githubusercontent.com/17884471/143861092-c3a4b36e-57c5-4bb8-badf-9f8d692a6b8e.png">

 12. Click Flash
        > DO NOT UNPLUG KEYBOARD BEFORE FLASHING NOT FINISHED

 13. Praise yourself, you are amazing!


## Useful links
 * [STEP-BY-STEP GUIDE TO CONFIGURING YOUR GMMK PRO USING QMK](https://www.pcgamingrace.com/blogs/news/step-by-step-guide-to-configuring-your-gmmk-pro-using-qmk)

 * [How to Install QMK on your GMMK Pro](https://www.youtube.com/watch?v=MxQeQoUHvEY)

 * [QMK documentation](https://beta.docs.qmk.fm)

 * [Fixing GMMK pro’s rotary knob after flashing firmware with QMK](https://iboss.medium.com/fixing-gmmk-pros-rotary-knob-after-flashing-firmware-with-qmk-28002e78cf3e)




[qmk-config]: https://config.qmk.fm/
[qmk-toolbox]: https://github.com/qmk/qmk_toolbox/
[gmmk-pro]: https://www.pcgamingrace.com/products/glorious-gmmk-pro-75-barebone-black
[keymap-json-file]: https://github.com/md5orsha256/gmmk_pro_qmk_firmware/blob/master/gmmk_pro_ansi_layout_mine.json