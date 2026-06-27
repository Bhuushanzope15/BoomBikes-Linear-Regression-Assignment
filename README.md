# Project Name : BoomBikes Bike-Sharing Linear Regression Assignment
> A Multiple Linear Regression model built to predict the daily demand for shared bikes post-lockdown for the US-based provider BoomBikes.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
- **Background:** 
BoomBikes, a prominent US bike-sharing provider, experienced a substantial revenue dip due to the COVID-19 pandemic. To survive, the company requires an actionable, data-driven strategy to accelerate revenue generation once normal operations resume.
- **Business Problem:** The objective is to model daily bike-sharing demand (`cnt`) to understand how structural, seasonal, and environmental variables influence bike aspirations. This helps management optimize deployment strategy and align supply with demand dynamics in a post-lockdown market.
- **Dataset:** The dataset utilized is `day.csv`, which tracks daily bike rental tallies across 2018 and 2019 alongside corresponding atmospheric, calendar, and seasonal parameters.

## Conclusions
- **Conclusion 1 (Weather Dominance):** Adverse weather situations—specifically `weathersit_Light_Snow_Rain`—constitute the single strongest negative driver of bike demand (Coefficient: `-0.3207`). Severe drops in usage occur during rain, snow, or thunderstorms.
- **Conclusion 2 (Organic Year-on-Year Growth):** The year variable `yr` exhibits a powerful positive contribution (Coefficient: `+0.2457`), demonstrating massive organic growth and market penetration in bike-sharing baseline popularity from 2018 to 2019.
- **Conclusion 3 (Seasonal Inhibitors):** The spring season (`season_spring`) acts as a significant negative constraint on demand (Coefficient: `-0.2381`), indicating that colder temperatures structurally depress active commuter and leisure bookings.
- **Conclusion 4 (Model Performance & Reliability):** The final pruned model achieves a **Training $R^2$ of 0.798** and a **Test Set $R^2$ of 0.7833**. The highly tight margin (<2%) validates that the model generalizes robustly and operates without any underlying multicollinearity issues (all final feature VIF values < 5).

## Technologies Used
- pandas - version 1.5.3
- numpy - version 1.23.5
- statsmodels - version 0.13.5
- scikit-learn - version 1.2.2
- seaborn - version 0.12.2
- matplotlib - version 3.7.1

## Acknowledgements
- This project was inspired by the Linear Regression curriculum from the Executive Post Graduate Programme in Data Science.
- The underlying source data dictionary was provided by upGrad to simulate real-world strategic analytics consulting.

## Contact
Created by [@Bhuushanzope15](https://github.com/Bhuushanzope15) - feel free to contact me!