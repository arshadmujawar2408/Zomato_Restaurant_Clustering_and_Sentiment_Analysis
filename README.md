# ML for Zomato Restaurant Clustering and Sentiment Analysis
  Zomato is an Indian restaurant aggregator and food delivery start-up founded by Deepinder Goyal and Pankaj Chaddah in 2008. Zomato provides information, menus and user-reviews of restaurants, and also has food delivery options from partner restaurants in select cities. India is quite famous for its diverse multi cuisine available in a large number of restaurants and hotel resorts, which is reminiscent of unity in diversity. Restaurant business in India is always evolving. More Indians are warming up to the idea of eating restaurant food whether by dining outside or getting food delivered. The growing number of restaurants in every state of India has been a motivation to inspect the data to get some insights, interesting facts and figures about the Indian food industry in each city. So, this project focuses on analysing the Zomato restaurant data for each city in India.

Project focuses on Customers and Company, you have to analyze the sentiments of the reviews given by the customer in the data and make some useful conclusions in the form of Visualizations. Also, cluster the zomato restaurants into different segments. The data is vizualized as it becomes easy to analyse data at instant. The Analysis also solves some of the business cases that can directly help the customers finding the Best restaurant in their locality and for the company to grow up and work on the fields they are currently lagging in. This could help in clustering the restaurants into segments. Also the data has valuable information around cuisine and costing which can be used in cost vs: benefit analysis Data could be used for sentiment analysis. Also the metadata of reviewers can be used for identifying the critics in the industry.

**Programming Language** : Python

**Libraries used** : Pandas, Numpy, Matplotlib, Seaborn, Sklearn

**NoteBook** : Google Colab

**Dataset Source** : Provided by Almabetter themself.
 
## Dataset 
We are given an Mobile Price Range dataset. It contains the following features.
```
- Name : Name of Restaurants
- Links : URL Links of Restaurants
- Cost : Per person estimated Cost of dining
- Collection : Tagging of Restaurants w.r.t. Zomato categories
- Cuisines : Cuisines served by Restaurants
- Timings : Restaurant Timings
- Zomato Restaurant Reviews
- Restaurant : Name of the Restaurant
- Reviewer : Name of the Reviewer
- Review : Review Text
- Rating : Rating Provided by Reviewer
- MetaData : Reviewer Metadata - No. of Reviews and followers
- Time: Date and Time of Review
- Pictures : No. of pictures posted with review
```

- Restaurant DataSet 

There are 105 total observation with 6 different features.
Feature like collection and timing has null values.
There is no duplicate values i.e., 105 unique data.
Feature cost represent amount but has object data type because these values are separated by comma ','.
Timing represent operational hour but as it is represented in the form of text has object data type.

- Review DataSet 

There are total 10000 observation and 7 features.
Except picture and restaurant feature all others have null values.
There are total of 36 duplicate values for two restaurant - American Wild Wings and Arena Eleven, where all these duplicate values generally have null values.
Rating represent ordinal data, has object data type should be integer.
Timing represent the time when review was posted but show object data time, it should be converted into date time.
 
  
## Exploratory Data Analysis
 Mainly performed using Matplotlib and Seaborn library and the following graph and plots had been used:
   - DisPlot.
   - Bar Plot.
   - Pie Chart.
   - Heatmap
   - Correction heatmap
             
## ML Model Used:

Several machine learning algorithms were utilized. These models include:
```
1. Logistic Regression
2. clustering technique
3. Sentiment analysis
4. XGboost Classifier
 ```

## Conclusion  
Clustering and sentiment analysis were performed on a dataset of customer reviews for the food delivery service Zomato. The purpose of this analysis was to understand the customer's experience and gain insights about their feedback.

The clustering technique was applied to group customers based on their review text, and it was found that the customers were grouped into two clusters: positive and negative. This provided a general understanding of customer satisfaction levels, with the positive cluster indicating the highest level of satisfaction and the negative cluster indicating the lowest level of satisfaction.

Sentiment analysis was then applied to classify the review text as positive or negative. This provided a more detailed understanding of customer feedback and helped to identify specific areas where the service could be improved.

Overall, this analysis provided valuable insights into the customer's experience with Zomato, and it could be used to guide future business decisions and improve the service. Additionally, by combining clustering and sentiment analysis techniques, a more comprehensive understanding of customer feedback was achieved.

Other important discoveries during analysis are -

- AB's - Absolute Barbecues, show maximum engagement and retention as it has maximum number of rating on average and Hotel Zara Hi-Fi show lowest engagement as has lowest average rating.
- Price point for high rated hotel AB's= Absolute Barbecues is 1500 and price point for low rated restaurant Hotel Zara Hi-Fi is 400.
- North Indian food followed by chinese are best or indeemand food as sold by most of the restaurants.
- Great Buffets is the most frequently used tags and other tags like great, best, north, Hyderabad is also used in large quantity.
- Satwinder singh is the most popular critic who has maximum number of follower and on an average he give 3.5 rating.
- restaurant Collage - Hyatt Hyderabad Gachibowli is most expensive restaurant in the locality which has a price of 2800 for order and has 3.5 average rating. Hotels like Amul and Mohammedia Shawarma are least expensive with price of 150 and has 3.9 average rating.

Some recommendation based on the analysis :

- Based on negative reviews like some focused on issues with delivery time or food quality, the company should prioritize addressing these issues to imporve customer satisfaction.
- Based on the clustering, or user interaction customer should be given recommendations.
- Also use the clustering results to target specific customer segments and tailor marketing and promotional efforts accordingly.
