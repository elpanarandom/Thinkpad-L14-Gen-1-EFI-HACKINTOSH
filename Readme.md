# EFI for Lenovo Thinkpad L14 Gen !
- macOS: Ventura 13.7 / Tested on Sonoma 14.0, Sonoma 14.7 and Sequoia 15.1
  
- Opencore Version: 1.0.1
  
This repository contains the EFI required to install macOS on a Lenovo Thinkpad L14 Gen 1, below are the specifications:

# Specs:
- Processor: Intel I5-10210U
- Ram: 12GB DDR4 3200MHZ (Due a Intel Limitation, The ram Works at 2400MHZ)
- IGPU: Intel UHD 630
- SSD: Kioxia M.2 512GB PCIE GEN 4
- Camera: 5MP 720P
- Battery: 3 Cels 47WH

## What Work:
✅ Battery percentage and Cycles

✅ Bluetooth - Intel AX200

✅ Wifi - Intel AX200 (Using itlwm Kext, works perfectly. The Wifi is Detected in the Online Installer)

✅ CPU power management

✅ iGPU Hardware Acceleration

✅ HDMI (Hot Plug Works Perfectly)

✅ iMessage, FaceTime, App Store, iTunes Store (Generate your own SMBIOS)

✅ Keyboard Keys (Media, Brightness and Action Keys [Like Disable Inalambric Network])

✅ Audio (alcid=11. At a random moment the audio is muted and when you try to turn up the volume you hear a squeak. It is fixed by opening Settings > Sound > Input Devices)

✅ Microphone

✅ Sleep/Wake (Needs 20 seconds to sleep. If anyone knows how to fix it and make the Sleep be immediate, let me know.)

✅ TrackPoint (Works Perfectly. Like Windows)

✅ USB Ports (USB Map Created. No need to Remap)

✅ Webcam (It is perfectly detected in facetime, zoom, google meet and discord)

✅ TouchPad (Works Perfect)

✅ Boot Chime

## What Doesnt Work:
❌ Sidecar or Handoff

❌ Micro SD Card Reader

❌ Fingerprint Reader

## ACPI FILES
- THINK.AML (This is The System SSDT Patch)
  
- SSDT-THINK.AML (This SSDT Make the YOGASMC Works)

## NOTES:
- Sleep and wake needs to be "Repaired" From closing the lid to going to sleep, it takes about 20 seconds. But to wake from sleep mode it is Immediately

- I haven't tested USB-C adapters or displays yet

## Initial Setup:
- You NEED to supply your own SMBIOS, Serial number, MLB and UUID using GenSMBIOS, configured for a MacbookPro16,3.
  In case you want to install a version of macOS higher or lower than Ventura, you have to change only the kext "Airportitlwm" for the kext appropriate to your version of Mac


