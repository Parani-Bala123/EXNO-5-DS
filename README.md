# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
from google.colab import drive
drive.mount('/content/drive')

import matplotlib.pyplot as plt
x_values=[0, 1, 2, 3, 4, 5]
y_values=[0, 1, 4, 9, 16, 25]
plt.plot(x_values, y_values)
plt.show()
![Screenshot 2024-12-13 133146](https://github.com/user-attachments/assets/92a7f890-86c6-40d8-985f-61185e8bf061)

import matplotlib.pyplot as plt
x=[1,2,3]
y=[2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My first graph!')
plt.show()
![Screenshot 2024-12-13 133140](https://github.com/user-attachments/assets/053a5d1a-44ed-47d4-a234-10a95adc56a8)

x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line 1")
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line 2")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lineson same graph!')
plt.legend()
plt.show()
![Screenshot 2024-12-13 133134](https://github.com/user-attachments/assets/af576efc-4821-4ac8-a7c0-0c3666888e95)
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
![Screenshot 2024-12-13 133128](https://github.com/user-attachments/assets/2796054e-5593-4e9c-a6ab-5f69da31d95d)

yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
![Screenshot 2024-12-13 133121](https://github.com/user-attachments/assets/f115b06f-0350-4000-9a24-4d7c8d343aae)


years=[2010,2011,2012,2013,2014,2015]
yields=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years, yields)
![Screenshot 2024-12-13 133115](https://github.com/user-attachments/assets/1aa27cbb-de6e-4b3e-a32d-5dabfa6a4714)

years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.932,0.939]
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896]
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('years')
plt.ylabel('Yield (tons per hectare)');
![Screenshot 2024-12-13 133109](https://github.com/user-attachments/assets/34e2bbae-94e9-403a-b462-8b0332bdb299)

plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('years')
plt.ylabel('yield (tons per hectare)')
plt.title("crop yields in kanto")
plt.legend(['apples', 'oranges']);
![Screenshot 2024-12-13 133104](https://github.com/user-attachments/assets/ecfdb856-a6a5-4eb9-ae77-2f2ec150c638)

years=[2010,2011,2012,2013,2014,2015]
yields=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yields)
plt.xlabel('years')
plt.ylabel('yield (tons per hectare)');
![Screenshot 2024-12-13 133057](https://github.com/user-attachments/assets/9d5b7d2d-8363-43f7-a326-ce08e4b4f2d7)

years=range(2000,2012)
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896]
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.xlabel('years')
plt.ylabel('yield (tons per hectare)')
plt.title("Yields of Oranges (tons per hectare)");
![Screenshot 2024-12-13 133052](https://github.com/user-attachments/assets/4b9a1693-a482-4455-84c5-bf845e5d9afb)

years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.932,0.939]
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896]
plt.plot(years,apples,marker='o')
plt.plot(years,oranges,marker='x')
plt.xlabel('years')
plt.ylabel('yield (tons per hectare)')
plt.title("crops yields in kanto");
plt.legend(['apples','oranges'])
![Screenshot 2024-12-13 133045](https://github.com/user-attachments/assets/cad01f39-f59a-41ad-b248-bfacc361ccd6)

x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=30,color="blue")
plt.show()
![Screenshot 2024-12-13 133039](https://github.com/user-attachments/assets/13b92cf5-0b74-4b22-8918-7da032f58184)

x=[1,2,3,4,5,6,7,8,9,10]
y=[2,4,5,7,6,8,9,11,12,12]
plt.scatter(x,y,label="stars",color="green",marker="*",s=30)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My Scatter plot!')
plt.legend()
plt.show()
![Screenshot 2024-12-13 133032](https://github.com/user-attachments/assets/ee438d91-cbba-4abe-af76-e2cea9ed2a77)

import matplotlib.pyplot as plt
import numpy as np
import pandas as pd

x=np.arange(0,10)
y=np.arange(11,21)



x
![Screenshot 2024-12-13 133556](https://github.com/user-attachments/assets/40428cf2-e0be-412d-84a0-8845025c00bc)

y
![Screenshot 2024-12-13 133603](https://github.com/user-attachments/assets/8226a70e-e441-4409-b516-1c6ea0e718a0)

plt.scatter(x,y,c='r')
plt.xlabel('x axis')
plt.ylabel('y axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')

y=x*x
y

plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.title('2D diagram')
plt.ylabel('Y axis')
plt.xlabel('X axis')
![Screenshot 2024-12-13 133019](https://github.com/user-attachments/assets/4005f6e3-2c54-4fa4-bd1f-48e469a601bb)

plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*-')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
![Screenshot 2024-12-13 133013](https://github.com/user-attachments/assets/23e4a046-4dae-48ab-865f-ee8cb55c44b6)

np.pi
![Screenshot 2024-12-13 133411](https://github.com/user-attachments/assets/92052063-038b-41ce-99ab-e6e6bed0e532)

x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
![Screenshot 2024-12-13 133007](https://github.com/user-attachments/assets/dfad8bf8-3842-426d-8318-37454d13bca9)

import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
![Screenshot 2024-12-13 133000](https://github.com/user-attachments/assets/0bba06c2-a492-4f57-b380-25f464071330)

plt.stackplot(x,y1,y2,y3,labels=['Line 1','Line 2','Line 3'])
plt.legend(loc='upper left')
plt.title('Stacked Line Chart')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.show()
![Screenshot 2024-12-13 132954](https://github.com/user-attachments/assets/8e0a6aff-8269-41da-94fb-ccff3b809b94)

import numpy as np
import matplotlib.pyplot as plt
from scipy.interpolate import make_interp_spline
x=np.array([1,2,3,4,5,6,7,8,9,10])
y=np.array([2,4,5,7,8,8,9,10,11,12])
spl=make_interp_spline(x,y)
x_smooth = np.linspace(x.min(),x.max(),100)
y_smooth=spl(x_smooth)
plt.plot(x,y,'o',label='data')
plt.plot(x_smooth,y_smooth,'-',label='spline')
plt.legend()
plt.show()
![Screenshot 2024-12-13 132948](https://github.com/user-attachments/assets/6ff61bab-16d0-4c7d-8904-56c9883e9cd5)

import matplotlib.pyplot as plt
values=[5,6,3,7,2]
names=["A","B","C","D","E"]
plt.bar(names,values,color='green')
plt.show()
![Screenshot 2024-12-13 132942](https://github.com/user-attachments/assets/cbbba550-741b-4d5a-9e49-a72cfdee5d2e)

plt.barh(names,values,color='yellowgreen')
plt.show()
![Screenshot 2024-12-13 132936](https://github.com/user-attachments/assets/8cbb028c-82b2-40d6-805d-7a6371e23800)

height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-label')
plt.title('My barchart!')
plt.show()
![Screenshot 2024-12-13 132930](https://github.com/user-attachments/assets/7685e64f-d054-4d64-83ca-2fc39eb3c165)

x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('y axis')
plt.xlabel('x axis')
plt.show()
![Screenshot 2024-12-13 132924](https://github.com/user-attachments/assets/76a56b21-92f4-4c9b-85d4-197384b5e389)

ages=[2,5,70,40,30,45,50,45,43,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no. of people')
plt.title('My histogram')
plt.show()
![Screenshot 2024-12-13 132918](https://github.com/user-attachments/assets/f002550a-4433-4ba8-b54c-36d595a441bb)

x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='blue',alpha=0.5)
plt.show()
![Screenshot 2024-12-13 132913](https://github.com/user-attachments/assets/24b38010-f885-4ac5-bf43-3780f3982518)

import matplotlib.pyplot as plt
import numpy as np

np.random.normal(loc=0,scale=1,size=100)
data=np.random.normal(loc=0,scale=1,size=100)
data
![Screenshot 2024-12-13 132907](https://github.com/user-attachments/assets/5c626d2a-af1a-4d76-832b-2cb0ec177125)

fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Value')
ax.set_title('Box Plot')
plt.show()
![Screenshot 2024-12-13 132901](https://github.com/user-attachments/assets/551f5107-8553-4c38-bd98-c89584008551)

activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
![Screenshot 2024-12-13 132853](https://github.com/user-attachments/assets/033caddc-109e-4aa7-91c9-d934527c21e1)

labels='python','c++','c','java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
![Screenshot 2024-12-13 132848](https://github.com/user-attachments/assets/cf6f89e1-386f-46f1-b9e9-522c4ca9b276)

activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()![Screenshot 2024-12-13 132842](https://github.com/user-attachments/assets/328fef02-a4f4-4207-82a7-12b305effd9d)

# Result:
 The above code is executed successfully.
