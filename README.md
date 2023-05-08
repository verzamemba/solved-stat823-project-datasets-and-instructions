Download Link: https://assignmentchef.com/product/solved-stat823-project-datasets-and-instructions
<br>
Choose <strong>only one </strong>of the questions and use the provided RMardown Project Template or a similar L<sup>A</sup>TEX Template to write your project report.

<strong>For the selected Data (question)</strong>,

<ol>

 <li>Create a title of your research question from the objective of the study.</li>

 <li>The response and exposure variables for each dataset are provided. The identification number (idnum) variable is not part of the covariates of interest.</li>

 <li>Fit appropriate statistical model(s). (See provided Hint/suggestions.) Explore the data. You may have to transform the response variable or covariates and/or standardize some covariates if necessary. Check for correlations among the variables. Use all important covariates or perform variable selections using standard statistics methods.</li>

 <li>Check for goodness of fit of the models and select the best that fits the data well.</li>

 <li>Produce residual plots to check for model assumptions including independence/multicollinearity, equal variance, outliers and normality of residuals. 6. In your report, make sure to produce Tables for Descriptive/summary statistics</li>

 <li>Create a Table(s) of inferential statistics from the final model.</li>

 <li>Select only a few important graphs (scatterplots/line graphs, boxplots, barchars, etc) and show the relationship between the response and the covariates of interest.</li>

 <li>Write your full report (in pdf format) and draw conclusions based on your study objective(s).</li>

</ol>

You are required to make slides from your final report and record your presentation.

<strong>Submit both your project report (in pdf format) and the recorded slides/powerpoint presentation for grading</strong>.

<h1>Qn 1: IPO Dataset</h1>

Model Hint/Suggestion: Multiple logistic regression model

Private companies often go public by issuing shares of stock referred to as initial public offerings (IPOs). A study of 482 IPOs was conducted to determine what are the characteristics of companies that attract venture capital funding. The response of interest is whether or not a company was financed with venture capital funds (Variable: funding). Potential predictors include the face value of the company (in millions), the number of shares offered (in millions), and whether or not the company underwent a leveraged buyout. Each line of the data set has an identification number and provides information on 4 other variables for a single person. The 5 variables are:

<table width="624">

 <tbody>

  <tr>

   <td width="77"><strong>Variable</strong></td>

   <td colspan="4" width="276"><strong>Variable Name</strong></td>

   <td colspan="4" width="270"><strong>Description</strong></td>

  </tr>

  <tr>

   <td width="77">1</td>

   <td colspan="4" width="276">idnum: Identification number</td>

   <td colspan="4" width="270">1 <em>− </em>482</td>

  </tr>

  <tr>

   <td width="77">2</td>

   <td colspan="4" width="276">funding: Venture capital funding</td>

   <td colspan="4" width="270">Presence or absence of venture capital funding: 1 if yes; 0 otherwise</td>

  </tr>

  <tr>

   <td width="77">3</td>

   <td colspan="4" width="276">facevalue: Face value company</td>

   <td colspan="4" width="270">Estimated face value of company from prospectus (in Million dollars)</td>

  </tr>

  <tr>

   <td width="77">4</td>

   <td colspan="4" width="276">shares: Number of shares offered</td>

   <td colspan="4" width="270">Total number of shares offered (in Millions)</td>

  </tr>

  <tr>

   <td width="77">5</td>

   <td colspan="4" width="276">buyout: Leverage buyout</td>

   <td colspan="4" width="270">Presence or absence of leveraged buyout: 1 if yes; 0 otherwise</td>

  </tr>

  <tr>

   <td colspan="2" width="157"> </td>

   <td width="59">idnum</td>

   <td width="68">funding</td>

   <td colspan="2" width="78">facevalue</td>

   <td width="58">shares</td>

   <td width="48">buyout</td>

   <td width="157"> </td>

  </tr>

  <tr>

   <td colspan="2" width="157"> </td>

   <td width="59">1</td>

   <td width="68">0</td>

   <td colspan="2" width="78">1.2</td>

   <td width="58">3</td>

   <td width="48">0</td>

   <td width="157"> </td>

  </tr>

  <tr>

   <td colspan="2" width="157"> </td>

   <td width="59">2</td>

   <td width="68">0</td>

   <td colspan="2" width="78">1.45</td>

   <td width="58">1.45</td>

   <td width="48">1</td>

   <td width="157"> </td>

  </tr>

  <tr>

   <td colspan="2" width="157"> </td>

   <td width="59">3</td>

   <td width="68">0</td>

   <td colspan="2" width="78">1.5</td>

   <td width="58">0.3</td>

   <td width="48">0</td>

   <td width="157"> </td>

  </tr>

  <tr>

   <td colspan="2" width="157"> </td>

   <td width="59">4</td>

   <td width="68">0</td>

   <td colspan="2" width="78">1.53</td>

   <td width="58">0.51</td>

   <td width="48">0</td>

   <td width="157"> </td>

  </tr>

  <tr>

   <td colspan="2" width="157"> </td>

   <td width="59">…</td>

   <td width="68">…</td>

   <td colspan="2" width="78">…</td>

   <td width="58">…</td>

   <td width="48">…</td>

   <td width="157"> </td>

  </tr>

  <tr>

   <td colspan="2" width="157"> </td>

   <td width="59">479</td>

   <td width="68">0</td>

   <td colspan="2" width="78">143.24</td>

   <td width="58">11.02</td>

   <td width="48">1</td>

   <td width="157"> </td>

  </tr>

  <tr>

   <td colspan="2" width="157"> </td>

   <td width="59">480</td>

   <td width="68">0</td>

   <td colspan="2" width="78">159.5</td>

   <td width="58">7.25</td>

   <td width="48">0</td>

   <td width="157"> </td>

  </tr>

  <tr>

   <td colspan="2" width="157"> </td>

   <td width="59">481</td>

   <td width="68">0</td>

   <td colspan="2" width="78">165</td>

   <td width="58">11</td>

   <td width="48">0</td>

   <td width="157"> </td>

  </tr>

  <tr>

   <td colspan="2" width="157"> </td>

   <td width="59">482</td>

   <td width="68">0</td>

   <td colspan="2" width="78">234.6</td>

   <td width="58">9.2</td>

   <td width="48">0</td>

   <td width="157"> </td>

  </tr>

  <tr>

   <td width="77"></td>

   <td width="80"></td>

   <td width="59"></td>

   <td width="68"></td>

   <td width="70"></td>

   <td width="8"></td>

   <td width="58"></td>

   <td width="48"></td>

   <td width="157"></td>

  </tr>

 </tbody>

</table>

<h1>Qn 2: Prostate Cancer Dataset</h1>

Model Hint/Suggestion: Multiple linear regression model

A university medical center urology group was interested in the association between prostate-specific antigen (<strong>PSA level</strong>) is the response variable and a number of prognostic clinical measurements in men with advanced prostate cancer. Data were collected on 97 men who were about to undergo radical prostectomies. Each line of the data set has an identification number and provides information on 8 other variables for each person. The 9 variables are:

<strong>Table 2: </strong><em>Adapted in part from: Hastie, T. J.; R. J. Tibshirani; and J. Friedman. The Elements of Statistical Learning: Data Mining. Inference. and Prediction. New York: Springer-Verlag, 2001.</em>

<table width="624">

 <tbody>

  <tr>

   <td colspan="2" width="77"><strong>Variable</strong></td>

   <td colspan="6" width="275"><strong>Variable Name</strong></td>

   <td colspan="5" width="272"><strong>Description</strong></td>

  </tr>

  <tr>

   <td colspan="2" width="77">1</td>

   <td colspan="6" width="275">idnum: Identification number</td>

   <td colspan="5" width="272">1 <em>− </em>972</td>

  </tr>

  <tr>

   <td colspan="2" width="77">2</td>

   <td colspan="6" width="275">psa: PSA level</td>

   <td colspan="5" width="272">Serum prostate-specific antigen level(<em>mg/ml</em>)</td>

  </tr>

  <tr>

   <td colspan="2" width="77">3</td>

   <td colspan="6" width="275">cancerv: Cancer volume</td>

   <td colspan="5" width="272">Estimate of prostate cancer volume (<em>cc</em>)</td>

  </tr>

  <tr>

   <td colspan="2" width="77">4</td>

   <td colspan="6" width="275">weight: Weight</td>

   <td colspan="5" width="272">Prostate weight (<em>gm</em>)</td>

  </tr>

  <tr>

   <td colspan="2" width="77">5</td>

   <td colspan="6" width="275">age: Age</td>

   <td colspan="5" width="272">Age of patient (<em>years</em>)</td>

  </tr>

  <tr>

   <td colspan="2" width="77">6</td>

   <td colspan="6" width="275">hyperplasia: Benign prostatic hyperplasia</td>

   <td colspan="5" width="272">Amount of benign prostatic hyperplasia(<em>cm</em><sup>2</sup>)</td>

  </tr>

  <tr>

   <td colspan="2" width="77">7</td>

   <td colspan="6" width="275">seminal: Seminal vesicle invasion</td>

   <td colspan="5" width="272">Presence Or absence of seminal vesicle invasion: 1 if yes; 0 otherwise</td>

  </tr>

  <tr>

   <td colspan="2" width="77">8</td>

   <td colspan="6" width="275">capsular: Capsular penetration</td>

   <td colspan="5" width="272">Degree of capsular penetration (<em>cm</em>)</td>

  </tr>

  <tr>

   <td colspan="2" width="77">9</td>

   <td colspan="6" width="275">score: Gleason score</td>

   <td colspan="5" width="272">Pathologically determined grade of disease using total score of two patterns (summed scores were either 6, 7, or 8 with higher scores indicating worse prognosis)</td>

  </tr>

  <tr>

   <td width="36"> </td>

   <td colspan="2" width="59">idnum</td>

   <td width="59">psa</td>

   <td width="68">cancerv</td>

   <td width="60">weight</td>

   <td width="38">age</td>

   <td colspan="2" width="94">hyperplasia</td>

   <td width="67">seminal</td>

   <td width="72">capsular</td>

   <td width="34">score</td>

   <td width="36"> </td>

  </tr>

  <tr>

   <td width="36"> </td>

   <td colspan="2" width="59">1</td>

   <td width="59">0.65</td>

   <td width="68">0.56</td>

   <td width="60">15.96</td>

   <td width="38">50</td>

   <td colspan="2" width="94">0</td>

   <td width="67">0</td>

   <td width="72">0</td>

   <td width="34">6</td>

   <td width="36"> </td>

  </tr>

  <tr>

   <td width="36"> </td>

   <td colspan="2" width="59">2</td>

   <td width="59">0.85</td>

   <td width="68">0.37</td>

   <td width="60">27.66</td>

   <td width="38">58</td>

   <td colspan="2" width="94">0</td>

   <td width="67">0</td>

   <td width="72">0</td>

   <td width="34">7</td>

   <td width="36"> </td>

  </tr>

  <tr>

   <td width="36"> </td>

   <td colspan="2" width="59">3</td>

   <td width="59">0.85</td>

   <td width="68">0.6</td>

   <td width="60">14.73</td>

   <td width="38">74</td>

   <td colspan="2" width="94">0</td>

   <td width="67">0</td>

   <td width="72">0</td>

   <td width="34">7</td>

   <td width="36"> </td>

  </tr>

  <tr>

   <td width="36"> </td>

   <td colspan="2" width="59">…</td>

   <td width="59">…</td>

   <td width="68">…</td>

   <td width="60">…</td>

   <td width="38">…</td>

   <td colspan="2" width="94">…</td>

   <td width="67">…</td>

   <td width="72">…</td>

   <td width="34">…</td>

   <td width="36"> </td>

  </tr>

  <tr>

   <td width="36"> </td>

   <td colspan="2" width="59">95</td>

   <td width="59">170.72</td>

   <td width="68">18.36</td>

   <td width="60">29.96</td>

   <td width="38">52</td>

   <td colspan="2" width="94">0</td>

   <td width="67">1</td>

   <td width="72">11.7</td>

   <td width="34">8</td>

   <td width="36"> </td>

  </tr>

  <tr>

   <td width="36"> </td>

   <td colspan="2" width="59">96</td>

   <td width="59">239.85</td>

   <td width="68">17.81</td>

   <td width="60">43.38</td>

   <td width="38">68</td>

   <td colspan="2" width="94">4.76</td>

   <td width="67">1</td>

   <td width="72">4.76</td>

   <td width="34">8</td>

   <td width="36"> </td>

  </tr>

  <tr>

   <td width="36"> </td>

   <td colspan="2" width="59">97</td>

   <td width="59">265.07</td>

   <td width="68">32.14</td>

   <td width="60">52.98</td>

   <td width="38">68</td>

   <td colspan="2" width="94">1.55</td>

   <td width="67">1</td>

   <td width="72">18.17</td>

   <td width="34">8</td>

   <td width="36"> </td>

  </tr>

  <tr>

   <td width="36"></td>

   <td width="41"></td>

   <td width="18"></td>

   <td width="59"></td>

   <td width="67"></td>

   <td width="60"></td>

   <td width="38"></td>

   <td width="32"></td>

   <td width="61"></td>

   <td width="67"></td>

   <td width="72"></td>

   <td width="35"></td>

   <td width="36"></td>

  </tr>

 </tbody>

</table>

<h1>Qn 3: Website Developer Dataset</h1>

Model Hint/Suggestion: Start with a Poisson regression model, check for over-dispersion, if present, consider fitting a Negative Binomial regression model

Recall that for Poisson regression, one of the assumptions for a valid model is that the mean and variance of the count variable are equal. The negative binomial distribution is a more generalized form of distribution used for ‘count’ response data, allowing for greater dispersion or variance of counts. In practice, it is quite common for the variance of the outcome to be larger than the mean. This is called overdispersion. If a count variable is overdispersed, Poisson regression underestimates the standard errors of the predictor variables. When overdispersion is evident, one solution is to specify that the errors have a negative binomial distribution.

Management of a company that develops websites was interested in determining which variables have the greatest impact on the number of websites developed and delivered to customers per quarter (Response variable: Websites delivered). Data were collected on website production output for 13 three-person website development teams, from January 2001 through August 2002. Each line of the data set has an identification number and provides information on 6 other variables for thirteen teams over time. The 8 variables are:

<table width="624">

 <tbody>

  <tr>

   <td colspan="2" width="77"><strong>Variable</strong></td>

   <td colspan="5" width="276"><strong>Variable Name</strong></td>

   <td colspan="5" width="271"><strong>Description</strong></td>

  </tr>

  <tr>

   <td colspan="2" width="77">1</td>

   <td colspan="5" width="276">idnum: Identification number</td>

   <td colspan="5" width="271">1 <em>− </em>73</td>

  </tr>

  <tr>

   <td colspan="2" width="77">2</td>

   <td colspan="5" width="276">delivered: Websites delivered</td>

   <td colspan="5" width="271">Number of websites completed and delivered to customers during the quarter</td>

  </tr>

  <tr>

   <td colspan="2" width="77">3</td>

   <td colspan="5" width="276">backlog: Backlog of orders</td>

   <td colspan="5" width="271">Number of website orders in backlog at the close of the quarter</td>

  </tr>

  <tr>

   <td colspan="2" width="77">4</td>

   <td colspan="5" width="276">teamnum: Team number</td>

   <td colspan="5" width="271">1 <em>− </em>13</td>

  </tr>

  <tr>

   <td colspan="2" width="77">5</td>

   <td colspan="5" width="276">experience: Team experience</td>

   <td colspan="5" width="271">Number of months team has been together</td>

  </tr>

  <tr>

   <td colspan="2" width="77">6</td>

   <td colspan="5" width="276">change: Process change</td>

   <td colspan="5" width="271">A change in the website development process occurred during the second quarter of 2002: 1 if quarter 2 or 3, 2002; 0 otherwise</td>

  </tr>

  <tr>

   <td colspan="2" width="77">7</td>

   <td colspan="5" width="276">year: Year</td>

   <td colspan="5" width="271">2001 or 2002</td>

  </tr>

  <tr>

   <td colspan="2" width="77">8</td>

   <td colspan="5" width="276">quarter: Quarter</td>

   <td colspan="5" width="271">1<em>,</em>2<em>,</em>3<em>, </em>or 4</td>

  </tr>

  <tr>

   <td width="48"> </td>

   <td colspan="2" width="59">idnum</td>

   <td width="77">delivered</td>

   <td width="67">backlog</td>

   <td width="80">teamnum</td>

   <td colspan="2" width="87">experience</td>

   <td width="62">change</td>

   <td width="47">year</td>

   <td width="50">quarter</td>

   <td width="48"> </td>

  </tr>

  <tr>

   <td width="48"> </td>

   <td colspan="2" width="59">1</td>

   <td width="77">1</td>

   <td width="67">12</td>

   <td width="80">1</td>

   <td colspan="2" width="87">3</td>

   <td width="62">0</td>

   <td width="47">2001</td>

   <td width="50">1</td>

   <td width="48"> </td>

  </tr>

  <tr>

   <td width="48"> </td>

   <td colspan="2" width="59">2</td>

   <td width="77">2</td>

   <td width="67">18</td>

   <td width="80">1</td>

   <td colspan="2" width="87">6</td>

   <td width="62">0</td>

   <td width="47">2001</td>

   <td width="50">2</td>

   <td width="48"> </td>

  </tr>

  <tr>

   <td width="48"> </td>

   <td colspan="2" width="59">3</td>

   <td width="77">7</td>

   <td width="67">26</td>

   <td width="80">1</td>

   <td colspan="2" width="87">9</td>

   <td width="62">0</td>

   <td width="47">2001</td>

   <td width="50">3</td>

   <td width="48"> </td>

  </tr>

  <tr>

   <td width="48"> </td>

   <td colspan="2" width="59">4</td>

   <td width="77">2</td>

   <td width="67">28</td>

   <td width="80">1</td>

   <td colspan="2" width="87">12</td>

   <td width="62">0</td>

   <td width="47">2001</td>

   <td width="50">4</td>

   <td width="48"> </td>

  </tr>

  <tr>

   <td width="48"> </td>

   <td colspan="2" width="59">…</td>

   <td width="77">…</td>

   <td width="67">…</td>

   <td width="80">…</td>

   <td colspan="2" width="87">…</td>

   <td width="62">…</td>

   <td width="47">…</td>

   <td width="50">…</td>

   <td width="48"> </td>

  </tr>

  <tr>

   <td width="48"> </td>

   <td colspan="2" width="59">70</td>

   <td width="77">7</td>

   <td width="67">28</td>

   <td width="80">13</td>

   <td colspan="2" width="87">11</td>

   <td width="62">0</td>

   <td width="47">2001</td>

   <td width="50">4</td>

   <td width="48"> </td>

  </tr>

  <tr>

   <td width="48"> </td>

   <td colspan="2" width="59">71</td>

   <td width="77">7</td>

   <td width="67">36</td>

   <td width="80">13</td>

   <td colspan="2" width="87">14</td>

   <td width="62">0</td>

   <td width="47">2002</td>

   <td width="50">1</td>

   <td width="48"> </td>

  </tr>

  <tr>

   <td width="48"> </td>

   <td colspan="2" width="59">72</td>

   <td width="77">19</td>

   <td width="67">37</td>

   <td width="80">13</td>

   <td colspan="2" width="87">17</td>

   <td width="62">1</td>

   <td width="47">2002</td>

   <td width="50">2</td>

   <td width="48"> </td>

  </tr>

  <tr>

   <td width="48"> </td>

   <td colspan="2" width="59">73</td>

   <td width="77">12</td>

   <td width="67">26</td>

   <td width="80">13</td>

   <td colspan="2" width="87">20</td>

   <td width="62">1</td>

   <td width="47">2002</td>

   <td width="50">3</td>

   <td width="48"> </td>

  </tr>

  <tr>

   <td width="48"></td>

   <td width="30"></td>

   <td width="29"></td>

   <td width="77"></td>

   <td width="67"></td>

   <td width="80"></td>

   <td width="23"></td>

   <td width="64"></td>

   <td width="62"></td>

   <td width="47"></td>

   <td width="50"></td>

   <td width="48"></td>

  </tr>

 </tbody>

</table>

<h1>Qn 4: Market Share Dataset</h1>

Model Hint/Suggestion: Multiple linear regression model

Company executives from a large packaged foods manufacturer wished to determine which factors influence the market share of one of its products (market share is the response variable). Data were collected from a national database (Nielsen) for 36 consecutive months. Each line of the data set has an identification number and provides information on 6 other variables for each month. The data presented here are for September, 1999, through August, 2002. The variables are:

<table width="624">

 <tbody>

  <tr>

   <td colspan="2" width="77"><strong>Variable</strong></td>

   <td colspan="5" width="275"><strong>Variable Name</strong></td>

   <td colspan="5" width="272"><strong>Description</strong></td>

  </tr>

  <tr>

   <td colspan="2" width="77">1</td>

   <td colspan="5" width="275">idnum: Identification number</td>

   <td colspan="5" width="272">1 <em>− </em>36</td>

  </tr>

  <tr>

   <td colspan="2" width="77">2</td>

   <td colspan="5" width="275">marketshare: Market share</td>

   <td colspan="5" width="272">Average monthly market share for product(percent)</td>

  </tr>

  <tr>

   <td colspan="2" width="77">3</td>

   <td colspan="5" width="275">price: Price</td>

   <td colspan="5" width="272">Average monthly price of product (dollars)</td>

  </tr>

  <tr>

   <td colspan="2" width="77">4</td>

   <td colspan="5" width="275">gnrpoints: Gross Nielson rating points</td>

   <td colspan="5" width="272">An index of the amount of advertising exposure that the product received</td>

  </tr>

  <tr>

   <td colspan="2" width="77">5</td>

   <td colspan="5" width="275">discount: Discount price</td>

   <td colspan="5" width="272">Presence or absence of discount price during period: 1 if discount, 0 otherwise</td>

  </tr>

  <tr>

   <td colspan="2" width="77">6</td>

   <td colspan="5" width="275">promotion: Package promotion</td>

   <td colspan="5" width="272">Presence or absence of package promotion during period: 1 if promotion present, 0 otherwise</td>

  </tr>

  <tr>

   <td colspan="2" width="77">7</td>

   <td colspan="5" width="275">month: Month</td>

   <td colspan="5" width="272">Month (Jan-Dec)</td>

  </tr>

  <tr>

   <td colspan="2" width="77">8</td>

   <td colspan="5" width="275">year: Year</td>

   <td colspan="5" width="272">Year (1999 – 2002)</td>

  </tr>

  <tr>

   <td width="43"> </td>

   <td colspan="2" width="59">idnum</td>

   <td width="99">marketshare</td>

   <td width="49">price</td>

   <td width="80">gnrpoints</td>

   <td colspan="2" width="73">discount</td>

   <td width="86">promotion</td>

   <td width="60">month</td>

   <td width="31">year</td>

   <td width="44"> </td>

  </tr>

  <tr>

   <td width="43"> </td>

   <td colspan="2" width="59">1</td>

   <td width="99">3.15</td>

   <td width="49">2.2</td>

   <td width="80">498</td>

   <td colspan="2" width="73">1</td>

   <td width="86">1</td>

   <td width="60">Sep</td>

   <td width="31">1999</td>

   <td width="44"> </td>

  </tr>

  <tr>

   <td width="43"> </td>

   <td colspan="2" width="59">2</td>

   <td width="99">2.52</td>

   <td width="49">2.19</td>

   <td width="80">510</td>

   <td colspan="2" width="73">0</td>

   <td width="86">0</td>

   <td width="60">Oct</td>

   <td width="31">1999</td>

   <td width="44"> </td>

  </tr>

  <tr>

   <td width="43"> </td>

   <td colspan="2" width="59">3</td>

   <td width="99">2.64</td>

   <td width="49">2.29</td>

   <td width="80">422</td>

   <td colspan="2" width="73">1</td>

   <td width="86">1</td>

   <td width="60">Nov</td>

   <td width="31">1999</td>

   <td width="44"> </td>

  </tr>

  <tr>

   <td width="43"> </td>

   <td colspan="2" width="59">4</td>

   <td width="99">2.55</td>

   <td width="49">2.42</td>

   <td width="80">858</td>

   <td colspan="2" width="73">0</td>

   <td width="86">1</td>

   <td width="60">Dec</td>

   <td width="31">1999</td>

   <td width="44"> </td>

  </tr>

  <tr>

   <td width="43"> </td>

   <td colspan="2" width="59">…</td>

   <td width="99">…</td>

   <td width="49">…</td>

   <td width="80">…</td>

   <td colspan="2" width="73">…</td>

   <td width="86">…</td>

   <td width="60">NA</td>

   <td width="31">…</td>

   <td width="44"> </td>

  </tr>

  <tr>

   <td width="43"> </td>

   <td colspan="2" width="59">33</td>

   <td width="99">2.88</td>

   <td width="49">2.42</td>

   <td width="80">145</td>

   <td colspan="2" width="73">1</td>

   <td width="86">1</td>

   <td width="60">May</td>

   <td width="31">2002</td>

   <td width="44"> </td>

  </tr>

  <tr>

   <td width="43"> </td>

   <td colspan="2" width="59">34</td>

   <td width="99">2.8</td>

   <td width="49">2.52</td>

   <td width="80">270</td>

   <td colspan="2" width="73">1</td>

   <td width="86">0</td>

   <td width="60">Jun</td>

   <td width="31">2002</td>

   <td width="44"> </td>

  </tr>

  <tr>

   <td width="43"> </td>

   <td colspan="2" width="59">35</td>

   <td width="99">2.48</td>

   <td width="49">2.5</td>

   <td width="80">322</td>

   <td colspan="2" width="73">0</td>

   <td width="86">1</td>

   <td width="60">Jul</td>

   <td width="31">2002</td>

   <td width="44"> </td>

  </tr>

  <tr>

   <td width="43"> </td>

   <td colspan="2" width="59">36</td>

   <td width="99">2.85</td>

   <td width="49">2.78</td>

   <td width="80">317</td>

   <td colspan="2" width="73">1</td>

   <td width="86">1</td>

   <td width="60">Aug</td>

   <td width="31">2002</td>

   <td width="44"> </td>

  </tr>

  <tr>

   <td width="43"></td>

   <td width="34"></td>

   <td width="25"></td>

   <td width="99"></td>

   <td width="49"></td>

   <td width="80"></td>

   <td width="22"></td>

   <td width="51"></td>

   <td width="86"></td>

   <td width="60"></td>

   <td width="33"></td>

   <td width="43"></td>

  </tr>

 </tbody>

</table>

<h1>Qn 5: Disease Outbreak Dataset</h1>

Model Hint/Suggestion: Multiple logistic regression model source = Book Website

Adapted in part from H.G. Dantes, J.S. Koopman, C.L. Addy, et. al., “Dengue Epidemics on the Pacific Coast of Mexico.” <em>International Journal of Epidemiology </em>17 (1988), <em>pp</em>. 178 <em>− </em>86

The data set below provides information from a study based on 196 persons selected in a probability sample within two sectors in a city. Assume that the response variable (main outcome of interest) is disease: (Disease status) which is coded 1 if the person has a disease or 0 if they do not have a disease. Each line of the dat set has an identification number (id) and provides information on 5 other variables (exposure/independent variables) for each person. The 6 variables are:

<table width="624">

 <tbody>

  <tr>

   <td width="77"><strong>Variable</strong></td>

   <td colspan="6" width="277"><strong>Variable Name</strong></td>

   <td colspan="3" width="270"><strong>Description</strong></td>

  </tr>

  <tr>

   <td width="77">1</td>

   <td colspan="6" width="277">id: Identification number</td>

   <td colspan="3" width="270">1 <em>− </em>196</td>

  </tr>

  <tr>

   <td width="77">2</td>

   <td colspan="6" width="277">ageyrs: Age</td>

   <td colspan="3" width="270">Age of person (in years)</td>

  </tr>

  <tr>

   <td width="77">3</td>

   <td colspan="6" width="277">ses: Socio-economic status</td>

   <td colspan="3" width="270">1 = upper, 2 = middle, 3 = lower</td>

  </tr>

  <tr>

   <td width="77">4</td>

   <td colspan="6" width="277">sector: Sector</td>

   <td colspan="3" width="270">Sector within city, where: 1 = sector 1, 2 = sector 2</td>

  </tr>

  <tr>

   <td width="77">5</td>

   <td colspan="6" width="277">disease: Disease status</td>

   <td colspan="3" width="270">1 = with disease, 0 = without disease</td>

  </tr>

  <tr>

   <td width="77">6</td>

   <td colspan="6" width="277">savings: Savings account status</td>

   <td colspan="3" width="270">1 = has savings account, 0 = does not have savings account</td>

  </tr>

  <tr>

   <td colspan="2" width="161"> </td>

   <td width="39">id</td>

   <td width="59">ageyrs</td>

   <td width="37">ses</td>

   <td width="56">sector</td>

   <td colspan="2" width="63">disease</td>

   <td width="49">savings</td>

   <td width="161"> </td>

  </tr>

  <tr>

   <td colspan="2" width="161"> </td>

   <td width="39">1</td>

   <td width="59">33</td>

   <td width="37">1</td>

   <td width="56">1</td>

   <td colspan="2" width="63">0</td>

   <td width="49">1</td>

   <td width="161"> </td>

  </tr>

  <tr>

   <td colspan="2" width="161"> </td>

   <td width="39">2</td>

   <td width="59">35</td>

   <td width="37">1</td>

   <td width="56">1</td>

   <td colspan="2" width="63">0</td>

   <td width="49">1</td>

   <td width="161"> </td>

  </tr>

  <tr>

   <td colspan="2" width="161"> </td>

   <td width="39">3</td>

   <td width="59">6</td>

   <td width="37">1</td>

   <td width="56">1</td>

   <td colspan="2" width="63">0</td>

   <td width="49">0</td>

   <td width="161"> </td>

  </tr>

  <tr>

   <td colspan="2" width="161"> </td>

   <td width="39">4</td>

   <td width="59">60</td>

   <td width="37">1</td>

   <td width="56">1</td>

   <td colspan="2" width="63">0</td>

   <td width="49">1</td>

   <td width="161"> </td>

  </tr>

  <tr>

   <td colspan="2" width="161"> </td>

   <td width="39">…</td>

   <td width="59">…</td>

   <td width="37">…</td>

   <td width="56">…</td>

   <td colspan="2" width="63">…</td>

   <td width="49">…</td>

   <td width="161"> </td>

  </tr>

  <tr>

   <td colspan="2" width="161"> </td>

   <td width="39">193</td>

   <td width="59">10</td>

   <td width="37">3</td>

   <td width="56">1</td>

   <td colspan="2" width="63">0</td>

   <td width="49">1</td>

   <td width="161"> </td>

  </tr>

  <tr>

   <td colspan="2" width="161"> </td>

   <td width="39">194</td>

   <td width="59">31</td>

   <td width="37">3</td>

   <td width="56">1</td>

   <td colspan="2" width="63">0</td>

   <td width="49">0</td>

   <td width="161"> </td>

  </tr>

  <tr>

   <td colspan="2" width="161"> </td>

   <td width="39">195</td>

   <td width="59">85</td>

   <td width="37">3</td>

   <td width="56">1</td>

   <td colspan="2" width="63">0</td>

   <td width="49">1</td>

   <td width="161"> </td>

  </tr>

  <tr>

   <td colspan="2" width="161"> </td>

   <td width="39">196</td>

   <td width="59">24</td>

   <td width="37">2</td>

   <td width="56">1</td>

   <td colspan="2" width="63">0</td>

   <td width="49">0</td>

   <td width="161"> </td>

  </tr>

  <tr>

   <td width="77"></td>

   <td width="83"></td>

   <td width="39"></td>

   <td width="59"></td>

   <td width="37"></td>

   <td width="56"></td>

   <td width="3"></td>

   <td width="60"></td>

   <td width="49"></td>

   <td width="161"></td>

  </tr>

 </tbody>

</table>

<h1>Qn 6: Mosquito larva infestation Dataset</h1>

Model Hint/Suggestion: Multiple Poisson regression and Negative Binomial regression Models

Recall that for Poisson regression, one of the assumptions for a valid model is that the mean and variance of the count variable are equal. The negative binomial distribution is a more generalized form of distribution used for ‘count’ response data, allowing for greater dispersion or variance of counts. In practice, it is quite common for the variance of the outcome to be larger than the mean. This is called overdispersion. If a count variable is overdispersed, Poisson regression underestimates the standard errors of the predictor variables. When overdispersion is evident, one solution is to specify that the errors have a negative binomial distribution.

Use the data set DHF99 from the R package epiDisplay. Type library(epiDisplay) then ?DHF99 to see more details about the dataset.

The main outcome of interest (response variable) is counts of water containers infested with mosquito larvae in a field survey. This is variable containers in the data.

<table width="632">

 <tbody>

  <tr>

   <td colspan="4" width="632"><strong>library</strong>(epiDisplay) <strong>data</strong>(“DHF99”)<em># create a new dataset to manipulate </em>malaria &lt;- DHF99 <strong>summ</strong>(malaria)</td>

  </tr>

  <tr>

   <td width="1"> </td>

   <td width="410">#### No. of observations = 300##</td>

   <td width="33"> </td>

   <td width="188"> </td>

  </tr>

  <tr>

   <td width="1"> </td>

   <td width="410">##          Var. name obs. mean             median s.d.          min.</td>

   <td width="33">max.</td>

   <td width="188"> </td>

  </tr>

  <tr>

   <td width="1"> </td>

   <td width="410">## 1 houseid                300 174.27 154.5           112.44 1</td>

   <td width="33">385</td>

   <td width="188"> </td>

  </tr>

  <tr>

   <td width="1"> </td>

   <td width="410">## 2 village                   300 48.56 51                  32.25 1</td>

   <td width="33">105</td>

   <td width="188"> </td>

  </tr>

  <tr>

   <td width="1"> </td>

   <td width="410">## 3 education 300 2.09                   1                 1.455 1</td>

   <td width="33">5</td>

   <td width="188"> </td>

  </tr>

  <tr>

   <td width="1"> </td>

   <td width="410">## 4 containers 299 0.35                  0               1.01       0</td>

   <td width="33">11</td>

   <td width="188"> </td>

  </tr>

  <tr>

   <td width="1"> </td>

   <td width="410">## 5 viltype                300 1.56         1                 0.754 1</td>

   <td width="33">3</td>

   <td width="188"> </td>

  </tr>

  <tr>

   <td width="1"></td>

   <td width="410"></td>

   <td width="33"></td>

   <td width="188"></td>

  </tr>

 </tbody>

</table>

<strong>codebook</strong>(malaria)

##

##

##

## houseid          :       no

## obs. mean                median s.d.            min.       max.

## 300 174.273 154.5                  112.439 1             385

##

## ==================

## village            :         Village

## obs. mean              median s.d.          min.       max.

## 300 48.56 51                         32.253 1              105

##

## ==================

## education              :           Educational level

##                             Frequency Percent

<table width="262">

 <tbody>

  <tr>

   <td width="123">## Primary</td>

   <td width="98">168</td>

   <td width="41">56.00</td>

  </tr>

  <tr>

   <td width="123">## Secondary</td>

   <td width="98">36</td>

   <td width="41">12.00</td>

  </tr>

  <tr>

   <td width="123">## High school</td>

   <td width="98">34</td>

   <td width="41">11.33</td>

  </tr>

  <tr>

   <td width="123">## Bachelor</td>

   <td width="98">25</td>

   <td width="41">8.33</td>

  </tr>

  <tr>

   <td width="123">## Other</td>

   <td width="98">37</td>

   <td width="41">12.33</td>

  </tr>

 </tbody>

</table>

##

## ==================

## containers              :           # infested vessels

## obs. mean              median s.d.          min.       max.

## 299 0.351 0                            1.014 0               11

##

## ==================

## viltype            :          Village type

##                 Frequency Percent

## rural           180      60 ## urban     72        24 ## slum           48        16

##

## ==================

<table width="380">

 <tbody>

  <tr>

   <td width="39"> </td>

   <td width="67">houseid</td>

   <td width="60">village</td>

   <td width="82">education</td>

   <td width="85">containers</td>

   <td width="47">viltype</td>

  </tr>

  <tr>

   <td width="39">1</td>

   <td width="67">1</td>

   <td width="60">22</td>

   <td width="82">Other</td>

   <td width="85">3</td>

   <td width="47">rural</td>

  </tr>

  <tr>

   <td width="39">2</td>

   <td width="67">2</td>

   <td width="60">22</td>

   <td width="82">Primary</td>

   <td width="85">1</td>

   <td width="47">rural</td>

  </tr>

  <tr>

   <td width="39">3</td>

   <td width="67">3</td>

   <td width="60">22</td>

   <td width="82">Primary</td>

   <td width="85">0</td>

   <td width="47">rural</td>

  </tr>

  <tr>

   <td width="39">4</td>

   <td width="67">4</td>

   <td width="60">22</td>

   <td width="82">Primary</td>

   <td width="85">0</td>

   <td width="47">rural</td>

  </tr>

  <tr>

   <td width="39">…</td>

   <td width="67">…</td>

   <td width="60">…</td>

   <td width="82">NA</td>

   <td width="85">…</td>

   <td width="47">NA</td>

  </tr>

  <tr>

   <td width="39">297</td>

   <td width="67">382</td>

   <td width="60">39</td>

   <td width="82">Primary</td>

   <td width="85">0</td>

   <td width="47">rural</td>

  </tr>

  <tr>

   <td width="39">298</td>

   <td width="67">383</td>

   <td width="60">39</td>

   <td width="82">Primary</td>

   <td width="85">0</td>

   <td width="47">rural</td>

  </tr>

  <tr>

   <td width="39">299</td>

   <td width="67">384</td>

   <td width="60">39</td>

   <td width="82">Primary</td>

   <td width="85">0</td>

   <td width="47">rural</td>

  </tr>

  <tr>

   <td width="39">300</td>

   <td width="67">385</td>

   <td width="60">39</td>

   <td width="82">Primary</td>

   <td width="85">0</td>

   <td width="47">rural</td>

  </tr>

 </tbody>

</table>


