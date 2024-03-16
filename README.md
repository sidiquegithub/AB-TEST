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


