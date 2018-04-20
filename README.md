# Group 6 Project
Group 6, Katherine Matthers, Akina Hays, Aiqi Chen, Yingjin Wang. We used 3 different datasets in this project.

## Description of datasets.yelp_business
This table includes various data gathered on Yelp including users, reviews, ratings, business addresses and catergories.

## Question #1
What are the top 5 states with the most 5 star businesses? 

```sql
Select count(stars) as count_of_5_stars, state
From datasets.yelp_business
where stars = 5
group by state
order by count_of_5_stars DESC
```

![An-analysis-of-yelp_business](Group6Visualizations/q1.png)



