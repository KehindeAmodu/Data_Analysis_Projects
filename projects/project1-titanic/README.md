# 🛳️ Titanic Survival Analysis

## 🎯 Business Problem
Analyzed factors influencing Titanic passenger survival to understand demographic and socioeconomic impacts on lifeboat allocation.

## 📊 Dataset
- **Source**: Kaggle Titanic Dataset
- **Size**: 891 passengers, 12 features
- **Key Variables**: Age, Class, Gender, Fare, Embarked

## 🛠️ Technical Approach

### 1. **Data Ingestion & Cleaning**
```python
# Loaded via pandas, handled missing values
df = pd.read_csv('titanic.csv')
df['Age'].fillna(df['Age'].median(), inplace=True)
