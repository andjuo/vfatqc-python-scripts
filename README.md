# vfatqc-python-scriptsi

1. For VFAT2s QC1 test:
   
	> python testing.py

	>> GLIB IP: e.g. 192.168.0.171

	Then hit "enter" 5 times 

2. For VFAT2s QC2/3 test: (Off detector: 35~40 mins per chip; On detector: 55~60 mins per chip!)
   
	> python pythonScript.py

	>> GLIB IP: e.g. 192.168.0.171

	>> QC Test Name: e.g. 2016_09_09_QC3

	Then hit "enter" 5 times 

3. To plot each VFAT's output results: (all the output files should in the same dir)
   
	> python read_and_plot.py

4. To plot all VFATs' results: (all the output files should in the same dir)
   
	> python read_and_plot_all.py

5. To set the TrimDAC values and scan the threshold: (70~80s 24 chips!) 
   
	First, we need to make a txt file to list all the TrimDAC files: TrimDACfiles.txt
   
	> python setTRIMDAC.py

	>> GLIB IP:  e.g. 192.168.0.171

	>> Test Name: e.g. 2016_09_09_SetTrimDAC

	Then hit "enter" 5 times 

6. To set the TrimDAC values and make the S-Curve scanning: (8~15 mins per chip!)
   
	First, we need to make a txt file to list all the TrimDAC files: TrimDACfiles.txt
   
	> python setTRIMDAC_and_Scurve.py

	>> GLIB IP:  e.g. 192.168.0.171

	>> Test Name: e.g. 2016_09_09_SetTrimDAC

	Then hit "enter" 5 times 

7. (Not a good idea!!) To set the TrimDAC values, set thresholds and make the S-Curve scanning:
   
	First, we need to make a txt file to list all the TrimDAC files: TrimDACfiles.txt

	Second, make a txt file to list all the Threshold files: Datafiles.txt
   
	> python setTRIMDAC_and_Threshold.py

	>> GLIB IP:  e.g. 192.168.0.171

	>> Test Name: e.g. 2016_09_09_SetTrimDAC

	Then hit "enter" 5 times 





