# EX. NO. 5

# COMPARING PROMPTING TECHNIQUES THROUGH ENGINEERING PROBLEM-SOLVING SCENARIOS

## AIM

To compare different prompting techniques and evaluate their effectiveness in solving real-world engineering problems by using a problem selected from a student's 3rd-year or final-year project work.

---

# PROBLEM SELECTED

## AI-BASED STUDENT PERFORMANCE PREDICTION SYSTEM

The selected engineering problem is an **AI-Based Student Performance Prediction System**. The main objective of this project is to develop an intelligent system that can predict the academic performance of students using various academic and attendance-related factors.

In a traditional educational environment, teachers generally evaluate student performance by manually analyzing attendance, internal examination marks, assignment marks, previous semester marks, and other academic information. When the number of students is large, manually analyzing all these factors can be time-consuming and may make it difficult to identify students who require additional academic support.

An AI-based prediction system can help analyze historical student data and identify patterns related to academic performance. The system can use machine learning algorithms to learn from previously available student records and generate predictions for new students.

The major input parameters considered in this project are:

* Attendance percentage
* Internal examination marks
* Assignment marks
* Previous semester marks
* Academic performance

The major stages involved in developing the system are data collection, data preprocessing, feature selection, model selection, model training, model testing, performance evaluation, and deployment.

Prompt engineering can be used to obtain better solutions from AI systems during different stages of the project. In this experiment, five prompting techniques are compared:

1. Zero-Shot Prompting
2. Few-Shot Prompting
3. Chain-of-Thought Prompting
4. Role Prompting
5. Structured Prompting

The effectiveness of each technique is evaluated based on the clarity, completeness, consistency, technical relevance, and usefulness of the generated response.

---

# 1. ZERO-SHOT PROMPTING

## Description

Zero-shot prompting is a prompting technique in which the AI is directly given a task without providing examples of how the task should be performed. The AI must understand the problem from the information provided in the prompt and generate an appropriate response.

This technique is simple and requires less prompt preparation. It is useful when the user wants a quick general solution to a problem.

## Prompt

"Develop a machine learning approach for an AI-based student performance prediction system. The system should predict student academic performance using attendance percentage, internal marks, assignment marks, and previous semester marks. Explain the data collection, data preprocessing, feature selection, model selection, training, testing, evaluation, and deployment steps."

## Generated Output

An AI-based student performance prediction system can be developed using supervised machine learning techniques.

The first step is to collect historical student academic data. The dataset should contain attendance percentage, internal marks, assignment marks, previous semester marks, and the corresponding academic performance of students.

After collecting the data, preprocessing should be performed. The dataset should be checked for missing values, duplicate records, incorrect values, and inconsistent data. Missing values can be handled using suitable techniques, and duplicate records should be removed.

The next step is feature selection. Attendance percentage, internal marks, assignment marks, and previous semester marks can be selected as the major input features because they provide useful information about student performance.

The dataset can then be divided into training and testing datasets. Suitable machine learning algorithms such as Linear Regression, Decision Tree, and Random Forest can be considered.

The selected models are trained using the training data. After training, the models are tested using unseen testing data. The performance of the models can be evaluated using suitable metrics.

For numerical prediction, metrics such as Mean Absolute Error, Mean Squared Error, Root Mean Squared Error, and R² score can be used. If the system predicts categories such as High, Average, and Low, classification metrics such as accuracy, precision, recall, and F1-score can be considered.

After comparing the models, the most suitable model can be selected and integrated into a web-based application. The user can enter student details, and the system can provide the predicted academic performance.

## Evaluation

The zero-shot prompt successfully generated a general solution for the student performance prediction problem. It identified the major stages of machine learning development and suggested suitable algorithms and evaluation metrics.

The main advantage of this technique is its simplicity. The user does not need to provide examples or a complex prompt structure.

However, the generated response is relatively general. It does not contain a specific output pattern, detailed project constraints, or examples. Additional prompts may be required if the user needs implementation-specific information.

Therefore, zero-shot prompting is **good for obtaining quick and general engineering solutions**, but it may not always provide highly customized project documentation.

---

# 2. FEW-SHOT PROMPTING

## Description

Few-shot prompting provides a small number of examples before asking the AI to solve the actual problem. These examples demonstrate the expected relationship between input and output.

This technique is useful when the AI needs to follow a particular pattern or classification style.

## Prompt

"Use the following examples to understand the expected student performance prediction pattern.

Example 1:

Attendance = 90%
Internal Marks = 85%
Assignment Marks = 90%
Previous Semester Marks = 88%
Expected Performance = High

Example 2:

Attendance = 60%
Internal Marks = 55%
Assignment Marks = 58%
Previous Semester Marks = 50%
Expected Performance = Low

Example 3:

Attendance = 75%
Internal Marks = 68%
Assignment Marks = 70%
Previous Semester Marks = 65%
Expected Performance = Average

Now analyze the following student:

Attendance = 82%
Internal Marks = 78%
Assignment Marks = 80%
Previous Semester Marks = 75%

Predict the expected performance and explain the factors influencing the prediction."

## Generated Output

### Predicted Performance: High

The student is expected to have **high academic performance** based on the given input values.

The attendance percentage is 82%, which indicates that the student has regular participation in academic activities. The internal mark of 78% indicates good performance in internal assessments.

The assignment mark of 80% also indicates that the student is consistently completing academic activities and performing well in continuous assessment.

The previous semester mark of 75% indicates that the student has maintained a relatively consistent academic performance over time.

When all these factors are considered together, the student is expected to have high or above-average academic performance.

The prediction is based on the pattern demonstrated in the examples. In a real machine learning application, the prediction would be generated from a trained model using a larger historical dataset.

## Evaluation

Few-shot prompting produces a more consistent response because examples are provided to the AI before the actual task.

The examples help define the expected relationship between the input features and the output category. This makes the technique useful for classification-based engineering applications.

Compared with zero-shot prompting, the few-shot prompt provides more context and guidance. It can also improve the consistency of the output format.

However, the quality of the response depends on the quality and relevance of the examples provided. If the examples are incomplete or misleading, the generated output may also be less reliable.

Therefore, few-shot prompting is **very useful when examples, patterns, or specific output formats are required**.

---

# 3. CHAIN-OF-THOUGHT PROMPTING

## Description

Chain-of-thought prompting encourages the AI to approach a complex problem through a sequence of logical stages. Instead of directly providing a final answer, the prompt asks the AI to organize the problem into smaller steps.

This technique is especially useful for engineering problems involving multiple processes.

## Prompt

"Analyze the AI-based student performance prediction problem systematically. Break the solution into logical stages. Explain each stage starting from problem identification and data collection to preprocessing, feature selection, model selection, training, testing, evaluation, deployment, and final prediction."

## Generated Output

### Step 1: Identify the Problem

The first step is to clearly define the problem. The objective is to predict student academic performance based on academic and attendance-related factors.

### Step 2: Collect Data

Historical student data should be collected. The dataset should contain attendance percentage, internal marks, assignment marks, previous semester marks, and the corresponding performance.

A sufficiently representative dataset should be used so that the model can learn useful patterns.

### Step 3: Clean the Data

The collected dataset should be examined for missing values, duplicate records, incorrect entries, and inconsistent data.

Missing values should be handled appropriately, and duplicate records should be removed.

### Step 4: Select Features

The major features include attendance percentage, internal marks, assignment marks, and previous semester marks.

These features are useful because attendance indicates regularity, internal marks represent current academic performance, assignment marks represent continuous assessment, and previous semester marks provide historical performance information.

### Step 5: Select the Machine Learning Model

Different algorithms can be considered depending on the type of prediction required.

Linear Regression can be used when the target is a continuous numerical score.

Decision Tree can be used to model relationships between different academic factors.

Random Forest can be used to handle more complex relationships and improve predictive performance by combining multiple decision trees.

### Step 6: Split the Dataset

The dataset should be divided into training and testing datasets.

The training dataset is used for learning, while the testing dataset is used to evaluate how well the trained model performs on unseen data.

### Step 7: Train the Model

The selected machine learning algorithms are trained using the training dataset.

During training, the model learns the relationship between student-related input features and academic performance.

### Step 8: Test the Model

After training, the model is tested using the testing dataset. The testing data should not be used during model training so that the model can be evaluated fairly.

### Step 9: Evaluate the Model

If the system predicts numerical marks, MAE, MSE, RMSE, and R² can be used.

If the system predicts categories such as High, Average, and Low, accuracy, precision, recall, and F1-score can be used.

### Step 10: Select the Best Model

The performance of different models should be compared. The most suitable model should be selected based on its performance, reliability, interpretability, and project requirements.

### Step 11: Deploy the System

The selected model can be integrated into a web-based application.

The application can contain fields where the user enters attendance, internal marks, assignment marks, and previous semester marks.

### Step 12: Generate Prediction

The entered student information is passed to the trained model. The model processes the input and produces the predicted academic performance.

## Evaluation

Chain-of-thought prompting is effective for multi-stage engineering problems because it organizes the solution into logical steps.

The technique provides more detailed information than zero-shot prompting. It makes the workflow easier to understand and helps ensure that important stages of the engineering problem are not missed.

The main advantage is systematic problem-solving. The main limitation is that very detailed reasoning prompts can produce longer responses than required for simple tasks.

Therefore, chain-of-thought prompting is **highly effective for complex, multi-stage engineering problems**.

---

# 4. ROLE PROMPTING

## Description

Role prompting assigns a specific professional or expert role to the AI. The AI then generates its response from the perspective of that role.

For an engineering project, assigning a role such as "Machine Learning Engineer" can help produce technically relevant and professionally structured suggestions.

## Prompt

"Act as a senior Machine Learning Engineer with experience in developing educational data analysis and prediction systems.

Design an AI-based student performance prediction system using attendance percentage, internal marks, assignment marks, and previous semester marks.

Provide a detailed engineering solution covering:

1. Problem definition
2. Data collection
3. Data preprocessing
4. Feature selection
5. Machine learning model selection
6. Model training
7. Model testing
8. Model evaluation
9. Deployment
10. Expected output

Recommend practical machine learning techniques that are suitable for a student engineering project."

## Generated Output

### Problem Definition

The objective is to develop an AI-based prediction system that can analyze student academic information and predict their expected academic performance.

The system should use historical data to identify relationships between attendance, marks, assignments, previous academic performance, and the final outcome.

### Data Collection

The dataset should contain student academic information collected from appropriate academic records.

The major attributes can include:

* Attendance percentage
* Internal examination marks
* Assignment marks
* Previous semester marks
* Final academic performance

The dataset should contain sufficient records to train and evaluate the machine learning model.

### Data Preprocessing

Before training the model, the dataset should be cleaned.

Missing values should be identified and handled. Duplicate records should be removed. Incorrect values should be corrected where possible.

The data should also be converted into a suitable numerical format for machine learning.

### Feature Selection

The most relevant features should be selected.

Attendance, internal marks, assignment marks, and previous semester marks can be used as the primary input features.

Feature importance techniques can also be used to determine which variables contribute more strongly to the prediction.

### Model Selection

Different machine learning algorithms can be tested.

Linear Regression can be considered for predicting numerical academic scores.

Decision Tree and Random Forest can be used for modeling more complex relationships between academic factors.

The models should be compared using suitable evaluation metrics.

### Model Training

The processed dataset should be divided into training and testing datasets.

The training data is used to train the machine learning algorithms. The model learns patterns from the historical student records.

### Model Testing

After training, the model should be tested using unseen data.

Testing helps determine whether the model can generalize its predictions to students whose data was not included during training.

### Model Evaluation

For regression-based prediction, MAE, MSE, RMSE, and R² can be used.

For classification-based prediction, accuracy, precision, recall, and F1-score can be considered.

### Deployment

After selecting a suitable model, it can be integrated into a web-based application.

The application can provide a user-friendly interface where student information is entered.

### Expected Output

The system should provide a predicted academic performance based on the student's input information.

The prediction can help teachers identify students who may require additional academic support and can assist in making data-driven academic decisions.

## Evaluation

Role prompting produces a professional and domain-specific response.

By assigning the role of a Machine Learning Engineer, the AI focuses on technical aspects such as feature selection, algorithm selection, model evaluation, and deployment.

The response is more relevant to an engineering project than a simple general-purpose answer.

Role prompting is particularly useful when the user needs recommendations from a particular professional perspective.

Therefore, role prompting is **very effective for obtaining domain-specific and professional engineering solutions**.

---

# 5. STRUCTURED PROMPTING

## Description

Structured prompting provides detailed instructions about the role, project context, problem, input data, task, requirements, constraints, and expected output format.

It is one of the most useful techniques for engineering projects because engineering problems often contain multiple requirements that must be addressed in a specific order.

## Prompt

"Role: Senior Machine Learning Engineer

Project: AI-Based Student Performance Prediction System

Problem:
Develop a system that predicts student academic performance using attendance percentage, internal marks, assignment marks, and previous semester marks.

Input Features:

1. Attendance percentage
2. Internal examination marks
3. Assignment marks
4. Previous semester marks

Task:
Design a complete machine learning solution for the project.

Requirements:

* Explain data collection.
* Explain data preprocessing.
* Identify important features.
* Recommend suitable machine learning algorithms.
* Explain model training.
* Explain model testing.
* Explain evaluation metrics.
* Explain deployment.
* Provide the expected system output.

Constraints:

* The solution should be simple.
* The solution should be practical.
* The solution should be suitable for an engineering project.
* The solution should be easy to implement and understand.

Output Format:

1. Problem Definition
2. Data Collection
3. Data Preprocessing
4. Feature Selection
5. Model Selection
6. Model Training
7. Model Testing
8. Model Evaluation
9. Deployment
10. Expected Output"

## Generated Output

### 1. Problem Definition

The objective of the project is to develop an AI-based student performance prediction system.

The system analyzes different academic parameters and predicts the expected performance of a student.

The prediction can help identify academic patterns and support teachers in monitoring student progress.

### 2. Data Collection

Historical student academic records are collected for developing the machine learning model.

The dataset should contain attendance percentage, internal examination marks, assignment marks, previous semester marks, and the corresponding target academic performance.

The quality and relevance of the dataset are important because the machine learning model learns patterns from the available historical information.

### 3. Data Preprocessing

The collected data must be prepared before it is supplied to the machine learning algorithm.

The dataset should be checked for:

* Missing values
* Duplicate records
* Incorrect values
* Inconsistent data
* Unnecessary columns

Missing values can be handled using suitable methods. Duplicate records should be removed.

The numerical data should be represented in an appropriate format. Feature scaling can be applied when required by the selected algorithm.

### 4. Feature Selection

The main input features are:

* Attendance percentage
* Internal examination marks
* Assignment marks
* Previous semester marks

These features are selected because they provide useful information about student academic behavior and performance.

Attendance represents student participation, internal marks represent current academic achievement, assignment marks indicate continuous academic activity, and previous semester marks provide historical performance information.

### 5. Model Selection

Multiple machine learning models can be considered.

**Linear Regression:**
Suitable when the target is a numerical performance score.

**Decision Tree:**
Useful for representing decision-based relationships between student features and performance.

**Random Forest:**
Combines multiple decision trees and can model more complex relationships between input features and academic performance.

The models should be trained and evaluated before selecting the final model.

### 6. Model Training

The cleaned dataset is divided into training and testing datasets.

The training data is provided to the selected machine learning algorithm.

The model learns the relationship between the input variables and the target performance from the training data.

During training, the algorithm identifies patterns that can be used to make predictions for new student records.

### 7. Model Testing

The testing dataset contains records that were not used during the training process.

The trained model is given the testing data and its predictions are compared with the actual values.

This helps determine whether the model can make accurate predictions on unseen student data.

### 8. Model Evaluation

If the target is a numerical academic score, the following metrics can be used:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

If the target is a category such as High, Average, or Low, classification metrics can be used:

* Accuracy
* Precision
* Recall
* F1-score

The model with suitable performance can be selected for deployment.

### 9. Deployment

The selected machine learning model can be integrated into a web-based application.

The application can provide input fields for:

* Attendance percentage
* Internal marks
* Assignment marks
* Previous semester marks

After the user enters the values, the application sends the information to the trained model.

The model processes the input and generates a prediction.

### 10. Expected Output

The system provides the predicted academic performance of the student.

For example, the system may produce an output such as:

**Predicted Performance: High**

or

**Predicted Performance: Average**

or

**Predicted Performance: Low**

The system can also be extended to display the factors used for prediction and provide academic monitoring information.

## Evaluation

Structured prompting produced the most comprehensive and organized response among all the prompting techniques used in this experiment.

The prompt clearly specified the AI's role, project title, problem statement, input features, requirements, constraints, and output format.

Because all the necessary information was explicitly provided, the generated response covered almost every important stage of the engineering project.

The structured response is also easier to use for project documentation because each section is clearly separated.

Therefore, structured prompting is considered **the most effective prompting technique for the selected engineering problem**.

---

# COMPARATIVE ANALYSIS

The five prompting techniques were compared based on their ability to generate useful engineering solutions.

| Prompting Technique        | Clarity   | Detail    | Consistency | Project Relevance | Overall Effectiveness |
| -------------------------- | --------- | --------- | ----------- | ----------------- | --------------------- |
| Zero-Shot Prompting        | Good      | Moderate  | Moderate    | Good              | Good                  |
| Few-Shot Prompting         | Good      | Good      | Very Good   | Very Good         | Very Good             |
| Chain-of-Thought Prompting | Very Good | High      | Very Good   | Very Good         | Very Good             |
| Role Prompting             | Very Good | High      | Very Good   | Excellent         | Very Good             |
| Structured Prompting       | Excellent | Very High | Excellent   | Excellent         | Excellent             |

### Zero-Shot Prompting

Zero-shot prompting is suitable when a quick and general response is required. It requires minimum input from the user and is easy to apply.

### Few-Shot Prompting

Few-shot prompting is useful when examples are available. It improves consistency and helps the AI follow a particular prediction or classification pattern.

### Chain-of-Thought Prompting

Chain-of-thought prompting is useful when the engineering problem contains multiple steps. It organizes the problem-solving process and makes the solution systematic.

### Role Prompting

Role prompting is effective when the user wants a domain-specific response. Assigning an expert role helps focus the response on engineering requirements.

### Structured Prompting

Structured prompting is the most comprehensive technique in this experiment. It provides detailed instructions and a specific output structure, resulting in a clear, complete, and project-oriented solution.

---

# OUTPUT

The experiment successfully demonstrated the use of different prompting techniques for solving an engineering problem based on an **AI-Based Student Performance Prediction System**.

The **Zero-Shot Prompting** technique generated a general machine learning solution without requiring examples. It was simple and useful for obtaining basic information about the project.

The **Few-Shot Prompting** technique used sample student data and expected performance categories. The examples helped the AI understand the required prediction pattern and generate a more consistent response.

The **Chain-of-Thought Prompting** technique divided the engineering problem into multiple logical stages, including problem identification, data collection, preprocessing, feature selection, model selection, training, testing, evaluation, and deployment.

The **Role Prompting** technique assigned the role of a senior Machine Learning Engineer. This resulted in a more professional and technically focused response.

The **Structured Prompting** technique specified the role, project, problem, input features, requirements, constraints, and expected output format. It generated the most detailed, organized, and project-specific response.

The comparison shows that different prompting techniques are useful for different engineering requirements. Simple prompts are suitable for general tasks, while detailed and structured prompts are more suitable for complex engineering projects.

---

# CONCLUSION

The experiment was successfully conducted to compare different prompting techniques for solving a real-world engineering problem. An **AI-Based Student Performance Prediction System** was selected as the project scenario because it involves data analysis, machine learning, prediction, and practical engineering decision-making.

Five prompting techniques were applied: **Zero-Shot Prompting, Few-Shot Prompting, Chain-of-Thought Prompting, Role Prompting, and Structured Prompting**.

Zero-shot prompting provided a quick and general solution. Few-shot prompting improved consistency by providing examples. Chain-of-thought prompting was effective for breaking the problem into multiple logical stages. Role prompting provided a professional and domain-specific perspective.

Structured prompting produced the most complete and organized solution because it clearly defined the role, project context, problem, input features, requirements, constraints, and output format.

From the comparison, it can be concluded that **no single prompting technique is suitable for every situation**. The technique should be selected according to the complexity and requirements of the engineering problem. For simple questions, zero-shot prompting may be sufficient. For pattern-based tasks, few-shot prompting can be useful. For complex problems, chain-of-thought prompting can provide a systematic approach. Role prompting is useful for domain-specific tasks, while structured prompting is highly suitable for complete engineering project development.

Therefore, **effective prompt engineering can significantly improve the clarity, quality, relevance, and usefulness of AI-generated solutions in real-world engineering applications**.

