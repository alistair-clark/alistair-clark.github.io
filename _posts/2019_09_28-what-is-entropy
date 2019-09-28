---
layout: post
title: What is Entropy?
---

Imagine you're in school and you have an important test next week. The test could cover five topics, but you only have time to study one. So, which topic should you study?

Like the diligent student that you are, you go digging for some information. First, you talk to your **teacher**. They say,
> "The test could cover any of the topics we've discussed in class."

Not much help there... Next, you go knocking on your **TAs** door, and they give you a helpful hint:
> "There's an 80% chance the test is going to focus on only topic 1."

Nice! Instead of choosing a topic to study at random, now you can be pretty sure that you should study topic 1. Finally, you visit your **friend**, who says,
>"I stole a copy of the test and ALL the questions are on topic 1."

Setting aside the ethical dilemma you're now facing, at least now you know *exactly* what topic to study!

This is a simple example, but it reveals our intuitive understanding of the relationship between probabilities and uncertainty.

1. **Uncertainty is highest** when the probabilities of all outcomes are the same. In our example, this was when we had no idea which of the 5 topics would be on the test.
2. **Uncertainty goes down** when the probabilities are unevenly distributed. In our example, this was when the TA told us there is an 80% chance that the test covers topic 1.
3. **Uncertainty is zero** when the probability of a specific outcome is equal to one. In our example, this was when our friend told us there is a 100% chance that the test covers topic 1.


<img src="img/probability_and_uncertainty.png" alt="Probability and Uncertainty" width="800"/>

Got it? Great, because if you understand that, you already understand entropy.


### Entropy = Uncertainty

In plain english, **entropy is a way to measure uncertainty.** Instead of using vague terms like, "I'm pretty sure X will happen" or "I have no idea what will happen", entropy gives us a tool for quantifying how uncertain or certain we are.

For example, I can take our three scenarios from above, plug them into the formula for entropy, and it spits out a real number.

|Scenario|Entropy|
|---|:---:|
|All 5 topics have a $p=0.2$ of being on the test|2.32|
|Topic 1 has a $p=0.8$ of being on the test|1.12|
|Topic 1 has $p=1$ of being on the test|0|

Here's the formula used to calculate entropy: $S=-\sum _{i}P_{i}\log {P_{i}}$, where $P_i$ equals the probability of each outcome. The focus of this article is on the intuition behind entropy, so I won't get into the mathematical reasons for why this formula makes sense. If you want to learn more, [others have written about it extensively](https://towardsdatascience.com/entropy-is-a-measure-of-uncertainty-e2c000301c2c), and [R](https://www.rdocumentation.org/packages/DescTools/versions/0.99.19/topics/Entropy) and [Python](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.entropy.html) come with packages for calculating it precisely. For now, just marvel at the fact that entropy let's us apply *real numbers* to an abstract concept like uncertainty.

An entropy value of 2.32 or 1.12 doesn't mean much on its own, but when used as an input to certain machine learning algorithms it becomes a powerful tool for solving problems.

### Entropy and the application to data science

Data science is about tackling questions where uncertainty and entropy are high: Does this patient have cancer? Will the stock market go up or down tomorrow? Is this email spam? In order to answer these questions confidently, we need to reduce the amount of uncertainty (and therefore entropy).

**Decision trees** are a popular method for answering questions like these. And one way to construct decision trees is using entropy. For example, the [ID3 algorithm](https://en.wikipedia.org/wiki/ID3_algorithm#Summary) uses a simple 4 step process for constructing decision trees by selecting features that will result in the highest reduction in entropy. This is repeated for each split of the tree until entropy is low and we can confidently predict the outcome.

### If you remember one thing, remember this...

Entropy = uncertainty.

1. **<strike>Uncertainty</strike> Entropy is highest** when the probabilities of all outcomes are the same.
2. **<strike>Uncertainty</strike> Entropy goes down** when the probabilities are unevenly distributed.
3. **<strike>Uncertainty</strike> Entropy is zero** when the probability of a specific outcome is equal to one.

If you remember this, you'll know more about entropy than most people who work in data science.

Now that you have an intuitive understanding of what entropy is, test your knowledge by reading this 1948 paper titled ["A Mathematical Theory of Communication"](http://www.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf). It was written by Claude Shannon, the man who introduced the concept of entropy as it relates to probability. Specifically read the section titled *CHOICE, UNCERTAINTY AND ENTROPY*, and see if you can map your current understanding of entropy to some of the more technical definitions he provides.

Let me know how it goes!
