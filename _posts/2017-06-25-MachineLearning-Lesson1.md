# 斯坦福公开课：《机器学习》课程学习笔记

# 第一节 `机器学习的动机与应用`
### Machine Learning Definition
- Arthur Samuel(1959).Machine Learnging: Field of study that gives computers the ability to learn without being explicitly programmed.
- Tom Mitchell(1998).Well-posed learning Problem: A computer program is said to learn from experience E with respect to some task T and some performance measure P, if its performance on T, as measured by P, improves with experience E.

### Supervised Learning(监督学习)
- Providing the algorithm a data set of a bunch of square footages, a bunch of square house sizes and as well as a sort of the right answer of what the actual prices of a number of houses were.
- So we call this supervised learning because we're supervising the algorithm or, in other words, we're giving the algorithm the quote, right answer for a number of houses. And then we want the algorithm to learn the association between the inputs and the outputs and to sort of give us more of the right anwsers.
- This is belong to regression problem. The variable to predict is continuous value.
- 监督学习是给定了一组“正确答案”，通过算法计算出来一组符合标准的答案。

### Unsupervised Learning(无监督学习)
- That's the unsupervised learning problem where you're sort of not given the right answer for everything.
- Clustering is sort of one example of an unsupervised learning problem.
- 无监督学习是无预设目标的获取结果。

### Reinforcement Learning(强化学习)
- This refers to problems where you don't do one-shot decision-making.
- You are usually asked to make a sequence of decisions over time.
- The basic idea behind a reinforcement learning algorighm is this idea of what's called a reward function.
- Reinforcement learning is it as a way for you to specify what you want done. So you have to specity what is a "good dog" and what is a "bad dog" behavior.
- Reinforcement learning is applied to other problem in rebotics. It's applied to things in web crawling and so on.
- 强化学习的基础是回报函数，通过不断的反馈培养出能区别“正确”和“错误”的决策。