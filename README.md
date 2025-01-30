# 🎵 Spotify Song Popularity Prediction 🎶  


## 🏆 **Motivation**
Spotify, as a leading music streaming platform, generates extensive datasets, offering an opportunity to apply **data mining techniques**. By analyzing this data, we aim to gain **valuable insights** into **user behavior** and **music trends**. This project aligns with the increasing relevance of **recommendation systems** in the digital age and contributes to understanding the factors influencing **song popularity**.

---

## ❓ **Research Questions**
- Which musical features (tempo, danceability, energy, etc.) are **most correlated** with song popularity on Spotify?  
- Can we identify specific **attributes** that dominate the most streamed songs?  
- Which **prediction model** is most suitable for forecasting song popularity?  
- How can we apply this knowledge to **music production and promotion**?  

---

## 📂 **Dataset Overview**
- **Source:** [Kaggle Spotify Dataset](https://www.kaggle.com)  
- **Total Records:** **20,000** songs  
- **Attributes:** **18 features**, including **acousticness, danceability, tempo, valence**, etc.  
- **Ranking:** Songs are ranked from **1 to 100** based on their popularity score.  

### 🎵 **Key Attributes**
| Feature         | Description |
|----------------|-------------|
| Genre         | Music genre of the song |
| Artist Name   | Name of the artist |
| Track Name    | Name of the song |
| Popularity    | Popularity score (1-100) |
| Danceability  | How suitable the track is for dancing |
| Tempo         | Speed of the song in beats per minute (BPM) |
| Loudness      | Overall loudness of the track |
| Energy        | Intensity of the track |
| Speechiness   | Presence of spoken words |
| Valence       | Musical positiveness |

---

## ⚙ **Methodology**
1. **Exploratory Data Analysis (EDA)**:  
   - **Visualizing relationships** between variables.  
   - Identifying **patterns and correlations** in popularity.  

2. **Data Preprocessing**:  
   - Handling **missing values** and **duplicates**.  
   - **Removing outliers** using the **Z-score method**.  
   - **Feature normalization** for consistency.  

3. **Feature Selection**:  
   - Using **correlation matrices** to determine **important features**.  

4. **Model Selection & Training**:  
   - Comparing **Linear Regression, Decision Trees, Random Forest, KNN, and Logistic Regression**.  
   - Splitting the dataset into **training (70%) and testing (30%)**.  
   - Further splitting training data into **training (60%) and validation (40%)**.  

5. **Model Evaluation**:  
   - Evaluating models using **Mean Absolute Error (MAE), Mean Squared Error (MSE), and Adjusted R²**.  

---

## 📊 **Exploratory Data Analysis (EDA)**
- **Scatter plots** to identify correlations.  
- **Bar plots** showing **popularity of each genre**.  
- **Graph of artists vs. popularity** to track top-performing musicians.  

### 🔎 **Key Insights**
- Popularity is **highly correlated** with **loudness, energy, and danceability**.  
- Certain **genres** and **artists** tend to have more popular tracks.  
- The **distribution of audio features** can help **predict song popularity**.

---

## 🔢 **Clustering Analysis**
### 🔹 **Methods Used**
- **Single Linkage Method**
- **Average Linkage Method**
- **K-Means Clustering**

### 📌 **Cluster Observations**
| Cluster | Description |
|---------|-------------|
| **Cluster 0** | High danceability, high popularity, high tempo & positive mood |
| **Cluster 1** | High instrumentalness & acousticness, low valence (less positive mood) |
| **Cluster 2** | High acousticness, low energy |
| **Cluster 3** | High energy, short duration |
| **Cluster 4** | High speechiness & tempo (spoken-word tracks) |
| **Cluster 5** | Low danceability, high loudness & energy |

### 📈 **Elbow Method**
- Used to determine the **optimal number of clusters** for **K-Means**.
- Helped in **segmenting** songs into meaningful clusters.

---

## 🏆 **Model Performance**
We trained and tested **5 different machine learning models**:

| Model             | MSE  | RMSE | MAE  | Adjusted R² |
|------------------|------|------|------|-------------|
| **Random Forest** | **0.75** | **0.87** | **0.65** | **0.22** |
| Linear Regression | 1.25 | 1.12 | 0.82 | 0.18 |
| KNN              | 1.40 | 1.18 | 0.90 | 0.15 |
| Naïve Model      | 1.50 | 1.22 | 0.95 | 0.10 |
| Decision Tree    | 1.60 | 1.26 | 1.00 | 0.05 |

**✅ Random Forest performed the best!**  
- **Lowest MSE & RMSE**
- **Highest Adjusted R²**

---

## 🔍 **Key Findings**
1. **Loudness, energy, and danceability** are the strongest **predictors of song popularity**.  
2. **Random Forest** is the most **accurate model** for predicting song popularity.  
3. **Music producers** can use these insights to **optimize song characteristics** for better engagement.  
4. **Playlist curators** can use these factors to create **popular playlists**.

---

## 🚀 **Future Work**
- **Deep Learning Models**: Use **RNNs, Transformers** for better predictions.  
- **Real-time Streaming Data**: Integrate **live Spotify data** for continuous updates.  
- **Feature Engineering**: Extract additional **metadata** for enhanced analysis.  


