# Temperature Calibration Files
This folder contains files used for calibration of the PINDA probe.
## temp_cal_veri.gcode
This gcode file is a demonstration - and very helpful tool - of the Prusa Firmware enhanced M860 command - which will be available in the upcoming firmware release AFTER 3.2.1 - M860 now waits also for the PINDA to cool down. The Gcode file prints six squares with each of the PINDA starting temperatures of 35C, 40C, 45C, 50C, 55C, and 60C all on the same print bed. You can easily see, if your ustep offsets in the EEPROM are consistent by inspecting the quality of each first layer.
Another use of the modified M860 command could be to make sure that your print starts at exactly the same PINDA temperature every time  - that would make a proper temperature calibration unnecessary.
Also the modified M860 command makes waiting for the PINDA to cool down an automatic process - very handy for the manual print based temperature calibration. E.g. You can wait until the PINDA has cooled down 30C, then throw on the heaters, wait until the PINDA has reached 35C and start the calibration print.
## 25x25x2mm.stl
This is a small box, 25mm square on X/Y and 0.2mm tall (Z). This makes a useful calibration target for the PINDA calibration process described on the PrusaOwners Wiki.