Basic Python
1. Split this string
s = "Hi there Sam!"
s.split(' ')
['Hi', 'there', 'Sam!']
2. Use .format() to print the following string.
Output should be: The diameter of Earth is 12742 kilometers.
planet = "Earth"
diameter = 12742
print("The diameter of {} is {}".format(planet,diameter))
The diameter of Earth is 12742
3. In this nest dictionary grab the word "hello"
d = {'k1':[1,2,3,{'tricky':['oh','man','inception',{'target':[1,2,3,'hello']}]}]}
d['k1'][-1]['tricky'][-1]['target'][-1]
'hello'
Numpy
import numpy as np
4.1 Create an array of 10 zeros?
4.2 Create an array of 10 fives?
z = np.zeros(10)
z
array([0., 0., 0., 0., 0., 0., 0., 0., 0., 0.])
f = np.ones(10)*5
f
array([5., 5., 5., 5., 5., 5., 5., 5., 5., 5.])
5. Create an array of all the even integers from 20 to 35
r = np.arange(20,35)
r
array([20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 32, 33, 34])
6. Create a 3x3 matrix with values ranging from 0 to 8
td = np.arange(0,9).reshape(3,3)
td
array([[0, 1, 2],
       [3, 4, 5],
       [6, 7, 8]])
7. Concatenate a and b
a = np.array([1, 2, 3]), b = np.array([4, 5, 6])
a= np.array([1,2,3])
b =np.array([4,5,6])
re = np.concatenate((a,b),axis=0)
re
array([1, 2, 3, 4, 5, 6])
Pandas
8. Create a dataframe with 3 rows and 2 columns
import pandas as pd
l = [['a','b'],['a','b'],['a','b']]
df = pd.DataFrame(l)
df
0	1
0	a	b
1	a	b
2	a	b
9. Generate the series of dates from 1st Jan, 2023 to 10th Feb, 2023
date_series = pd.date_range('01-01-2023','10-02-2023')
date_series
DatetimeIndex(['2023-01-01', '2023-01-02', '2023-01-03', '2023-01-04',
               '2023-01-05', '2023-01-06', '2023-01-07', '2023-01-08',
               '2023-01-09', '2023-01-10',
               ...
               '2023-09-23', '2023-09-24', '2023-09-25', '2023-09-26',
               '2023-09-27', '2023-09-28', '2023-09-29', '2023-09-30',
               '2023-10-01', '2023-10-02'],
              dtype='datetime64[ns]', length=275, freq='D')
10. Create 2D list to DataFrame
lists = [[1, 'aaa', 22], [2, 'bbb', 25], [3, 'ccc', 24]]

lists = [[1, 'aaa', 22], [2, 'bbb', 25], [3, 'ccc', 24]]
ndf = pd.DataFrame(lists)
ndf
0	1	2
0	1	aaa	22
1	2	bbb	25
2	3	ccc	24

