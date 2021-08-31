# Radar-1D-CA-CFAR-
1D CA-CFAR implementation in MATLAB
% The following steps here can be used to implement CFAR in the next MATLAB exercise.

% T: Number of Training Cells

% G: Number of Guard Cells

% N: Total number of Cells

% Define the number of training cells and guard cells.

% Start sliding the window one cell at a time across the complete FFT 1D array. The total window size should be 2(T+G)+CUT. In the starter code below, we are considering 1 CUT cell. Hence the total window size is 2(T+G)+1.

For each step, sum the signal (noise) within all the leading or lagging training cells.

Average the sum to determine the noise threshold.

Using an appropriate offset value scale the threshold.

Now, measure the signal in the CUT, which is T+G+1 from the window starting point.

Compare the signal measured in step 5 against the threshold measured in step 4.

If the level of the signal measured in CUT is smaller than the threshold measured, then assign 0 value to the signal within CUT.
