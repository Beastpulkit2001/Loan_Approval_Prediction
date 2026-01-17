<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

  <h1>Loan Approval Prediction System</h1>
    <p>
        This project focuses on automating the loan approval process using machine learning. By analyzing historical data of <strong>4,269 applicants</strong>, the model predicts whether a loan will be <code>Approved</code> or <code>Rejected</code> based on financial indicators and personal assets.
    </p>

   <h2>📌 Project Highlights</h2>
    <ul>
        <li><strong>Automated Decisioning:</strong> Reduces manual review time for financial institutions.</li>
        <li><strong>Accuracy:</strong> Achieved a predictive accuracy of <strong>90.4%</strong> using Logistic Regression.</li>
        <li><strong>Feature Rich:</strong> Analyzes CIBIL scores, multiple asset classes (residential, luxury, bank), and employment status.</li>
    </ul>

  <h2>📊 Dataset Overview</h2>
    <p>The dataset includes the following key features:</p>
    <table>
        <thead>
            <tr>
                <th>Feature</th>
                <th>Description</th>
            </tr>
        </thead>
        <tbody>
            <tr><td><code>no_of_dependents</code></td><td>Number of family members dependent on the applicant.</td></tr>
            <tr><td><code>education</code></td><td>Graduate or Not Graduate.</td></tr>
            <tr><td><code>income_annum</code></td><td>Total annual income.</td></tr>
            <tr><td><code>cibil_score</code></td><td>Credit history score (critical factor).</td></tr>
            <tr><td><code>asset_values</code></td><td>Values for Residential, Commercial, Luxury, and Bank assets.</td></tr>
            <tr><td><code>loan_status</code></td><td><strong>Target:</strong> Approved (1) or Rejected (0).</td></tr>
        </tbody>
    </table>

  <h2>⚙️ Methodology</h2>
    <h3>1. Data Preprocessing</h3>
    <p>The data underwent rigorous cleaning, including stripping whitespace from categorical values and column headers. Categorical variables were encoded numerically: <code>Graduate</code> as 1, <code>Self-Employed</code> as 1, and <code>Approved</code> as 1.</p>
    
  <h3>2. Exploratory Data Analysis (EDA)</h3>
    <p>The project utilizes <strong>Kernel Density Estimate (KDE)</strong> plots to visualize the distribution of financial features and identify skewness or outliers in the data.</p>

  <h3>3. Model Training</h3>
    <p>Features were normalized using <code>StandardScaler</code> to ensure consistent weight distribution. A <strong>Logistic Regression</strong> model was trained on the processed data to produce binary classifications.</p>

  <h2>📈 Model Performance</h2>
    <p>The final model performance metrics on the test set (854 records) are as follows:</p>
    <table>
        <thead>
            <tr>
                <th>Status</th>
                <th>Precision</th>
                <th>Recall</th>
                <th>F1-Score</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td><strong>Rejected (0)</strong></td>
                <td>0.88</td>
                <td>0.86</td>
                <td>0.87</td>
            </tr>
            <tr>
                <td><strong>Approved (1)</strong></td>
                <td>0.92</td>
                <td>0.93</td>
                <td>0.92</td>
            </tr>
        </tbody>
    </table>
    <p><span class="badge">Overall Accuracy: 90.4%</span></p>

  <h2>🚀 Installation & Usage</h2>
    <p>To reproduce this analysis, clone the repository and install the dependencies:</p>
    <pre><code>pip install pandas numpy matplotlib seaborn scikit-learn</code></pre>
    <p>Run the Jupyter Notebook:</p>
    <pre><code>jupyter notebook "Loan-Approval-Prediction Project.ipynb"</code></pre>

  <h2>🛠️ Tech Stack</h2>
    <ul>
        <li><strong>Language:</strong> Python</li>
        <li><strong>Data Handling:</strong> Pandas, NumPy</li>
        <li><strong>Visualization:</strong> Matplotlib, Seaborn</li>
        <li><strong>Machine Learning:</strong> Scikit-learn</li>
    </ul>

</body>
</html>
