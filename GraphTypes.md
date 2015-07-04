Graph Types
========================================================
author: QUARC data visualization workshop
date: July 7, 2015






Identifying variable types
========================================================


Identifying variable types
========================================================
transition: none

* Categorical (nominal, qualitative, factor)

Classifies data by category.

> color, species, sex

* Quantitative (numeric, interval/scale)

Numerical measurements, usually with meaningful units.

> height, GDP, score


Identifying variable types
========================================================
transition: none

**CAREFUL!**

Numerical data is not always quantitative.

> *Do you own a car?*
>> 0 = "No", 1 = "Yes"

> *What is your zip code?*


Single variable
========================================================
type: section

* Single variables generally won't answer very interesting questions by themselves.
* Graphs of single variables are often valuable for exploring your data, but generally not suitable for inclusion in the final product.


Single categorical variable
========================================================


Single categorical variable
========================================================
transition: none


```
Source: local data frame [189 x 1]

    Race
1  Black
2  Other
3  White
4  White
5  White
6  Other
7  White
8  Other
9  White
10 White
..   ...
```

***

Table

<!-- html table generated in R 3.2.1 by xtable 1.7-4 package -->
<!-- Sat Jul 04 16:28:07 2015 -->
<table border=1>
<tr> <th> Race </th> <th> Count </th>  </tr>
  <tr> <td> White </td> <td align="right">  96 </td> </tr>
  <tr> <td> Black </td> <td align="right">  26 </td> </tr>
  <tr> <td> Other </td> <td align="right">  67 </td> </tr>
   </table>


Single categorical variable
========================================================
transition:none


```
Source: local data frame [189 x 1]

    Race
1  Black
2  Other
3  White
4  White
5  White
6  Other
7  White
8  Other
9  White
10 White
..   ...
```

***

Bar chart

![plot of chunk unnamed-chunk-5](GraphTypes-figure/unnamed-chunk-5-1.png) 


Single categorical variable
========================================================
transition:none


```
Source: local data frame [189 x 1]

    Race
1  Black
2  Other
3  White
4  White
5  White
6  Other
7  White
8  Other
9  White
10 White
..   ...
```

***

Pie chart

![plot of chunk unnamed-chunk-7](GraphTypes-figure/unnamed-chunk-7-1.png) 

**Danger! Danger!**

Single categorical variable
========================================================
transition:none

* Why do pie charts suck?

> ["Pie Charts Are the Worst"](http://www.businessinsider.com/pie-charts-are-the-worst-2013-6)

> ["Countdown of Top 10 Reasons to Never Ever Use a Pie Chart"](https://blogs.oracle.com/experience/entry/countdown_of_top_10_reasons_to_never_ever_use_a_pie_chart)

> ["Save the Pies for Dessert"](http://www.perceptualedge.com/articles/visual_business_intelligence/save_the_pies_for_dessert.pdf)

* And to be fair, one guy who defends pie charts:

> ["Why Tufte is Flat-Out Wrong about Pie Charts"](http://speakingppt.com/2013/03/18/why-tufte-is-flat-out-wrong-about-pie-charts/)


Single quantitative variable
========================================================
transition:none


Single quantitative variable
========================================================
transition:none


```
Source: local data frame [189 x 1]

   birth_weight
1          2523
2          2551
3          2557
4          2594
5          2600
6          2622
7          2637
8          2637
9          2663
10         2665
..          ...
```

***

Histogram

![plot of chunk unnamed-chunk-9](GraphTypes-figure/unnamed-chunk-9-1.png) 


Single quantitative variable
========================================================
transition:none


```
Source: local data frame [189 x 1]

   birth_weight
1          2523
2          2551
3          2557
4          2594
5          2600
6          2622
7          2637
8          2637
9          2663
10         2665
..          ...
```

***

Tabular summaries

* Five-number summary (or use other quantiles)

<table border=1>
<tr> <th>  </th> <th> Birth Weight (gm) </th>  </tr>
  <tr> <td align="right"> 0% </td> <td align="right"> 709.00 </td> </tr>
  <tr> <td align="right"> 25% </td> <td align="right"> 2414.00 </td> </tr>
  <tr> <td align="right"> 50% </td> <td align="right"> 2977.00 </td> </tr>
  <tr> <td align="right"> 75% </td> <td align="right"> 3487.00 </td> </tr>
  <tr> <td align="right"> 100% </td> <td align="right"> 4990.00 </td> </tr>
   </table>

Single quantitative variable
========================================================
transition:none

* Bunch of other types I don't prefer:

> boxplot, stem-and-leaf plot, dotplot
