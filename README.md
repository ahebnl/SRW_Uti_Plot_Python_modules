# SRW_Uti_Plot_Python_modules
SRW has python module uti_plot.py uti_plot_matplotlib.py, uti_math.py, uti_plot_com.py and SRWLIB_ExampleViewDataFile.py to support the SRW output data processing. Here we mainly explain how to use the plotting and image processing functions by these "uti_plot" python modules.
## 1, plot SRW data file
```bash
python SRWLIB_ExampleViewDataFile.py -f test_data.dat -j
```
# ![Sirepo](https://github.com/ahebnl/SRW_Uti_Plot_Python_modules/blob/master/images/figure_1.png)
Figure (1) shows the 2D intensity image, figure (2) shows the intensity cut at y=0, figure (3) shows the intensity cut at x=0

## 2, plot SRW data file with a scale option
```bash
python SRWLIB_ExampleViewDataFile.py -f test_data.dat -j -s log10
```
# ![Sirepo](https://github.com/ahebnl/SRW_Uti_Plot_Python_modules/blob/master/images/figure_2_scale.png)
Several scale options can be used in plots (linear, log, log2, log10).

## 3, plot SRW data file with color 
```bash
python SRWLIB_ExampleViewDataFile.py -f test_data.dat -j -s log10 -c jet
```
# ![Sirepo](https://github.com/ahebnl/SRW_Uti_Plot_Python_modules/blob/master/images/figure_3_scale_color.png)
Several colormap options can be used in plots (Greys_r, afmhot, coolwarm, jet, PiYG....).

## 4, plot SRW data file and get the data cuts with the defined line: y = tan(\theta)*x + y0
### 4_1, intensity cut at y = y0, intensity cut at x = x0
```bash
python SRWLIB_ExampleViewDataFile.py -f test_data.dat -j -s log10 -c jet -y 1e-4 -x 2e-4
```
# ![Sirepo](https://github.com/ahebnl/SRW_Uti_Plot_Python_modules/blob/master/images/figure_4_xcut_ycut.png)
Figure (2) shows the intentsity cut at y=0.0001 [m], figure (3) shows the intensity cut at x=0.0002 [m].
### 4_2, intensity cut at y = tan(theta)*x, intensity cut at x = x0
```bash
python SRWLIB_ExampleViewDataFile.py -f test_data.dat -j -s log10 -c jet -r 45
```
# ![Sirepo](https://github.com/ahebnl/SRW_Uti_Plot_Python_modules/blob/master/images/figure_6_scale_color_rotation.png)
Figure (1) shows the 2D image when Figure 4_1(1) is rotated 45 degree clockwise. Figure(2) shows the intensity cut at y= tan(45^0)*x (i.e., Cut line 2 in Figure 4_1(1)).
