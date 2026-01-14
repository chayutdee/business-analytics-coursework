# Reflective Report

#### Name: Chayut Deekongsieng 
#### Student ID: 46800883

## Section 1: Process of solving problems and learning to use 'Notebooks.'

In term of the process of solving problems with 'Notebook' utilization, I would align with the process of data analysis. I would summarize the step as follows:
1. **Define Objectives** -  Start by clearly defining what you aim to solve. Set clear objectives and formulate specific questions that your data analysis aims to answer. It's also helpful to propose initial hypotheses about the expected outcomes.
2. **Load and Prepare Data**
    - Import and Setup: Use libraries such as pandas for data manipulation, matplotlib for visualization, and scikit-learn for modeling. Load your dataset into the notebook.
    - Data Preparation: Clean the data by addressing missing values and incorrect data types, and prepare it for analysis by transforming data as needed.
4. **Data Exploratory** - Perform exploratory data analysis (EDA) using statistical summaries, distribution of data, and visualizations to investigate and understand the data's structure, trends, and relationships.
5. **Analyze** - Apply statistical tests to validate your hypotheses. Build predictive or analytical models using techniques like regression or classification to delve deeper into the data.
6. **Interpret and Communicate Results** - Extract insights and document your findings. Document your analytical process and findings in Markdown cells for clarity and reproducibility. Use visual plots to effectively communicate the results and insights derived from the data.\n,
8. **Make Decisions** - Use the insights derived from the analysis to informed decisions or propose actionable recommendations. This step translates analytical findings into practical outcomes to solve the targeted problem

## Section 2: Progress Throughout the Unit and Future Aspirations
 
At the beginning of this unit, my knowledge of data science was limited. My previous work experience involved data analysis, but it mostly focused on Excel and SQL, with no hands-on experience in Python. As a result, my coding and modeling skills had room for improvement

Through the course, I significantly developed both my theoretical understanding and practical skills. Initially, I found it challenging to work with complex algorithms, but through hands-on exercises and lectures, I gained confidence, particularly in using models like regression analysis. My familiarity with Python, along with libraries such as pandas, scikit-learn, and matplotlib, also improved. Frequent coding practice solidified my understanding of data preprocessing and modeling techniques.

Moving forward, I am keen to further explore data science, especially its business applications. I am particularly interested in artificial intelligence, which is becoming increasingly important across industries. I plan to continue developing these skills in my master's degree and pursue a data analytics role in the tech industry, contributing to projects that leverage data to drive impactful decisions.

## Section 3: Discussion Points on Portfolio 4

### 1)  Reason Behind Dataset Selection

I have selected the **'Flight Delay Data'** dataset for my assignment. On an emotional level, I was drawn to real-world data, rather than synthetic, because I wanted something I could relate to and find genuinely interesting. I have a strong personal connection to the airport business, and this dataset aligns with that interest. Moreover, I believe it has the potential to provide valuable insights and support decision-making in the aviation field.

From a more rational standpoint, this dataset contains key features like arrival time, departure time, and information on delays and cancellations, which makes it well-suited for answering important questions and even predicting flight outcomes. However, the dataset is enormous, with nearly 2 million rows of data collected from flights in 2008. To make the analysis more manageable while still maintaining a representative sample, I used the .sample() method to extract 5% of the dataset, which should still provide significant insights into the broader population.

### 2) Objective of Analysis and Modeling

To identify the problem I aimed to solve, I explored the dataset and considered key challenges in air travel that were both impactful and actionable. After reviewing features such as departure time, arrival time, delay time, and flight status, I focused on **'arrival delays'**, which is a critical issue for passengers, airlines, and operations.

My goal was to identify the factors most strongly related to arrival delays. Specifically, I aimed to determine which variables (up to taxi-off when departing) have the most significant impact on arrival time. I developed models to predict not only the extent of these delays but also to forecast flight statuses—whether a flight would be on-time, slightly delayed, highly delayed, canceled, or diverted. These insights can help improve scheduling, optimize resource allocation, and ultimately enhance operational efficiency, especially on the arrival side. ultimately enhance operational efficiency, especially on the arrival side.

### 3) Reason Behind Machine Model Selectione

**Linear Regression for Arrival Delay Prediction:** \
I chose Linear Regression because it's straightforward and works well for predicting continuous numbers like the minutes of arrival delay. It helps us see how different things like the time a flight is supposed to leave, how long it spends taxiing, and information about the airline connect to how late it arrives.

**K-Nearest Neighbors (KNN) for Flight Status Prediction:** \
I selected K-Nearest Neighbors (KNN) to predict the flight status—whether a flight is on time, sightly or highly delayed, canceled, or diverted—because it's good at handling categories. KNN looks at the closest examples in the data to decide the status of a new flight. I used GridSearchCV to find the best settings for KNN, making sure it fits our problem as well as possible. Although the accuracy and F1-score show there's room to get better, but KNN is a strong starting point for classification.

**MLP Classifier for Flight Status Prediction:** \
I also utilized MLPClassifier in prediction of Flight Status in comparison with KNN. Theorically, it can handle complex, non-linear relationships in the data better than simpler models like KNN.\n,
By using the 'logistic' activation function, the model is well-suited for multi-class classification tasks, like predicting flight status (on-time, delayed, canceled, or diverted). The 'adam' solver was chosen for its efficiency, especially with large datasets, as it adjusts the learning rate automatically to help the model converge faster.

