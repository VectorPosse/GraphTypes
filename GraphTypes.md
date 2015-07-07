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

* Quantitative (numeric, scale, interval/ratio)

Numerical measurements, usually with meaningful units.

> height, GDP, score


Identifying variable types
========================================================
transition: none

**CAREFUL!**

Numbers are not always quantitative.

> *Do you own a car?*
>> 0 = "No", 1 = "Yes"

> *What is your zip code?*

Data set
========================================================

Risk factors associated with low infant birth weight, collected at Baystate Medical Center, Springfield, Mass during 1986.

189 women measured on 10 variables.


Single variable
========================================================
type: section

* Single variables usually won't answer very interesting questions by themselves.
* Graphs of single variables are often valuable for exploring your data, but generally not suitable for inclusion in the final product.


Single categorical variable
========================================================


Single categorical variable
========================================================
transition: none

Mother's race (white, black, or other)


```
Source: local data frame [189 x 1]

    race
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

Single categorical variable
========================================================
transition: none

* Frequency table

<!-- html table generated in R 3.2.1 by xtable 1.7-4 package -->
<!-- Mon Jul 06 17:43:25 2015 -->
<table border=1>
<tr> <th> Race </th> <th> Count </th>  </tr>
  <tr> <td> White </td> <td align="right">  96 </td> </tr>
  <tr> <td> Black </td> <td align="right">  26 </td> </tr>
  <tr> <td> Other </td> <td align="right">  67 </td> </tr>
   </table>


Single categorical variable
========================================================
transition:none

* Bar chart

![plot of chunk unnamed-chunk-4](GraphTypes-figure/unnamed-chunk-4-1.png) 


Single categorical variable
========================================================
transition:none

* <s>Pie chart</s> **Danger! Danger!**

![plot of chunk unnamed-chunk-5](GraphTypes-figure/unnamed-chunk-5-1.png) 


Single categorical variable
========================================================
transition:none

* Relative frequency table

<!-- html table generated in R 3.2.1 by xtable 1.7-4 package -->
<!-- Mon Jul 06 17:43:25 2015 -->
<table border=1>
<tr> <th> Race </th> <th> Count </th> <th> Percent </th>  </tr>
  <tr> <td> White </td> <td align="right">  96 </td> <td align="right"> 0.51 </td> </tr>
  <tr> <td> Black </td> <td align="right">  26 </td> <td align="right"> 0.14 </td> </tr>
  <tr> <td> Other </td> <td align="right">  67 </td> <td align="right"> 0.35 </td> </tr>
   </table>


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

Infant birth weight in grams


```
Source: local data frame [189 x 1]

    bwt
1  2523
2  2551
3  2557
4  2594
5  2600
6  2622
7  2637
8  2637
9  2663
10 2665
..  ...
```


Single quantitative variable
========================================================
transition:none

* Histogram

![plot of chunk unnamed-chunk-8](GraphTypes-figure/unnamed-chunk-8-1.png) 


Single quantitative variable
========================================================
transition:none

* Tabular summaries

("Five-number summary" or other quantiles)

<table border=1>
<tr> <th>  </th> <th> Birth Weight (gm) </th>  </tr>
  <tr> <td align="right"> 0% </td> <td align="right"> 709 </td> </tr>
  <tr> <td align="right"> 5% </td> <td align="right"> 1801 </td> </tr>
  <tr> <td align="right"> 25% </td> <td align="right"> 2414 </td> </tr>
  <tr> <td align="right"> 50% </td> <td align="right"> 2977 </td> </tr>
  <tr> <td align="right"> 75% </td> <td align="right"> 3487 </td> </tr>
  <tr> <td align="right"> 95% </td> <td align="right"> 3997 </td> </tr>
  <tr> <td align="right"> 100% </td> <td align="right"> 4990 </td> </tr>
   </table>


Single quantitative variable
========================================================
transition:none

* A bunch of other types I don't prefer:

> boxplot, stem-and-leaf plot, dotplot


Multiple variables
========================================================
type: section

There are at least six elements of a plot that can be assigned to variables:

* x-axis
* y-axis
* facets
* color/fill
* size
* shape (e.g., dots vs crosses, solid vs dashed lines, etc.)

Two categorical variables
========================================================


Two categorical variables
========================================================
transition: none

Mother's race and the number of previous premature labors.


```
Source: local data frame [189 x 2]

    race ptl
1  Black   0
2  Other   0
3  White   0
4  White   0
5  White   0
6  Other   0
7  White   0
8  Other   0
9  White   0
10 White   0
..   ... ...
```


Two categorical variables
========================================================
transition: none

* Side-by-side bar chart (okay)

![plot of chunk unnamed-chunk-11](GraphTypes-figure/unnamed-chunk-11-1.png) 


Two categorical variables
========================================================
transition: none

* Side-by-side bar chart (better)

![plot of chunk unnamed-chunk-12](GraphTypes-figure/unnamed-chunk-12-1.png) 


Two categorical variables
========================================================
transition: none

* <s>Stacked bar chart</s> **Danger! Danger!**

![plot of chunk unnamed-chunk-13](GraphTypes-figure/unnamed-chunk-13-1.png) 


One categorical and one quantitative variable
========================================================


One categorical and one quantitative variable
========================================================
transition: none

Mother's race and infant birth weight in grams


```
Source: local data frame [189 x 2]

    race  bwt
1  Black 2523
2  Other 2551
3  White 2557
4  White 2594
5  White 2600
6  Other 2622
7  White 2637
8  Other 2637
9  White 2663
10 White 2665
..   ...  ...
```


One categorical and one quantitative variable
========================================================
transition: none

* Side-by-side boxplot

![plot of chunk unnamed-chunk-15](GraphTypes-figure/unnamed-chunk-15-1.png) 


One categorical and one quantitative variable
========================================================
transition: none

* Stacked histogram (okay)

![plot of chunk unnamed-chunk-16](GraphTypes-figure/unnamed-chunk-16-1.png) 


One categorical and one quantitative variable
========================================================
transition: none

* Stacked histogram (better)

![plot of chunk unnamed-chunk-17](GraphTypes-figure/unnamed-chunk-17-1.png) 


Two quantitative variables
========================================================


Two quantitative variables
========================================================
transition: none

Mother's age and infant birth weight


```
Source: local data frame [189 x 2]

   age  bwt
1   19 2523
2   33 2551
3   20 2557
4   21 2594
5   18 2600
6   21 2622
7   22 2637
8   17 2637
9   29 2663
10  26 2665
.. ...  ...
```


Two quantitative variables
========================================================
transition: none

* Scatterplot

![plot of chunk unnamed-chunk-19](GraphTypes-figure/unnamed-chunk-19-1.png) 


Two quantitative variables
========================================================
transition: none

* If one variable is ordered (like time) and there is only one observation of y for each x value, use a lineplot.

![plot of chunk unnamed-chunk-20](GraphTypes-figure/unnamed-chunk-20-1.png) 

Three or more variables
========================================================

![plot of chunk unnamed-chunk-21](GraphTypes-figure/unnamed-chunk-21-1.png) 


Three or more variables
========================================================
transition: none

![plot of chunk unnamed-chunk-22](GraphTypes-figure/unnamed-chunk-22-1.png) 
