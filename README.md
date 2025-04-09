# Machine Learning assignment 1

# House Prices - Advanced Regression Techniques

## კონკურსის მიმოხილვა
ამ კონკურსის მიზანია საცხოვრებელი სახლის გაყიდვის ფასის პროგნოზირება სხვადასხვა თვისებების მიხედვით.

## ჩემი მიდგომა
მონაცემთა გაწმენდის შემდეგ, გავატარე Feature Engineering, გამოვიყენე Random Forest და სხვა მოდელები, ჩავატარე ჰიპერპარამეტრების ტესტირება და შევარჩიე საუკეთესო მოდელი.

## რეპოზიტორიის სტრუქტურა
- `DecisionTreeRegressor.ipynb`:notebook ექსპერიმენტებისთვის decision tree ze
- `LinearRegression.ipynb`:notebook ექსპერიმენტებისთვის Linear Regression ze
- `random_forest_model.ipynb`:notebook ექსპერიმენტებისთვის random forest ze
- `model_inference.ipynb`: საუკეთესო მოდელის გამოყენებით პროგნოზირება
- `README.md`: პროექტის აღწერა

## Feature Engineering
- კატეგორიული ცვლადები გადაყვანილია OneHot/Label-ად
- Nan მნიშვნელობები ჩანაცვლებულია საშუალო/მოდი/0 მნიშვნელობებით

## Feature Selection
- Drop-ი მაღალი ნაკლიანი სვეტებისთვის
- კორელაციის ანალიზი

## Training
- გამოვიყენე LinearRegression, DecisionTree, RandomForest
- ჰიპერპარამეტრების GridSearch
- საბოლოოდ RandomForest ყველაზე კარგი შედეგი აჩვენა

## MLflow Tracking
- ყველა ექსპერიმენტი დალოგილია [DagsHub MLflow Experiments](https://dagshub.com/nurch22/my-first-repo.mlflow)
- ლოგირებული პარამეტრები: `model_type`, `n_estimators`, `imputer_strategy`
- საუკეთესო მოდელის შედეგები:
                              test_rmse    28838.16465593191
                              test_mae     18081.33470319635
                              train_rmse   11166.377707021082
                              train_mae    6696.779172374429
                              train_r2     0.9790951566913154
                              test_r2      0.8915770049071198


