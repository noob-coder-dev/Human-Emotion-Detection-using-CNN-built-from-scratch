# Human Emotion Detection using CNN built from scratch
![image](https://user-images.githubusercontent.com/66888595/120300904-fea00300-c2e9-11eb-843e-22b240cffc9c.png)![image](https://user-images.githubusercontent.com/66888595/120300994-11b2d300-c2ea-11eb-9592-5b2e672bac76.png)![image](https://user-images.githubusercontent.com/66888595/120301028-18414a80-c2ea-11eb-8e4f-7d7bc05b113a.png)![image](https://user-images.githubusercontent.com/66888595/120301051-1f685880-c2ea-11eb-826c-4734e2b7c50c.png)![image](https://user-images.githubusercontent.com/66888595/120301086-268f6680-c2ea-11eb-8635-39af9b264645.png)![image](https://user-images.githubusercontent.com/66888595/120301111-2b541a80-c2ea-11eb-8ceb-520283b17acd.png)



## Table of Content
<ul>
  <li>
    <a href="#overview">
      <span>
      1. Overview
      </span>
    </a>
  </li>
  <li>
      <a href="#data">
        <span>
        2. Dataset
        </span>
      </a>
    </li>
    <li>
    <a href="#motivation">
      <span>
      3. Motivation
      </span>
    </a>
   </li>
   <li>
    <a href="#aspects">
      <span>
      4. Technical Aspects
      </span>
    </a>
   </li>



</ul>

<h3>
  <span id="overview">Overview</span>
</h3>

> The model, `model_2.h5`, built on the dataset, `FER-2013`, predicts the human face emotion with a 52.43%.

<h3>
  <span id="data">Dataset</span>
</h3>

> This dataset is known as FER-2013(Face Emotion Recognition). It's a public dataset, can be downloaded by clicking this <a href="https://www.kaggle.com/msambare/fer2013"> dataset link</a>. This dataset contains 3 human emotional class, though in real life the number should be more!


<h3>
  <span id="motivation">Motivation</span>
</h3>

> This project is nothing but a foundation of the project of Real Human Emotion Project using OpenCV.

<h3>
  <span id="aspects">Technical Aspects</span>
</h3>

> The following are the technical info. related to this project:<br>1. The dataset, used in this project, is FER-2013. That's publicly available in Kaggle(link provided in the Dataset section).<br>2. Next, the dataset has been taken from the drive, where the dataset is saved, generates batches(batch size=32) of augmented data with color_code="greyscale", target_size=(48,48), with class_code as "categorichal".<br>3. This sequential model contains 17 layers(`Conv2D`,`MaxPool2D`,`Dense`,`Dropout`,`Flatten`). The total number of trainable features is 167,239.<br>4. The model is trained over 60 epochs. After 6th epoch, the validation accuarcy is 52.43% and training accuracy is 54.22%. Obviously this models requires more work on it.<br>5. A curve is provided as follows:<br>![image](https://user-images.githubusercontent.com/66888595/120334588-610afa80-c30e-11eb-9a82-8cd115b3a76d.png)<br>6. Next for manual inspection, some images are being chosen to predict. Out of 7 such examples, this predicted 3 of them correctly!


