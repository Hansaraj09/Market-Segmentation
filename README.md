# Market-Segmentation
This project leverages k-means clustering algorithms to uncover meaningful patterns within the dataset. 

## Dependencies
To facilitate this analysis, the following Python libraries were employed:
- Seaborn: For comprehensive data visualization, enabling rich insights and clear communication of findings.
- NumPy: For efficient numerical computations and array manipulation, underpinning the core calculations within clustering algorithms.
- Pandas: For data ingestion, manipulation, and analysis, ensuring data integrity and streamlining the process.
- Scikit-Learn: For the implementation of clustering algorithms, offering a diverse array of techniques for effective pattern identification.

The strategic integration of these libraries provides a robust and versatile framework for exploring and extracting valuable insights from the data through clustering.

## Dataset Explanation
The project takes into account two metrics for market segmentation i.e. brand loyalty and consumer satisfaction.

**Consumer Satisfaction:** In this the consumers are allowed to rate their shopping experience from 1 to 10. This datatype is discrete and it takes integer values.

**Brand Loyalty:** This dataset takes into account yearly purchases and other factors. This data type is continuous.

## Project Explanation
1. In this project, our main aim is to divide the market into different clusters and correspondingly target those customers who have high brand loyalty and satisfaction.
2. To achieve that we  initially divide our dataset into 2 clusters in the "Loyalty" vs "Satisfaction" plane.

![image](https://github.com/Hansaraj09/Market-Segmentation/assets/93324559/902bd4ae-0e0b-4ecf-bb4b-cc7a4c2ec8b3)

From the above figure, we see that 2 clusters are not enough to properly quantify the above problem.

3. To know the actual number of clusters needed we standardize the variables and apply the elbow method(WCSS vs Number of Clusters).
  
 ![image](https://github.com/Hansaraj09/Market-Segmentation/assets/93324559/95fb459e-add6-4587-a562-d05909cbd139)
   
From the above figure, we see the elbow is at  4 points i.e. at n=2,3,4,5 where n is the number of clusters.

4. Now we plot the clusters at these points and  we see that n=4 gives us the optimum number of clusters.

![image](https://github.com/Hansaraj09/Market-Segmentation/assets/93324559/6c83b9fb-f8e6-43e4-b355-c14dab2dc562)

## Insights
 We can divide the 4 clusters obtained above as follows:
   
1.**Blue:** High satisfaction and high loyalty (or fans).
  
2. **Yellow:** Low satisfaction and high loyalty (or supporters).
     
3. **Red:** High satisfaction and low loyalty (or roamers).
     
4. **Purple:** Low satisfaction and low loyalty (or alienated).

Thus from the above insights we can say that more number of **fans** is better for the business and we should try to convert more **supporters** into **fans** by increasing their satisfaction levels. And we can also convert more **roamers** by increasing their loyalty say by giving vouchers and coupons.






