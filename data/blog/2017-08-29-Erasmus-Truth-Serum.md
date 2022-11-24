---
title: 'Bayesian truth serum'
date: '2017-08-26'
tags: ['incentive compatibility']
---

Summary: Bayesian truth serum is a methodology for eliciting subjective judgments. Information score is estimated on question level and assigns high values to common answers and low values to the opposite. The prediction score component of BTS measures the accuracy of the respondent's estimate. A high prediction score indicates a high degree of accuracy and a low score implies a low degree of accuracy. The information score and prediction score are combined to produce a BTS score. The higher the score, the higher the incentive for truth telling.

### Intro

Bayesian truth serum is a methodology for eliciting subjective judgments and "unverifiable truths", developed by an MIT professor <sup>prelec2004bayesian</sup>. Prelec recognizes the necessity of assessing subjective beliefs in absence of objective truth as opinions, attitudes, and intentions are often used in science and policymaking.

For example, in marketing research, companies have been using respondents' subjective beliefs in order to create policies about products, prices, packages, features, etc. Prelec recognizes that the quality of the subjective data is limited by "its quality of the source" and argues that if respondents act as if they are being evaluated by an "onmicenter scorer in possession of the truth" the data quality will be enhanced. The mechanisms of BTS methodology grants maximum incentives for truth-telling based on Bayesian reasoning.
Scoring system

BTS is a scoring system that assigns different scores to opinions based on their truthfulness where high scores imply high incentives. BTS consists of two components: information score and prediction score.

### Information score intuition

Information score is estimated on question level and assigns high values to common answers and low values to the opposite. Surprisingly common answers are considered those whose actual frequency is higher than collectively predicted by the same population of interest <sup>prelec2004bayesian</sup>. Once considered an irrational bias, afterward proven as a purely rational effect, the idea behind common/uncommon answers is that opinion holders would overestimate the frequency of their own opinion amongst the population.
<sup>ross1977false</sup> describe this effect as one "tend to perceive a "false consensus"-to see their own behavioral choices and judgments as relatively common and appropriate to existing circumstances while viewing alternative responses as uncommon, deviant, or inappropriate." More precisely, it is a systematic deviation of assigning higher estimations or probabilities with regards to population frequency in directions of one's own opinion in a group of which the subject is a member.

In his paper, <sup>dawes1989statistical</sup> referred to the "false consensus bias" as "an egocentric bias to overestimate the degree in which others are like us". <sup>ross1977false</sup> executed four studies in which they tested the "false consensus bias" in various settings such as behavioral choices, situations, and judgments as well as personal problems, expectations preferences, and characteristics. For example, a study among Stanford undergraduates <sup>ross1977false</sup> showed that students who think about dying expected that 44% of students, in general, would share their problem against students who don't think about dying expected only 25.6% of the students to think about dying. Within the same experiment subjects who believed to die before turning age of 70 indicated that 57.6% of the students share their expectations while this number was only 43.9% for students with the opposite expectation.

This pattern was considered to be an irrational systematic deviation before <sup>dawes1989statistical</sup> has proven it to be a rational effect. Using Bayesian reasoning Dawes argues that subjects are considering their own opinion to be an "informative sample of one" which shifts the estimation of endorsers of a certain opinion in a direction toward their own opinion.

Using Dawes' interpretation <sup>prelec2004bayesian</sup> constructed a critical assumption; the information score component of BTS which indicates that ones' opinion frequency will be underestimated by the others and vice versa, one will overestimate the frequency of his own opinion. Consequently, this implies that surprisingly common answers are those whose actual frequency overweighs the collectively predicted frequency. For example, let's consider we have data about respondents being asked to state their preferences at binary choice (e.g. Yes/No) question. The respondents are asked to provide their own opinion as well as their estimates about the fraction of people endorsing their answer. If the actual frequency is 10% per "Yes" and the predicted frequency is 5%, the respondents who indicated "Yes" will receive a positive score as their answer will be considered "surprisingly common". However, given the same actual frequency, if the collectively predicted frequency is 25% respondents will be penalized with a negative score as their answers will be considered uncommon.

### Information score formula

<sup>prelec2004bayesian</sup> defines the following formula for estimation of information score component for answer $$k$$:

$$
\text{information score} = log(\frac{\overline{x}_{k}}{\overline{y}_{k}})
$$

Each respondent $$r$$ information score per $$k$$ number of answers:

$$
\text{information score} = \sum_{k}x_{k}^{r}log(\frac{\overline{x}_{k}}{\overline{y}_{k}})
$$

Where:

- $$\overline{x}_{k}$$ is the actual frequency of answer $$k$$ or $$\overline{x}_{k} = \frac{1}{n}\sum_{r=1}^{n}x_{k}^{r}$$
- $$\overline{y}_{k}$$ is the geometric average of predicted frequencies for answer $$k$$ or $$\overline{y}_{k} = \left ( \prod_{i=1}^{n}y_{k}^{r} \right )^{\frac{1}{n}}$$

### Prediction score intuition

The second component of BTS scoring is the prediction score, which is "a penalty proportional to the relative entropy (Kullback-Leibler divergence) between the empirical distribution and respondent's prediction of that distribution" <sup>prelec2004bayesian</sup>. In other words, this score assigns zero value to accurate prediction (i.e. best prediction score) when one's prediction matches the actual frequency and penalizes for inaccurate one. It is an asymmetric estimate of the difference between two probability distributions which produces a number smaller than zero.

### Prediction score formula

$$
\text{prediction score} = \alpha \cdot \sum\limits_{k}^{} \overline{x}_{k} \cdot log \frac{y^{r}_k }{\overline{x}_{k} }
$$

$$\alpha$$ is a constant used for assigning different weights to the prediction score relative to the information score in the BTS final score. Setting $$\alpha$$ equal to 1 will assign equal weights to the score of the equation which will result in a zero-sum game. In the zero-sum game, the average of all BTS scores is equal to zero. When $$\alpha$$ approaches zero BTS game results in "Pareto-dominate expected scores" in which at least one individual has a positive score.

### BTS formula

The overall score for each respondent is:

$$
\text{BTS score} = \text{Information score} + \text{Prediction score}
$$

### BTS Assumptions

<sup>prelec2004bayesian</sup> relies on several assumptions for constructing BTS algorithm:

Bayesian Nash equilibrium

"Truth-telling is individually and collectively optimal" <!-- --><sup>prelec2004bayesian</sup>. Taking into account the BTS assumptions, agents stating their true preferences is BTS Nash equilibrium for any α>0. Thus, it is individually optimal as BTS Nash equilibrium results in a maximum expected payoff. It is collectively optimal because there is no other equilibrium which results in a higher information score for any agent. The equilibrium relies on two assumptions:

1. There is a large enough sample so that a single answer can not affect the overall distribution;
2. All agents are Bayesians. They have a common prior and they update their beliefs based on their opinions;

### BTS validity

Although the BTS is a relatively easy method that can be implemented within a study design, little has been done to assess its validity. So far, the results are positive regarding the usage of the approach.

In an attempt to eliminate hypothetical bias in contingent valuation (CV) <sup>barrage2010penny</sup> compared three mechanisms to elicit subjects' true preferences along with real and hypothetical CV in two settings. The results showed that BTS was able to eliminate the hypothetical bias in one of the settings but only reduce it in the other. The authors conclude that BTS eliminates the hypothetical bias inconsistently. Interestingly enough, the authors also found an interaction between BTS and subjects' characteristics.

<sup>howie2011predicting</sup> emphasized that accurate prediction of performance on the market when products are not yet available is crucial to the business's success. In a study that aims to predict a medical product adoption on the market, the authors made the first empirical validation of BTS. In order to improve the predictive performance, the approach is adopted, based on the notion that "bad" respondents "hurt" the data, hence the authors exclude respondents with a low score (i.e. the untruthful ones). Applying BTS on data from 1763 physicians, BTS improved the overall performance up to 21% compared to a simple average from the full sample. An interesting particularity, contradictory to the original BTS article by <sup>prelec2004bayesian</sup>, is that the authors did not explain the BTS scoring concept to the participants, arguing that it is impractical and it hasn't been empirically validated to improve the data.

In the study of <sup>weaver2013creating</sup>, the authors conducted 5 experiments testing different aspects of BTS. They tested the validity of BTS upon respondents recognizing real and fake items from different categories such as brands, movies, journals, etc. The authors tested BTS in the following settings: Recognition questionnaires, in 2x2 between-subject design which consists of truth-telling (Control vs. BTS) and deception incentives (incentives for recognizing items vs. none). For the first experiment, the authors noted that it is not clear whether the performance of BTS is because of the truth-telling incentives or because of the claim made about them. To eliminate this doubt, keeping the same experimental settings, respondents were presented with their information score after each question. BTS was also compared to another "truth serum", the solemn oath. It requires participants to sign a declaration of their honesty, and again, respondents were given incentives to exaggerate their knowledge. BTS was also applied in the evaluation of a public good, e.g. it was applied on CV, in an attempt to eliminate the hypothetical bias. The experiments results showed good performance of BTS in recognizing real and fake items. The method performed well even when respondents were given incentives to overclaim item recognition. The results indicated there is strong evidence that instructing respondents about BTS has a positive impact on truth-telling. BTS results outperformed the "solemn oath" and successfully eliminated the hypothetical bias in CV. Important to notice in this research is that the authors provided empirical evidence that proper BTS instructions will result in higher data quality, a claim that was fairly questioned by <sup>howie2011predicting</sup>. Furthermore, the results showed that BTS eliminated the hypothetical bias in CV and the authors speculated that the mixed evidence about BTS performance in <sup>barrage2010penny</sup>, possibly result from a difference in the instructions. <sup>weaver2013creating</sup> also addresses interesting pragmatic issues that will be discussed in another part of the paper.

In an interesting article about Questionable Research Practices (QRPs) <sup>john2012measuring</sup> used by the scientific community, the authors applied BTS to a big sample (2155) of research psychologists. The BTS condition showed a significant difference in the results compared to the control group in 4 out of 10 measures of QRPs. The authors argue that the answers obtained with BTS incentives are more truthful. Following the fashion of investigating shameful activities from the QRPs article, <sup>kukla2015we</sup> apply BTS to investigate downloading intellectual property from unauthorized sources. BTS elicited around 60 percent higher self-admission rates on average compared to the control group. The authors interpreted the results as plausible in favor of BTS.

BTS has not been applied in the preference measurement domain yet. As there might be a discrepancy between one's preference in real life and in a conjoint context, BTS can play a significant role when measuring respondents' preferences when constructing new products, services, or policies. The successful introduction of an optimal combination of attributes for a new product, service, or policy will crucially depend on respondents' truthfulness. Given the importance of accurately predicting the optimal product, service, or policy product features, truthful elicitation is key when obtaining respondents' preferences.

### References

_The post has been originally published as part of my master thesis [Bayesian Truth Serum Fused Conjoint](https://thesis.eur.nl/pub/39589/) on 29 August 2017_

<details>
<summary>Literature Reference List</summary>
{% include citation.html label="prelec2004bayesian" %}
{% include citation.html label="ross1977false" %}
{% include citation.html label="dawes1989statistical" %}
{% include citation.html label="barrage2010penny" %}
{% include citation.html label="howie2011predicting" %}
{% include citation.html label="weaver2013creating" %}
{% include citation.html label="john2012measuring" %}
{% include citation.html label="kukla2015we" %}
</details>
