## SUR Revived 

This fork patches the original tool to provide full out-of-the-box compatibility with modern Windows 11 builds:

* **Native File Picker:** Replaced the deprecated `mshta` HTML file dialog with a native PowerShell `OpenFileDialog`, fixing the blank ROM selection bug (`ECHO is off.` error).
* **Modern Privilege Elevation:** Swapped obsolete `cacls` calls for modern UAC elevation checks via `net session` and PowerShell `Start-Process -Verb RunAs`.
* **Reliable Extraction:** Restored reliable file path parsing when selecting ROM `.zip` packages from the interactive menu.

---

## Credits & Disclaimer

* **Original Developer:** All core features, repack/unpack scripts, and binary integrations were developed by **JamFlux** ([Original Repository](https://github.com/jamflux/SUR)).
* **License & Attribution:** Per the original author's terms, this tool remains free to use. Proper credits to **JamFlux** and associated tool authors must remain visible wherever modified ROMs created with this tool are distributed or published.
