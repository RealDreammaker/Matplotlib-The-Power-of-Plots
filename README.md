# Matplotlib - The Power of Plots

## Background

Pymaceuticals Inc. specializes in anti-cancer pharmaceuticals. In its most recent efforts, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

In their most recent animal study, 249 mice identified with SCC tumor growth were treated through a variety of drug regimens. Over the course of 45 days, tumor development was observed and measured. The purpose of this study was to compare the performance of Pymaceuticals' drug of interest, Capomulin, versus the other treatment regimens. 

## Requirements
The required task is to generate all of the tables and figures needed for the technical report of the study. The executive team also has asked for a top-level summary of the study results.

## Outcomes
Please see [notebooks](pymaceuticals_starter.ipynb) for more details 

### Initial Preparation

Merge DataFrames, remove duplicate data and use cleaned dataframe for futher analaysis.
</br>
<img src="images\pie_chart.png" width="40%" height="40%">
</br>

### Summary Statistics

1.	From the summary statistic table below, the average tumour volume appeared smallest in mouse treated with Ramicane, Capomulin, Propriva, Ceftamin and Infubinol. This proves the effectiveness of these drugs in reducing tumour volume in mouse.
<table class="dataframe" border="1">
  <thead>
    <tr style="text-align: right;">
      <td>Drug Regimen</td>
      <td>mean</td>
      <td>variance</td>
      <td>standard deviation</td>
      <td>SEM</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Capomulin</td>
      <td>40.675741</td>
      <td>24.947764</td>
      <td>4.994774</td>
      <td>0.329346</td>
    </tr>
    <tr>
      <td>Ceftamin</td>
      <td>52.591172</td>
      <td>39.290177</td>
      <td>6.268188</td>
      <td>0.469821</td>
    </tr>
    <tr>
      <td>Infubinol</td>
      <td>52.884795</td>
      <td>43.128684</td>
      <td>6.567243</td>
      <td>0.492236</td>
    </tr>
    <tr>
      <td>Ketapril</td>
      <td>55.235638</td>
      <td>68.553577</td>
      <td>8.279709</td>
      <td>0.603860</td>
    </tr>
    <tr>
      <td>Naftisol</td>
      <td>54.331565</td>
      <td>66.173479</td>
      <td>8.134708</td>
      <td>0.596466</td>
    </tr>
    <tr>
      <td>Placebo</td>
      <td>54.033581</td>
      <td>61.168083</td>
      <td>7.821003</td>
      <td>0.581331</td>
    </tr>
    <tr>
      <td>Propriva</td>
      <td>52.393463</td>
      <td>43.138803</td>
      <td>6.568014</td>
      <td>0.525862</td>
    </tr>
    <tr>
      <td>Ramicane</td>
      <td>40.216745</td>
      <td>23.486704</td>
      <td>4.846308</td>
      <td>0.320955</td>
    </tr>
    <tr>
      <td>Stelasyn</td>
      <td>54.233149</td>
      <td>59.450562</td>
      <td>7.710419</td>
      <td>0.573111</td>
    </tr>
    <tr>
      <td>Zoniferol</td>
      <td>53.236507</td>
      <td>48.533355</td>
      <td>6.966589</td>
      <td>0.516398</td>
    </tr>
  </tbody>
</table>

2.	Ramicane on average reduces tumour volume more than Capomulin. However, from the bar chart Timepoints by drug regimen below, it shows that mouse is less likely to die in drug regime Capomulin compared to Ramicane (230 versus 228 timepoints).
</br>
<img src="images\bar_chart.png" width="80%" height="80%">
</br>
Therefore, it is safest to treat tumour with Capomulin.
</br>
<img src="images\line_chart.png" width="80%" height="80%">
</br>


3.	The average tumour volume in mouse strongly and positively corelates to the mouse weight (r = 0.84) and it can be estimated based on a linear equation: y = 0.95x + 21.55 (x: mouse weight, y: average tumour volume)
</br>
<img src="images\linear_regression.png" width="80%" height="80%">
</br>
4.	From whisker box, we found only one outliner from Infubinol regimen, this means that the above statistical analysis is not negatively bias by outliners
</br>
<img src="images\box_plot.png" width="80%" height="80%">
</br>
