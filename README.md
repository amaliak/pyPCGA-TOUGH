# pyPCGA-TOUGH: A Python-based package for geostatistical inversion in TOUGH2

The pyPCGA-TOUGH connects the Python library for Principal Component Geostatistical Approach (https://github.com/jonghyunharrylee/pyPCGA) with pyTOUGH, the TOUGH Python for automating TOUGH2 simulations of subsurface fluid and heat flow (https://github.com/acroucher/PyTOUGH).

This README file provides:
- Software description and relevant literature
- Installation guides
- Instructions for running a tutorial

## Method description and literature


### References

- J Lee, H Yoon, PK Kitanidis, CJ Werth, AJ Valocchi, "Scalable subsurface inverse modeling of huge data sets with an application to tracer concentration breakthrough data from magnetic resonance imaging", Water Resources Research 52 (7), 5213-5231

- AK Saibaba, J Lee, PK Kitanidis, Randomized algorithms for generalized Hermitian eigenvalue problems with application to computing Karhunen–Loève expansion, Numerical Linear Algebra with Applications 23 (2), 314-339

- J Lee, PK Kitanidis, "Large‐scale hydraulic tomography and joint inversion of head and tracer data using the Principal Component Geostatistical Approach (PCGA)", WRR 50 (7), 5410-5427

- PK Kitanidis, J Lee, Principal Component Geostatistical Approach for large‐dimensional inverse problems, WRR 50 (7), 5428-5443

### Applications

- A Kokkinaki, J Lee, H Ghorbanidehno, PK Kitanidis, EF Darve Subsurface characterization for large scale systems: An integrated python-based inversion tool for TOUGH2, TOUGH2 Symposium 2018. Slides can be found [here](https://github.com/amaliak/pyPCGA-TOUGH/blob/master/TOUGH2018_Kokkinaki.pdf). 

- J Lee, A Kokkinaki, PK Kitanidis, Fast large-scale joint inversion for deep aquifer characterization using pressure and heat tracer measurements, Transport in Porous Media, 123(3): 533-543, 2018

## Installating pyPCGA-TOUGH

### Install pyPCGA

Download pyPCGA from the git repository in your chosen folder:

``` git clone https://github.com/jonghyunharrylee/pyPCGA.git ```

After the download finishes, you should have a folder called pyPCGA. Run the makefile to complete the installation.

``` make install  ```

Troubleshooting:
- The make file will complain if you don't have numpy and matplotlib installed.
- If you use Anaconda you can install the packages using 'conda install <package_name>'

If you have multiple versions of python installed (e.g. 2.x and a more recent 3.x. verison), it is possible that pyPCGA may be installed in the wrong location (e.g. in /usr/lib64/python2.7/ as opposed to the python 3 library directory. 

To check if pyPCGA was installed in the right place, go to one of the examples e.g. pyPCGA/examples/pumping_history_identification and from within that directory try:
``` from pyPCGA import PCGA ```

If the libraries were not installed properly, you will get a message that module pyPCGA was not found. 


### Install pyTOUGH

Download pyTOUGH from the git repository in your chosen folder:

``` git clone https://github.com/acroucher/PyTOUGH.git ```

After the download finishes, you should have a folder called PyTOUGH. While in that directory, do:

```python setup.py install ```

For complete installation instructions and troubleshooting, see PyTOUGH instructions [manual](https://github.com/acroucher/PyTOUGH/blob/master/doc/PyTOUGH-guide.pdf)



## Running the tutorial

### Running a single variable inversion: Hydraulic tomography

For this tutorial, use file inv_tough_pre.py 



### Running joint inversion: Heat tracer tomography


For this tutorial, use file inv_tough_joint.py 

