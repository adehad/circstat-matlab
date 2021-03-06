CircStat for Matlab
=======================

Toolbox for circular statistics with Matlab. 

## Authors:
Philipp Berens 

*Email*: philipp.berens@uni-tuebingen.de

*Homepage*: www.berenslab.org

## Contributors:
Tal Krasovsky & Marc J. Velasco

## Reference:
P. Berens, *CircStat: A Matlab Toolbox for Circular Statistics*, Journal of Statistical Software, Volume 31, Issue 10, 2009
http://www.jstatsoft.org/v31/i10

Please cite this paper when the provided code is used. See licensing terms for details.

## Contents (`Contents.m`):
### Descriptive Statistics.
- `circ_mean`     - Mean direction of a sample of circular data
- `circ_axialmean`- Axial corrected mean direction of a sample of circular data
- `circ_median`   - Median direction of a sample of circular data
- `circ_r`        - Resultant vector length
- `circ_var`      - Circular variance
- `circ_std`      - Circular standard deviation
- `circ_moment`   - Circular p-th moment 
- `circ_skewness` - Circular skewness
- `circ_kurtosis` - Circular kurtosis

### Inferential Statistics.
#### Testing for Circular Uniformity.
- `circ_rtest`    - Rayleigh's test for nonuniformity
- `circ_otest`    - Hodges-Ajne test (omnibus test) for nonuniformity
- `circ_raotest`  - Rao's spacing test for nonuniformity
- `circ_vtest`    - V-Test for nonuniformity with known mean direction

#### Tests Concerning Mean and Median.
- `circ_confmean` - Confidence intervals for mean direction
- `circ_mtest`    - One-sample test for specified mean direction
- `circ_medtest`  - Test for median angle
- `circ_symtest`  - Test for symmetry around median angle

#### Paired and Multisample Tests.
- `circ_wwtest`     - Two and multi-sample test for equal means; one-factor ANOVA
- `circ_hktest`     - Two-factor ANOVA
- `circ_cmtest`     - Non-parametric multi-sample test for equal medians
- `circ_ktest`      - Test for equal concentration parameter
- `circ_kuipertest` - Test for equality of distributions (KS-test)

### Measures of Association.
- `circ_corrcc`   - Circular-circular correlation coefficient
- `circ_corrcl`   - Circular-linear correlation coefficient

### The Von Mises Distribution
- `circ_vmpdf`    - Probability density function of the von Mises distribution
- `circ_vmpar`    - Parameter estimation
- `circ_vmrnd`    - Random number generation

### Others.
- `circ_axial`      - Convert axial data to common scale
- `circ_dist`       - Distances around a circle
- `circ_dist2`      - Pairwise distances around a circle
- `circ_stats`      - Summary statistics
- `circ_kappa`      - Compute concentration parameter of a von Mises distribution
- `circ_plot`       - Visualization for circular data
- `circ_clust`      - Simple clustering
- `circ_samplecdf`  - Evaluate CDF of a sample
- `circ_rad2ang`    - Convert radian to angular values
- `circ_ang2rad`    - Convert angular to radian values


All functions take arguments in radians (expect for `ang2rad`). For a detailed description of arguments and outputs consult the help text in the files.

Since 2010, most functions for descriptive statistics can be used in Matlab style matrix computations. As a last argument, add the dimension along which you want to average. This changes the behavior slightly from previous relaeses, in that input is not reshaped anymore into vector format. Per default, all computations are performed along the **first non-singular dimension**.

## References:
- E. Batschelet, *Circular Statistics in Biology*, Academic Press, 1981
- N.I. Fisher, *Statistical analysis of circular data*, Cambridge University Press, 1996
- S.R. Jammalamadaka et al., *Topics in circular statistics*, World Scientific, 2001
- J.H. Zar, *Biostatistical Analysis*, Prentice Hall, 1999


The implementation follows in most cases '*Biostatistical Analysis*' and all referenced equations and tables are taken from this book, if not otherwise noted. In some cases, the other books were preferred for implementation was more straightforward for solutions presented there.

If you have suggestions, bugs or feature requests or want to contribute code, please email us.

## Disclaimer:
All functions in this toolbox were implemented with care and tested on the examples presented in '*Biostatistical Analysis*' were possible. Nevertheless, they may contain errors or bugs, which may affect the outcome of your analysis. We do not take responsibility for any harm coming from using this toolbox, neither if it is caused by errors in the software nor if it is caused by its improper application. Please email us any bugs you find.

Distributed under Open Source BSD License
