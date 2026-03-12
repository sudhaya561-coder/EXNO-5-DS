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
~~~ python
 
    import pandas as pd
    import numpy as np
    import matplotlib.pyplot as plt
    df=pd.read_csv('Iris.csv')

    plt.scatter(x,y,c='b')
    plt.xlabel('sepal_lenght')
    plt.ylabel('sepal_width')
    plt.title('Graph in 2D')
    plt.savefig('Test.png')
    y=x
    x=np.arange(1.5,9.5)
    y=np.arange(1.5,9.5)
    plt.plot(x,y,color='b',marker='o',linestyle='dashed',linewidth=1, markersize=8)
    plt.xlabel('sepal_lenght')
    plt.ylabel('sepal_width')
    plt.title('sepal_lenght vs sepal_width')
    plt.xlim(1.5,9.5)
    plt.ylim(2.5,4.5)
    plt.show()

    #pie
    count=df['sepal_width'].value_counts()
    plt.pie(count.values,labels=count.index,autopct='%1.0f%%',color=)
    plt.title('sepal_width distribution')
    plt.axis('equal')
    plt.show()
    # subplot with pie 
    plt.subplot(2,2,1)
    plt.plot(x,y,color='yellow',linestyle='--')
    plt.subplot(2,2,2)
    plt.plot(x,y,color='blue',linestyle='--',marker='o')
    plt.subplot(2,2,3)
    plt.plot(x,y,color='cyan',marker='^',linestyle='--')
    plt.subplot(2,2,4)
    plt.plot(x,y,color='magenta',linestyle='-')
    plt.show()
    plt.plot(x,y,marker='*',color="magenta",linestyle='dashed',linewidth=2, markersize=8) 
    plt.show()

    plt.scatter(data['sepal_length'], data['sepal_width'], c='yellow', edgecolor='purple')
    plt.xlabel('sepal_length')
    plt.ylabel('sepal_width')
    plt.title('sepal_length vs sepal_width')
    plt.show()

    x = np.arange(1,11) 
    y = 3 * x + 5 
    plt .title("Matplotlib demo") 
    plt.xlabel("x axis caption") 
    plt.ylabel("y axis caption") 
    plt.plot(x,y,color='darkgreen',linestyle='dashed',linewidth=2, markersize=8,marker='*')
    plt.show()
    # Compute the x and y coordinates for points on sine and cosine curves 
    x = np.arange(0, 5 * np.pi, 0.1) 
    y_cosh = np.cosh(x) 
    y_tanh = np.tanh(x)
 
   
    # Set up a subplot grid that has height 2 and width 1, 
    # and set the first such subplot as active. 
    plt.subplot(2, 1, 1)
   
    # Make the first plot 
    plt.plot(x, y_cosh,'b',marker='^') 
    plt.title('Cosh')  
   
    # Set the second subplot as active, and make the second plot. 
    plt.subplot(2, 1, 2) 
    plt.plot(x, y_tanh,color='r',marker='*') 
    plt.title('Tanh')  
    plt.show()
    
    ## Bar plot

    plt.bar(df['sepal_length'],df['petal_length'], color = 'gold',edgecolor='black') 

    plt.title('Bar graph') 
    plt.ylabel('Y axis') 
    plt.xlabel('X axis')  
    plt.show()

    a = df['sepal_length'].values
    plt.hist(a,color='cyan',edgecolor='black') 
    plt.title("HISTOGRAM",color='green') 
    plt.xlabel('SEPAL_LENGTH',color='red')
    plt.ylabel('SEPAL_WIDTH',color='blue')
    plt.show()

    # Data to plot
    labels = 'sepal_length', 'sepal_width', 'petal_length', 'petal_width'
    sizes=df['sepal_length'].count(),df['sepal_width'].count(),df['petal_length'].count(),df['petal_width'].count()
    colors = ['purple', 'darkorange', 'darkgreen', 'red']
    explode = (0.4, 0, 0, 0)  # explode 1st slice

    # Plot
    plt.pie(sizes, explode=explode, labels=labels, colors=colors,
    autopct='%1.1f%%', shadow=False,wedgeprops={'edgecolor':'black'})

    plt.axis('equal')
    plt.show()
~~~
# output:
[vertopal.com_mathplotlib (1).pdf](https://github.com/user-attachments/files/25597833/vertopal.com_mathplotlib.1.pdf)

<img width="707" height="567" alt="Screenshot 2026-02-27 132057" src="https://github.com/user-attachments/assets/2e01eafb-9cbf-40f9-be7f-52246c7d024e" />

<img width="695" height="559" alt="Screenshot 2026-02-27 132104" src="https://github.com/user-attachments/assets/f9e7d395-ff53-49fa-890b-09563eea7212" />

<img width="675" height="519" alt="Screenshot 2026-02-27 132118" src="https://github.com/user-attachments/assets/4718de1b-f831-4046-a292-20d05065114a" />

<img width="644" height="480" alt="Screenshot 2026-02-27 132045" src="https://github.com/user-attachments/assets/3cf35ebe-4394-4c9b-8443-005fbc629bc2" />

### Result:
successfully Performed Data Visualization using matplot python library for the given data.
