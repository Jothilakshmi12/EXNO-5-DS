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
```
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```
```
x = [1, 2, 3, 4, 5]
y = [3, 6, 2, 7, 1]
```
```
plt.plot(x,y,label='line1')
```

![Screenshot 2025-05-06 112052](https://github.com/user-attachments/assets/4a1daedb-40d8-4327-9fc5-dd4760fe6214)

```
x1 = [1,2,3]
y1 = [2,4,1]
x2 = [1,2,3]
y2 = [4,1,3]
```
```
plt.plot(x1,y1,label='line1')
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```

![Screenshot 2025-05-06 112421](https://github.com/user-attachments/assets/b7c4fce5-491e-4dd4-ba09-96b7feb827a9)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
```

![Screenshot 2025-05-06 112514](https://github.com/user-attachments/assets/45f3cf7b-0633-45bd-9b09-62ecde117231)

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```

![Screenshot 2025-05-06 112610](https://github.com/user-attachments/assets/ea14ddba-cc56-4421-83f4-7633ddc62848)

```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```

![Screenshot 2025-05-06 112706](https://github.com/user-attachments/assets/10374ac0-6295-4a7d-9342-33137841370d)

```
ars=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);
```

![Screenshot 2025-05-06 112806](https://github.com/user-attachments/assets/d9969610-763c-4bfd-a1a9-73d8499e195b)

```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```

![Screenshot 2025-05-06 112921](https://github.com/user-attachments/assets/16b3d01e-00a3-491d-a9f0-d7c3a591e8a2)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```

![Screenshot 2025-05-06 113003](https://github.com/user-attachments/assets/da1503e6-873c-4acd-863d-f3ff803040ce)

```
y
```

![Screenshot 2025-05-06 113053](https://github.com/user-attachments/assets/5f7486cf-9076-4521-8c89-c648f3b2bf56)

```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```

![Screenshot 2025-05-06 113144](https://github.com/user-attachments/assets/f35a0bab-7b6c-4db3-9447-41d843764c35)

```
y=x*x
y
```

![Screenshot 2025-05-06 113220](https://github.com/user-attachments/assets/dfd328db-1f53-4d45-bfbd-a78a88d27b04)

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.legend(['y-values']);
```

![Screenshot 2025-05-06 113302](https://github.com/user-attachments/assets/804e32a3-5266-412d-8056-31c6c4b7fd4e)

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```

![Screenshot 2025-05-06 113354](https://github.com/user-attachments/assets/fa844e1b-9f4a-49ae-830f-5ddd3124e521)

```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
```

![Screenshot 2025-05-06 113515](https://github.com/user-attachments/assets/674365ab-bcdc-4a0e-976b-023cc70becdd)

```
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
```

![Screenshot 2025-05-06 113725](https://github.com/user-attachments/assets/ab85b3a6-678e-4d96-bccb-c2e3f1e2c1dc)

```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```

![Screenshot 2025-05-06 113805](https://github.com/user-attachments/assets/8569b5fd-1458-4a77-8cb3-9f8802cc00d6)

```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```

![Screenshot 2025-05-06 113853](https://github.com/user-attachments/assets/6962dd92-64f9-4258-8d94-7dc10d76cac6)

```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```

![Screenshot 2025-05-06 114017](https://github.com/user-attachments/assets/367b9c19-2984-401f-a947-b650b1163a72)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```

![Screenshot 2025-05-06 114104](https://github.com/user-attachments/assets/5d15097e-80f8-46e2-9ee7-99f75fe648a0)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

![Screenshot 2025-05-06 114150](https://github.com/user-attachments/assets/2eb893c4-fe0c-412e-8545-aa2b1c55f92d)

```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
```
```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```

![Screenshot 2025-05-06 114241](https://github.com/user-attachments/assets/5f6e7bb5-8238-4003-aa41-98d8baa446b4)

```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```

![Screenshot 2025-05-06 114334](https://github.com/user-attachments/assets/27cf54d0-8065-4807-aff1-87dfaeb006a7)



# Result:
Thus, the Data Visualization using matplot python library has successfully executed.
