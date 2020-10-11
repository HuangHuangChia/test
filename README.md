import  pandas as pd
import numpy as np
from scipy.stats import skew
from scipy.stats import kurtosis

mydata = pd.read_excel("d:\Exceldata.xlsx", sheet_name="一月")
print("北區  均值：",np.mean(mydata['北區']))
print("北區標準差：",np.std(mydata['北區']))
print("北區偏態值：",skew(mydata['北區']))
print("北區峰態值：",kurtosis(mydata['北區']))
