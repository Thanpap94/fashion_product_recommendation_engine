<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/papailth/fashion_product_recommendation_engine">
    <img src="https://studyingreece.edu.gr/wp-content/uploads/2021/06/AUEB_LOGO-PNG.png" alt="Logo" width="210" height="210">
        <img src="https://i.ibb.co/LSrQVQR/download.jpg" alt="Logo" width="180" height="180">
 </a>

<a name="readme-top"></a>
  <h3 align="center">Course: Machine Learning & Content Analytics</h3>
 <p align="center">
    Part Time 2022
    <br />
    <a href="https://e-mscba.dmst.aueb.gr/course/info.php?id=115&lang=en"><strong>Explore the Course »</strong></a>
    <br />
    <br />
    
<img align="center" alt="Saket Prag" width="1000px" src="https://i.ibb.co/vHQz0zh/Shop-The-Look-Project-8-26-2022.png" />






  <p align="center">
    <br />
    <a href="">Script</a>
    ·
    <a href="">Report</a>
    ·
    <a href="">Presentation</a>
  </p>
</div>



<!-- ABOUT THE PROJECT -->
## About The Project

**In [this](https://drive.google.com/drive/folders/1vsUGiCy1Ae86ntI-9MNcOAfl9ZYds24e?usp=sharing) Google Drive link you can find all the model weights and the dataset used for the implementation.**


<p align="center"  width="650px">
    <img width="90%" src="https://i.ibb.co/dgR09sy/shop-the-look-n-final.gif">
</p>


Every day, consumers waste a lot of time on searching for clothes, especially when they know exactly what they want. Since fashion is about the look – combining multiple items together – we thought it would be a great idea to give to users a faster tool to search outfits online, rather than typing multiple textual keywords in search engines. In our case, the adage “A picture is worth a thousand words” was valid, since the images were the “key” solution to our problem. Due to the fact that people are familiar with snaping pictures (e.g. for their social media) and also pictures contain a variety of information, we focused on providing an easy going solution to the users: “Snap and Shop”. We believe that our new tool will give many advantages for customers and online business too.</p>
Specifically, for customers the “Shop The Look” tool, will give a personalized user experience, with a fully automated process of matching products to scenes. Having an app which recognizes the clothes of a photo and search for similar products in online stores, will be more practical and time efficient. Secondly, by pointing out relevant alternatives based on what they are looking at, customers could be inspired and discover a much more bigger variety of similar outfits. Thirdly, many times users find they want, but they cant find where to find it online available. Giving that information instantly, will create more enjoyable customer journeys.</p>

For online fashion businesses, the new tool will increase conversion and basket size. When shoppers are better engaged with their brand and its personalized style suggestions, they will probably also increase the frequency of purchases. Secondly, enabling consumers to buy the entire look in the picture with one click, removes the pain of complex human processes and their maintenance. So, companies could save time and costs, from every party that is involved in apparel purchases. Thirdly, the companies can leverage huge amounts of data from users and create detailed reports (e.g. sales performance, user queries) and create personalized landing pages or campaigns.


<p align="right">(<a href="#readme-top">back to top</a>)</p>




<!-- A Fashion Product Recommendation Engine -->
## A Fashion Product Recommendation Engine


<p align="center"  width="650px">
    <img width="90%" src="https://i.ibb.co/VM8qkHR/Capture22.png">
</p>



**[The model weights and the dataset used for the implementation](https://drive.google.com/drive/folders/1vsUGiCy1Ae86ntI-9MNcOAfl9ZYds24e?usp=sharing) :**

### Model weights:
1. **Gender Classification**
   - `gender_classification_model.h5`
   
   <p align="center"  width="650px">
    <img width="90%" src="https://i.ibb.co/cD7fRyR/train22.gif">
</p>
   
2. **Object Detection** 
   - `object_detection.pt`
   
      <p align="center"  width="650px">
    <img width="90%" src="https://i.ibb.co/Z29ZynV/YOLO.png">
</p>
   
   
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
-  The embedding generation model is trained using [this github repo](https://github.com/kang205/STL-Dataset) and the training data are extracted into STL-Dataset/embeddings_train_data inside Google Drive  


**In order to run the Jupyter notebook in Google Colab, you should first upload the [Google Drive folder](https://drive.google.com/drive/folders/1vsUGiCy1Ae86ntI-9MNcOAfl9ZYds24e?usp=sharing) to your drive and load the Drive into the Colab environment, using the following:**
   ```
   from google.colab import drive
   drive.mount('/content/drive')
   ```
