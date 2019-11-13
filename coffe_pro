#importing the relevent libraries
import pandas as pd 
import numpy as np 
import matplotlib.pyplot as plt 
import seaborn as sns

df = pd.read_csv('ICO_CROP_DATA.csv',parse_dates = ['YEAR', 'MONTH'])
df.dropna(inplace= True)


dfBrazil = df[df['COUNTRY'] == 'Brazil']

plt.figure(figsize= (10,10))
plt.scatter(dfBrazil.TOTAL_PRODUCTION,dfBrazil.DOMESTIC_CONSUMPTION)
dfBrazilnum = dfBrazil.loc[:,['TOTAL_PRODUCTION','DOMESTIC_CONSUMPTION','EXPORTABLE_PRODUCTION','GROSS_OPENING_STOCKS']]

sns.heatmap(dfBrazilnum)
plt.show()