# Credit_Risk_Analysis
## Analysis Overview
This project shows how to build, test, and train with machine learning models in order to predict credit risk.
We use **RandomOverSampler**, **SMOTE**, **ClusterCentroids**, **SMOTEENN**, **BalancedReandomForestClassifier**, and **EasyEnsembleClassifier**.
Using these machine learning process, we are able to predict credit risk and test the data to see how the machine is learning!
Using the resampling model, SMOTEENN, and the Ensemble Classifiers, we can predict the credit risk analysis.
## Results:
BalancedRandomForestClassifier model:

<img width="1124" alt="Screenshot 2023-04-12 at 10 18 49 AM" src="https://user-images.githubusercontent.com/117100491/231503851-1ea2a20e-b57f-4c48-9e2f-d39589cba252.png">

<img width="522" alt="Screenshot 2023-04-12 at 10 21 25 AM" src="https://user-images.githubusercontent.com/117100491/231504554-f48fd4a1-4652-410f-8218-9dfafa409e12.png">

<img width="1027" alt="Screenshot 2023-04-12 at 10 19 10 AM" src="https://user-images.githubusercontent.com/117100491/231503943-515be48f-77f0-4df3-94ec-bf80f29f63df.png">

The balanced accuracy score is 79% with a high_risk precision still low at 4% only with 67% sensitivity. The low_risk sensitivity is 91% with 100% precision! Awesome!

EasyEnsembleClassifier model:

<img width="1104" alt="Screenshot 2023-04-12 at 10 25 23 AM" src="https://user-images.githubusercontent.com/117100491/231505659-0e1af07a-01c0-40e9-81fa-8a8f87c08005.png">

<img width="512" alt="Screenshot 2023-04-12 at 10 25 37 AM" src="https://user-images.githubusercontent.com/117100491/231505727-94ae4ea7-1516-4bef-8c54-66d8ea19daab.png">

<img width="718" alt="Screenshot 2023-04-12 at 10 25 54 AM" src="https://user-images.githubusercontent.com/117100491/231505812-3bf430cd-36c6-4625-9736-d532bed2420b.png">

At this point, the balance accuracy score is about 93%.
The high_risk precision is still low at 7% w/91% sensitivity. The low_risk is now 94% with 100% precision.

NaiveRandomOversampling (SMOTE) model:

<img width="534" alt="Screenshot 2023-04-12 at 10 29 40 AM" src="https://user-images.githubusercontent.com/117100491/231506931-7f114887-93c7-429b-b4c8-447d7d10a9a0.png">

<img width="459" alt="Screenshot 2023-04-12 at 10 29 52 AM" src="https://user-images.githubusercontent.com/117100491/231506979-dfdc95fc-04f7-4b98-ab1c-699f7c6f0b5f.png">

<img width="747" alt="Screenshot 2023-04-12 at 10 30 01 AM" src="https://user-images.githubusercontent.com/117100491/231507006-03241ab3-d50e-49df-bf37-634f8455c6c2.png">

The results are similar to the RandomOverSampler model. The balance accuracy score is 64% and the high-risk precision is 1%ish with 63% senstivity. Its precision is almost 100% with 66% sensitivity.

SMOTE Oversampling model:

<img width="283" alt="Screenshot 2023-04-12 at 10 34 14 AM" src="https://user-images.githubusercontent.com/117100491/231508152-49613c67-a87b-4e5d-904b-5e3afddb36e4.png">

<img width="490" alt="Screenshot 2023-04-12 at 10 34 23 AM" src="https://user-images.githubusercontent.com/117100491/231508202-cd53b715-05dd-4c93-a098-58ef0b3405f1.png">

<img width="842" alt="Screenshot 2023-04-12 at 10 34 37 AM" src="https://user-images.githubusercontent.com/117100491/231508280-5147a877-9815-4cc9-86d3-ed550e209bcc.png">

The model is very similar to the last model. The balanced accuracy score is 64%, and the high_risk precision is about 1% w/63% sensitivity. The precision is almost 100% with sensitivity of 66%.

ClusterCentroids model:

<img width="490" alt="Screenshot 2023-04-12 at 10 37 06 AM" src="https://user-images.githubusercontent.com/117100491/231508913-1cdc20cc-0e8c-4ea3-8b04-c2846f68aa2e.png">

<img width="472" alt="Screenshot 2023-04-12 at 10 37 15 AM" src="https://user-images.githubusercontent.com/117100491/231508956-57dc95b8-497e-4e7e-bddd-a0466c2be68a.png">

<img width="731" alt="Screenshot 2023-04-12 at 10 37 40 AM" src="https://user-images.githubusercontent.com/117100491/231509085-aeb9c12b-8e89-4732-a425-e5efdc9612d5.png">

The balanced accuracy scor is down to 52%. The high_risk precision is 1% w/63% sensitivity. The low_risk sensitivity is 40%. Oh no!

SMOTEENN model:

<img width="445" alt="Screenshot 2023-04-12 at 10 39 02 AM" src="https://user-images.githubusercontent.com/117100491/231509452-f6860845-71d0-4965-bcbe-4d9ba38a2e6e.png">

<img width="493" alt="Screenshot 2023-04-12 at 10 39 11 AM" src="https://user-images.githubusercontent.com/117100491/231509497-06784085-caf7-4988-82af-387c9c9209bd.png">

<img width="748" alt="Screenshot 2023-04-12 at 10 39 20 AM" src="https://user-images.githubusercontent.com/117100491/231509535-95048f7f-7729-41e3-9fff-4a385ffac736.png">

The balanced accuracy score is 62%. The high_risk precision is still 1% w/68% sensitivity. The low_risk sensitivity is 57%.

## Summary
The models used in this project show an overall weak precision when determining if the credit risk is high. When the Ensemble models were introduced, we see a lot of improvement in the sensitivity of the high risk credits. The EasyEnsembleClassifier model shows a 92% recall to detect almost all the high risk credit, the best option. But with low precision, the low risk credits are still falsely detected as high risk which is a problem. At the end of the day, I do not think these models are sufficient to predict credit risk.
