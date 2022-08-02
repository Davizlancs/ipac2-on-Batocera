# ipac2-on-Batocera Pi4b
Help with config for ipac2 using batocera on the pi4b

If you intend to use your existing ipac2 to use on the new Raspberry pi 4b running a new Batocera image you may wonder why after you are prompted to map your controller input,
That
1. Although it maps, it doesn't save.
2. It doesn't create a config file usually expect to see '#0_Ultimarc_ipac_2_keyboard'

This is because unlike previous versions of Retropie on the older Raspberry pi models, Batocera is simply reading the ipac as a keyboard only, therefore not encoding into a controller.

You may need to complete the following steps to enable your ipac2 to run correctly on Batocera image.

Install the winipacv2 app if not already done so.

Link to download (ipac2 2015 onwards) https://www.ultimarc.com/winipacv2setup.exe

1. Plug Ipac2 into a pc/laptop 
2. Open your installed winipac app
3. Select file 
4. Firmware Upgrade

It Will then update your ipac2 firmware to enable  ‘Multi-mode’ 

Once Updated after around 30sec

4. Go back into file
5. Select New

Once you see your ipac2 configuration board, you are ready to begin to reconfigure your board to Gamepad mode.
To do this you will need to:

6. Go through selecting each pin on the ipac and enable game mode for the selected pin
7. Change the pre-configured button to ‘P1 button 1’ to the corresponding swf pin on the ipac2.
for eg:
ipac2 ‘1sw1’ = gamepad ‘button Y'
ipac2 ‘1sw2’ = gamepad ‘button X'
And so on, 
Repeat step 6.7. For player 2

After you have configured each control pin on your ipac2 

8. Select 'Force board reconfigure'

9. Save file
You can now unplug your ipac2 from your laptop or PC

Once you reattach to your pi, follow prompts to re-map new controls, or using a keyboard or other controller open the Batocera settings and select 'configure new controller'
It will now recognise both controls as Ultimarc ipac2 gamepads #0 and #1 


