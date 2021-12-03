# Challenge_11
Growth Analysis of MercadoLibre Based on Google Search Traffic

This project is built to analyze hourly Google search trend data and stock closing prices for MercadoLibre to detect trends and predict potential forecasts for both. It uses the FBProphet library to build the model and provide answers to the research questions presented throughout the project file. In addition to the trend and stock data, there is also an analysis and model built to provide a revenue growth forecast for MercadoLibre. 

The project first analyzes time series patterns and trends in the hourly data and across the seasons and relates them to trends within the stock price data. It provides an analysis of the correlation between the two across the timeframe. It then builds a model and near-term forecast prediction for the hourly Google search trend data. Finally, it builds another model based on the revenue data to predict potential cases for revenue growth over the next quarter.


---

## Technologies

This project is built in Python 3.6 and designed to be run in Google Colab. In order to properly utilize the project, the following Python libraries will be used:

   [pandas](https://pandas.pydata.org/docs/)

   [hvplot](https://hvplot.holoviz.org/user_guide/index.html)

   [holoviews](https://holoviews.org/index.html)
   
   [pystan](https://pystan.readthedocs.io/en/latest/)
   
   [fbprophet](https://facebook.github.io/prophet/)
   
   [datetime](https://docs.python.org/3/library/datetime.html)


---

## Installation Guide

This project requires the user to install the additional libraries not included in the base version of Python run by Google Colab. The project contains the code to succesfully install the required libraries and it is listed below. Be sure to run these lines of code before running the imports and project. 

```python
  
  # Install the required libraries
  from IPython.display import clear_output
  try:
    !pip install pystan
    !pip install fbprophet
    !pip install hvplot
    !pip install holoviews
  except:
   print("Error installing libraries")
  finally:
    clear_output()
    print('Libraries successfully installed')

```


---

## Usage

This project can be run by opening Google Colab within the user's web browser and opening the notebook file, forecasting_net_prophet.ipynb. Be sure to run each cell from start to finish beginning with the installation code shown above. This will ensure succesful running of the project and provide the user with the contained data anlysis and predictions. 


---

## Contributors

Briggs Lalor
email: briggsclalor@gmail.com

---

## License

MIT License

Copyright (c) [2021] [Briggs Lalor]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
