# Assignment-2-Data-Bias

  # Assignment-2-Data-Bias

  For this assignment, I utilized the provided set of Wikipedia comments made available by Jigsaw and the Perspective API to analyze data bias within the dataset. After parsing in the data, I was interested in obtaining the toxicity scores for various gendered curse words in order to see if any bias could be traced back to misogynistic insults/swears. I hypothesized that Perspective is more likely to mark anti-female gendered swears as toxic/the toxicity score will be higher when compared to non-gendered or anti-male swears (excluding "f***"). Additionally, I mainly focused on the "Score" column/label from the dataset, and determined the threshold for toxic/abusive terms would be >0.2.

  Through my analysis, I learned that Perspective is more likely to mark anti-female gendered swear words as more toxic than when compared to non-gendered or anti-male swears. This was surprising to me, as I assumed prior to this testing that anti-male swears would be documented as more toxic based on societal values. However, I think it is also important to take into account that a significant amount of offensive language is not contained within a single swear word alone; additionally, I was not able to test every swear word for toxicity level. I also found that more complicated anti-female phrases, such as "stay in the kitchen where you belong," had a far lower toxicity score (0.458) than swear words alone, which allows me to assume that Perspective does not account for all offensive sayings, and the toxicity score is likely higher based on certain singular words.

  Additionally, I found that: 
  The amount of "toxic" anti-female swears compares 24 'toxic' words under the label to 155 predicted. (545.833% increase in prediction compared to actual)
  The amount of "toxic" anti-male swears compares 43 'toxic' words under the label to 222 predicted. (416.279% increase in prediction compared to actual)
  The amount of "toxic" non-gendered/other swears compares 95 'toxic' words under the label to 637 predicted. (570.526% increase in prediction compared to actual)
  The amount of "toxic" non-gendered/less offensive swears compares 283 'toxic' words under the label to 396 predicted. (39.9293% increase in prediction compared to actual)

  Based on public documentation, https://developers.google.com/machine-learning/practica/fairness-indicators, there seems to exist a bias between identity terms and an increased toxicity score. Though this seems to be focused on sexual orientation and race, there likely exists a bias between gendered terms. My results reflect a difference between toxicity scores and anti-female swear words versus anti-male swear words; though it seems anti-female swears have an increased toxicity score, there may exist many anti-female phrased language that is under-accounted for in terms of toxicity level. With a more in-depth analysis on longer phrases, I’d hypothesize that anti-male content would be marked as less toxic; I’d theorize that Perspective is less accurate with longer phrases.
 






