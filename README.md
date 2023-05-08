Download Link: https://assignmentchef.com/product/solved-sta309-assignment2-data-visualization
<br>
If an aircraft is present in a certain area, a radar correctly registers its presence with probability 0.99. If it is not present, the radar falsely registers an aircraft presence with probability 0.10. Suppose that on average across all days, an aircraft is present with probability 0.05.

The radar today just registered the presence of an aircraft. What is the probability that an aircraft is actually present? Make sure to show your work.

<h1>Problem 2</h1>

Download the data in creatinine.csv. Each row is a patient in a doctor’s office. The variables are:

<ul>

 <li>age: patient’s age in years.</li>

 <li>creatclear: patient’s creatinine clearance rate in mL/minute, a measure of kidney health (a higher rate means better clearance, i.e., more healthy).</li>

</ul>

Use this data, together with your knowledge of linear regression, to answer three questions:

<ol>

 <li>What creatinine clearance rate should we expect for a 55-year-old? Explain briefly (using one or two sentences and equations) how you determined this.</li>

 <li>How does creatinine clearance rate change with age? (This should be a single number whose units are ml/minute per year.) Explain briefly (one or two sentences) how you determined this.</li>

 <li>Whose creatinine clearance rate is healthier (higher) for their age: a 40-year-old with a rate of 135, or a 60-year-old with a rate of 112? Explain briefly (a few sentences + equations) how you determined this.</li>

</ol>

<h1>Problem 3</h1>

Epidemiologists are investigating a cluster of respiratory disease around a coal-powered electricity generating station. Of 1072 elderly residents living within 5 miles of the coal plant, 49 of them have COPD, or chronic obstructive pulmonary disease, which is an inflammatory lung disease that causes breathing problems [<a href="https://www.cdc.gov/copd/index.html">ref</a><a href="https://www.cdc.gov/copd/index.html">]</a>. The baseline rate of COPD among elderly people across the country is 3.3%. Is the observed data (49 cases out of 1072) consistent with the null hypothesis that, over the long run, elderly residents within 5 miles of the power plant experience COPD at the national background rate?

Use Monte Carlo simulation (with at least 100,000 simulations) to calculate a p-value under this null hypothesis. Include the following items in your write-up:

<ul>

 <li>the null hypothesis your are testing;</li>

 <li>the test statistic you used to measure evidence against the null hypothesis;</li>

 <li>a picture of the probability distribution of the test statistic, assuming that the null hypothesis is true; • the p-value itself;</li>

</ul>

1

<ul>

 <li>and a one-sentence conclusion about whether you think the null hypothesis looks plausible in light of the data.</li>

</ul>

<h1>Problem 4</h1>

An important model that finance professionals use to understand asset prices is called the Capital Asset Pricing Model (CAPM). You will learn more about the CAPM in a future finance course. But the basic assumption of the model is that the rate of return on an individual stock is linearly related to the rate of return on the overall stock market. That is, each stock’s rate of return is assumed to follow a linear regression model:

<em><sup>Y</sup></em><em><sub>t</sub></em>(<em>k</em>) = <em><sup>β</sup></em><sub>0</sub>(<em>k</em>) + <em><sup>β</sup></em><sub>1</sub>(<em>k</em>)<em>X<sub>t </sub></em>+ <em>e</em>(<em><sub>t</sub></em><em>k</em>) <em>,</em>

where <em>Y<sub>t</sub></em><sup>(<em>k</em>) </sup>is the rate of return of an individual stock (<em>k</em>) in some given time period <em>t</em>; <em>X<sub>t </sub></em>is the rate of return of the entire stock market in that same time period; and <em>e</em><sup>(</sup><em><sub>t</sub><sup>k</sup></em><sup>) </sup>is the residual for stock <em>k </em>in that time period. The superscript (<em>k</em>)’s here are simply denoting the different stocks (Apple, Target, etc), while the subscript <em>t</em>’s are denoting the different time periods. Note that the market rate of return (<em>X<sub>t</sub></em>) is a predictor common to all stocks. (The rate of return can be interpreted similarly to an interest rate. For example, if a stock was worth $100 yesterday and $102 today, then it gained 2%, for an implied daily rate of return of 0.02.)

The <em>β</em><sub>1 </sub>(slope) term in this regression model is super important to finance professionals; they just call it

“beta”, and they refer to the <em>β</em><sub>0 </sub>(intercept) term as “alpha.” Please watch <a href="https://www.youtube.com/watch?v=B168aNJYywc">this short YouTube video</a> to understand how beta is used to think about different stocks.

Once you’ve watched the video, please turn to the data in marketmodel.csv, which contains information on the daily returns for the S&amp;P 500 stock index, denoted SPY, along with the returns for 6 individual stocks: Apple (AAPL), Google (GOOG), Merck (MRK), Johnson and Johnson (JNJ), Wal-Mart (WMT), and Target

(TGT). (We can think of the return of the S&amp;P 500 as a proxy for the whole market.) The data start from the beginning of 2019. The entries are interpretable as percentage returns, expressed on a 0-to-1 decimal scale—for example, if the S&amp;P 500 gained 1.5% in value on a given day, the corresponding entry in the data frame would be 0.015.

Regress the returns for each of the 6 stocks individually on the return of S&amp;P 500 (which is like <em>X<sub>t</sub></em>, the market return, in the equation above). Make a clean, professional looking table (e.g. in Excel) that shows the ticker symbol, intercept, slope, and <em>R</em><sup>2 </sup>for each of the 6 regressions.

In your write-up, you should include:

<ul>

 <li>a two-to-three paragraph introduction, in your own words, on what the “beta” of a stock is measuring and how it is calculated. (Watch the video and summarize it in your own words, making sure to connect it to the regression model we’ve written down above—this is a bridge you will have to make yourself, using what you know about regression models.) A reasonable aim for your summary is about 250 words here, but this is approximate; nobody on our end is breaking out the word counter.</li>

 <li>the table itself, along with an informative caption below the table, no more than 2-3 sentences in length, to give readers the information necessary to interpret the table.</li>

 <li>a conclusion that answers two questions: in light of your analysis, which of these six stocks has the <em>lowest </em>systematic risk? And which has the <em>highest </em>systematic risk? (Again, watch the video to understand how this is measured using the regression model.)</li>

</ul>