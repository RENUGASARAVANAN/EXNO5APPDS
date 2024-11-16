# EXNO5APPDS

# AIM:

      To implement Dashboards creation with Plotly and Dash using python.
      

# About Dash and Plotly tools:

Dash is a Python framework for building analytical web applications. Dash helps in building responsive web dashboards that is good to look at and is very fast without the need to understand complex front-end frameworks or languages such as HTML, CSS, JavaScript. Let’s build our first web dashboard using Dash.

Plotly library in Python is an open-source library that can be used for data visualization and understanding data simply and easily. Plotly supports various types of plots like line charts, scatter plots, histograms, box plots, etc.


# ALGORITHM:

Step 1: Import Necessary Library like dash and plotly.

Step 2: Load the dataset.

Step 3: Add dropdown using layout function and include the necessary options.

Step 4: Display the necessary visualization tools and include the necessary parameters.

Step 5: Display the output.


# PROGRAM:
```
Developed By: RENUGA S
Register No : 212222230118
```


# CODING :
```
pip install dash plotly pandas
import dash
from dash import dcc, html
from dash.dependencies import Input,Output
import plotly.express as px
import pandas as pd
import plotly.graph_objects as px
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df = sns.load_dataset('tips')
```

```
plot=px.Figure(data=[px.Scatter(x=df['day'],y=df['tip'],mode='markers')])
plot.update_layout(updatemenus=[dict(buttons=list([dict(args=["type","scatter"],label="Scatter Plot",method="restyle"),dict(args=["type","bar"],label="Bar Chart",method="restyle")]),direction="down",)])
plot.show()

```

```
import plotly.express as px
df=px.data.tips()
fig = px.bar(df, x='day',y='total_bill',color='sex',facet_row='time',facet_col='sex')
fig.show()
```

```
import plotly.express as px
df=px.data.tips()
fig = px.histogram(df, x='total_bill',color='sex',nbins=50,histnorm='percent',barmode='overlay')
fig.show()
```

```
import plotly.express as px
df=px.data.tips()
fig = px.pie(df, values='total_bill',names='day')
fig.show()

```

# OUTPUT :


<table>
<tr>
<td>
      
![Screenshot 2024-11-16 213614](https://github.com/user-attachments/assets/56c8fc0b-7ac0-4a87-9393-01fad3723ff1)


</td>

<td>
      
![Screenshot 2024-11-16 213628](https://github.com/user-attachments/assets/b35ddee2-f685-4eaf-9037-fceedd531831)


</td>
            
</tr>
</table>

![Screenshot 2024-11-16 213724](https://github.com/user-attachments/assets/24307ab5-00e0-4b07-8224-34b2c5753132)

![Screenshot 2024-11-16 213738](https://github.com/user-attachments/assets/4dd34c28-0424-4a08-a82f-3b76753d4ed4)

![Screenshot 2024-11-16 213834](https://github.com/user-attachments/assets/77ccf3a0-c272-4b7c-b286-902ada22a654)

![Screenshot 2024-11-16 213847](https://github.com/user-attachments/assets/c0cc111e-34de-485f-96d2-c12a0f7c9b03)




# RESULT:
Thus , To implement Dashboards creation with Plotly and Dash using python is successfully done.
