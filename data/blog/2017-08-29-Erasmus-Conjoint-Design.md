---
title: 'Conjoint Foundations - Design'
date: '2017-08-26'
tags: ['conjoint']
---

Summary: In a nutshell, conjoint analysis is a research methodology that uses surveys to understand how people make choices. It relies heavily on subjective data (beliefs, opinions, expectations, etc.) to understand individuals' behavior, attitude, intentions, and choices. Check the intro [here]({{ site.baseurl }}{% link _posts/2017-08-29-Erasmus-Conjoint-Design.markdown %})

### Designing a choice-based conjoint

There are several critical steps involved in designing conjoint experiments that are common for all CA <sup>green1978conjoint</sup>; <sup>green1990conjoint</sup>; <sup>hauser2004conjoint</sup>.

1.  Decomposition of product on product attributes
2.  Stimuli representation
3.  Stimuli configuration
4.  Data collection
5.  Estimation

Due to the broadness of the term CA, it is difficult to assign a meaningful explanation of each step without focusing on a particular CA approach. Although the first 2 steps are common for all types of CA, stimuli configuration, data collection, and estimation tasks are interlinked. @louviere1988conjoint refers to the first three common steps as experimental design techniques and explains that researchers rely on them to create profile configuration. However, the data collection and estimation vary per different "paradigms" (or approaches used above). For example, collection and employing judgmental data implies evaluation of one profile at a time by rating it on an ordinal scale, which is referred to as "Rating-based conjoint", while choice data implies a choice of one profile among several at a time mimicking real purchase behavior which is referred to as "Choice-based conjoint". Depending on the different data collection techniques, the method of analysis and estimation of the "part-worth" utilities differs. The focus of data collection and estimation will be on CBC while briefly describing the other possible approaches.

#### Decomposition of product on product attributes

2 critical issues should be taken into account in this first step <sup>hauser2004conjoint</sup>. First, defining product's attributes and respectively the levels in which each attribute is divided. Second, defining the function of each attribute, respectively each attribute level, in the overall model of respondents' preferences. Functions can be vector monotone preference (approximately linear), ideal point preference (convex or concave), and part-worth preference (discrete or categorical). In contemporary literature on the topic, all preference functions are referred to as "part-worths", although they may have different functions in the overall preference structure according to earlier articles.

To illustrate the steps better, I will use an example. Company X is planning to release a new smartphone on the market. After preliminary research, company X decides that the most important features of their smartphone are: Product name, Screen size, Memory, and Price. After consultation with engineering and marketing departments, the following product attribute levels can be distinguished:

Table 1

If we consider independently price and memory, they would have approximately linear utility for the respondents (i.e. the higher the price, the lower utility). However, considering the screen size, we can expect a concave shape of the preference (i.e. most people would probably prefer neither too small nor too big a phone). As the brand name is a discrete preference, it belongs to the so-called part worth preferences.

#### Stimuli representation

There are many ways that stimuli can be presented to subjects such as text, pictures, video, physical objects, and even verbal description. However, as in recent years, the established way of conducting marketing research interviews is in online web-based forms, researchers are taking advantage of various kinds of available multimedia <sup>dahan2000predictive</sup>. Naturally, the more realistic the stimuli are presented to the subjects the better quality of the data is to be expected.

#### Stimuli configuration

Once the product is decomposed on its attributes and attributes' levels, a large number of product profiles can be generated per each combination. However, ever since the emergence of CA, researchers recognized that showing all possible products profiles is not feasible as it is tiresome for the respondents and therefore, it is not cost-effective and can potentially lead to biased estimates <sup>carmone1978robustness</sup>.

To limit respondents' burden and provide more robust estimates, several approaches to reduce product profiles can be applied. However, product profile configuration is closely related to the data collection method and estimations, thus, collection and estimation cannot be examined independently. For example, one way to reduce product profiles is orthogonal fractional factorial design or just "orthogonal design". In an orthogonal design, only the extreme combinations of products' features are being evaluated, "the levels of the features are chosen such that, for each pair of features, say a and b, the high level a appear equally often in profiles that have a high-level b as in profiles that have a low level of b, and vice versa" <sup>hauser2007note</sup>. In a demonstration paper, @green1974design applied orthogonal design to an extreme example of 4x3x27 (1536) product profiles, was able to reduce the product profiles to only 16 to estimate the main effects. As expected, such reduction comes with certain trade-offs, that is, preference independence assumption, which does not allow any interactions among the different attributes to be estimated.

Table 2 Orthogonal design example

| Card ID | Brand Name | Screen Size | Memory | Price |
| ------- | ---------- | ----------- | ------ | ----- |
| 1       | ProductA   | 4'          | 32     | 300   |
| 2       | ProductB   | 3'          | 32     | 400   |
| 3       | ProductB   | 5'          | 32     | 200   |
| 4       | ProductB   | 6'          | 64     | 300   |
| 5       | ProductA   | 5'          | 16     | 300   |
| 6       | ProductB   | 5'          | 16     | 200   |
| 7       | ProductB   | 6'          | 16     | 400   |
| 8       | ProductA   | 5'          | 64     | 400   |
| 9       | ProductA   | 3'          | 16     | 200   |
| 10      | ProductA   | 6'          | 32     | 200   |
| 11      | ProductB   | 3'          | 16     | 300   |
| 12      | ProductA   | 6'          | 16     | 200   |
| 13      | ProductA   | 3'          | 64     | 200   |
| 14      | ProductB   | 4'          | 64     | 200   |
| 15      | ProductB   | 4'          | 16     | 200   |
| 16      | ProductA   | 4'          | 16     | 400   |

For instance, our smartphone example would generate a total of 72 (2x4x3x3) possible product profiles. As seen in Table 2, using the orthogonal design we can reduce this number to 16. Orthogonal design, full factorial design, and fractional factorial design are the starting point for more advanced stimuli configurations that are used in practice nowadays.

#### Data collection

The methods described below are proven to be reliable in large-scale commercial applications (see <sup>hauser2004conjoint</sup> for discussion).

- Partial profile CA

Also known as Two-attribute-at-a-time trade-off analysis, in this setting, respondents are presented to two attribute trade-off tables where they rank their preferences for different attribute levels. The number of stimuli can vary from two to many, nonetheless, two attributes at a time are the most popular <sup>hauser2004conjoint</sup>.

- Full-Profile CA

Products are described by the levels of the attributes they contain. Respondents are then asked to rank order all stimuli or to provide a metric rating of each stimulus. By controlling the attribute combinations, based on correlations of the attributes with respondents' preferences, the utility for each level of each attribute tested can be estimated.

- Choice-Based (CBC)/Discrete-Choice CA

Respondents are presented with a given set of product profiles, once they make their choice a new set is presented. The utilities are estimated based on respondents' choices. Also known as stated preference models, they are based on random utility models (RUM). Respondent's utility is presented as a combination of the product's features and an error term. Based on the assumption about the distribution of the error term, the probability of purchase of a product assembled out of a given set of features can be estimated.

- Adaptive CA

Currently, the most preferred way of data collection is computer-based interviews, this enables the researcher to make computations during the interview itself and adapt consecutive questions based on utilities estimated during the initial stage of the exercise. This method allows for reducing the survey length without losing valuable information or diminishing the power of the analysis.

#### Estimation

- Regression-based models

If the data obtained from the respondents for their preferences is an interval scale, then the part worths can be represented by dummy variables and ordinary least square (OLS) estimation can be adopted.

- Random utility models (RUM)

If the data obtained is from CBC, RUM can be adopted. The assumption of utility maximization combined with distributional assumptions of the unobserved term states that there is "a known function that maps the part-worth levels onto the probabilities that each profile is chosen from a given choice set" <sup>hauser2004conjoint</sup>.

- Hierarchical Bayes Estimation (HB)

To improve the predictive power of CA, researchers approached the problem using HB estimation. However, using HB slightly changes the idea of the analysis i.e. researchers do not try to estimate the patchworks, but rather attempt to characterize the uncertainty behind them <sup>hauser2004conjoint</sup>; e.g. the HB estimation allows for more accurate results while showing respondents fewer choice tasks.

Conjoint analysis has been widely used in many different domains in market research, allowing businesses to optimize their product development, pricing strategy, find the optimal product or portfolio configuration, etc. However, in a marker research workplace, typically the conjoint exercise is administered in a hypothetical environment. In such an environment, respondents could potentially give 'hypothetical answers' <sup>scott1965valuation</sup> as respondents are not offered a strong incentive to carefully and thoughtfully think about their answers <sup>ding2005incentive</sup>. Recently, researchers have examined different incentive-compatible methods that could measure better respondents' true preferences in the conjoint analysis <sup>ding2005incentive</sup>; <sup>ding2007incentive</sup>; <sup>toubia2012measuring</sup>. In the next section, I will focus on specific problems of online opinion taking and how incentive-compatible methodologies can improve model performance while at the same time increasing respondents' engagement and motivation.

## References

_The post has been originally published as part of my master thesis [Bayesian Truth Serum Fused Conjoint](https://thesis.eur.nl/pub/39589/) on 29 August 2017_

<details>
<summary>Literature Reference List</summary>
{% include citation.html label="green1971conjoint" %}
{% include citation.html label="ding2005incentive" %}
{% include citation.html label="hauser2004conjoint" %}
{% include citation.html label="louviere1988conjoint" %}
{% include citation.html label="green1978conjoint" %}
{% include citation.html label="krantz1971foundations" %}
{% include citation.html label="louviere1983design" %}
{% include citation.html label="mcfadden1973condition" %}
{% include citation.html label="chrzan2000overview" %}
{% include citation.html label="green1990conjoint" %}
{% include citation.html label="dahan2000predictive" %}
{% include citation.html label="carmone1978robustness" %}
{% include citation.html label="hauser2007note" %}
{% include citation.html label="scott1965valuation" %}
{% include citation.html label="ding2007incentive" %}
{% include citation.html label="toubia2012measuring" %}
</details>
