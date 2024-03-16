# AB-TEST
## AB-TEST IN E COMMERCE WEBSITE DATA

In this project, I worked on analyzing the outcomes of an A/B test conducted by an e-commerce website. The company introduced a new webpage hoping to increase the number of users who "convert," meaning those who decide to purchase the company’s product. My objective was to sift through this notebook to assist the company in deciding whether to implement this new page, stick with the old page, or perhaps extend the experiment to make an informed decision.


## HOW DOES THE DATA LOOK

<table>
  <tr>
    <th>id</th>
    <th>time</th>
    <th>con_treat</th>
    <th>page</th>
    <th>converted</th>
  </tr>
  <tr>
    <td>851104</td>
    <td>11:48.6</td>
    <td>control</td>
    <td>old_page</td>
    <td>0</td>
  </tr>
  <tr>
    <td>804228</td>
    <td>01:45.2</td>
    <td>control</td>
    <td>old_page</td>
    <td>0</td>
  </tr>
  <tr>
    <td>661590</td>
    <td>55:06.2</td>
    <td>treatment</td>
    <td>new_page</td>
    <td>0</td>
  </tr>
  <tr>
    <td>853541</td>
    <td>28:03.1</td>
    <td>treatment</td>
    <td>new_page</td>
    <td>0</td>
  </tr>
  <tr>
    <td>864975</td>
    <td>52:26.2</td>
    <td>control</td>
    <td>old_page</td>
    <td>1</td>
  </tr>
</table> 

Total Number of Raws = 294478

## STEPS 
### STEP 1: First calculate the following probabilities
- The probability that an individual received the new page 
- The probability of an individual converting regardless of the page they receive 
- Given that an individual was in the control group, the probability they converted 
- Given that an individual was in the treatment group, the probability they converted

### STEP 2: Based on the above probabilities, infer the impact of implementing the new page.

### STEP 3: Conduct an A/B Testing Analysis

#### Probabilities
- The probability that an individual received the new page is 50%
- The probability of an individual converting regardless of the page they receive is 11.96%
- Given that an individual was in the control group(old_page), the probability they converted is 12.04%
- Given that an individual was in the treatment group(new_page), the probability they converted is 11.88%

#### Inference
Above results suggests that there is no significant difference in convergence between treatment and control groups. Therefore we may conclude that the new treatment page has no impact and does not lead to more conversions.

#### The Proportion Z Test
The proportions_ztest function is specifically designed to perform z-tests for proportions. It's commonly used when you want to test the hypothesis that the proportion of successes in one group is different from the proportion of successes in another group, which is a common scenario in A/B testing. This type of test is suitable when you are dealing with binary outcomes (e.g., converted vs. not converted, clicked vs. not clicked) and want to compare these outcomes between two independent groups.

#### Results from Proportion Z Test
z_score = -1.3109241984234394
p value = 0.9050583127590245

## CONCLUSION
Since the p-value (0.9050) is significantly higher than the common alpha levels (e.g., 0.05 or 0.01) used to determine statistical significance, we do not have sufficient evidence to reject the null hypothesis. This means that, based on the data from the proportions_ztest, there is no statistically significant difference between the proportions being compared.
