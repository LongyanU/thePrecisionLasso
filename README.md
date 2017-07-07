# the Precision Lasso

Implementation of the Precision Lasso in this paper:

    ''Wang H, Lengerich BJ, Aragam B, Xing EP. Precision Lasso: Accounting for Correlations and Linear Dependencies in High-Dimensional Genomic Data. Bioinformatics. 2017''

## Introduction

the Precision Lasso is a Lasso variant that is showed to work better compared to other Lasso variants in terms of variable selection when there are correlated and linearly dependent variables existing.

## File Structure:

* models/ main method for the Precision Lasso
* utility/ other helper files
* runPL.py main entry point of using the Precision Lasso to work with your own data

## An Example Command:

```
python runPL.py -v --bfile data/snps.132k.clean.noX --phenofile data/snps.132k.clean.noX.fake.phenos out.txt
```

## Installation
You will need to have numpy and scipy installed on your current system.
You can install precision lasso using pip by doing the following

```
   pip install git+https://github.com/nickFurlotte/pylmm
```
This should make the module pylmm available as well as the two scripts pylmmGWAS.py and pylmmKinship.py.

You can also clone the repository and do a manual install.
```
   git clone https://github.com/HaohanWang/thePrecisionLasso
   python setup.py install
```