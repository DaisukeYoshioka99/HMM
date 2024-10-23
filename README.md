# HMM

This Python code (HMM_GitHub.ipynb) analyzes the two-dimensional trajectory of Brownian particles like single fluorescent molecules observed under a TIRF microscope based on an Expectation-Maximization (EM) algorithm and a Hidden Markov Model (HMM). The following two test data are included here:

1) Spot_test.csv: CSV file of “Spots in tracks statistics” output by Fiji’s “TrackMate” plug-in.

2) Stat_test.csv: CSV file of “Track statistics” output by Fiji’s “TrackMate” plugin.

Expected run time for the demo using “Spot_test.csv” and “Stat_test.csv” on a normal desktop computer is about 7 minutes. The following three results will be output when the analysis is successfully completed using the test data:

  1) Pdf_test.csv: Parameter table quantified by the EM algorithm 

  2) HMM_test.csv: Parameter table quantified by the HMM 

  3) state_test.csv: Input data (Spot_test.csv) with information such as the diffusion state of each bright spot.

We have tested the Python code on the following software:

Python 3.10.12

How to run the program on Google Colab:

1. Upload the following two files to any folder on Google Drive:

  1) CSV file of “Spots in tracks statistics” output by Fiji’s plugin “TrackMate” (equivalent to “Spot_test.csv”). 
     * Please change the file name to start with “Spot_”.

  2) CSV file of “Track statistics” output by Fiji’s plug-in “TrackMate” (equivalent to “Stat_test.csv”). 
     * Please change the file name to start with “Stat_”.

2. Set the path in cell 5.

3. Set the hyperparameters in cell 7.

4. Run.
