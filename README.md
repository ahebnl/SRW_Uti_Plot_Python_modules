# SRW_Uti_Plot_Python_modules
SRW has python module uti_plot.py uti_plot_matplotlib.py, uti_math.py, uti_plot_com.py and SRWLIB_ExampleViewDataFile.py to support the SRW output data processing. Here we mainly explain how to use the plotting and image processing functions by these "uti_plot" python modules.
### 1, plot a SRW data file
```bash
python SRWLIB_ExampleViewDataFile.py -f test_data.dat -j
```
# ![Sirepo](https://github.com/ahebnl/SRW_Uti_Plot_Python_modules/blob/master/images/figure_1.png)
Figure (1) shows the 2D intensity image, figure (2) shows the intensity cut at y=0, figure (3) shows the intensity cut at x=0

### 2, plot a SRW data file with a scale option
```bash
python SRWLIB_ExampleViewDataFile.py -f test_data.dat -j -s log10
```
# ![Sirepo](https://github.com/ahebnl/SRW_Uti_Plot_Python_modules/blob/master/images/figure_2_scale.png)
Several scale options can be used in plots (linear, log, log2, log10).
