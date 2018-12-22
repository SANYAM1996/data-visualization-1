import requests
import json
import matplotlib.pyplot as plt
a = requests.get('https://www.quandl.com/api/v3/datasets/OPEC/ORB.json?api_key=Uz15XqryNcxxwRgva6jx&start_date=1970-01-01&end_date=1970-01-01')
b = json.loads(a.text)
my_data = b['dataset']['data']
useful_data = [i[1] for i in my_data]
x_data = [i for i in range(len(useful_data))
plt.plot ('x_data','useful_data')
plt.show()
