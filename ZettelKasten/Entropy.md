202409251103
Status: #idea
Tags: [[math]]
# Surprise
If an event is rare, we will be very surprised when it happens. 
If we know the chance of the event is 1 or 100%, there will be no surprise when it happens.
If an event happens 5 times, the surprise will increase by 5 times
$$h(x) = \log \left( \frac{1}{p(x)} \right)$$
# Entropy
Entropy is the weighted average sum of surprise.
$$\text{Entropy} = \sum p(x_i) \cdot h(x_i) = \sum p(x_i) \log \left( \frac{1}{p(x_i)} \right)$$
# Cross Entropy
When we have believe Q, and the practical event P. 
We can calculate the weighted average sum of surprise of event P on our believe Q.
$$\text{CrossEntropy(P, Q)} = \sum p_P(x_i) \cdot h_Q(x_i) = \sum p_P(x_i) \log \left( \frac{1}{p_Q(x_i)} \right)$$

# KL divergent
Show the difference between 2 distributions by CrossEntropy remove the entropy of data.
$$ KL(P, Q) = CrossEntropy(P, Q) - Entropy(P) $$ $$= \sum p_P(x_i) \log \left( \frac{1}{p_Q(x_i)} \right) - \sum p_P(x_i) \log \left( \frac{1}{p_P(x_i)} \right) $$ $$ = \sum p_P(x_i) \log \left( \frac{p_P(x_i)}{p_Q(x_i)} \right)$$


---
# Reference
1. Entropy
![Entropy](https://www.youtube.com/watch?v=KHVR587oW8I)