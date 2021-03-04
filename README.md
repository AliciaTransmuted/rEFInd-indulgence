![Screenshot](https://i.imgur.com/nKtPOUp.png)

# rEFInd-indulgence
rEFInd-indulgence is a luxurious soft leather icon theme with a custom hand stitched font for the rEFInd UEFI boot manager

[rEFInd](http://www.rodsbooks.com/refind/) is a boot manager for UEFI systems and scans for kernels & EFI at boot.

### Usage

 1. Locate your refind EFI directory. This is commonly `/boot/EFI/refind`
    though it will depend on where you mount your ESP and where rEFInd is
    installed.

 2. Create a folder called `themes` inside it, if it doesn't already exist

 3. Clone this repository into the `themes` directory as `themes/rEFInd-indulgence`.

 4. To enable the theme add `include themes/rEFInd-indulgence/theme.conf` at the end of
    `refind.conf`.
    
Entries should be autodetected and shown with the proper icons.

Manual entry can be done via `menuentry` option.

Example:

```
menuentry "Windows" {
	icon /EFI/refind/themes/rEFInd-indulgence/icons/os_windows.png
	loader /EFI/Microsoft/Boot/bootmgfw.efi
}
```

Other examples are in the `refind.conf` file.

-------------------------------
rEFInd-indulgence notes
-------------------------------

September 12, 2018: Initial release of rEFInd-indulgence to DeviantArt.

December 30, 2018: rEFInd-indulgence theme uploaded to github.

January 6, 2019: Added icons for Sparky Linux, GameDrift, and Lakka

March 30, 2019: Added icons for Pop OS and Pisi Linux

April 10, 2019: Added icons for Parrot Sec OS, PureOS, and Qubes OS

December 18, 2020: Added new function icons func_bootorder.png and func_install.png

March 3, 2021: Added icon for Garuda Linux
