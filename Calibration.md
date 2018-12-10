; Calibration code to be added to slicer for the bed tilt calibration
;
M104 200 ;Heat hot end to 200C
G1 E-12 F100 ;Retract filament to stop oozing during calibration
M140 60 ;Heat bed to 60C
G28 XYZ ;Home axis X Y Z
BED_TILT_CALIBRATE ;Perform a bed tile calibration
G1 X116 Y116 F3000 ;Move head to center of bed
