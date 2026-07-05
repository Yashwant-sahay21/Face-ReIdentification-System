# Face Re-Identification System

An end-to-end **Face Re-Identification System** that automatically groups images of the same individual captured under different lighting conditions, camera angles, and facial expressions.

The project uses **MTCNN** for face detection, **FaceNet** for feature extraction, and **DBSCAN** for unsupervised clustering, producing confidence scores and comprehensive reports.

---

## Features

- Face Detection using MTCNN
- Face Embedding using FaceNet (512-dimensional embeddings)
- Identity Clustering using DBSCAN
- Cosine Similarity Analysis
- Confidence Score Generation
- Cluster Visualization
- Similarity Matrix Heatmap
- CSV Report Generation
- Automatic Output Organization

---

## Project Pipeline

```
Input Images
      │
      ▼
Face Detection (MTCNN)
      │
      ▼
Face Alignment & Cropping
      │
      ▼
Face Embeddings (FaceNet)
      │
      ▼
Cosine Similarity
      │
      ▼
DBSCAN Clustering
      │
      ▼
Confidence Score Calculation
      │
      ▼
Clustered Images + Reports + Visualizations
```

---

## Technologies Used

- Python 3.11
- PyTorch
- facenet-pytorch
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Pillow
- tqdm

---

## Folder Structure

```
Face-ReIdentification-System/
│
├── data/
│   └── person_identification/
│
├── notebook/
│   └── Face_ReIdentification.ipynb
│
├── output/
│   ├── clusters/
│   ├── reports/
│   └── visualization/
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Dataset

Total Images : 6

Clusters Found : 3

Embedding Model : FaceNet

Clustering : DBSCAN

Similarity Metric : Cosine Similarity

Average Confidence

85.48%
---



## Installation

Clone the repository:

```bash
git clone https://github.com/Yashwant-sahay21/Face-ReIdentification-System.git
```

Move into the project folder:

```bash
cd Face-ReIdentification-System
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Usage

1. Place the dataset inside:

```
data/person_identification/
```

2. Open the notebook:

```
notebook/Face_ReIdentification.ipynb
```

3. Run all notebook cells sequentially.

---

## Output

The system generates:

- Clustered images
- Face embeddings
- Similarity matrix
- Confidence scores
- CSV report
- Cluster summary
- Visualizations

---

## Results

- Successfully groups images belonging to the same individual.
- Robust against pose, lighting, and facial expression variations.
- Produces confidence scores for each identified image.
- Automatically exports reports and clustered outputs.

---

## Future Improvements

- ArcFace embeddings
- FAISS for large-scale similarity search
- Real-time face re-identification
- Video-based person tracking
- Web application using FastAPI or Streamlit

---

## Author

**Yashwant Sahay**

GitHub: https://github.com/Yashwant-sahay21

---

## License

This project is intended for educational and assessment purposes.

