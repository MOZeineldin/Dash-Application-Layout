# Dash-Application-Layout
Creation of Dash Application Layout
# Install python packages required to run the application.
python3.8 -m pip install packaging
python3.8 -m pip install pandas dash
pip3 install httpx==0.20 dash plotly

theia@theia-mohamedzeine:/home/project$ python3.8 -m pip install packaging
Defaulting to user installation because normal site-packages is not writeable
Requirement already satisfied: packaging in /home/theia/.local/lib/python3.8/site-packages (21.3)
Requirement already satisfied: pyparsing!=3.0.5,>=2.0.2 in /home/theia/.local/lib/python3.8/site-packages (from packaging) (3.0.9)

[notice] A new release of pip is available: 23.0.1 -> 24.0
[notice] To update, run: python3.8 -m pip install --upgrade pip
theia@theia-mohamedzeine:/home/project$ python3.8 -m pip install --upgrade pip
Defaulting to user installation because normal site-packages is not writeable
Requirement already satisfied: pip in /usr/local/lib/python3.8/dist-packages (23.0.1)
Collecting pip
  Downloading pip-24.0-py3-none-any.whl (2.1 MB)
     ━━━━━━━━━━━━━━ 2.1/2.1 MB 42.5 MB/s eta 0:00:00
Installing collected packages: pip
Successfully installed pip-24.0

[notice] A new release of pip is available: 23.0.1 -> 24.0
[notice] To update, run: python3.8 -m pip install --upgrade pip
theia@theia-mohamedzeine:/home/project$ python3.8 -m pip install pandas dash
Defaulting to user installation because normal site-packages is not writeable
Collecting pandas
  Downloading pandas-2.0.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.metadata (18 kB)
Collecting dash
  Downloading dash-2.17.0-py3-none-any.whl.metadata (10 kB)
Requirement already satisfied: python-dateutil>=2.8.2 in /home/theia/.local/lib/python3.8/site-packages (from pandas) (2.8.2)
Requirement already satisfied: pytz>=2020.1 in /home/theia/.local/lib/python3.8/site-packages (from pandas) (2022.1)
Collecting tzdata>=2022.1 (from pandas)
  Downloading tzdata-2024.1-py2.py3-none-any.whl.metadata (1.4 kB)
Collecting numpy>=1.20.3 (from pandas)
  Downloading numpy-1.24.4-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.metadata (5.6 kB)
Requirement already satisfied: Flask<3.1,>=1.0.4 in /home/theia/.local/lib/python3.8/site-packages (from dash) (2.2.2)
Requirement already satisfied: Werkzeug<3.1 in /home/theia/.local/lib/python3.8/site-packages (from dash) (2.2.2)
Collecting plotly>=5.0.0 (from dash)
  Downloading plotly-5.22.0-py3-none-any.whl.metadata (7.1 kB)
Collecting dash-html-components==2.0.0 (from dash)
  Downloading dash_html_components-2.0.0-py3-none-any.whl.metadata (3.8 kB)
Collecting dash-core-components==2.0.0 (from dash)
  Downloading dash_core_components-2.0.0-py3-none-any.whl.metadata (2.9 kB)
Collecting dash-table==5.0.0 (from dash)
  Downloading dash_table-5.0.0-py3-none-any.whl.metadata (2.4 kB)
Requirement already satisfied: importlib-metadata in /home/theia/.local/lib/python3.8/site-packages (from dash) (4.12.0)
Requirement already satisfied: typing-extensions>=4.1.1 in /home/theia/.local/lib/python3.8/site-packages (from dash) (4.3.0)
Requirement already satisfied: requests in /home/theia/.local/lib/python3.8/site-packages (from dash) (2.28.0)
Collecting retrying (from dash)
  Downloading retrying-1.3.4-py3-none-any.whl.metadata (6.9 kB)
Requirement already satisfied: nest-asyncio in /home/theia/.local/lib/python3.8/site-packages (from dash) (1.5.6)
Requirement already satisfied: setuptools in /home/theia/.local/lib/python3.8/site-packages (from dash) (67.4.0)
Requirement already satisfied: Jinja2>=3.0 in /home/theia/.local/lib/python3.8/site-packages (from Flask<3.1,>=1.0.4->dash) (3.1.2)
Requirement already satisfied: itsdangerous>=2.0 in /home/theia/.local/lib/python3.8/site-packages (from Flask<3.1,>=1.0.4->dash) (2.1.2)
Requirement already satisfied: click>=8.0 in /home/theia/.local/lib/python3.8/site-packages (from Flask<3.1,>=1.0.4->dash) (8.1.3)
Requirement already satisfied: zipp>=0.5 in /home/theia/.local/lib/python3.8/site-packages (from importlib-metadata->dash) (3.8.1)
Requirement already satisfied: tenacity>=6.2.0 in /home/theia/.local/lib/python3.8/site-packages (from plotly>=5.0.0->dash) (8.0.1)
Requirement already satisfied: packaging in /home/theia/.local/lib/python3.8/site-packages (from plotly>=5.0.0->dash) (21.3)
Requirement already satisfied: six>=1.5 in /home/theia/.local/lib/python3.8/site-packages (from python-dateutil>=2.8.2->pandas) (1.16.0)
Requirement already satisfied: MarkupSafe>=2.1.1 in /home/theia/.local/lib/python3.8/site-packages (from Werkzeug<3.1->dash) (2.1.1)
Requirement already satisfied: charset-normalizer~=2.0.0 in /home/theia/.local/lib/python3.8/site-packages (from requests->dash) (2.0.12)
Requirement already satisfied: idna<4,>=2.5 in /home/theia/.local/lib/python3.8/site-packages (from requests->dash) (3.3)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in /home/theia/.local/lib/python3.8/site-packages (from requests->dash) (1.26.11)
Requirement already satisfied: certifi>=2017.4.17 in /home/theia/.local/lib/python3.8/site-packages (from requests->dash) (2022.6.15)
Requirement already satisfied: pyparsing!=3.0.5,>=2.0.2 in /home/theia/.local/lib/python3.8/site-packages (from packaging->plotly>=5.0.0->dash) (3.0.9)
Downloading pandas-2.0.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (12.4 MB)
   ━━━━━━━━━━━━━ 12.4/12.4 MB 112.6 MB/s eta 0:00:00
Downloading dash-2.17.0-py3-none-any.whl (7.5 MB)
   ━━━━━━━━━━━━━━━━ 7.5/7.5 MB 86.0 MB/s eta 0:00:00
Downloading dash_core_components-2.0.0-py3-none-any.whl (3.8 kB)
Downloading dash_html_components-2.0.0-py3-none-any.whl (4.1 kB)
Downloading dash_table-5.0.0-py3-none-any.whl (3.9 kB)
Downloading numpy-1.24.4-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl (17.3 MB)
   ━━━━━━━━━━━━━━ 17.3/17.3 MB 80.1 MB/s eta 0:00:00
Downloading plotly-5.22.0-py3-none-any.whl (16.4 MB)
   ━━━━━━━━━━━━━━ 16.4/16.4 MB 67.0 MB/s eta 0:00:00
Downloading tzdata-2024.1-py2.py3-none-any.whl (345 kB)
   ━━━━━━━━━━━━━ 345.4/345.4   31.0 MB/s eta 0:00:00
                 kB                                 
Downloading retrying-1.3.4-py3-none-any.whl (11 kB)
Installing collected packages: dash-table, dash-html-components, dash-core-components, tzdata, retrying, numpy, plotly, pandas, dash
Successfully installed dash-2.17.0 dash-core-components-2.0.0 dash-html-components-2.0.0 dash-table-5.0.0 numpy-1.24.4 pandas-2.0.3 plotly-5.22.0 retrying-1.3.4 tzdata-2024.1
theia@theia-mohamedzeine:/home/project$ pip3 install httpx==0.20 dash plotly
Defaulting to user installation because normal site-packages is not writeable
Collecting httpx==0.20
  Downloading httpx-0.20.0-py3-none-any.whl.metadata (49 kB)
     ━━━━━━━━━━━━━ 49.5/49.5 kB 6.2 MB/s eta 0:00:00
Requirement already satisfied: dash in /home/theia/.local/lib/python3.8/site-packages (2.17.0)
Requirement already satisfied: plotly in /home/theia/.local/lib/python3.8/site-packages (5.22.0)
Requirement already satisfied: certifi in /home/theia/.local/lib/python3.8/site-packages (from httpx==0.20) (2022.6.15)
Requirement already satisfied: charset-normalizer in /home/theia/.local/lib/python3.8/site-packages (from httpx==0.20) (2.0.12)
Requirement already satisfied: sniffio in /home/theia/.local/lib/python3.8/site-packages (from httpx==0.20) (1.2.0)
Requirement already satisfied: rfc3986<2,>=1.3 in /home/theia/.local/lib/python3.8/site-packages (from rfc3986[idna2008]<2,>=1.3->httpx==0.20) (1.5.0)
Collecting httpcore<0.14.0,>=0.13.3 (from httpx==0.20)
  Downloading httpcore-0.13.7-py3-none-any.whl.metadata (13 kB)
Requirement already satisfied: Flask<3.1,>=1.0.4 in /home/theia/.local/lib/python3.8/site-packages (from dash) (2.2.2)
Requirement already satisfied: Werkzeug<3.1 in /home/theia/.local/lib/python3.8/site-packages (from dash) (2.2.2)
Requirement already satisfied: dash-html-components==2.0.0 in /home/theia/.local/lib/python3.8/site-packages (from dash) (2.0.0)
Requirement already satisfied: dash-core-components==2.0.0 in /home/theia/.local/lib/python3.8/site-packages (from dash) (2.0.0)
Requirement already satisfied: dash-table==5.0.0 in /home/theia/.local/lib/python3.8/site-packages (from dash) (5.0.0)
Requirement already satisfied: importlib-metadata in /home/theia/.local/lib/python3.8/site-packages (from dash) (4.12.0)
Requirement already satisfied: typing-extensions>=4.1.1 in /home/theia/.local/lib/python3.8/site-packages (from dash) (4.3.0)
Requirement already satisfied: requests in /home/theia/.local/lib/python3.8/site-packages (from dash) (2.28.0)
Requirement already satisfied: retrying in /home/theia/.local/lib/python3.8/site-packages (from dash) (1.3.4)
Requirement already satisfied: nest-asyncio in /home/theia/.local/lib/python3.8/site-packages (from dash) (1.5.6)
Requirement already satisfied: setuptools in /home/theia/.local/lib/python3.8/site-packages (from dash) (67.4.0)
Requirement already satisfied: tenacity>=6.2.0 in /home/theia/.local/lib/python3.8/site-packages (from plotly) (8.0.1)
Requirement already satisfied: packaging in /home/theia/.local/lib/python3.8/site-packages (from plotly) (21.3)
Requirement already satisfied: Jinja2>=3.0 in /home/theia/.local/lib/python3.8/site-packages (from Flask<3.1,>=1.0.4->dash) (3.1.2)
Requirement already satisfied: itsdangerous>=2.0 in /home/theia/.local/lib/python3.8/site-packages (from Flask<3.1,>=1.0.4->dash) (2.1.2)
Requirement already satisfied: click>=8.0 in /home/theia/.local/lib/python3.8/site-packages (from Flask<3.1,>=1.0.4->dash) (8.1.3)
Requirement already satisfied: h11<0.13,>=0.11 in /home/theia/.local/lib/python3.8/site-packages (from httpcore<0.14.0,>=0.13.3->httpx==0.20) (0.12.0)
Requirement already satisfied: anyio==3.* in /home/theia/.local/lib/python3.8/site-packages (from httpcore<0.14.0,>=0.13.3->httpx==0.20) (3.6.1)
Requirement already satisfied: idna>=2.8 in /home/theia/.local/lib/python3.8/site-packages (from anyio==3.*->httpcore<0.14.0,>=0.13.3->httpx==0.20) (3.3)
Requirement already satisfied: zipp>=0.5 in /home/theia/.local/lib/python3.8/site-packages (from importlib-metadata->dash) (3.8.1)
Requirement already satisfied: MarkupSafe>=2.1.1 in /home/theia/.local/lib/python3.8/site-packages (from Werkzeug<3.1->dash) (2.1.1)
Requirement already satisfied: pyparsing!=3.0.5,>=2.0.2 in /home/theia/.local/lib/python3.8/site-packages (from packaging->plotly) (3.0.9)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in /home/theia/.local/lib/python3.8/site-packages (from requests->dash) (1.26.11)
Requirement already satisfied: six>=1.7.0 in /home/theia/.local/lib/python3.8/site-packages (from retrying->dash) (1.16.0)
Downloading httpx-0.20.0-py3-none-any.whl (82 kB)
   ━━━━━━━━━━━━━━━ 82.5/82.5 kB 8.5 MB/s eta 0:00:00
Downloading httpcore-0.13.7-py3-none-any.whl (58 kB)
   ━━━━━━━━━━━━━━━ 58.8/58.8 kB 6.8 MB/s eta 0:00:00
Installing collected packages: httpcore, httpx
  Attempting uninstall: httpcore
    Found existing installation: httpcore 0.15.0
    Uninstalling httpcore-0.15.0:
      Successfully uninstalled httpcore-0.15.0
  Attempting uninstall: httpx
    Found existing installation: httpx 0.23.0
    Uninstalling httpx-0.23.0:
      Successfully uninstalled httpx-0.23.0
ERROR: pip's dependency resolver does not currently take into account all the packages that are installed. This behaviour is the source of the following dependency conflicts.
datasette 0.59.1 requires click<8.1.0,>=7.1.1, but you have click 8.1.3 which is incompatible.
datasette 0.59.1 requires Jinja2<3.1.0,>=2.10.3, but you have jinja2 3.1.2 which is incompatible.
Successfully installed httpcore-0.13.7 httpx-0.20.0
theia@theia-mohamedzeine:/home/project$


# Import required packages
import pandas as pd
import plotly.express as px
import dash
from dash import dcc
from dash import html

# Read the airline data into pandas dataframe
airline_data =  pd.read_csv('https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DV0101EN-SkillsNetwork/Data%20Files/airline_data.csv', 
                            encoding = "ISO-8859-1",
                            dtype={'Div1Airport': str, 'Div1TailNum': str, 
                                   'Div2Airport': str, 'Div2TailNum': str})

# Randomly sample 500 data points. Setting the random state to be 42 so that we get same result.
data = airline_data.sample(n=500, random_state=42)

# Pie Chart Creation
fig = px.pie(data, values='Flights', names='DistanceGroup', title='Distance group proportion by flights')

# Error Message
theia@theia-mohamedzeine:/home/project$ /usr/bin/python3
Python 3.6.9 (default, Nov 25 2022, 14:10:45) 
[GCC 8.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> fig = px.pie(data, values='Flights', names='DistanceGroup', title='Distance group proportion by flights')
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'px' is not defined
>>> theia@theia-mohamedzeine:/home/project$ /usr/bin/python3
Python 3.6.9 (default, Nov 25 2022, 14:10:45) 
[GCC 8.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> fig = px.pie(data, values='Flights', names='DistanceGroup', title='Distance group proportion by flights')
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'px' is not defined
>>> theia@theia-mohamedzeine:/home/project$ /usr/bin/python3
Python 3.6.9 (default, Nov 25 2022, 14:10:45) 
[GCC 8.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> fig = px.pie(data, values='Flights', names='DistanceGroup', title='Distance group proportion by flights')
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'px' is not defined
>>> 
