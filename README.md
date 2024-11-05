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
~~~
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1, y1, label='line 1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2, y2, label='line 2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph')
plt.legend()
~~~
![Screenshot 2024-10-23 101407](https://github.com/user-attachments/assets/cb3bec44-f73b-466b-821e-c91b96c2b175)
~~~
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y, color='blue', linestyle='dashed', linewidth=3, marker='o', markerfacecolor='red', markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customization')
~~~
![Screenshot 2024-10-23 101439](https://github.com/user-attachments/assets/790905fb-050c-4351-86b3-96a214c4294b)
~~~
years=range(2000, 2012)
apples=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931, 0.934, 0.936, 0.937, 0.9375, 0.9372, 0.939]
oranges=[0.962, 0.941, 0.930, 0.923, 0.918, 0.908, 0.907, 0.904, 0.901, 0.898, 0.9, 0.896]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectre)')
plt.title('Crops yield in Kento')
plt.legend(['Apples', 'Oranges'])
~~~
![Screenshot 2024-10-23 101506](https://github.com/user-attachments/assets/67137c40-c5c2-440a-a1d0-d672638ef19b)
~~~
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
~~~
![Screenshot 2024-10-23 101535](https://github.com/user-attachments/assets/fbd68a5f-619b-49ec-ab91-3183393639ae)
~~~
import numpy as np
np.pi
~~~
![Screenshot 2024-10-23 101556](https://github.com/user-attachments/assets/4443771a-e863-4e07-be0f-2446304de462)
~~~
x=np.arange(0,4 * np.pi, 0.1)
y=np.sin(x)
plt.title('Sine Wave form')
plt.plot(x,y,'g--', linewidth=3)
~~~
![Screenshot 2024-10-23 101620](https://github.com/user-attachments/assets/208c7ab4-44c8-4fd8-b691-8b5fb07ece4f)
~~~
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='pink')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
~~~
![Screenshot 2024-10-23 101701](https://github.com/user-attachments/assets/a201dd20-dd0d-49a6-b314-79ba38221ee1)
~~~
plt.stackplot(x,y1,y2,y3,labels=['Line1','Line2', 'Line3'])
plt.legend(loc='upper left')
plt.title('Stacked Line Chart')
plt.xlabel('X-axis')
plt.xlabel('Y-axis')
~~~
![Screenshot 2024-10-23 101725](https://github.com/user-attachments/assets/c0c1d90e-df57-4772-8530-703395cb6d4e)
~~~
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar Graph')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
~~~
![Screenshot 2024-10-23 101806](https://github.com/user-attachments/assets/9721d47f-a059-4b03-b8bb-08ca1d197748)
~~~
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
~~~
![Screenshot 2024-10-23 101829](https://github.com/user-attachments/assets/4c64d3d5-3b87-4002-91a3-d03cdcc4227e)
~~~
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,80,19,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no. of. people')
plt.title('My Histogram')
~~~
![Screenshot 2024-10-23 101851](https://github.com/user-attachments/assets/c6bcddbd-af8c-4cb0-91c7-9939fbc1829a)
~~~
x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10, color='blue',alpha=0.5)
~~~
![Screenshot 2024-10-23 101913](https://github.com/user-attachments/assets/8ebc390e-e93b-48a7-9ca7-96484117decf)
~~~
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
~~~
![Screenshot 2024-10-23 101935](https://github.com/user-attachments/assets/30a3d46e-b6ed-462f-a4b4-2831a73c46df)
~~~
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
~~~
![Screenshot 2024-10-23 101957](https://github.com/user-attachments/assets/554d93cc-bbdd-4b4d-8850-49ea9cb21983)
~~~
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
~~~
![Screenshot 2024-10-23 102020](https://github.com/user-attachments/assets/c01c117d-f3bd-403e-b4a1-9d3918a2fa00)
~~~
labels='Python', 'C++', 'Ruby', 'Java'
sizes=[215, 130, 245, 210]
colors=['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
~~~
![Screenshot 2024-10-23 102042](https://github.com/user-attachments/assets/e98a9499-0190-4264-b275-1c0cefa8abb4)

# Result:
 Thus Data Visualization using matplot python library for the given datas was executed successfully.
