# Project Name : Bike Lending - Multiple Linear Regression

## Table of Contents

- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Business Goal](#business-goal)
- [Model: Multiple Linear Regression Equation](#model-multiple-linear-regression-equation)
- [Driver Features](#driver-features)
- [Major Insights from the Model](#major-insights-from-the-model)
- [Suggested Next Business Steps](#suggested-next-business-steps)
- [Libraries Used](#libraries-used)
- [Acknowledgements](#acknowledgements)
- [Created by](#created-by)

## Project Overview

BoomBikes, a US-based bike-sharing provider, has been struggling with significant revenue drops due to the COVID-19 pandemic. To recover and accelerate their growth once the lockdown ends, BoomBikes aims to understand the factors affecting bike demand. The goal is to develop a predictive model to help the management adjust their business strategy to meet customer demand and identify opportunities in new markets.

## Problem Statement

Bike-sharing systems provide bikes for short-term use, either for a fee or free, through computer-controlled docks. BoomBikes, a provider affected by the pandemic, is exploring ways to rebound by understanding the demand for shared bikes post-lockdown. They have gathered data on various factors influencing daily bike demand in the US market and seek to know:

1. Which variables significantly predict bike demand.
2. How well these variables explain the bike demand.

The objective is to use this analysis to adjust their business strategy and improve their market positioning.

## Business Goal

The main objective is to model the demand for shared bikes using the available independent variables. This model will help management understand how different features affect demand, allowing them to refine their strategy to align with customer needs. Additionally, it will provide insights into demand dynamics in new markets.

## Model: Multiple Linear Regression Equation

The multiple linear regression model developed is as follows:

total_count = 0.1822  
               + (0.4878 * temperature) 
               + (0.2433 * year) 
               - (0.2777 * weather_situation_Light_Precipitation_Thunderstorms) 
               - (0.1476 * season_Winter) 
               + (0.0925 * month_Sep) 
               - (0.0802 * weather_situation_Mist_Cloudy) 
               - (0.0743 * holiday) 
               + (0.0609 * month_Oct) 
               - (0.0449 * season_Summer) 
               - (0.0418 * month_Jul)

## Driver Features

1. Temperature
2. Year
3. Weather situation (Light Precipitation/Thunderstorms, Mist/Cloudy)
4. Season (Winter, Summer)
5. Month (September, October, July)
6. Holiday

## Major Insights from the Model

1. **Positive Impact Factors**:
   - **Temperature (0.4878)**: Higher temperatures boost bike rentals significantly.
   - **Year (0.2433)**: Demand increases over time, suggesting a growing preference for bike-sharing.
   - **Month: September (0.0925)** and **October (0.0609)**: Bike rentals peak during these months, indicating seasonality.

2. **Negative Impact Factors**:
   - **Weather: Light Precipitation/Thunderstorms (-0.2777)** and **Mist/Cloudy (-0.0802)**: Adverse weather conditions significantly decrease bike rentals.
   - **Season: Winter (-0.1476)**: Rentals drop substantially in winter.
   - **Holiday (-0.0743)**: Lower rentals on holidays, likely due to reduced commuter traffic.

## Suggested Next Business Steps

1. **Maximize Opportunities During Warm Weather:**
   - Increase marketing and promotions during warmer months, emphasizing the comfort of riding in good weather.
   - Expand the fleet and rental locations to meet higher demand during these periods.

2. **Minimize Impact of Poor Weather:**
   - Introduce rain check policies or weather-related incentives to encourage usage despite bad conditions.
   - Offer weather-resistant gear rentals and discounts during mild bad weather to maintain usage levels.

3. **Increase Winter Rentals:**
   - Launch winter promotions like bundled deals or discounts and collaborate with warm indoor venues for perks.

4. **Boost Rentals on Holidays:**
   - Offer holiday-specific deals, guided tours, and special events to attract tourists and leisure riders.

5. **Support Yearly Rental Growth:**
   - Continue expanding bike availability and rental locations to keep up with growing demand.

## Libraries Used

- python -  3.11.7
- numpy -  1.26.4
- pandas -  2.1.4
- matplotlib -  3.8.0
- seaborn -  0.13.2
- sklearn -  1.2.2
- statsmodels -  0.14.0

## Acknowledgements

- This project was inspired by IIITB's Lecture on Linear Regression
- References:
  - [Seaborn Documentation](https://seaborn.pydata.org/)
  - [Anscombe’s quartet Documentation](https://matplotlib.org/stable/gallery/specialty_plots/anscombe.html)
  - [Pearson’s R](https://statistics.laerd.com/statistical-guides/pearson-correlation-coefficient-statistical-guide.php)
  - [Q-Q Plot](https://www.geeksforgeeks.org/quantile-quantile-plots/)

## Created by 
[Rahul Singh](https://github.com/RahulMukeshSingh) - feel free to contact me!