

---

# AI-Generated-Art-Trends-2024

## Overview
This project analyzes trends in **AI-generated art** to predict future popularity using **XGBoost**. By examining factors such as art style, medium, and tools, we aim to uncover patterns that influence the success of AI art and forecast its evolution in 2024.

---

## Workflow and Methodology

### 1. **Data Collection**
- Compiled a dataset of AI-generated artworks, including:
  - **Art Styles**: Abstract, surrealism, photorealistic, generative, etc.
  - **Mediums**: Digital painting, 3D renders, sketches, animations, etc.
  - **Tools**: AI models and software used (e.g., DALL·E, MidJourney, Stable Diffusion).
  - **Popularity Metrics**: Engagement on social platforms (likes, shares, comments).

### 2. **Data Preprocessing**
- Cleaned and standardized the dataset:
  - Removed duplicate and incomplete entries.
  - Handled missing values using imputation techniques.
- Performed feature encoding:
  - Categorical variables like **Art Style** and **Tool Used** were one-hot encoded.
  - Log-transformed skewed metrics like social engagement.

### 3. **Exploratory Data Analysis (EDA)**
- Identified trends and patterns in the data:
  - Popular art styles and tools by year.
  - Correlations between tools and engagement metrics.
- Visualized:
  - Style distribution across platforms.
  - Popularity trends over time.

### 4. **Model Development**
- Developed predictive models using **XGBoost**:
  - Input: Art style, medium, tool, and engagement metrics.
  - Output: Predicted popularity score.
- Conducted hyperparameter tuning to optimize model performance.
- Validated the model using cross-validation techniques.

### 5. **Evaluation**
- Assessed model performance using:
  - **Mean Absolute Error (MAE)**: For prediction accuracy.
  - **R² Score**: To evaluate explained variance.

---

## Results and Insights
- Identified the most influential factors driving AI art popularity:
  - **Art Styles**: Generative and surrealist styles showed the highest engagement.
  - **Tools**: MidJourney and Stable Diffusion dominate in popularity metrics.
- The model achieved:
  - **R² Score**: 0.67
  - **MAE**: 5.3 (normalized popularity units)

### Sample Visualizations
- Engagement trends by style and tool.
- Popularity predictions for upcoming AI-generated art.

---

## Installation

To set up the project locally:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/ENKI0311/AI-Generated-Art-Trends-2024.git
   cd AI-Generated-Art-Trends-2024
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

---

## Usage

### Analyze the Data
1. Run the **EDA notebook** to explore trends:
   ```bash
   jupyter notebook notebooks/exploratory_data_analysis.ipynb
   ```

### Train and Evaluate the Model
2. Train the XGBoost model:
   ```bash
   python scripts/train.py
   ```

3. Evaluate the model:
   ```bash
   python scripts/evaluate.py
   ```

---

## Project Structure

```
AI-Generated-Art-Trends-2024/
├── data/                   # Raw and preprocessed datasets
├── notebooks/              # Jupyter notebooks for EDA and modeling
├── scripts/                # Python scripts for training and evaluation
├── models/                 # Saved XGBoost models
├── results/                # Visualizations and evaluation outputs
├── requirements.txt        # Dependencies for the project
└── README.md               # Project documentation
```

---

## Future Work
1. **Expand Dataset**:
   - Include more platforms and tools for broader analysis.
2. **Incorporate Time-Series Analysis**:
   - Analyze seasonal trends in AI-generated art.
3. **Explore Alternative Models**:
   - Experiment with neural networks or ensemble methods for improved prediction accuracy.

---

## Contributing
We welcome contributions! To contribute:
1. Fork the repository.
2. Create a branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m "Add feature-name"`).
4. Push to your branch (`git push origin feature-name`).
5. Submit a pull request.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments
We extend our gratitude to all platforms, creators, and tool developers whose data and innovations made this analysis possible.

---

