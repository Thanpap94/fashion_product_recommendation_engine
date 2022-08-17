# Fashion product recommendation engine


![Screenshot 2022-06-23 154847](https://user-images.githubusercontent.com/97535586/185087096-c3983acb-7b01-402e-9cce-c59a8d2b65d8.png)


**In [this](https://drive.google.com/drive/folders/1vsUGiCy1Ae86ntI-9MNcOAfl9ZYds24e?usp=sharing) Google Drive link you can find all the model weights and the dataset used for the implementation.**


### Model weights:
1. **Gender Classification**
   - `gender_classification_model.h5`
   
2. **Object Detection** 
   - `object_detection.pt`
   
3. **Embeddings** 
   - `topwear_embedding.h5`
   - `bottomwear_embedding.h5`
   - `footwear_embedding.h5`
   
 ### Embeddings datasets:
 
 The dataset used to generate the embeddings, consisting of fashion products to recommend is saved in `skroutz_images.zip` and `skroutz_images.csv`.
 The embeddings for the catalog/database, are saved in the following CSVs:
 
- `mens_topwear_embeddings.csv`
- `mens_bottomwear_embeddings.csv`
- `mens_footwear_embeddings.csv`
- `womens_topwear_embeddings.csv`
- `womens_bottomwear_embeddings.csv`
- `womens_footwear_embeddings.csv`
   
### Training datasets:

- `gender_classification_dataset.zip` contains the dataset used for the gender classification model
-  [This](https://universe.roboflow.com/new-workspace-w4orl/fashion_obj_detection/browse) Roboflow dataset is used to train the Object Detection YOLOv5 model
-  The embedding generation model is trained using [this gituhub repo](https://github.com/kang205/STL-Dataset) and the training data are extracted into STL-Dataset/embeddings_train_data inside Google Drive  


**In order to run the Jupyter notebook in Google Colab, you should first upload the [Google Drive folder](https://drive.google.com/drive/folders/1vsUGiCy1Ae86ntI-9MNcOAfl9ZYds24e?usp=sharing) to your drive and load the Drive into the Colab environment, using the following:**
   ```
   from google.colab import drive
   drive.mount('/content/drive')
   ```
