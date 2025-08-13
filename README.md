# Predicting Homeownership in Washington State: A Support Vector Machine Analysis of Demographic and Housing Data

## Table of Contents
- [Table of Contents](#table-of-contents)
- [Abstract](#abstract)
- [Introduction](#introduction)
- [Theoretical Background](#theoretical-background)
- [Methodology](#methodology)
- [Computational Results](#computational-results)
- [Discussion](#discussion)
- [Conclusion](#conclusion)
- [References](#references)
---  

## Abstract

This report delves into the application of Support Vector Machines (SVM) for classification to predict homeownership status based on demographic and housing-related factors. Leveraging data from the US Census in Washington State, including variables such as age, income, education level, household characteristics, and housing attributes, we employed strategic subsetting to focus on specific demographic populations, such as married individuals under 40 with at least 1 year of college education. This tailored approach was necessary due to the substantial size of the dataset, ensuring computational feasibility while maintaining dataset balance. By testing various SVM kernels, including linear, radial, and polynomial, and fine-tuning their parameters, we aimed to identify the most accurate predictive model. Throughout our analysis, we explored the relationships among variables and their implications for homeownership status, addressing associated challenges and discussing potential policy implications. In this study, we employed three different kernel functions of Support Vector Machines (SVM) to predict whether homes are owned or rented, analyzing a dataset comprising 1119 instances. The Linear SVM model achieved an accuracy of 82.2%, with a precision of 0.84 and recall of 0.94 for owned homes, and a precision of 0.76 and recall of 0.48 for rented homes. The Radial Basis Function (RBF) SVM model demonstrated superior performance, achieving the highest accuracy of 84.1%, and improved recall for rented homes at 0.53. The Polynomial SVM model, while slightly less effective, still posted a commendable accuracy of 82.8%, with a similar trend in precision and recall for the two classes. These results indicate that the RBF SVM model is the most effective in balancing the classification between owned and rented homes, suggesting its potential utility in applications requiring robust differentiation between these two categories.

[Back to top](#table-of-contents)

---

## Introduction

Homeownership stands as a fundamental pillar of the American dream, symbolizing economic stability and personal achievement. Yet, accurately predicting homeownership status based on demographic and housing-related factors poses a multifaceted challenge. In light of the growing abundance of data, particularly from sources like the US Census, there arises an opportunity to harness advanced machine learning methodologies to elucidate and anticipate homeownership patterns. Among these methodologies, Support Vector Machines (SVM) present a robust framework for classification tasks, holding promise for advancing our understanding of homeownership dynamics. This study endeavors to explore the application of SVM in predicting homeownership status in Washington State, drawing on comprehensive
demographic and housing data from the US Census. By focusing on specific demographic cohorts and deploying SVM with diverse kernels, including linear, radial, and polynomial, our aim is to discern the most effective predictive model. Recognizing the immense scale of the dataset, strategic subsetting was employed to ensure computational tractability while upholding dataset equilibrium. Although all the models performed well, our choice was brf as it showed the had the Through this inquiry, we aspire to unveil the determinants of homeownership and contribute insights that can inform housing policy and scholarly discourse.

[Back to top](#table-of-contents)

---

## Theoretical Background
Support Vector Machines (SVM) are a powerful category of supervised learning algorithms that excel in both classification and regression tasks. The primary mechanism of SVM involves finding an optimal hyperplane that effectively separates different classes in the dataset with the maximum possible margin. This is achieved by projecting the data points into a higher-dimensional space where a clearer division between classes can be established.
The unique strength of SVM lies in its use of kernel functions to transform the original data into a format where complex, non-linear relationships can be linearly separable. Common choices for these kernel functions include linear, radial basis function (RBF), and polynomial kernels, each tailored to different data characteristics and specific analytical needs. The choice of kernel function plays a crucial role in the model's ability to adapt to the complexity and nature of the data, thereby affecting the accuracy and robustness of the classifications.
In practical applications, such as predicting homeownership status, SVM's ability to handle high-dimensional and nonlinear data makes it an ideal tool for parsing complex demographic and housing-related information. Through careful tuning of SVM parameters, including the regularization parameter C, and kernel-specific settings, researchers can enhance the model's performance to capture subtle patterns in the data that are indicative of homeownership trends.
By leveraging SVM's robust framework and its adaptability through various kernels, analysts can uncover nuanced insights into critical factors influencing homeownership, thus supporting sophisticated decision-making and policy formulation in the housing sector. This methodological approach not only clarifies the underlying dynamics of housing markets but also enriches the strategic interventions aimed at stabilizing and stimulating homeownership.

[Back to top](#table-of-contents)

---

## Methodology
In our analysis, we utilized a dataset comprising various demographic and housing-related factors to predict homeownership status. The dataset was preprocessed to encode categorical variables into dummy variables and standardize continuous variables for improved model
performance. The target variable, representing homeownership status, was labeled as 'OWNERSHP', while the predictor variables included features such as population density ('DENSITY'), electricity cost ('COSTELEC'), household income ('HHINCOME'), number of rooms ('ROOMS'), and age ('AGE'), along with other encoded categorical variables such as marital status ('MARST') and education level ('EDUC').
Through strategic subsetting, we focused on specific demographic populations, such as married individuals under 40 with at least 1 year of college, to ensure computational tractability while maintaining dataset balance. This tailored approach allowed us to extract meaningful insights while effectively addressing the challenges posed by the dataset's size.
Using Support Vector Machines (SVM) with different kernels, including linear, polynomial, and radial basis function (RBF), we aimed to develop accurate predictive models for homeownership status. By fine-tuning SVM parameters and selecting appropriate kernel functions, we sought to optimize model performance and achieve reliable predictions.
The analysis involved training and evaluating SVM models with different kernels to identify the most suitable approach for predicting homeownership status. The results revealed the best parameters for each SVM kernel, along with their corresponding cross-validation scores, providing valuable insights into the performance of each model variant.

[Back to top](#table-of-contents)

---

## Computational Results

<img width="934" height="528" alt="image" src="https://github.com/user-attachments/assets/74707704-f241-4347-9483-047c358228f0" />


<img width="866" height="564" alt="image" src="https://github.com/user-attachments/assets/a323e195-a89a-4577-823a-c0539c5c23f4" />


<img width="803" height="499" alt="image" src="https://github.com/user-attachments/assets/ce24c176-edee-4e94-9947-20330e4b5fba" />


<img width="902" height="552" alt="image" src="https://github.com/user-attachments/assets/04b56738-c06e-441a-a2c2-cd2c62376946" />


<img width="1149" height="494" alt="image" src="https://github.com/user-attachments/assets/f59cc282-6979-4aeb-812e-36009e64898e" />


<img width="835" height="660" alt="image" src="https://github.com/user-attachments/assets/5b2e6990-fbc1-4b90-b017-cce75f90d283" />


<img width="1196" height="593" alt="image" src="https://github.com/user-attachments/assets/22cbacfe-7749-4a18-9cbe-6761b0c65f65" />


[Back to top](#table-of-contents)

---

## Discussion

In our analysis, we explored the application of Support Vector Machines (SVM) with different kernels (linear, polynomial, and radial basis function) to predict homeownership status based on demographic and housing-related factors. All SVM models exhibited high training and test accuracies, indicating their effectiveness in capturing the underlying patterns within the data.
The Linear SVM model achieved a training accuracy of 82.6% and a test accuracy of 82.2%, with a relatively low computational time of approximately 1.10 seconds. This suggests that the Linear kernel is efficient, although it sacrifices some accuracy for speed, making it suitable for scenarios where rapid predictions are more critical than achieving the highest possible accuracy.
Conversely, the Polynomial SVM model displayed a higher training accuracy of 86.9% but only a slightly better test accuracy of 82.7%, requiring about 1.84 seconds to execute. This increase in execution time reflects the additional computational complexity introduced by the Polynomial kernel, which might capture more nuanced interactions in the data that the Linear model overlooks.
The Radial Basis Function (RBF) SVM model demonstrated the best performance among the three, boasting the highest training accuracy of 88.7% and a test accuracy of 83.9%, albeit at the longest execution time of 2.21 seconds. The RBF kernel's ability to handle non-linear data and complex patterns effectively translates into better accuracy but also indicates greater computational demands. The extended execution time, while a marker of increased computational load, is justified by the significant gains in predictive accuracy.
Overall, the findings suggest that SVM models, particularly those with RBF and polynomial kernels, offer robust solutions for predicting homeownership status based on demographic and housing-related factors. These models not only provide valuable insights into the factors influencing homeownership outcomes but also underscore the balance between computational efficiency and predictive accuracy that must be considered in practical applications.
Furthermore, our analysis identified household income, total income, and number of bedrooms as the most influential features for predicting homeownership status. These findings underscore the importance of economic factors and housing characteristics in determining homeownership outcomes. They highlight potential areas for intervention and policy development aimed at improving access to homeownership opportunities. The identification of key features suggests targeted strategies that policymakers and stakeholders can implement to enhance homeownership rates, such as financial assistance programs or zoning laws designed to increase affordable housing availability.
This detailed understanding of the trade-offs and capabilities of each SVM kernel helps in tailoring machine learning solutions to specific needs within the housing market, providing a strategic edge in policy formulation and economic planning.

[Back to top](#table-of-contents)

---

## Conclusion

Our study has highlighted the efficacy of Support Vector Machines (SVM) with different kernel functions—Linear, Polynomial, and Radial Basis Function (RBF)—in predicting homeownership status based on demographic and housing-related data. The Linear SVM model, known for its speed and satisfactory accuracy, is particularly suited for scenarios requiring quick decisions. In
contrast, the Polynomial SVM excels in recognizing complex data patterns, offering valuable insights despite its slightly higher computational cost. The RBF SVM stands out as the top performer, combining high accuracy with the ability to handle complex, non-linear data patterns, even though it incurs the highest computational expense.
The significant impact of economic factors, notably household and total income, alongside physical characteristics like the number of bedrooms, plays a pivotal role in homeownership outcomes. Our analysis further revealed that education level, particularly completion of a four-year college degree, correlates strongly with higher homeownership rates, underscoring the importance of educational attainment in securing housing stability.
Additionally, the Seattle housing market presents a stark illustration of broader economic pressures. According to The Seattle Times, the cost of homeownership in the area has surged nearly 80% in recent years due to rising home prices and interest rates. This drastic increase highlights the growing disparity between home prices and income growth, with homebuyers now requiring an annual income of almost $214,000 to afford a typical home—a 79% increase since 2020, compared to a mere 22% rise in median incomes. Many residents are extending their financial limits, with some allocating up to 40% of their income towards housing. Strategies such as relying on family support for down payments and opting for condominiums are becoming more prevalent.
These conditions not only emphasize the need for innovative policy measures to enhance housing affordability but also validate the importance of leveraging advanced machine learning techniques like SVM. By understanding the factors influencing homeownership and employing targeted interventions, policymakers and stakeholders can better address disparities and improve access to housing.
Therefore, our study contributes substantially to the body of knowledge on housing dynamics, providing crucial insights that can guide future research and policy decisions aimed at promoting equitable homeownership opportunities. The critical path forward involves enhancing housing affordability through increased home construction and strategic policy adjustments to manage the high costs of housing.

[Back to top](#table-of-contents)

---

## References

Heidi Groover(Feb. 29, 2024 at 6:15 pm Updated Feb. 29, 2024 at 7:15 pm). Here’s how much you need to earn to afford a Seattle-area home. The Seattle Times. https://www.seattletimes.com/business/real-estate/heres-how-much-you-need-to-earn-to-afford-a-seattle-area-home/ 

Steven Ruggles, Sarah Flood, Matthew Sobek, Danika Brockman, Grace Cooper, Stephanie Richards and Megan Schouweiler. IPUMS USA: Version 13.0 [dataset]. Minneapolis, MN: IPUMS, 2023. https://doi.org/10.18128/D010.V13.0

Steven Ruggles, Matt A. Nelson, Matthew Sobek, Catherine A. Fitch, Ronald Goeken, J. David Hacker, Evan Roberts, and J. Robert Warren. IPUMS Ancestry Full Count Data: Version 4.0 [dataset]. Minneapolis, MN: IPUMS, 2024. https://doi.org/10.18128/D014.V4.0

[Back to top](#table-of-contents)

---

