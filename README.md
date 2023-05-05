<h1 align="center"> Appliance Detection Benchmark </h1>

<p align="center">
    <img width="450" src="https://github.com/adrienpetralia/ApplianceDetectionBenchmark/blob/master/ressources/Intro.png" alt="Intro image">
</p>

<h2 align="center">Appliance Detection Using Very Low-Frequency Smart Meter Time Series (ACM e-Energy '23) </h2>

### Abstract

In recent years, smart meters have been widely adopted by electricity suppliers to improve the management of the smart grid system. 
These meters usually collect energy consumption data at a very low frequency (every 30min), enabling utilities to bill customers more accurately. 
To provide more personalized recommendations, the next step is to detect the appliances owned by customers, which is a challenging problem, due to the very-low meter reading frequency.
Even though the appliance detection problem can be cast as a time series classification problem, with many such classifiers having been proposed in the literature, no study has applied and compared them on this specific problem.
This paper presents an in-depth evaluation and comparison of state-of-the-art time series classifiers applied to detecting the presence/absence of diverse appliances in very low-frequency smart meter data. 
We report results with five real datasets. 
We first study the impact of the detection quality of 13 different appliances using 30min sampled data, and we subsequently propose an analysis of the possible detection performance gain by using a higher meter reading frequency. 
The results indicate that the performance of current time series classifiers varies significantly. 
Some of them, namely deep learning-based classifiers, provide promising results in terms of accuracy (especially for certain appliances), even using 30min sampled data, and are scalable to the large smart meter time series collections of energy consumption data currently available to electricity suppliers.
Nevertheless, our study shows that more work is needed in this area to further improve the accuracy of the proposed solutions. 

### Prerequisites 

Python version : <code> >= Python 3.7 </code>

Overall, the required python packages are listed as follows:

<ul>
    <li><a href="https://numpy.org/">numpy</a></li>
    <li><a href="https://pandas.pydata.org/">pandas</a></li>
    <li><a href="https://scikit-learn.org/stable/">sklearn</a></li>
    <li><a href="https://imbalanced-learn.org/stable/">imbalanced-learn</a></li>
    <li><a href="https://pytorch.org/docs/1.8.1/">pytorch==1.8.1</a></li>
    <li><a href="https://pypi.org/project/torchinfo/0.0.1/">torchinfo</a></li>
    <li><a href="https://scipy.org/">scipy</a></li>
    <li><a href="http://www.sktime.net/en/latest/">sktime</a></li>
    <li><a href="https://matplotlib.org/">matplotlib</a></li>
</ul>

### Installation

Use pip to install all the required libraries listed in the requirements.txt file.

<code> pip install -r requirements.txt </code>

### Data
The data used in this project comes multiple sources:

<ul>
  <li>CER smart meter dataset from the ISSDA archive.</li>
  <li>REFIT smart meter dataset.</li>
  <li>UKDALE smart meter dataset.</li>
  <li>Private smart meter dataset provide by EDF (Electricité De France).</li>
</ul> 

To download the preprocessed subsample of the CER dataset (data/labels) :

<code>cd data</code>

Copy and paste the data from the link drive folder indicate in the README.md file.

### References:
If you re-use this work, please cite:
