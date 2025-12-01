# Thermal Label Printer Printing Wrong Size / Multiple Labels

**Printer:** Nelko PL70e-BT (applies to most thermal label printers)
**Problem:** Printer prints labels at wrong size, spits out multiple labels, prints sideways/upside down, or ignores custom paper size settings
**Date Fixed:** 2025-12-01

## Symptoms

- Set custom label size (e.g., 25x75mm) but printer acts like 100x150mm labels are loaded
- Prints across 4 small labels instead of 1
- Portrait prints sideways, landscape prints upside down
- Custom paper size shows in Preferences but not in "Paper available" list
- Calibration (feed button hold) works but printing still broken

## Things That DON'T Work

- Creating custom paper sizes in Printing Preferences
- Changing default paper in driver settings
- Long-pressing feed button to calibrate (helps physical detection but driver ignores it)
- Adjusting gap settings
- Praying

## The Actual Fix

**Nuke the driver and reinstall fresh.**

### Step-by-Step

1. **Remove the printer from Windows**
   - Settings → Devices → Printers & Scanners
   - Click the printer → Remove device

2. **Delete the driver completely**
   - Search "Print Management" in Start menu
   - Go to "All Drivers"
   - Find your printer driver, right-click → Delete
   - If it won't delete, restart and try again

3. **Unpair from Bluetooth** (if Bluetooth printer)
   - Settings → Devices → Bluetooth
   - Find the printer → Remove device

4. **Restart computer**

5. **Reinstall driver from manufacturer**
   - For Nelko: https://www.nelkoprint.com/pages/driver-user-manual
   - Let the installer handle Bluetooth pairing (don't manually pair first)

6. **Calibrate after install**
   - Load your labels
   - Long-press feed button ~3 seconds until it beeps

7. **Test print**

## Why This Happens

The Windows print driver caches paper size settings somewhere deep in the registry/driver config. Changing settings in the UI doesn't always update these cached values. A fresh install clears all the garbage.

## Notes

- Bluetooth printing is slower than USB on these printers
- If reinstalling doesn't work, try USB instead of Bluetooth
- The Nelko mobile app sometimes handles sizes better than Windows

## Time Wasted Before Finding Fix

~2 hours of adjusting settings, creating custom paper sizes, and calibrating repeatedly.

## Time To Fix Once You Know

~5 minutes.
