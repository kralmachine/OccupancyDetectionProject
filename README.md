
<p>In this project, the environment data from an IOT device in an office environment should be investigated. Office space is controlled by the amount of people in the office. Incoming data are date, carbon dioxide, light, temperature, humidity, humidity ratio and occupancy. There are three data sets in the documents. One of these data sets is the train set. Other data sets are test data sets. In this test data, the office room of the first test data is closed. The second test data room is open. Methods for such problems will be developed. Sci-kit library will be used when analyzing and modeling. Our aim here is to make sure that there are no people in the office. For this purpose, analysis of data will be done and machine learning algorithms will be used through both test and training data.</p>

<p>Kullanılan araçlar;</p>
<ul>
<li>Anaconda</li>
<li>Python</li>
<li>Jupyter</li>
<li>Scikit-Learn</li>
<li>Pandas</li>
<li>Seaborn</li>
<li>Matplotlib</li>
<li>Datas<li/>
</ul>

<p>We will perform analysis on the training data. The relationship between the features found in the training data is observed. In this way, comments about the properties can be made.</p>

![scatter matrix 1](https://user-images.githubusercontent.com/28226570/51667361-9843a100-1fc8-11e9-9a16-8fb3190d5d62.png)

<p>There are different data defined in the "occupancy" section of the training data. I will show it on Seaborn library. How many data are available?</p>

![occupancy value counts](https://user-images.githubusercontent.com/28226570/51667394-abef0780-1fc8-11e9-8dd0-1a74702e2d31.png)

<p>We had unique dates. The IOT device worked exactly 1 week. I must check out how much data I have collected during the entire week. Because I have to check if there is a big difference between the data.</p>

![unique dates value counts](https://user-images.githubusercontent.com/28226570/51667461-d17c1100-1fc8-11e9-8486-a13159f2da18.png)

<p>All Week Analsis Temperature</p>
![all wekeend analysis temperature](https://user-images.githubusercontent.com/28226570/51667488-ed7fb280-1fc8-11e9-9ecf-0a1281e0a9f8.png)

<p>All Week Alaysis CO2</p>

![all weekend analysis co2](https://user-images.githubusercontent.com/28226570/51667514-f96b7480-1fc8-11e9-9d33-5d6f2aaba3b0.png)

<p>All Weekend Analysis HumidityRatio</p>

![all weekend analysis humidityratio](https://user-images.githubusercontent.com/28226570/51667562-05efcd00-1fc9-11e9-94cf-2e0875ae6f93.png)

<p>All Weekend Analysis Light</p>

![all weekend analysis light](https://user-images.githubusercontent.com/28226570/51667633-0e480800-1fc9-11e9-97cc-7fc8d92e89de.png)

<p>All Wekeen Analysis Humidity</p>

![all wekeen analysis humidity](https://user-images.githubusercontent.com/28226570/51667658-143de900-1fc9-11e9-947f-ea22c0730516.png)

<p>We have drawn the results. We have drawn out the missing data. Because, in any way, we do not want incomplete data or incomplete data. There may be a big problem training our training set.</p>

![unique dates anaysis for all feature](https://user-images.githubusercontent.com/28226570/51667688-2cae0380-1fc9-11e9-82fd-ee5217bc42c8.png)

<p>As a result of our evaluation, we analyzed according to the hour. This way we can make comments on the graph. The graph shows how high the data is within certain study areas. Sometimes it is seen how much data is below the value.
Thus, we can make inferences about the data. Office workers may have a day at lunch. Then maybe they could have gone to lunch.
In addition, there is a possibility that it will coincide with the end of the week. We will continue to take action considering all situations.</p>

![all time analysis for all data_v2](https://user-images.githubusercontent.com/28226570/51667715-3e8fa680-1fc9-11e9-96a2-642273138dda.png)

<p>As a result of all our evaluations are described in the following scatter matrix. The next evaluation will be adding new features.</p>

![the last scatter matrix](https://user-images.githubusercontent.com/28226570/51667739-4fd8b300-1fc9-11e9-8563-882b99271253.png)

<p>3. Modeling, Training and Testing
Now, data analysis.
We have to divide all of our data sets while analyzing data. Because the data in our model will be trained first and then the test data will be used to predict the values.
In addition I have defined the feature list. The algorithm I developed will be used to test models. So, the features will be tested by dividing them into different combinations.
List of Algorithms to Use :
Logistic Regression
Naïve Bayes
K-Nearest Neighbors
Decision Tree
Random Forest
Gradient Boosting Machine
Kernelized Support Vector Machine
Generally, the model I followed in algorithms is as follows
Defining parameters
Defining feature combinations
I've created a Cross-validation value.
Fit the model and predict train, test1, and test2 sets.
Print classification report.
After running each model I wrote the results of a table halide. In addition, I have made various evaluations.</p>

<p>Thus, if we want to examine the changes in all datasets in the knn algorithm, we see the graph above. As you can see, there is good progress in the data training section. In addition, it is effective in progress in test1 data. But test2 presents problems in the data set. Here we need to do in the test2 data set, I will either extract and export outlier data, or add data.</p>

![knn 1-100 between analysis](https://user-images.githubusercontent.com/28226570/51667857-95957b80-1fc9-11e9-8da7-e9c57167dcc7.png)





















