Block 9 is only modified: See comment on the change.

Simulation 1: Rescales the largest dimension (width or length) of the image to 595 while preservating aspect ratio. Zero pad image so resulting dimension is 600 x 600.
Simulation 2: Same as simulation 1, then horizontal flip.
Simulation 3: Rescales the largest dimension (width or length) of the image to 295 while preservating aspect ratio. Add Gaussian noise from mean = 50, std dev = 1 to image. Zero pad image so resulting dimension is 300 x 300.
Simulation 4: (TRY TO SEE IF RUNS) Take only 1 x-ray per patient and run simulation 1 (this might not run since I've included a line of code in block #9 that uses list_unique_x_ray)
Simulation 5: Same as simulation #1 but rotate each images by 10 degrees counterclockwise.

NOTE: Simulation 1-3,5 should run with no issue. Simulation #4 may or maynot run (I'm not well versed with the code, so I'm not 100% sure on how it works with that added line). Run #1-3. Run #4 if possible. If not, run #5.