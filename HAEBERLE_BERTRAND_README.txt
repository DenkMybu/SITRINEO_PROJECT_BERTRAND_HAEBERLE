In order to compile and use the code : 
code line 16465-16639 in MRaw.cxx

Other code modified during the project: code/src/DGlobalTools.cxx to veto the noisy pixels.

[OPTION 1] : Download root, and the taf archive at https://github.com/jeromebaudot/taf, should be updated





[OPTION 2] :    - Access login@sbgli2.in2p3.fr + password 
		- ssh -XYC  dphe1@sbgat597      // paswd : GPicsel@Cms1
		- cd physics/taf



[THEN]
		- maketaf
		- taf -run XXXX -cfg ./config/sitrineo.cfg -guiw   // XXXX is the run number. Here with source and magnet [11,12,13]/ with source without magnet [14,15,16] / without source without magnet [17]
		inside TAF : gTAF->GetRaw()->SitrineoCumul(100000)