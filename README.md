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

- A Kokkinaki, J Lee, H Ghorbanidehno, PK Kitanidis, EF Darve Subsurface characterization for large scale systems: An integrated python-based inversion tool for TOUGH2, TOUGH2 Symposium 2018. Slides can be found [here](https://github.com/amaliak/pyPCGA-TOUGH/blob/master/Kokkinaki_Inverse_Subsurface_characterization_final.pdf). 

- J Lee, A Kokkinaki, PK Kitanidis, Fast large-scale joint inversion for deep aquifer characterization using pressure and heat tracer measurements, Transport in Porous Media, 123(3): 533-543, 2018

## Installating pyPCGA-TOUGH

### Install pyPCGA

Download pyPCGA from the git repository in your chosen folder:

``` git clone https://github.com/jonghyunharrylee/pyPCGA.git ```

After the download finishes, you should have a folder called pyPCGA. Run the makefile to complete the installation.

``` make install  ```

Troubleshooting:
- The make file will complain if you don't have numpy installed. 


### Install pyTOUGH

``` git clone https://github.com/acroucher/PyTOUGH.git ```



## Running the tutorial

