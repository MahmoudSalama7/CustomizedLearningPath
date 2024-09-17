![Untitled-1](https://github.com/user-attachments/assets/e705eaae-8fa2-404b-bcf8-7e03b98ac5a6)


# Personalized Learning Path Recommender System

**Semi-Final Project** for the **Samsung Innovation Campus (SIC)**

## Overview

This project aims to create a **Personalized Learning Path Recommender System** by analyzing student engagement and learning preferences using the Open University Learning Analytics Dataset (OU-LAD). Our system clusters students based on their engagement levels and classifies them according to their preferred learning style. Based on these features, the system provides personalized recommendations for courses, PDFs, books, videos, and other educational materials.

## Project Features

- **Student Clustering:** 
  - Grouping students based on their engagement patterns with course content.
  
- **Learning Style Classification:** 
  - Identifying students' learning preferences (e.g., visual, auditory, reading/writing, kinesthetic).
  
- **Recommendation System:** 
  - Suggesting relevant courses, learning resources (PDFs, books, videos), and study paths based on a student's learning style and engagement level.
  
## Dataset

The project uses the **Open University Learning Analytics Dataset (OU-LAD)**, which contains data on students, courses, assessments, and interactions. The dataset consists of 7 separate files, each representing different aspects of the learning journey:
1. **studentInfo** – demographic and academic information of students
2. **courses** – details of the courses offered
3. **assessments** – assessment details for each course
4. **studentAssessment** – student performance on assessments
5. **vle** – virtual learning environment activities
6. **studentVLE** – student interactions with the virtual learning environment
7. **studentRegistration** – student registration details for courses

You can find more details about the dataset (https://analyse.kmi.open.ac.uk/open_dataset).

## Methodology

### 1. Data Preprocessing
- Data cleaning and preprocessing were applied to all seven datasets.
- We performed feature engineering to create meaningful features related to student engagement and learning style.

### 2. Clustering Students by Engagement
- We used **K-Means Clustering** to group students based on their interactions with course materials and engagement levels.

### 3. Learning Style Classification
- A **classification model** (using Random Forest) was built to predict each student’s learning style (visual, auditory, reading/writing, kinesthetic) based on their engagement patterns and course performance.

### 4. Recommender System
- Combining the clustering and classification features, we developed a **recommendation engine** to provide personalized learning resources (courses, PDFs, books, videos, etc.) tailored to each student’s preferences and engagement profile.

### 5. Model Evaluation
- We evaluated the performance of our clustering and classification models using **silhouette scores** (for clustering) and standard classification metrics (accuracy, precision, recall, F1-score) for learning style classification.

## Results

- The clustering model effectively grouped students into distinct engagement levels.
- The classification model achieved strong performance in predicting learning styles, leading to accurate and relevant recommendations.

## How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/personalized-learning-recommender-system.git
   cd personalized-learning-recommender-system
   ```

2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Download the **Open University Learning Analytics Dataset (OU-LAD)** from (https://analyse.kmi.open.ac.uk/open_dataset) and place it in the appropriate folder (e.g., `data/`).

4. Run the Jupyter notebook to train models and generate recommendations:
   ```bash
   jupyter notebook
   ```
   Open the notebook and run the cells sequentially.

## Dependencies

The project was developed using the following libraries:
- Python 3.7+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- jupyter

You can install all dependencies via:
```bash
pip install -r requirements.txt
```

## Team

- **Yousef Albasel** – Data Science and Machine Learning
- **Ali Amr** – Data Preprocessing and Clustering
- **Haneen Eldaly** – Project Facilitator and Mentor

## Acknowledgments

Special thanks to **Samsung Innovation Campus (SIC)** for giving us this incredible learning opportunity and to **Haneen Eldaly** for her invaluable guidance and support throughout this project.

## Project Link

Check out the project on Kaggle: (https://www.kaggle.com/code/yousefalbasel/oulad-personalized-learning-path-recommender-sys)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
