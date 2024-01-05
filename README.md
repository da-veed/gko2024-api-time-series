# 2024 GKO - Machine Learning Hackathon

## 🎯 Task Description 
Welcome to the **GKO 2024 Machine Learning Hackathon**! In this event, your team will be working on a time-series 
prediction challenge for API usage. Your goal is to predict API usage based on historical logs.

## 💾 Data 
The data for this hackathon can be accessed [HERE](https://drive.google.com/file/d/1m9Otzb-kh5SmyQOC-6tJEODy3UKoZaw2/view) 
or via the command (might take a few seconds to download)
```bash
curl -s -L "https://drive.google.com/uc?confirm=t&export=download&id=1m9Otzb-kh5SmyQOC-6tJEODy3UKoZaw2" -o "./logs_df.parquet"
```

Web sever logs contain information on any event that was registered/logged during a few days in 2019. This contains a 
lot of insights on website visitors, behavior, crawlers accessing the site, business insights, security issues, and more.

The dataset contains ~11M of logs from an Iranian ecommerce website zanbil.ir.

## 🚀 Getting started 
This might be a completely new topic to many so here is a [gentle introduction to Time-series forecasting](https://wandb.ai/site/articles/a-gentle-introduction-to-time-series-analysis-forecasting)

If you need a primer to start coding check out this [Google colab notebook](https://colab.research.google.com/drive/1bA0nN53AVofr_m07HoCMHFy7Yu0Tsf3Y).
It contains basic instructions for pandas (Python package for data manipulation) and data analysis.

## ✅ Results & evaluation
The performance of your model will be evaluated using the Root Mean Squared Error (RMSE). The lower the value, the 
better. Here is a great guide on [how to interpret RMSE](https://www.statology.org/how-to-interpret-rmse/). 

Here are some constraints which have to be integrated into your solution:
- aggregate the data by minute (count API hits per minute)
- split the data into train and validation sets. The validation set should consist of the last 6 hours of data

Once the challenge time runs out, your team will present the results to the remaining teams. The form of the 
presentation.

## 🔥 Extra points
1. Think and explain how this can be implemented into Gravitee.
2. Try different models to get a lower RMSE. Check out [Cross validation](https://forecastegy.com/posts/time-series-cross-validation-python/) for better results.
3. Dive into the topic of [Anomaly detection](https://medium.com/@jelkhoury880/introduction-to-anomaly-detection-methods-part-i-b1a2f389ffcb) and try to implement it as something extra.

## 💥 Have Fun!
The primary goal for the hackathon is to learn and have fun. Don't hesitate to reach out if you have any questions or 
need assistance.

Good luck!
