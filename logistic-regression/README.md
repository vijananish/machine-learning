# LOGISTIC REGRESSION

# Introduction
LogistIc regression is a classification technique. It is simple and geometrically elegant algorithm.
LR: Geometric Intuition
Logistic Regression
1. Geometry (Visual)
2. Probability
3. Loss Function

If we have two classes of points let it be positive and negative classes. Inorder to separate we can draw hyperplane and in 2-D it is line and for n-D it is hyperplane and n-1-D to separate. If the data is linearly separable or almost linearly separable then plane or line are called linear surfaces. Quadratic surfaces are parabola, circle.

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

Case:4 ------> if y(i) = -1 and transpose(w)*x(i) > 0 its concluding that x(i) is positive point then y(i)*transpose(w)*x(i) < 0. There fore this is mis-classified point as actual is -1 but LR is positive.

Classifier to be classifier to be good: if min number of mis-classification and max number of correct classification.

So we can see:

max ∑ y(i)*transpose(w)*x(i) where ```x(i)``` and ```y(i)``` are fixed and only variable that varies is ```w```

We need to find the optimal ```w(^*)``` = arg max ∑ y(i)*transpose(w)*x(i) here what value of ```w``` maximises the value to solve optimization.

## Squashing and Sigmoid Function

optimal(W) maximises  = argmax(∑ y(i)transpose(w)x(i))

y(i)transpose(w)x(i) = signed distance

transpose(w)x(i) distance from c(i) to plane (w is unit vector)

![alt text](https://qphs.fs.quoracdn.net/main-qimg-12534c8eed0cc147aeaa0504ea0d2b88)

Let's assume a plane and all points i.e. positive(5 points) and negative(5 points) at a distance 1 and there is one negative point at a distance of 100 in positive side(mis classified) so as per oue objective:

So, 1+1+1+1+1+1+1+1+1+1-100 = -90

argmax(∑ y(i)transpose(w)x(i)) with all the positive and negative points will make it negative so......

We can think max sum of signed distance.

Let's make another plane i.e. plane2 and say make all the classified points as positive and mis classified point as negative:
    
Here ∑ y(i)transpose(w)x(i) so positive and negative cancel each other and that mis-classifier will make it positive

= 1+2+3+4+5-1-2-3-4-5+1 = +1

From above two as per our objective plane2 is better classifier but intuitively plane1 is better as it classifies more points correctly.

In Plane 1 accuracy = 10/11

In plane 2 accuracy = 6/11

Because of argmax(∑ y(i)transpose(w)x(i)) plane2 is favoured due to single outlier point. Thus, this is not outlier prone.

## SQUASHING

In order to overcome outlier we use squashing.

Instead of using signed distance: If signed distance is small use at it is and if large make it small.

If the value is larger than threshold taper it off.

![alt text](https://www.justintodata.com/wp-content/uploads/2020/05/logistic-function.png)

We can use sigmoid function for values:

![alt text](https://miro.medium.com/max/1400/1*a04iKNbchayCAJ7-0QlesA.png)

here
```
min = -1
max = +1
at 0 it is 0.5
```

So the equation becomes:

```argmax(∑ sigmoid(y(i)transpose(w)x(i)))```

## Optimization Problem

Here we use monotonic function:

A function g(x) is monotonic as x increases g(x) also increases not necessarily linearly or as x decreases g(x) decreases.

log(x) for x>0 is monotonic increasing function.

Therefore ```argmin f(x) = argmin g(f(x))```

We can think f(x) = x^2 and g(x) = ln(x) so argmin x^2 = argmin ln(x^2)

Similarly ```argax f(x) = argmax g(f(x))```

So as per our objective ```argmax(∑ sigmoid(y(i)transpose(w)x(i)))```

so use g(x) = ln(x)

also argmax ```f(x) = -argmin f(x)```

optimized w = argmin ∑(log(1+e^(-y(i)transpose(w)x(i))))

here y(i) = +1 or -1

as per geometry

If 1 is not there in sigmoid then equation becomes: then this becomes same as original equation without squashing.

As per probability:

```
optimized w = argmin ∑(-y(i)log(p(i)) - (i-y(i))log(1-p(i))) 
here y(i) = +1 or 0
p(i) = sigmoid(transpose(w)x(i))
```

## Interpretation of 'w'

Case 1: If w(i) = +ve, x(qi) increases the w(i)*x(qi) increases

Therefore ∑(w(i)*x(qi)) increases then sigmoid(w(i)*x(qi)) increases and P(y(i)=+1) increases.

Case 2: If w(i) = -ve, x(qi) increases the w(i)*x(qi) decreases

Therefore ∑(w(i)x(qi)) decreases then sigmoid(w(i)x(qi)) decreases and P(y(i)=+1) decreases and P(y(i)=-1) increases.

```P(y(i)=+1) = 1-P(y(i)=-1)```