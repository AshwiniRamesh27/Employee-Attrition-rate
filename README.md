<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>👥 Employee Attrition & Performance Prediction System</title>
</head>
<body>

  <h1>📊 Employee Attrition & Performance Prediction System</h1>

  <p>
    <strong>employee_attrition(updated).py</strong> is an advanced end-to-end analytics and machine learning pipeline designed to predict
    employee attrition, analyze satisfaction and performance factors, and visualize insights through interactive dashboards.
    The project combines <strong>classification, regression, and explainable visualization</strong> to support HR decision-making.
  </p>

  <h2>🎯 Objective</h2>
  <p>
    To analyze employee attrition patterns and build predictive models that help organizations retain valuable employees and
    improve workplace satisfaction and performance using interpretable ML techniques.
  </p>

  <h2>🧠 Key Features</h2>
  <ul>
    <li><strong>Comprehensive Preprocessing:</strong> Cleans, encodes, and engineers new features from HR datasets.</li>
    <li><strong>Attrition Prediction Models:</strong> Logistic Regression, Random Forest, XGBoost, and Stacking Classifier.</li>
    <li><strong>Model Tuning:</strong> Uses RandomizedSearchCV for hyperparameter optimization based on ROC-AUC.</li>
    <li><strong>Visualization Suite:</strong> Generates histograms, correlation heatmaps, confusion matrices, and ROC curves.</li>
    <li><strong>Interactive Dashboards:</strong> Built using <strong>Gradio</strong> for visual insights and employee-level prediction lookup.</li>
    <li><strong>Performance Regression:</strong> Predicts employee performance ratings using Linear Regression, Random Forest, and Gradient Boosting.</li>
  </ul>

  <h2>📁 Workflow</h2>
  <ol>
    <li><strong>Data Ingestion:</strong> Loads <code>Employee-Attrition.csv</code> and applies feature renaming and encoding.</li>
    <li><strong>Feature Engineering:</strong> Combines satisfaction metrics, removes redundant columns, and encodes categorical variables.</li>
    <li><strong>EDA:</strong> Visualizes distributions, correlations, and trends in key employee metrics.</li>
    <li><strong>Attrition Modeling:</strong> 
      <ul>
        <li>Models: Logistic Regression, Random Forest, XGBoost, and Stacking Ensemble</li>
        <li>Evaluates using Accuracy, Precision, Recall, F1-score, and ROC-AUC</li>
      </ul>
    </li>
    <li><strong>Performance Analysis:</strong> Uses regression to predict employee performance ratings.</li>
    <li><strong>Visualization:</strong> Gradio interface provides heatmaps, confusion matrices, ROC curves, and insights.</li>
  </ol>

  <h2>📊 Model Performance Summary</h2>
  <p>
    The following models were evaluated on test data for predicting employee attrition:
  </p>
  <ul>
    <li>✅ <strong>XGBoost:</strong> Best for accuracy and precision.</li>
    <li>✅ <strong>Logistic Regression:</strong> Excellent recall and interpretability.</li>
    <li>✅ <strong>Stacked Model:</strong> Balanced overall ROC-AUC (~0.9).</li>
  </ul>

  <h2>📈 Visualization Outputs</h2>
  <ul>
    <li><strong>Heatmap:</strong> Correlation between HR variables (Age, Salary, Work-Life Balance, etc.).</li>
    <li><strong>ROC Curve:</strong> Model comparison for attrition classification performance.</li>
    <li><strong>Histograms:</strong> Feature distributions showing attrition tendencies.</li>
    <li><strong>Confusion Matrix:</strong> Evaluation of model predictions.</li>
  </ul>

  <h2>💡 Interactive Dashboards</h2>
  <ul>
    <li><strong>Employee Insight Dashboard:</strong> Built using Gradio with visualizations and model outputs.</li>
    <li><strong>Attrition Risk Viewer:</strong> Allows users to adjust thresholds and view top high-risk employees.</li>
    <li><strong>Performance Lookup Tool:</strong> Lets HR query predicted vs. actual employee performance by ID.</li>
  </ul>

  <h2>🧮 Technologies & Libraries</h2>
  <ul>
    <li><code>pandas</code>, <code>numpy</code> — Data wrangling</li>
    <li><code>scikit-learn</code> — Classification, regression, and model tuning</li>
    <li><code>xgboost</code> — Gradient boosting for attrition prediction</li>
    <li><code>matplotlib</code>, <code>seaborn</code> — Data visualization</li>
    <li><code>gradio</code> — Interactive dashboards</li>
  </ul>

  <h2>📦 Dependencies</h2>
  <pre><code>pip install pandas numpy scikit-learn xgboost matplotlib seaborn gradio</code></pre>

  <h2>🚀 Run the Project</h2>
  <pre><code>
# 1️⃣ Train attrition prediction models
python employee_attrition(updated).py

# 2️⃣ Launch Gradio dashboard
python -m gradio app
  </code></pre>

  <h2>📁 Output Files</h2>
  <ul>
    <li><code>job satisfaction.csv</code> — Cleaned dataset used for performance prediction.</li>
    <li><code>heat map.png</code>, <code>roc curve.png</code>, <code>confusion_matrix.png</code> — Visualization outputs.</li>
    <li><code>Perfomance Metrics.png</code> — Model performance summary.</li>
  </ul>

  <h2>📊 Evaluation Metrics</h2>
  <ul>
    <li><strong>Accuracy:</strong> Percentage of correct predictions.</li>
    <li><strong>Precision & Recall:</strong> Measures balance of true positives and false positives.</li>
    <li><strong>ROC-AUC:</strong> Assesses discrimination between attrition and non-attrition cases.</li>
    <li><strong>R², MAE, MSE:</strong> Used for performance regression models.</li>
  </ul>

  <h2>📈 Example Output</h2>
  <pre><code>
Model               Accuracy  Precision  Recall  F1-Score  ROC-AUC
-----------------------------------------------------------------
Logistic Regression   0.85      0.82      0.88     0.85      0.91
Random Forest         0.87      0.83      0.84     0.84      0.90
XGBoost               0.89      0.86      0.87     0.86      0.93
Stacked Model         0.90      0.88      0.88     0.88      0.94
  </code></pre>

  <h2>💬 Insights & Interpretation</h2>
  <ul>
    <li>🧑‍💼 Younger employees with fewer years at the company and frequent travel show higher attrition.</li>
    <li>💰 Salary hikes and promotions strongly correlate with retention.</li>
    <li>📈 XGBoost performed best overall for predicting attrition risk.</li>
    <li>🔍 Linear Regression provides accurate performance estimation for high performers.</li>
  </ul>

  <h2>🔒 Ethical Considerations</h2>
  <ul>
    <li>Ensure data anonymization before deployment.</li>
    <li>Avoid bias in model training by balancing class weights.</li>
    <li>Use predictions to support HR decisions, not replace human judgment.</li>
  </ul>

  <h2>📧 Contact</h2>
  <p>
    <strong>Ashwini Ramesh</strong><br>
    📧 <a href="mailto:ashwiniramesh2709@gmail.com">ashwiniramesh2709@gmail.com</a><br>
    🔗 <a href="https://linkedin.com/in/ashwini27" target="_blank">LinkedIn</a>
  </p>

</body>
</html>
