---
layout: post
title:  "Seaborn Colormaps"
date:   2020-03-06 02:56:43 +0530
category : visualizations
author: "Rajaram Parab"
---


<div class="jumbotron">
  <h1>Be Colorful!!! </h1>
  <p>
    <h2>Seaborn.heatmap </h2>
    <h5>Colormap(cmap) Examples</h5>
    <p>Seaborn Heatmap is used to visualize Numerical Data where 
      each cell is colored based on the value it contains. <br>
      
      When we plot Seaborn Heatmap and want to make it colorful.
      then we often try out defferent inbuilt cmaps.
      Just see how they look and choose your cmap!
  <br>Check these Out : </p>
    
  <div class="row">
      <div class="col-lg-4">
        Make necessary imports: <br>
          <div id="codeblock">
            
  <code>import numpy as np <br>
    import pandas as pd <br>
    import matplotlib.pyplot as plt <br>
    import seaborn as sns <br>
    %matplotlib inline</code>
  </div>
</div>

<div class="col-lg-8">
Here we are creating dummy data to visualize heatmap as below(Changing cmap Gives the result as below): <br>
    <div id="codeblock">               
    <code>df = pd.DataFrame(np.random.random((10,10)), columns=["a","b","c","d","e","f","g","h","i","j"]) <br>
      customfontdict={'family': 'fantasy','color':  'blue', 'weight': 'bold','size':60} <br>
      plt.figure(figsize=(20,15),edgecolor='black')<br>
      sns_plot=sns.heatmap(df,cmap='Accent')<br>
      plt.title('Accent',fontdict=customfontdict,y=-0.01) </code>
    </div>
  </div>
</div>

<div class="container pt-3 text-center">
  <div class="row pt-3" >
  <div id="plot" class="col-sm"></div>
  <div id="plot" class="col-sm"></div>
  <div id="plot" class="col-sm"></div>
  <div id="plot" class="col-sm"></div>
  </div>
  <div class="row pt-3" >
  <div id="plot" class="col-sm"></div>
  <div id="plot" class="col-sm"></div>
  <div id="plot" class="col-sm"></div>
  <div id="plot" class="col-sm"></div>
  </div>

  <div class="row btn-group  p-3">
  <button id="prev" onclick=prevImage() type="button" class="btn btn-primary p-3 btn-block">Previous</button>
  <button id="next" onclick=nextImage() type="button" class="btn btn-primary p-3 btn-block">Next</button>
    </div>
  </div>
</div>
