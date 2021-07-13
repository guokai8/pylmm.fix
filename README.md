# pylmm  A lightweight linear mixed-model solver
# pylmmfix
fixed some issues from https://github.com/nickFurlotte/pylmm 
tested on with python 3.9
## Installation
```
git clone https://github.com/guokai8/pylmmfix
python setup.py install
```

## Example

```
import sys
import time

import numpy as np
from pylmm import lmm
K = np.load('data/K.npy')
Y = np.load('data/Y.npy')
snp = np.load('data/snp.npy')
TS,PS = lmm.GWAS(Y,snps,K,REML=True,refit=True)
```


