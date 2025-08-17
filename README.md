# Big-Data-Project

This repository contains the analysis and machine learning modelling work for the **Big Data Analysis and Project** course at the University of Adelaide.  
The project investigates **air quality in Indian cities**, focusing on predicting **Air Quality Index (AQI)** and analyzing the influence of **festivals** and **crop stubble burning** on pollution levels.

---

## Repository Structure

### Data Files
- `India_city_states.csv` – Mapping of Indian cities to their respective states.
- `Indian_festival_dates_2015-2020.xlsx` – Festival dates (Diwali, etc.) for 2015–2020.
- `crop_production_major_3_crops.csv` – Annual production data of three major crops contributing to stubble burning.
- `ml_model_data.rds` – Processed dataset used for machine learning.

### Project Parts
- `Part_A_Initial_questions.Rmd` – Formulation of research questions and data exploration.
- `Part_B_Big_Data_Analysis.Rmd` – Data cleaning, preprocessing, and exploratory analysis.
- `Part_C_Big_Data_Modelling.Rmd` – Machine learning models (Lasso, Random Forest, XGBoost, Linear Regression) with training/testing evaluation.
- `Part_D_Comprehensive_Report.pdf` – Final comprehensive report summarizing methodology, results, and conclusions.

---

## Project Workflow
Each part has to be run sequentially one after the other, part D may take significant running for the first time depending on the device and memory, however, later runs will be faster due to usage of saved files being run instead of computing the results every single time  
### Part A – Problem Formulation  
- Defined research questions around AQI prediction, seasonal variations, and event-based pollution spikes (festivals, crop burning).

### Part B – Data Analysis  
- Performed initial analysis and visualisation of the data 
- Visualisation of relationships in the dataset 
- Problem statement refinement

### Part C – Machine Learning Modelling  
- Built predictive models: **Lasso Regression, Random Forest, XGBoost, and Linear Regression**.  
- Evaluated models on training and testing sets using **RMSE, MAE, and R²**.  
- Selected **XGBoost** as the best-performing model.

### Part D – Comprehensive Report  
- Summarized results in a report.  
- Found **PM2.5 and PM10** as dominant pollutants in Delhi and Ahmedabad.  
- Highlighted **severe AQI spikes during Diwali** and impact of policies on **air quality**.
---

## How to Reproduce same results 
1. Open the .Rmd files in RStudio.

2. Run the parts sequentially in order:

2.1. Part_A_Initial_questions.Rmd

2.2. Part_B_Big_Data_Analysis.Rmd

2.3. Part_C_Big_Data_Modelling.Rmd 

Note: The first run of Part D may take significant time depending on your device and available memory.
Subsequent runs will be faster, as saved intermediate files are reused instead of recomputing results each time.

Part_D_Comprehensive_Report.pdf is the final report compiled using the results from Part A, B and C.

---
## References
 
1.	Rao, R 2020, _Air Quality Data in India (2015 - 2020)_, Kaggle, viewed 3 June 2025, <https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india>
2.	Kumar, A 2025, _Pollution in India_, Encyclopedia Britannica, viewed 5 June 2025, <https://www.britannica.com/topic/pollution-in-India.>
3.	Unified Portal for Agricultural Statistics: UPAg 2025, _APY Cropwise Insights_, UPAG, viewed 5 June 2025, <https://upag.gov.in/.>
4.	Central Pollution Control Board n.d., _About National Air Quality Index_, Central Pollution Control Board, viewed 3 June 2025, <https://cpcb.nic.in/displaypdf.php?id=bmF0aW9uYWwtYWlyLXF1YWxpdHktaW5kZXgvQWJvdXRfQVFJLnBkZg>
5.	Basu, M 2019, ‘The Great Smog of Delhi’, _Lung India_, vol. 36(3), pp. 239, DOI:10.4103/lungindia.lungindia_363_18.
6.	Regan, H 2024, _Air pollution in Asia worsened in 2023, with Bangladesh, Pakistan, and India among the worst hit_, CNN, viewed 5 June 2025, <https://edition.cnn.com/2024/03/18/climate/air-pollution-report-2023-asia-climate-intl-hnk.>
7.	Dybwad, A 2022, 'What to Know About India’s Crop Burning Season', _PurpleAir_, 16 November, viewed 1 July 2025, <https://www2.purpleair.com/blogs/blog-home/what-to-know-about-india-s-crop-burning-season#:~:text=India's%20crop%20burning%20season%20usually,rural%20areas%20to%20metropolitan%20cities>
8.	Pandey, P 2020, _Indian cities database_, Kaggle, viewed 1 July 2025, <https://www.kaggle.com/datasets/parulpandey/indian-cities-database>
9.	Chanana I, Sharma A, Kumar P, Kumar L, Kulshreshtha S, Kumar S, Patel SKS, 2023, 'Combustion and Stubble Burning: A Major Concern for the Environment and Human Health', _Fire_ 2023, 6, 79, DOI: https://doi.org/10.3390/fire6020079
10.	Gouder, C., & Montefort, S 2014, 'Potential impact of fireworks on respiratory health', _Lung India_, 31(4), 375–379, DOI: https://doi.org/10.4103/0970-2113.142124
11.	GeeksforGeeks (2024), _Difference Between Random Forest and XGBoost_, GeeksforGeeks, <https://www.geeksforgeeks.org/machine-learning/difference-between-random-forest-vs-xgboost/.>
12.	Ganguli, I , Nakum, M., Das, B. & Kshetrimayum, N. 2025, Comprehensive analysis of air quality trends in India using machine learning and deep learning models, pp. 313–318, https://doi.org/10.1145/3700838.3703681.
13.	Mujtaba, M.A., Munir, M.A., Ali, S., Petrů, J., Ansar, T., Akhlaq, W., Ahmad, M., Iqbal, H., Ali, F., Bashir, M.N. & Alexander, T. 2025, Using machine learning for air quality prediction and sustainable urban planning, Sustainable Futures, vol. 10, p. 100981, [online], https://doi.org/10.1016/j.sftr.2025.100981.
14.	Pande, C.B., Kushwaha, N.L., Alawi, O.A., Sammen, L.S., Sidek, L.M., Yaseen, Z.M., Pal, S.C. & Katipoğlu, O.M. 2024, Daily scale air quality index forecasting using bidirectional recurrent neural networks: Case study of Delhi, India, Environmental Pollution, p. 124040, https://doi.org/10.1016/j.envpol.2024.124040.
15.	Rahman, M.M., Nayeem, M.E.H., Ahmed, M.S., Tanha, K.A., Sakib, M.S.A., Uddin, K.M.M. & Babu, H.M.H. 2024, AirNet: predictive machine learning model for air quality forecasting using web interface, Environmental Systems Research, vol. 13, no. 1, https://doi.org/10.1186/s40068-024-00378-z.
16.	Ravindiran, G., Hayder, G., Kanagarathinam, K., Alagumalai, A. & Sonne, C. 2023, Air quality prediction by machine learning models: A predictive study on the Indian coastal city of Visakhapatnam, Chemosphere, vol. 338, p. 139518, [online], https://doi.org/10.1016/j.chemosphere.2023.139518.
17.	Vajiram Editor 2023, SC says cracker order applies to country, not just NCR, [online], Vajiram and Ravi, viewed 5 August 2025,  https://vajiramandravi.com/current-affairs/sc-cracker/ 
18.	World Health Organization (WHO) 2025, Air quality, energy and health, [online], World Health Organization, , viewed 5 August 2025, https://www.who.int/teams/environment-climate-change-and-health/air-quality-energy-and-health/health-impacts 
19.	Shagun (2024). Centre doubles fine for stubble burning; farmers to pay up to Rs 30,000, Down To Earth, viewed 5 August 2025, https://www.downtoearth.org.in/air/centre-doubles-fine-for-stubble-burning-farmers-to-pay-up-to-rs-30000 
20.	ShareAmerica 2024, India’s initiatives for cleaner air, [online], ShareAmerica, viewed 5 August 2025, https://share.america.gov/indias-initiatives-for-cleaner-air/ 






