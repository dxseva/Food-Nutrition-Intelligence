# Food-Nutrition-Intelligence
A machine learning-powered nutritionist application that predicts recipe ratings, analyzes nutritional content, and recommends similar dishes based on ingredient lists.
<br><br>

## **Project Overview**
This application combines **data science techniques** with practical **nutrition analysis** to help users make informed food choices.  
The system takes **ingredient lists** as input and provides three key insights:  
• **Taste predictions** using ML models (regression/classification)  
• **Comprehensive nutritional breakdowns** with daily value percentages  
• **Recipe recommendations** based on similarity matching  

<br><br>

## **File Structure**
```
src/
├── nutritionist.py
├── recipes.py
├── recipes.ipynb
├── data/
└── models/
```

• **`src/`** – Core application directory containing all implementation files  
• **`data/`** – Processed datasets including nutrition facts and recipe collections  
• **`models/`** – Trained machine learning models for rating predictions  

<br><br>

## **Core Components**
• **`nutritionist.py`**  
&nbsp;&nbsp; Main **command-line interface** that orchestrates the entire prediction pipeline. Handles input parsing, model inference, and formatted output generation.  

• **`recipes.py`**  
&nbsp;&nbsp; Core module containing the application's **class architecture** and **data processing methods**. Implements ML predictions, nutrition analysis, and recipe similarity algorithms.  

• **`recipes.ipynb`**  
&nbsp;&nbsp; Research notebook documenting the complete **data science workflow** from exploration through model selection and validation. Includes regression & classification experiments.  

<br><br>

## **Example Usage**
```bash
$ ./nutritionist.py milk, honey, jam
I. OUR FORECAST
You might find it tasty, but in our opinion, it is a bad idea to have a
dish with that list of ingredients.

II. NUTRITION FACTS
Milk
Protein - 6% of Daily Value
Total Carbohydrate - 1% of Daily Value
Total Fat - 1% of Daily Value
Calcium - 12% of Daily Value
...
Honey
...
Jam
...

III. TOP-3 SIMILAR RECIPES:
- Strawberry-Soy Milk Shake, rating: 3.0, URL:
  https://www.epicurious.com/recipes/food/views/strawberry-soy-milk-shake-239217
- ...
- ...
```
<br><br>

## **Technical Implementation**
### **Machine Learning Pipeline**
• Cross-validation across **regression & classification algorithms**  
• **Ensemble methods** for improved prediction accuracy  
• **Custom evaluation metrics** balancing false positives & negatives  
• **Feature engineering** from ingredient boolean matrices  

### **Data Processing**
• **USDA FoodData Central API** integration for nutritional data  
• **% Daily Value** calculations following FDA guidelines  
• **Cosine similarity** for recipe matching  
• Preprocessing with **outlier detection & feature scaling**  

### **External Dependencies**
• **scikit-learn** – ML model implementation & validation  
• **pandas** – Data manipulation & analysis  
• **numpy** – Numerical computing  
• **requests** – HTTP client for API interactions  
• **jupyter** – Interactive development & analysis  

<br><br>

## **Data Sources**
• **Epicurious Recipe Collection** – 20k+ recipes with ratings & ingredient lists  
• **USDA FoodData Central** – Comprehensive nutritional database via API  

<br><br>

## **Model Performance**
The final implementation uses the **optimal model** selected through **systematic cross-validation** across regression and classification approaches.  

Metrics include:  
• **RMSE** for continuous rating prediction  
• **Accuracy** and **Precision-Recall** for categorical classification  
• Comparisons against **naive baseline predictors**  


