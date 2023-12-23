The task of evaluating innovations in online and mobile applications is ubiquitous. One of the most reliable and popular ways to address this challenge is the double-blind randomized experiment, also known as an A/B test.

The primary mathematical toolkit applied in A/B testing is already implemented in standard libraries such as SciPy, Statsmodels, Scikit-learn, Pandas, and others. Additionally, there are ready-made turnkey solutions, including open-source ones, that combine features for enabling and disabling functionality for various users, calculating metrics, and presenting results of statistical criteria.

This naturally leads to a desire to fully automate the process of designing, maintaining, and analyzing A/B tests to reduce the workload on company analysts.

**Complete Automation**

Why write a new Jupyter notebook every time after the completion of another A/B test if the part of the code related to calculating p-values and handling outliers repeats from test to test? If all frequently used metrics are described, there is no need to download data and run a t-test or bootstrap to calculate p-values every time. It is reasonable to perform these calculations automatically for all metrics and tests. After thorough validation on historical data, synthetic data, and in A/A tests, a small monitoring and launch service can be organized.

In this case, the role of the analyst is almost entirely eliminated, especially if access to monitoring and launching is provided to clients, such as managers. Thus, after implementing a new idea, clients can independently create an A/B test, assign users to desired groups, and visually verify that the new feature has impacted certain metrics - detecting statistical significance.

From the statistical significance of a set of metrics, conclusions can be drawn about the success of the idea and its implementation. This way, the analyst's time can be spent on more critical tasks.

However, ill-considered automation can lead to unexpected problems.
