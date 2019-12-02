# driver-zboard-merc
Windows10 Driver for the Zboard Merc Keyboard
![alt text](https://tpucdn.com/reviews/ZBoard/MERCKeyboard/images/merc_title.jpg "ZBoard Merc")

## Background
Zboard Merc is a keyboard which no longer receive driver-updates to work with new Windows updates. Last time I got stuck I stumbled up on [this solution](https://answers.microsoft.com/en-us/windows/forum/windows_10-hardware/merc-stealth-zboard-not-working-after-windows-10/c444c8ec-14cc-4df7-b0ec-6767b6bedb93?auth=1) to solve the problem, covering how to edit the old drivers. Given that software is required and the instructions might not be super obvious to everyone, I compiled the new drivers and provide them in the Kernel2k folder.

## Requirements
1. Windows 10
1. Legacy Software: [32bit](https://downloads.steelseriescdn.com/drivers/keyboards/zengine/ZE_25030_NA_32.exe), [64bit](https://downloads.steelseriescdn.com/drivers/keyboards/zengine/ZE_25030_NA_64.exe)
1. [Disable Signed Driver Enforcement](http://packard-bell-uk.custhelp.com/app/answers/detail/a_id/38288)

## Usage
1. Browse to your Ideazone install location (eg. C:\Program Files (x86)\Ideazon\ZEngine )
1. Replace the Kernel2k folder with the one provided [here](/Kernel2k).
1. In Device Manager locate the entries "Ideazon Merc MM USB Human Interface Device" and "Ideazon Merc USB Human Interface Device" (they could be under Keyboards or Human Interface Devices).
1. Right click > update driver > browse computer > Let me pick > Have Disk > Browse > 
1. Navigate to the Kernel2k folder and select **merc.inf**. Acknowledge any unsigned driver warnings.
1. Enjoy a working zMerc again!

# Alternatives
Someone else at Reddit decided to provide his own [signed drivers here](https://1drv.ms/u/s!ArmFcPzlv8puyUJnTW16KSPhktd9), you can read [the post here](https://www.reddit.com/r/Windows10/comments/6nmb1r/help_on_zboard_keyboard_driver_incompatibility/dnmwhxl/). It claimed to remove the requirement to Disable signed driver enforcement, but at least from the latest Windows update that is no longer true and it is stil a requirement.
