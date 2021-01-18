# Hackintosh-EFI
Asrock H61M-VS3 Opencore Sources

This folder contain all needed files for booting and install MacOS Bigsur (Online Methor) on PC.
Doublecheck your PC specs to be sure they're the same with my Hackintosh PC. If all are the same, just grab and put to your USB to boot and Install (Before, just check your Bios option are corrected)
-- Specs --
* Bootloader: Opencore 0.6.5 Release | SMBios iMac15,1 | MacOS Bigsur (latest update)
* Mainboard: Asrock H61M-VS3 (latest Bios ver. updated)
* Processor: Intel Core i3 3220 Ivy Bridge (3rd gen) with Intel HD Graphic Intergrated
* Graphic: 
- Onboard Intel HD2500 Graphic (enabled in Bios and use for calulator)
- Zotac Nvidia Geforce GT730 (GK208) 1Gb DDR5 PCI-E (DP/HDMI/DSub) (use for drive my Display via VGA-DSub Port)
* Memory: 8Gb DDR3 1067Mhz Dual channel
* Network: Realtek RTL8105E Gigabit Networking Family
* Audio: Realtek ALC662 Sound Chipset (5.1 Channel)

-- Working --
1. CPU (HT, Multicore, Power Managerment, Sleep/Wakeup)
2. Graphic: Both Graphic Processor are working perfectly (Full QE/CI)
3. Network: Working perfecty with RTL8100.kext (not RTL8111.kext)
4. Audio: Working good with AppleALC.kext and Layout-id=5 (or 11) but all front panel jacks have no sound, only onboard back jacks working normanly.

-- Not woking --
1. All Front panel audio jacks (line-out, mic-in)
2. As your reports.

-- Others --
1. Bootpicker was set to GUI with LightSlim Iconpack.
2. Total booting time about 3 mins from touch power button. I was tried to reduce booting time but no luck. Maybe course of Ivy Bridge system must use HFSPlusLegacy.efi drive instead HFSPlus.efi and there're some "false" in verbose log.
3. I get jagged (dock background + widget) when using 22inch 1080p Monitor because Real iMac15,1 has built with 5K Retina Display, much higher resolution than my display. I think with 2K display, this issue can be solve.
