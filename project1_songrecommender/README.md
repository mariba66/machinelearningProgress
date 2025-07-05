#  Song Recommendation System

This is a simple content-based recommendation system built using TF-IDF and cosine similarity.

##  What It Does

- You input a song name (e.g., "My Little One")
- The system finds and recommends similar songs based on lyrics/text
- Uses cosine similarity on TF-IDF vectors

## 🛠 Tools & Libraries

- Python 
- scikit-learn
- pandas
- Google Colab
## Dataset

The song lyrics dataset used in this project was downloaded from **Kaggle** using the Kaggle API.

- 📦 Dataset: [Song Lyrics Dataset](https://www.kaggle.com/datasets/yamaerenay/spotify-dataset-19212020-160k-tracks)  
  *(Or replace with your actual dataset link)*

### 🔽 How to Download via Kaggle API (on Colab)

To download the dataset in Google Colab using the Kaggle API:

1. Upload your `kaggle.json` API token to Colab:
   - You can get this from your Kaggle profile under **"API Token"**.
2. Then run this code in a Colab cell:

```python
# Step 1: Install Kaggle
!pip install kaggle

# Step 2: Upload kaggle.json (do this manually in Colab)
from google.colab import files
files.upload()  # upload kaggle.json

# Step 3: Move it to the correct location
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json

# Step 4: Download the dataset
!kaggle datasets download -d <dataset-id>

# Step 5: Unzip it
!unzip <downloaded-zip-file>.zip


## 🎯 What I Learned

- How content-based recommendation systems work
- How to apply TF-IDF vectorization to song lyrics
- How to use cosine similarity for similarity scoring
- Organizing a notebook project and uploading to GitHub

## 📺 Source Credit

This project was inspired by a tutorial from **Siddhardhan** on YouTube.  
[Watch it here](https://www.youtube.com/watch?v=ic1tlRD0VoE&list=PLfFghEzKVmjvII5ZcBnFWQOUjtUVdDnmo&index=6&pp=iAQB0gcJCcEJAYcqIYzv))

## 🔗 How to Run

1. Clone the repo or open the notebook in Google Colab
2. Run all cells
3. Try searching for a song in the dataset

---

 This is my first ML mini-project! 
