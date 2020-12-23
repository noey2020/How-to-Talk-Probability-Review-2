# How-to-Talk-Probability-Review-2

December 23, 2020

I appreciate comments. Shoot me an email at noel_s_cruz@yahoo.com!

Hire me! 😊

- In our first probability review,
we talked about the notion of a probability space,
so now we are ready to move on to the next major concept,
which is that of a random variable.
What exactly is a random variable, and how do we compute
their expected value, variance, and standard deviation?
As usual, let's start with an example.
Suppose you roll two dice,
and you're interested in their sum.
Let's call this X.
So you aren't interested
in exactly what die one comes out to,
or die two comes out to,
just in what their sum is, just in what they add up to.
For example, if the first die is one and the second is one,
then X equals two.
If the first die is one and the second is two,
then X equals three, and so on.
This is a situation where the probability space
has 36 different outcomes: six choices for the first die,
and six choices for the second die.
But we're only interested
in a particular aspect of this outcome,
the sum of the two die,
and this aspect, which we call X,
can only take on 11 possible values:
two, three, all the way up to 12.
X is a random variable.
In general, when we have a probability space,
a random variable is any function of the outcome.
It captures some aspect of the outcome that we care about.
That's it.
Let's see how we can determine
the distribution of a random variable
from the information in the underlying probability space.
Here's another simple example.
We roll a die, and this time we don't care about
exactly what the die comes out to.
All we care about
is whether or not it's greater than or equal to three.
Given our interest,
the way we define a random variable is we say:
we have X,
and we're only gonna have it take on two possible values.
We'll say X is one
if the die is greater than or equal to three,
and otherwise X is zero.
So the random variable we've defined in this case
takes on values either zero or one,
and let's go ahead and compute its distribution.
The probability that X is zero
is the probability that this die comes out
to either one or two, which is 1/3,
and the probability that X is one
is simply the probability that the die comes out
to three, four, five, or six, which is 2/3.
In this way we can figure out
the distribution of a random variable
just by looking at the underlying probabilities of outcomes.
Once we have a random variable's distribution,
the next order of business
is usually to compute the expected value
of the random variable, also known as its mean.
The expected value of X is simply the average value of X
if we were to repeat the experiment
over and over and over again.
It is a weighted average
of all the possible values that X can take,
where each value is weighted
by its probability of occurring.
It's a simple formula, and let's see it in use.
Let's look at a simple example.
We roll a die, let X be the number observed.
What is its expected value?
In this case, X is something
that takes on values one, two, three, four, five, or six,
and so the expected value of X, plugging into this formula,
is simply an enumeration over all its possible values,
so it takes on value one with probability 1/6,
it takes on value two with probability 1/6,
three with probability 1/6, four times 1/6,
five times 1/6, and six times 1/6.
So you get the sum of numbers from one to six, which is
21,
so 21/6, which is 3.5,
and so that's the expected value of X.
Let's do another example.
This time you have a coin, but it's a biased coin,
so the chance that it comes up heads
is some number p, in the range zero to one.
You flip this coin,
and the random variable is
the random variable X is one if the coin comes up heads,
and zero if it comes up tails.
What is the expected value of X?
Once again, we just write out the formula.
We look at all the possible values that X can take.
It can take on the value zero,
or it can take on the value one.
The probability that it's zero is one minus p,
and the probability that it's one is p,
and so the expected value of X is p.
Now that we've some examples of expected values,
let's look at a key property of these means.
Suppose you have a bunch of numbers,
and you double all the numbers.
What happens to the average?
Well, if you double all the numbers,
the average also gets doubled.
What if, instead of doubling the numbers,
you increase every number by one.
What happens to the average?
So if every number increases by one,
then the average also increases by one.
Let's summarize this in a slightly more general way.
If you have any random variable X,
and you define a new random variable V,
to be some constant times X plus some other constant,
like two X plus one, or four X minus three,
what is the expected value of V?
What is the mean of V?
Can you figure it out from the mean of X?
Yes, it's simply the mean of X times a plus b,
and this is the linearity property
that helps simplify many calculations.
In general, a random variable X
can take on many possible values.
What if we just wanted
to summarize the distribution of X by a single number?
What number would we pick?
Probably its mean.
Let's go ahead and denote the mean by the Greek letter mu.
This is a nice summary.
This is a concise and useful summary,
but one of the things that it does not capture
is the spread of X.
Here's an example of two different distributions.
They both have exactly the same mean mu,
but the one on the left is much more tightly concentrated
around its mean,
while the one on the right is much more diffused.
They have the same mean, but their spread is very different.
So the mean isn't capturing
certain very important properties of the distribution.
What if we were allowed a second number
with which to summarize the distribution?
Could we pick a number that somehow captures this spread?
Here's an idea:
why not use the average distance from the mean?
So the expected value
of the absolute difference between X and its mean,
so in the distribution on the left,
the average distance of X from its mean
would probably be something like this,
whereas the distribution on the right,
the average distance of X from its mean
might be something like this.
This would actually work very well,
and we could certainly use it,
and in fact some people do use it,
but it turns out that mathematically it's more convenient
to look at the average square distance of X from the mean,
and this is what we call the variance of X.
The variance is the average square distance from the mean,
and we'll see some properties of this in a second.
Now intuitively, what we do want
is the typical distance from the mean,
rather than the typical square distance,
and so what we end up doing
is to take the square root of the variance,
and this is the standard deviation of X.
The standard deviation behaves in the way we'd want it to.
On the left, for example,
the standard deviation would be something small,
whereas on the right it's something larger.
Let's see how we'd compute these quantities
in a simple example.
We pick a random variable X
from one, two, three, four, five, all equally likely.
What is the variance of X?
The first thing we need to do
is to compute the expected value of X, the mean,
and in this case we'd expect it
to just be the number in the middle, which is three.
But let's double-check.
We'll plug it into the formula.
The expected value of X is enumerated
over all possible outcomes.
It's one with probability 1/5, two with probability 1/5,
three times 1/5, four times 1/5, and five times 1/5.
So you add up the numbers from one to five,
so that is nine and three,
15/5, which is three,
which is exactly what we expected.
Good.
Now we have the expected value of X.
This is what we've been calling mu.
To compute the variance,
we need the expected value
of X minus mu squared.
Let's look at the different values that X can take on,
and X minus mu squared.
When X is one, X minus mu squared,
so mu is equal to three, is two squared.
When X is two, X minus mu squared is one squared.
When X is three, X minus mu squared is zero squared.
Four, one squared.
And five, two squared.
So the expected value of X minus mu squared
well, X minus mu squared
can take on just three possible values: zero, one, or four.
It takes on value zero with probability 1/5,
that's this line of the table.
It takes on value one with probability 2/5,
that's these two lines of the table.
And it takes on value four with probability 2/5,
that's these two lines of the table.
So this works out to two.
So the variance of X is two,
which means that the standard deviation of X
is the square root of two.
The square root of the variance.
Let's look at some properties of the variance.
First of all, the variance is always a non-negative number.
Why?
Because it's the average square distance from the mean,
and the average of positive numbers has to be positive.
Then let's do the same thought experiment
we did with averages.
Suppose you have a bunch of numbers,
and you increase each number by one.
What happens to the variance?
If you increase each number by one,
everything shifts over a little bit,
but the spread remains the same,
so the standard deviation remains the same,
and the variance remains the same,
so the variance is unaffected if you shift numbers by one.
What happens if you double each number?
Well if you double the numbers,
then the spread also gets doubled,
so the standard deviation is doubled,
which means that the variance,
which is the square of the standard deviation
gets multiplied by four.
Let's summarize this by a general formula.
If you have a random variable X,
and then you define a new variable,
which is something like two X plus one,
or in general a X plus b,
then the variance of this new variable
is a squared times the variance of X.
There's one last property of variance
that will be very useful,
and that is that there's another formula for it.
There's a different way to calculate it.
It's this one over here.
The variance of X, it turns out,
is also the expected value of X squared
minus the mean squared.
It always works out to the same number.
Let's see this at work,
so let's go back to our earlier example,
where we chose X uniformly from one, two, three, four, five.
Now in this case, we saw that the variance was two,
using the original formula.
Let's try it again using the new formula.
What is the expected value of X squared?
X squared could be one squared with probability 1/5,
or two squared with probability 1/5,
or three squared with probability 1/5,
or four squared with probability 1/5,
or five squared with probability 1/5.
What does this work out to?
One plus four, plus nine,
plus 16, plus 25, over 5,
which is 55/5, which is 11.
So the variance of X
is the expected value of X squared minus mu squared.
Now mu is the mean, we already know that's three.
So it's 11 minus nine, which is two,
exactly as we got before.
We've seen some basic properties of random variables,
and next time we'll get to the situation
that we've gradually been building towards,
a situation where we have multiple random variables:
blood pressure, temperature, heart rate, disease,
and we're interested in how they interact with each other.
That's what we're gonna be needing
to build generative models in higher dimension.

I included some posts for reference.

https://github.com/noey2020/How-to-Talk-Generative-Modeling-in-One-Dimension

https://github.com/noey2020/How-to-Talk-Probability-Review-1

https://github.com/noey2020/How-to-Talk-Generative-Approach-to-Classification

https://github.com/noey2020/How-to-Talk-of-Fitting-a-Distribution-to-Data-

https://github.com/noey2020/How-to-Talk-of-Host-of-Prediction-Problems

https://github.com/noey2020/How-to-Talk-of-Useful-Distance-Functions

https://github.com/noey2020/How-to-Talk-of-Improving-Nearest-Neighbor

https://github.com/noey2020/How-to-Talk-of-Prediction-Problems

https://github.com/noey2020/How-to-Talk-Matlab-Tricks-and-Tweaks

https://github.com/noey2020/How-to-Talk-Trading-and-Investing

https://github.com/noey2020/How-to-Work-in-Matlab-Development-Environment

https://github.com/noey2020/How-to-Talk-Vaccines

https://github.com/noey2020/How-to-Talk-Regression-in-Matlab

https://github.com/noey2020/How-to-Get-Started-in-Matlab

https://github.com/noey2020/How-to-Convert-Data-from-Web-Service-Using-Matlab

https://github.com/noey2020/Quote-for-the-Day

https://github.com/noey2020/How-to-Talk-Good-Investment-Strategy

https://github.com/noey2020/How-to-Talk-of-Good-Plan

https://github.com/noey2020/Thought-for-the-Day

https://github.com/noey2020/How-to-Talk-Stock-Watch-of-the-Day

https://github.com/noey2020/How-to-Talk-Data-Science

https://github.com/noey2020/How-to-Talk-Fundamental-Analysis

https://github.com/noey2020/How-to-Read-Company-Profiles

https://github.com/noey2020/How-to-Import-Data-from-Spreadsheets-and-Text-Files-Matlab-Without-Coding

https://github.com/noey2020/How-to-Talk-Model-of-Stock-Market-Prices-

https://github.com/noey2020/How-to-Talk-Digital-Wallets

https://github.com/noey2020/How-to-Talk-Investing

https://github.com/noey2020/How-to-Double-Your-Money-in-5years

https://github.com/noey2020/How-to-Talk-Matlab

I appreciate comments. Shoot me an email at noel_s_cruz@yahoo.com!
