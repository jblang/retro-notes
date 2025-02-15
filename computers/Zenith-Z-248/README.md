# Zenith Z-248 AT-compatible 8MHz 286

The Zenith ZW-248-84 is an AT-compatible 8MHz 286 system in the Z-200 series. It has a backplane-based design where the motherboard only contains slots and passive components, and the CPU and chipset are on plugin boards.

![front](front.jpeg)
![rear](rear.jpeg)

## Acquisition

Bought from the [Bits Please](https://www.ebay.com/str/bitsplease) store on eBay in January 2025.

## Original Components

- [Zenith Z-248 10-slot passive backplane](Z248-Backplane/README.md)
- [Zenith Z-248 CPU board with 286 CPU and 512K RAM](Z248-CPU/README.md)
- [Zenith Z-248 I/O board with chipset, RTC, serial, and parallel ports](Z248-IO/README.md)
- [Zenith Z-445 Memory expansion boards (2)](Z445-RAM/README.md)
  - Extra 128K base memory for 640K total 
  - 2.5M extended memory
- [DTC 5290-CZ Floppy and MFM hard drive controller](DTC-5290CZ/README.md)
- [Seagate ST-4051 42MB MFM hard drive](Seagate-ST4051/README.md)

## Added Components

- [DFI VG-3000 VGA card with OTI037C chip](DFI-VG3000/README.md)
- [Sound Blaster 2.0 (CT1350B)](SoundBlaster-CT1350B/README.md)
- [Teac FD-235HF 3.5" 1.44MB floppy drive](Teac-FD235HF/README.md)
- [Teac FD-55GFR 5.25" 1.2MB floppy drive](Teac-FD55GFR/README.md)
- [Lo-Tech XT-CF 8-bit IDE inteface](Lotech-XTCF/README.md)
  - Rear slot CF adapter
  - 512MB CF Card

## Removed Components

- [Compex ANET/1 ARCNET adapter](../../parts/Compex-ANET1/README.md)
- [Paradise AutoSwitch EGA card with PEGA1A chip](../../parts/Paradise-PEGA1A/README.md)

## Restoration Notes

### Power supply
- For initial testing of the power supply, I removed all the components from the backplane and powered up it with a known bad IDE hard drive connected to provie a load.  
- After the power supply stabilized, I checked all the voltages and confirmed that they were correct before putting the other parts back in.
- Originally the system seemed a bit unstable and wouldn't always boot, with the diagnostic LED indicating a CPU fault. 
- After running for a few hours, it fully stabilized (most likely after all the electrolytic caps fully reformed).

### 3.5" floppy drive
- The drive's mechanism was so stiff that it wouldn't accept disks that I tried to insert.
- I attempted to clean and lubricate it, but the mechanism is very corroded and it wouldn't seek even after my attempts to revive it.
- I removed it and replaced it with the TEAC 3.5" drive. I successfuly booted DOS 3.31 from the new floppy drive.

### MFM hard drive
- After reconnecting the drive, it spun up and booted DOS, but it had a ton of bad sectors and very few files were readable.
- I used SpeedStor 6.5 to low-level format the drive and then installed DOS 3.31 on it. It has worked reliably for many hours since then.
- I eventually disconnected it from power and the controller and disabled it in the BIOS, but left it in the case. My reasons were to reduce system noise and prevent wear to the drive.

### Upgrades
- Replaced EGA card with a VGA card since I don't have an EGA monitor.
- Added the Sound Blaster
- Added the XT-CF IDE adapter
- Removed the ARCNET adapter since I have no way to test or use it currently and I needed the slot.

## Personal Notes

My dad ran his pharmacy on a similar Z-200 system from the mid-80s to early 90s. Originally he had the 286 model, but he upgraded it to a 386 with a kit sold by Zenith. He brought it home before using it at his store, and I have memories around 7 or 8 of watching him play Zork and King's Quest on it, and playing Mixed-Up Mother Goose myself. Later in junior high, I had a 16MHz 386SX at home, which was the source of the VGA board and keyboard I am using with this system.  The 386SX also had a Sound Blaster 1.5 and the same modela Sound Blaster 1.5 TEAC floppy drives that I installed in this system.  My current configuration is therefore a bit of a hybrid between these two systems.

## Documentation

- [Z-248 Brochure](Z-248_Brochure.pdf)
- [Z-200 PC Series Owner's Manual](Z-200_PC_Series_Owners_Manual.pdf) (from [BitSavers](https://bitsavers.org/pdf/zenith/z200/))
- [Z-200 PC Diagnostics](Z-200_PC_Diagnostics.pdf) (from [BitSavers](https://bitsavers.org/pdf/zenith/z200/))

## Software
- [Zenith Z-200 PC Diagnostics](Z-200_Diagnostics.zip) (from [WinWorld](https://winworldpc.com/download/c2ae0951-5247-6211-c3a4-c28d587054ef))
- [Zenith Z-200 GW-BASIC Version 3](Z-200_GW-Basic_Version_3.zip) (from [WinWorld](https://winworldpc.com/download/5563142e-4763-11c3-a4c2-8d587054c392))

## Additional Photos

### Current Configuration

#### Case Open

![front-open-current.jpeg](front-open-current.jpeg)
![top-open-current.jpeg](top-open-current.jpeg)

#### Case Labels

![case-labels.jpg](case-labels.jpg)

### Original Configuration

#### Front and Rear

![front-original.jpeg](front-original.jpg)
![rear-original.jpeg](rear-original.jpg)

#### Case Open

![front-open-original.jpeg](front-open-original.jpg)
![top-open-original.jpeg](top-open-original.jpg)