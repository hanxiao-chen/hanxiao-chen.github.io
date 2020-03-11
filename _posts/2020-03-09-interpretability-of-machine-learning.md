---
layout: post
title: Interpretability of machine learning
subtitle: A mind map
comments: true
image: /img/inter_img2.png
---

![map](/img/inter_map.png){: .center-block :}

# Opacity of 3 dimensions:
1. Some parties want to keep their models confidential.
2. Some people do not understand code, math, and models.
3. It is hard to interpret some models like neural network.
*For AI community, **Interpretability** usually mean the 3rd dim of opacity.*

# Interpretability
### What is interpretability?
Degree of human comprehensibility of a model

### Why do we need interpretability?
Incompleteness in problem formalization

### How to evaluate it? 
Three methods

### Factors influence interpretability
- Task-related

- Method-related 

### Solutions
- Avoid using ML. ML is useful only if the task we are dealing with cannot be formulated specifically.

- Simplify model. A simple model is as accurate as a complex model sometimes (usually require domain knowledge).

- Using approximate methods. (LIME, Shap, etc.)

# Explanation
- Philosophically, The approximate models mentioned here are limited to scientific explanations.

- Contrastive approaches should be applied as new alternatives.


# Reference
[1] Mittelstadt, Brent and Russell, Chris and Wachter, Sandra, Explaining Explanations in AI (November 4, 2018). Proceedings of FAT* ’19: Conference on Fairness, Accountability, and Transparency (FAT* ’19), January 29–31, 2019, Atlanta, GA, USA. ACM, New York, NY, USA, doi/10.1145/3287560.3287574, ISBN: 978-1-4503-6125-5. Available at SSRN: https://ssrn.com/abstract=3278331

[2] Burrell, J. (2016). How the machine ‘thinks’: Understanding opacity in machine learning algorithms. Big Data & Society. https://doi.org/10.1177/2053951715622512

[3] Finale Doshi-Velez and Been Kim(2017), Towards A Rigorous Science of Interpretable Machine Learning. arXiv. https://arxiv.org/abs/1702.08608 
