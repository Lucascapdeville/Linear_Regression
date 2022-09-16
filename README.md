# Linear regression model 

# Intro

This project has the objective to improve my skills in training a linear regression model 

# Project objective

Predict the price of the diamonds in data/rick_diamonds.csv using the information from data/diamonds.csv

## Methods
Linear regression
### Technologies
pandas
sklearn


# Project Description
Using the data from previous diamonds information predict the price of a list of diamonds that cointains:
Price:Price in Us dollars
Carat:Weitght of the diamond
Cut: Quality of the cut(Fair,Good,Very Good,Premium,Ideal)
Color:Diamond colour,from J(worst) to D(best)
Clarity: A measurement of how clear the diamond is(I1(worst),SI2,SI1,VS2,VS1,VVS2,VVS1,IF(best))
x:Length in mm
y:Width in mm
z:Depth in mm
Depth:Total depth percentage = z/mean(x,y) = 2*z/(x+y)(43-79)
Table: Width of top of diamond relative to widest point(43-95)

## Steps
1 - Price predicted as the mean of prices from diamonds.csv(3980)

2 - Price predicted using carat as the only variable from diamonds.csv(1605)

3 - Price predicted using carat and depth variables from diamonds.csv(1598)

4 - Price predicted using carat and table variables from diamonds.csv(1595)

5 - Price predicted using carat,table and depth variables from diamonds.csv(1583)

6 - Price predicted using carat,table,depth and clarity variables from diamonds.csv(1217); Cut does not seen to influence the model

7 - Price predicted using carat,table,depth, clarity and color variables from diamonds.csv(987); Cut does not seen to influence the model

8 - Price predicted using carat,table,depth,x, clarity and color variables from diamonds.csv(709); Cut does not seen to influence the model

X was the missing piece in this linear regression model

9 - Price predicted using carat,table,depth,x, clarity , color and cut(grouped by Fair and Good) variables from diamonds.csv(688)

# Conclusion
Using most of the data of the original DataFrame impoved significantly the preciseness of the model.

But the breakthrought point was understand how the 'x' is especially important when you start to add categorical data