
## Essential A/B Testing Questions and Answers


## Basic Knowledge
### What is A/B Testing?
A/B testing, or split testing, is a methodological approach for comparing two versions of a web page, application feature, or other digital assets to determine which one performs better in achieving a specified goal, such as enhancing user engagement, conversion rates, or other key performance indicators (KPIs).

### Why is A/B testing important?
Conducting A/B tests is crucial because it enables data-driven decision-making, allowing businesses and developers to optimize their digital offerings based on empirical evidence. This approach helps improve user experiences, increase conversion rates, and meet business objectives more effectively by identifying and implementing the most effective changes.

### What are Control Group and Treatment Group in A/B Testing?

In A/B testing, the **control group** is exposed to the original version (A) of the asset being tested, serving as a benchmark, while the **treatment group** is exposed to the modified version (B). Comparing the outcomes of these groups helps in assessing the impact of the change implemented in the treatment group, guiding decisions on whether to adopt the changes broadly.

### What are Common Mistakes to Avoid in A/B Testing?
Some common pitfalls in A/B testing include: not running the test long enough to gather conclusive data, making changes to the test environment mid-test, testing too many elements simultaneously, which can muddy the results, and failing to ensure a statistically significant sample size, which might lead to incorrect conclusions.

### How Do A/B Tests Differ from A/A Tests and Ramp Tests?
- **A/B Tests:** Compare two versions, A and B, where B has a specific change aimed at improving a certain metric.
- **A/A Tests:** Both groups are shown the same version (A) to check the testing tool's accuracy and to ensure that there is no significant difference in metrics between the two groups, validating the test's reliability.
- **Ramp Tests:** Also known as phased rollouts, involve gradually increasing the percentage of users exposed to the new version (B) while monitoring performance and feedback, allowing for adjustments before full deployment.


## What are AB test stages?
A/B testing is a structured process that involves several key stages. Briely main stages include: Hypothesis, Experimental Design, Data Collection, Statistical Analysis, Metrics. Each stage plays a critical role in ensuring the test is designed, executed, and analyzed effectively to make data-driven decisions. Here are the stages involved in conducting an A/B test:

### 1. Objective Setting
- **Description:** Begin by defining clear, measurable objectives for the A/B test. Objectives could be increasing conversion rates, improving user engagement, or reducing bounce rates.

### 2. Hypothesis Formation
- **Description:** Formulate a hypothesis based on data, observations, or insights, predicting how a change might impact the objective. This serves as the foundation for the test.

### 3. Test Design
- **Description:** Design the experiment by selecting the variable(s) to test, creating control (A) and treatment (B) groups, and deciding on success metrics.

### 4. Audience Selection and Segmentation
- **Description:** Identify the test's audience and, if necessary, segment it to ensure relevant insights. Ensure participants are randomly assigned to control or treatment groups to prevent bias.

### 5. Sample Size Determination
- **Description:** Calculate the necessary sample size to achieve results with statistical significance, based on expected effect size, desired statistical power, and alpha level.

### 6. Implementation and Monitoring
- **Description:** Execute the test by exposing the control group to the original version and the treatment group to the variant. This stage requires careful setup and monitoring to ensure accurate execution. Monitor the test's progress to ensure it's running as planned and to identify any issues promptly. This involves tracking both groups' performance and the test's technical aspects.

### 8. Data Collection
- **Description:** Collect and record data from both the control and treatment groups. Focus on the metrics defined during the test design phase to assess the impact of the change.

### 9. Analysis and Interpretation
- **Description:** Analyze the collected data using statistical methods to determine if there are significant differences between the control and treatment groups' performance.

### 10. Learning and Action
- **Description:** Draw conclusions from the analysis, decide on the next steps, and if successful, consider implementing the change. Document the findings and insights for future reference.

### 11. Iteration
- **Description:** Use the insights gained to refine the hypothesis or test new hypotheses. A/B testing is an iterative process aimed at continuous improvement.


## Hypothesis

### What is a hypothesis in the context of A/B testing? What is an example of a clear hypothesis for an A/B test?
A hypothesis in A/B testing is an assumption or prediction that guides the test. It states what change you expect to see in your key metrics as a result of a variation you are testing against the control.


### How does a hypothesis impact the design of an A/B test?
The hypothesis determines what variable will be changed, what metrics will be measured, and how long the test needs to run. It directly influences the experimental setup, including the selection of the control and variation groups.

### What makes a hypothesis testable?
A testable hypothesis is one that can be supported or refuted through direct experimentation and data analysis. It should be specific, measurable, and have a clear variable and outcome.

### Can you explain the role of null and alternative hypotheses in A/B testing?
In A/B testing, the null hypothesis states that there is no difference in the metric of interest between the control and variation groups. The alternative hypothesis suggests that there is a difference. Statistical analysis is used to determine which hypothesis is supported by the experiment data.


## Experimental Design

### What are the key elements of experimental design in A/B testing?
Key elements include the selection of variables to test, identification of control and treatment groups, determination of sample size, choice of significant metrics for evaluation, and the test duration.

### What is the purpose of having a control group in an A/B test?
The control group serves as a benchmark to measure the effect of the change. By comparing the performance of the treatment group against the control, you can isolate the impact of the variable being tested.

### How do sample size and duration affect the reliability of an A/B test?
Sample size and duration affect the statistical power and significance of the test. A larger sample size and appropriate duration ensure that the test results are reliable and can be generalized to the entire population.

### What considerations are important for ensuring the ethical conduct of an A/B test?
Ethical considerations include informed consent, privacy protection, minimizing user discomfort, and avoiding deception. Tests should also be designed to provide value to both the organization and its users.


### How do you determine sample size for AB tests? List all important parameters and explain in an example data set 

Determining the correct sample size for A/B tests is critical to ensure the reliability of the test results. The important parameters for determining sample size include:

- **Baseline Conversion Rate (BCR):** The current conversion rate without any changes.
- **Minimum Detectable Effect (MDE):** The smallest change in conversion rate you wish to detect, which is meaningful for your business.
- **Statistical Significance (α):** Typically set at 5%, this is the probability of finding a difference when there isn't one (false positive).
- **Statistical Power (1 - β):** Often set at 80% or 90%, this is the probability of detecting a difference when there is one (true positive).

#### Example Dataset:

- **BCR:** 15%
- **MDE:** 2% increase
- **α:** 5%
- **Power:** 80%

Using an online sample size calculator, inputting these values might suggest you need approximately 3,700 participants per group to reliably detect the effect.

### How samples are randonmized for A/B tests? What factors do we need to consider? 

Randomization in A/B testing is the process of assigning participants to either the control or treatment group randomly to avoid bias. Factors to consider include:

- **Ensuring Equal Distribution:** Aim for an equal number of participants in each group.
- **Controlling for Variables:** Account for variables like time of day or user demographics that might affect the outcome.

Randomization can be achieved through algorithms that assign participants based on a random number generator or other systematic methods to ensure fairness and unbiased results.


### What effects are from over sampling or under sampling? What are the solutions? How do they influence A/B test results

- **Over Sampling:** Can lead to unnecessary resource expenditure and may also increase the risk of detecting insignificant differences as significant (false positives).
- **Under Sampling:** May result in the test lacking the statistical power to detect real differences between the control and treatment groups (false negatives).

### Solutions and Influence on A/B Test Results:

- **Balancing Sample Size:** Use statistical formulas or sample size calculators to determine the optimal sample size that balances cost and the ability to detect meaningful effects.
- **Sequential Testing:** Monitor your test's progress and conduct interim analyses to adjust sample size if necessary without compromising the test's integrity.

Properly sized and balanced samples ensure that A/B test results are both reliable and actionable, minimizing the risks of false conclusions.

### What is the difference between A/B testing and multivariate testing?

- **A/B Testing:** Compares two versions (A and B) of a single variable to see which performs better on a specified metric.
- **Multivariate Testing (MVT):** Tests multiple variables and their combinations simultaneously to understand their individual and combined impact on the outcome.

While A/B testing is simpler and good for testing single changes, multivariate testing allows for more complex insights into how different elements interact with each other. However, MVT requires a larger sample size and more complex analysis to interpret the results accurately.


### What does the max 75% traffic mean? Why do we set up 25% for system test? 

Allocating a maximum of 75% of your user traffic to participate in an A/B test (or multiple A/B tests) means that at any given time, three-quarters of your audience is exposed to the test variations. This allocation allows for a substantial portion of users to experience and interact with the new features or changes being evaluated.

Reserving 25% of the traffic for a system test or as a control group serves multiple important purposes:
1. **Performance Benchmarking:** The control group (which experiences the original version without any changes) acts as a benchmark, helping to measure the impact of the new features or changes implemented in the A/B test.
2. **System Stability:** Keeping a portion of the traffic on the original system can help ensure stability and provide a fallback option in case the new variations negatively impact user experience or system performance.
3. **Risk Mitigation:** Limiting the test to 75% of traffic helps mitigate the risk of widespread issues. If unforeseen problems arise with the test variations, only a portion of the user base is affected.
4. **Continuous Testing:** The reserved 25% can be used for further system tests or for testing other new features, ensuring that there is always a segment of traffic that can be used to evaluate system performance independently of the ongoing A/B tests.








## Visitor Selection and Segmentation


### What is the process for Visitor selection, qualification, segmentation for AB tests?

- **Visitor Selection:** Involves choosing a group of users to participate in the test, often based on their likelihood of encountering the test scenario during their visit.
- **Qualification:** Refers to ensuring that selected visitors meet certain criteria relevant to the test, such as being a first-time visitor or having a specific item in their shopping cart.
- **Segmentation:** This step divides the qualified visitors into more specific groups based on demographics, behavior, or other relevant characteristics to analyze how different segments react to the variations in the test.

### How are the test visitors different from other non-test visitors? How do you track the test visitors during the test period?

- Test visitors are specifically selected based on the test's target audience and qualification criteria, making them potentially more relevant to the hypothesis being tested compared to non-test visitors.
- Tracking test visitors is usually done through cookies, session IDs, or user login information to ensure that they consistently see the same version of the test content during their entire visit or across multiple visits, depending on the test design.

### Why is visitor selection important in A/B testing?

Audience selection is crucial because it ensures that the results of the A/B test are relevant and can be generalized to the broader target audience. Proper selection helps in obtaining accurate, actionable insights that can guide optimization strategies effectively.

### Can segmenting your visitors impact the statistical power of an A/B test? How?

Yes, segmenting your audience can impact the statistical power of an A/B test. While segmentation can provide deeper insights into how different groups react to the changes, it also reduces the sample size for each segment. This reduction can decrease the statistical power, making it harder to detect a significant difference unless adjustments are made to the sample size or the test duration is extended.

### What are some best practices for visitor segmentation in A/B testing?

- **Consistency:** Apply consistent criteria when segmenting audiences across different tests to ensure comparability of results.
- **Relevance:** Choose segmentation criteria that are relevant to the test hypothesis and the overall business objectives.
- **Balance:** Ensure segments are large enough to achieve statistical significance but specific enough to yield actionable insights.
- **Clear Definition:** Clearly define each segment to avoid overlap and ensure that each user is only included in one segment.
- **Iterative Segmentation:** Use insights from previous tests to refine segmentation strategies and hypotheses for future tests.

### What is the process to randomize visitors into buckets?

Randomizing visitors into buckets is a crucial step in A/B testing, ensuring that the experiment's results are due to the changes made rather than external factors. Here’s a step-by-step overview of the process:

Step 1: Define the Buckets
- **Description:** Start by defining the number and nature of the buckets. Typically, there's at least a control group (A) and one variation group (B), but there can be more variations depending on the test's complexity.

Step 2: Use a Randomization Algorithm
- **Description:** Implement a randomization algorithm that assigns each visitor to a bucket in a completely random manner. Common methods include:
- **Random Number Generation:** Use a random number generator to assign visitors to buckets based on predefined probabilities.
- **Hashing:** Apply a hashing function to some unique visitor identifier (like a session ID or cookie value) and use the hash value to assign the visitor to a bucket.

Step 3: Ensure Even Distribution
- **Description:** Monitor the distribution of visitors across buckets to ensure it remains even. Adjustments may be needed if significant imbalances occur, although true randomization should, over time, lead to evenly distributed groups.

Step 4: Segment Consistency
- **Description:** For visitors who are part of ongoing experiments or return during the testing period, ensure they remain in the same bucket to maintain the integrity of the test. This is usually achieved by storing the bucket assignment in the visitor's cookie or session data.

Step 5: Account for Segment Conditions
- **Description:** If the test involves specific segments (e.g., returning users or users from a particular geographic location), apply the randomization process only to visitors who meet these segment conditions.

Step 6: Validate the Randomization Process
- **Description:** Conduct pre-test checks, such as A/A tests, to ensure that the randomization process does not introduce any bias and that both groups are indeed statistically identical in terms of conversion rate or other baseline metrics before introducing any changes.

Considerations
- **Balancing:** While randomization aims to balance groups, for very specific segments or smaller sample sizes, consider using stratified sampling techniques to ensure that key demographics or behaviors are balanced across the groups.
- **Compliance and Privacy:** Ensure that the randomization and bucket assignment processes comply with data protection regulations (like GDPR or CCPA), particularly when using visitor identifiers for bucket assignment.

Randomization is a foundational element of A/B testing that supports the validity of the experiment by ensuring that the observed differences between the control and variation groups are due to the changes being tested and not to pre-existing differences between the groups.


## Data Collection

### What types of data are typically collected in an A/B test?
Data collected includes quantitative metrics such as click-through rates, conversion rates, time spent on page, as well as qualitative feedback through surveys or user comments.

### How do you ensure data accuracy and integrity during an A/B test?
Ensuring data accuracy involves using reliable data collection tools, regularly auditing data for anomalies or errors, and maintaining a consistent data collection methodology throughout the test.

### How can data collection duration influence A/B test results?
The duration needs to be long enough to collect adequate data for statistical significance but short enough to be relevant. Too short may not capture the full effect, and too long may introduce noise from external factors.

### What challenges might you face in data collection for A/B testing and how can they be addressed?
Challenges include dealing with low traffic, seasonal variations, and user behavior changes. These can be addressed by extending the test duration, segmenting the data for more insights, and using historical data for adjustments.


### What are visitorID, sessions, cookies? 

VisitorID, sessions, and cookies are key components in tracking and analyzing web user behavior. VisitorID is a unique identifier assigned to each user to track their interactions across multiple visits to a website. Sessions represent individual visits by a user, tracking all their actions from entry to exit or timeout. Cookies are small data files stored on the user's device by the website, used to remember the user's preferences, login details, and track their activities across sessions and visits, facilitating a personalized and seamless web experience.

### What does Sapphire platform do for the AB tests?


### How is raw data collected at Farscape and Firefly? How are the displays, clicks, add to cart determined? 


### Where are the 'raw' data for AB tests at PRZ?




### What is per-visitor counting for displays and clicks? What is session-based counting for displays and clicks? Please provide an example

Tracking how users interact with website elements, such as advertisements or call-to-action buttons, is key to evaluating their performance. Two common methods are per-visitor counting and session-based counting.

Per-Visitor Counting

- **Description:** Per-visitor counting tracks the number of displays and clicks per individual user over a specified period, regardless of how many sessions they initiate. This method is focused on the user's overall interaction with the site's elements, providing insights into user engagement and interest.

Example:
Imagine a user visits a website three times in one week and sees the same advertisement during each visit. They click on the advertisement once. In per-visitor counting:
- **Displays:** The advertisement is counted as 1 display per visitor, assuming the count is unique per visitor.
- **Clicks:** The click is counted as 1 per visitor, regardless of the number of sessions.

Session-Based Counting

- **Description:** Session-based counting measures the displays and clicks within individual sessions. If a user interacts with the same element multiple times across different sessions, each interaction is counted separately. This method helps in understanding the immediate impact of site elements during a single visit.

Example:
Using the same scenario as above, but with session-based counting:
- **Displays:** The advertisement is counted as 1 display per session, resulting in 3 displays if the user sees it in each of their three sessions.
- **Clicks:** If the user clicks on the advertisement in two different sessions, it's counted as 2 clicks.

Key Differences and Implications:

- **Per-Visitor Counting:** Offers a broader view of user engagement over time, useful for long-term performance analysis and user interest.
- **Session-Based Counting:** Provides insight into the immediate effectiveness of site elements and user behavior within a single session, helpful for understanding session-specific engagement and optimizing for short-term interactions.

Understanding these counting methods is essential for accurately measuring and interpreting the effectiveness of website content, ads, and features, informing strategies for improvement and optimization.



### What is Purchase Amount or Attribute Demand? 

- **Purchase Amount:**
  - **Description:** Refers to the total value of purchases made by a customer or within a transaction. In e-commerce analytics, it's a critical metric indicating revenue generated from sales. It can be analyzed to understand buying patterns, average order value, and overall business performance.
  
- **Attribute Demand:**
  - **Description:** Often related to the demand generated for specific product attributes or features. It helps in understanding what particular aspects of a product are driving sales. For instance, a color or size in clothing, or a specific feature in electronics, that is highly sought after by consumers.


### What is the difference for Purchase Amount and Purchase from per-visitor counting or session-based counting?

A/B testing is essential for understanding user behavior and optimizing website performance. When it comes to metrics like Purchase Amount and Purchase Frequency, the method of counting—per-visitor or session-based—can yield different insights.

Per-Visitor Counting in A/B Testing

- **Per-Visitor Counting** tracks and aggregates user interactions (such as Purchase Amount and Frequency) across all sessions a specific visitor engages in over the duration of the A/B test.

Implications:
- Offers a holistic view of how each version of the test influences customer behavior and loyalty over time.
- Helps identify which version encourages higher overall spending or repeat purchases by the same visitor.

Session-Based Counting in A/B Testing

Definition:
- **Session-Based Counting** evaluates user interactions within the confines of a single session, without considering the visitor's behavior across multiple sessions.

Implications:
- Useful for understanding immediate reactions to changes introduced in the A/B test, such as the impact on impulse buys or single-visit conversion rates.
- Determines which version of the test is more effective at driving sales within the same session of exposure.

Example:
If Visitor A makes a purchase in one session and then another purchase in a separate session, each purchase is evaluated independently in relation to the test version the visitor was exposed to during those specific sessions.

Key Differences in A/B Test Scenarios:

- **Per-Visitor Counting:**
  - More suited for long-term behavioral analysis, such as assessing customer lifetime value or repeat purchase behavior influenced by the A/B test variations.
  - Helps in understanding the overall effectiveness of each variation in cultivating loyal customers or increasing customer spend over time.

- **Session-Based Counting:**
  - Ideal for immediate conversion optimization, assessing the direct impact of test variations on user actions within a single visit.
  - Crucial for evaluating the effectiveness of specific changes in driving conversions or purchases without the influence of prior or subsequent visits.


Example:

Consider an online store with a customer who made three visits over a month:

- Visit 1: Purchased items totaling $100
- Visit 2: Purchased items totaling $50
- Visit 3: Browsed without making a purchase

#### Per-Visitor Counting:
- **Purchase Amount:** $150 (over the month from this customer)
- **Purchases:** 2 (total number of purchases made by this customer)

#### Session-Based Counting:
- **Purchase Amount per Session:** 
  - Session 1: $100
  - Session 2: $50
  - Session 3: $0 (no purchase)
- **Purchases per Session:** 
  - Session 1: 1
  - Session 2: 1
  - Session 3: 0

## Key Takeaways:

- **Per-Visitor Counting** provides a holistic view of customer value and loyalty, showing long-term engagement and spending behavior.
- **Session-Based Counting** offers insights into the immediate effectiveness of marketing efforts, site usability, and session-specific factors influencing purchasing decisions.

Both counting methods are valuable, and their use depends on the specific analytical goals, whether understanding long-term customer value or assessing short-term sales performance.





## Statistical Analysis


### What statistical methods are used to analyze A/B test data? And how are they different for AB tests?
Methods include t-tests, chi-square tests for proportions, and analysis of variance (ANOVA) for comparing means, depending on the type of data and the test design.

### How do you determine statistical significance in A/B testing results? Provide an example data to illustrate
Statistical significance is determined using a p-value, which measures the probability that the observed results occurred by chance. A common threshold for significance is a p-value of less than 0.05.

### What is a p-value and how is it interpreted in the context of A/B testing? What is drawback for p-value?
A p-value in A/B testing indicates the likelihood that the difference in metrics between the control and variation groups could have occurred by chance. A lower p-value suggests a higher likelihood that the observed differences are due to the change made.


### What is lift? Provide an example of lift with an example dataset
Lift in A/B testing refers to the increase in performance metrics, such as conversion rate, resulting from a change tested against a control group, expressed as a percentage to quantify improvement. For example, if an e-commerce site tests a new landing page design (Variant B) against the original (Variant A), and Variant A has a conversion rate of 10% (100 conversions out of 1,000 visitors), while Variant B increases the conversion rate to 12% (120 conversions out of 1,000 visitors), the lift is calculated as ( 12 % − 10 % ) / 10 % = 20 % (12%−10%)/10%=20%. This means the new landing page design resulted in a 20% lift in the conversion rate, demonstrating the effectiveness of Variant B over Variant A in enhancing customer conversions.


### Can you explain what confidence intervals are and why do we want confidence intervals? Illustrate with an example
Confidence intervals provide a range within which the true difference between the control and variation groups is likely to lie. They give an idea of the uncertainty around the estimated effect size and help assess the practical significance of the test results.

### Why is it important to consider both statistical significance and practical significance in A/B testing analysis?
Statistical significance tells us if the results are likely not due to chance, while practical significance addresses whether the size of the effect is meaningful in a real-world context. Both are crucial for making informed decisions based on A/B test results.

### What errors do we consider for statistical tests for AB tests?

In statistical tests for A/B testing, we consider two main types of errors: Type I and Type II errors. A Type I error, or false positive, occurs when the test incorrectly concludes that there is a difference between the control and test groups when, in fact, there isn't one. This error leads to the mistaken rejection of the null hypothesis. Conversely, a Type II error, or false negative, happens when the test fails to detect a real difference between the groups, incorrectly retaining the null hypothesis. Managing these errors involves choosing appropriate significance levels and ensuring sufficient test power, respectively, to minimize the risk of making incorrect conclusions about the effect of the variables being tested.


## Metrics

### What are some common metrics used in A/B testing?
Common metrics include conversion rate, bounce rate, average order value, time on site, and user engagement metrics such as page views per session.

### How do you choose which metrics to focus on in an A/B test?
The choice of metrics is guided by the test's goals, the hypothesis, and the specific aspects of user behavior or performance that the test aims to influence.

### Why is it important to select the right metrics for an A/B test?
Selecting the right metrics is crucial because they directly impact how the success of the test is evaluated. The wrong metrics may lead to misleading conclusions or missed insights.

### Can you give an example of how a metric can be misleading if interpreted incorrectly?
If an increase in average time on page is interpreted as increased engagement without considering context, it could be misleading. The increase could be due to confusion or difficulty in finding information, not higher engagement.

### How do leading and lagging indicators differ, and how might they be used in A/B testing?
Leading indicators provide early signs of future performance, such as newsletter sign-ups indicating future sales. Lagging indicators measure outcomes, like actual sales. In A/B testing, leading indicators can predict long-term effects, while lagging indicators assess immediate impact.

### What are metrics of CTR, CVR, Purchase amount, Purchase rate and formulas in terms of recommendation scenarios? 

CTR: Measures the ratio of users who click on a specific recommendation to the total number of users who viewed the recommendation

CTR = (Number of Clicks on Recommendations / Number of Recommendations Displayed) * 100

Conversion Rate (CVR): Indicates the percentage of users who take a desired action (such as making a purchase) after clicking on a recommendation.

CVR = (Number of Conversions from Recommendations / Number of Clicks on Recommendations) * 100

Purchase Amount: Refers to the total revenue generated from transactions where the purchase was made following a recommendation.

Purchase Amount = Sum of Revenue from Recommended Product Purchases

Purchase Rate: The percentage of displayed recommendations that resulted in a purchase, indicating the efficacy of recommendations in driving sales.

Purchase Rate = (Number of Purchases from Recommendations / Number of Recommendations Displayed) * 100












