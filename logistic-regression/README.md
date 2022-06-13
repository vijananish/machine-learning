# LOGISTIC REGRESSION

# Introduction
LogistIc regression is a classifiaction technique. It is simple and geometrically elegant algorithm.
LR: Geometric Intuition
Logistic Regression
1. Geometry (Visual)
2. Probability
3. Loss Function

If we have two classes of points let it be positive and negative classes. Inorder to seperate we can draw hyperplane and in 2-D it is line and for n-D it is hperplane and n-1-D to seperate. If the data is linearly seperable or alomost linearly seperable then plane or line are called linear surfaces. Quadratic surfaces are parabola, circle.

A plane can be represented by

```plane:(w, b)``` where ```w is normal``` to plane and ```b is intercept```.

Therefor as per equation of line which is ```y=mx+c``` so this can be represented as ```y=transpose(w)x+c```

If the equation passes through origin ```b=0``` therefor ```transpose(w)x=0``` so ```transpose(w)x+c=0```

In the equation ```x is vector belongs to R```, ```w is vector belongs to R``` and ```c is scalar```.

Assumption according to LR is classes are almost/perfect Linearly Separable.

![alt text](https://automaticaddison.com/wp-content/uploads/2019/07/linearly-separable.png)

Let x(i) be a point with distance d(i) from plane. 

Let y(i) = +1 for positive and -1 for negative therefor y(i) belongs {-1, 1}

![alt text](https://miro.medium.com/max/952/1*rMUBWr-6RF04TajdS0P32A.jpeg)

d(i)  = transpose(w)x(i)/||w||; Lets assume w is normal to plane and ||w||=1 therefore unit vector.

Therefor ```d(i) = transpose(w)*x(i) > 0``` since it is in direction of w i.e. positive then y(i) = +1

Similarly ```d(j) = transpose(w)*x(i) < 0``` since it is in opposite direction of w i.e. negative then y(i) = -1

Case:1 ------> y(i)*transpose(w)*x(i) > 0 if y(i) = +1 and transpose(w)*x(i) > 0 then we can say that ```w```  is correctly classifying the data.

Case:2 ------> if y(i) = -1 and transpose(w)*x(i) < 0 its concluding that x(i) is negative point then y(i)*transpose(w)*x(i) > 0 

``` y(i)transpose(w)x(i) > 0 means model is correctly classifying the data```

Case:3 ------> if y(i) = +1 and transpose(w)*x(i) < 0 its concluding that x(i) is negative point then y(i)*transpose(w)*x(i) < 0. There fore this is mis-classified point as actual is +1 but LR is negative.

Case:4 ------> if y(i) = -1 and transpose(w)*x(i) > 0 its concluding that x(i) is positive point then y(i)*transpose(w)*x(i) < 0. There fore this is miscalssified point as actual is -1 but LR is positive.

Classifier to be classifier to be good: if min number of mis-classification and max number of correct classification.

So we can see:

max ∑ y(i)*transpose(w)*x(i) where ```x(i)``` and ```y(i)``` are fixed and only variable that varies is ```w```

We need to find the optimal ```w(^*)``` = arg max ∑ y(i)*transpose(w)*x(i) here wwhat value of ```w``` maximises the value to solve optimization.