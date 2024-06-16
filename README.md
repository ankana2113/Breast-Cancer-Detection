# Breast Cancer Detection
<div>
  <img src="https://th.bing.com/th/id/OIP.7jeJ0rj2Ii4UVrinpeZ5HwHaD4?w=345&h=180&c=7&r=0&o=5&dpr=1.5&pid=1.7" alt="breast-cancer-detection.jpeg" height=500 width=1000>
</div>
<div>
  <h2>Objective:</h2>
  <p>
    1. Apply the fundamental concepts of machine learning from an available dataset. <br>
    2. Evaluate and interpret the results and justify the interpretation based on observed dataset. <br>
    3. Create notebooks that serve as computational and observations. <br>
    4. The analysis is divided into 3 sections, saved in separate juypter notebooks in this repository. <br>
</p>
</div>

<div>
  <h2>Workflow</h2>
  <p>
    1. Understanding the problem. <br>
    2. Exploratory Data Analysis. <br>
    3. Data pre-processing. <br>
    4. Build and train model to predict whether tumor is <code><bold>Malignant</bold></code> or <code><bold>Benign</bold></code>. <br>
  </p>
</div>

<div>
  <h2>Models deployed</h2>
  <h3>Support Vector Machines (SVM)</h3>
  <img src="https://th.bing.com/th?id=OIP.OKO_JOxkTZWAfVk3cOEX3wHaEK&w=333&h=187&c=8&rs=1&qlt=90&o=6&dpr=1.5&pid=3.1&rm=2" alt="SVM.jpeg" width=300 height=200>
  <p>
    <code>Support Vector Machine(SVM)</code> is a supervised machine learning algorithm which can be used for both classification or regression challenges. However, it is mostly
    used in classification problems. In this algorithm, each data item is plotted as a point in n-dimensional space (where n is number of features you have) with the
    value of each feature being the value of a particular coordinate. Then, we perform classification by finding the hyper-plane that differentiate the two classes
    very well.
  </p>
  <h3>K-Nearest Neighbor Classifier (KNN)</h3>
  <img src="https://th.bing.com/th/id/OIP.r00eWT6npui8_JV5BTKrsgHaFR?w=242&h=180&c=7&r=0&o=5&dpr=1.5&pid=1.7" alt="KNN.jpeg" width=300 height=200>
  <p>
    <code>K-Nearest Neighbors(KNN)</code> classifier is a popular machine learning method known for its simplicity and intuitive approach to classification. It works by     
    finding the closest data points (neighbors) to a new data point and assigning a class label based on the majority vote of those neighbors. KNN is versatile, 
    handling both numerical and categorical data, and doesn't require complex assumptions about the data structure.
  </p>
</div>

<div>
  <h2>Metrics</h2>
  <p>
    Classification metrics are tools to evaluate how well a particular classification model performs. Here's a quick rundown of some common ones:
  </p>
  <h4>Accuracy</h4>
  <p>
    The overall proportion of correct predictions. It's a good starting point, but can be misleading in imbalanced datasets.
  </p>
  <h4>Precision</h4>
  <p>
    Measures how many of the predicted positives were actually positive. Useful when false positives are costly.
  </p>
  <h4>Recall</h4>
  <p>
    Measures how well the model captures all the actual positives. Important when missing positive cases is critical.
  </p>
  <h4>F1-Score</h4>
  <p>
    A harmonic mean of precision and recall, combining both metrics into a single score.
  </p>
  <h4>ROC-AUC</h4>
  <p>
    Area Under the Receiver Operating Characteristic Curve. It reflects how well the model distinguishes between classes, independent of class distribution.
  </p>
</div>

<div>
  <h3>Metrics of this Use-Case</h3>
  <p>
    In <strong>Breast Cancer Classification</strong>, both precision and recall are likely very important. You want to minimize both false positives and false negatives. Here's why:<br>
    <strong>High Recall</strong>: You don't want to miss any potential cancer cases, so a high recall ensures you catch most, if not all, of the cancerous tumors.<br>
    <strong>High Precision</strong>: Biopsies are invasive and can cause anxiety. High precision helps avoid unnecessary biopsies on healthy tissue.<br>
    Therefore, it's often recommended to consider both metrics together,  perhaps using the <code>F1-Score</code>code> (harmonic mean of precision and recall) as a combined measure,
    though I have not used it in this model as it often provides equal weight both <code>Recall</code> and <code>Precision</code> whereas We need to keep check of <bold>Recall</bold> slightly more as we dont want to misdiagnose any potential <code>Malignant</code> case as <code>Benign</code> which might be fatal to the patient.<br>
    Additionally, the <code>ROC-AUC</code> can be helpful to assess the model's ability to differentiate between cancerous and healthy cases.<br>
    Ultimately, the best metric(s) depend on the specific context and priorities of the medical team using the model.
  </p>
</div>

