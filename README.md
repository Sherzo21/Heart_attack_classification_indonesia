# Heart_attack_classification_indonesia

Implementation Steps Description

1. Data Loading and Initial Analysis

English: Loaded the heart attack dataset from a CSV file and inspected its structure using functions like head(), info(), and describe(). Checked for missing values to ensure data quality.
Korean: CSV 파일에서 심장마비 데이터셋을 불러오고, head(), info(), describe() 등의 함수로 데이터 구조를 확인했습니다. 데이터 품질을 보장하기 위해 결측치를 확인했습니다.

2. Target Variable Encoding

English: Encoded the HeartAttack target variable as binary values (Yes = 1, No = 0) using LabelEncoder.
Korean: LabelEncoder를 사용하여 HeartAttack 목표 변수를 이진 값(예 = 1, 아니요 = 0)으로 인코딩했습니다.

3. Categorical Feature Encoding

English: Used one-hot encoding for categorical features, excluding irrelevant columns like ID and State.
Korean: ID와 State 같은 관련 없는 열을 제외하고 범주형 특징에 대해 원-핫 인코딩을 사용했습니다.

4. Data Splitting

English: Split the dataset into training and testing sets (70%-30%) while maintaining class balance using train_test_split.
Korean: train_test_split을 사용하여 클래스 균형을 유지하며 데이터셋을 70%-30% 비율로 학습 및 테스트 세트로 분할했습니다.

5. Data Scaling

English: Standardized numerical features using StandardScaler to ensure all features had a similar scale.
Korean: StandardScaler를 사용하여 모든 특성이 유사한 스케일을 가지도록 수치형 특성을 표준화했습니다.

6. Hyperparameter Tuning for Random Forest

English: Performed hyperparameter tuning on the Random Forest model using GridSearchCV to find the best parameters for optimal performance.
Korean: GridSearchCV를 사용하여 Random Forest 모델의 하이퍼파라미터 튜닝을 수행하여 최적의 성능을 위한 최적의 매개변수를 찾았습니다.

7. Model Training

English: Trained the Random Forest model with the best hyperparameters obtained from the grid search.
Korean: 그리드 검색에서 얻은 최적의 하이퍼파라미터로 Random Forest 모델을 학습시켰습니다.

8. Model Evaluation

English: Evaluated the model using metrics such as accuracy, ROC-AUC, and classification report. Visualized the confusion matrix.
Korean: 정확도, ROC-AUC, 분류 보고서와 같은 지표를 사용하여 모델을 평가했습니다. 혼동 행렬을 시각화했습니다.

9. Feature Importance Analysis

English: Identified and visualized the most important features using the feature importance scores from the Random Forest model.
Korean: Random Forest 모델의 특성 중요도 점수를 사용하여 가장 중요한 특성을 식별하고 시각화했습니다.

10. SHAP Analysis

English: Applied SHAP (SHapley Additive exPlanations) to understand the impact of each feature on the model predictions and visualized the results.
Korean: SHAP(Shapley Additive exPlanations)을 적용하여 각 특성이 모델 예측에 미치는 영향을 이해하고 결과를 시각화했습니다.

11. LIME Analysis

English: Used LIME (Local Interpretable Model-Agnostic Explanations) to explain individual predictions. Visualized results for a specific test instance.
Korean: LIME(Local Interpretable Model-Agnostic Explanations)을 사용하여 개별 예측을 설명했습니다. 특정 테스트 인스턴스에 대한 결과를 시각화했습니다.

