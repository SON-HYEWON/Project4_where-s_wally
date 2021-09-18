# 🔍 Where's Wally? with U-Net
`Image Segmentation`을 통해 Wally의 위치를 찾아내고, 
새로운 이미지가 들어와도 Wally를 찾아낼 수 있는 `U-Net Model`을 구축하였습니다.

## 1. DataSet
[해당 링크](https://www.kaggle.com/kairess/find-waldo)의 데이터 셋을 사용했습니다. 이 데이터 셋은 다음과 같이 분류되어 있습니다.

* imgs_uint8 : 전체 이미지
* labels_uint8 : wally가 있는 위치는 1, 그 외는 0으로 표시 된 마스킹 이미지
* waldo_sub_imgs_uint8 : wally가 있는 부분이 확대된 이미지
* waldo_sub_labels_uint8 : wally가 있는 위치는 1, 그 외는 0으로 표시 된 확대 마스킹 이미지

## 2. Model Structure
<img width="400" alt="image" src="https://user-images.githubusercontent.com/75603262/124211042-6df65600-db27-11eb-9dcb-11dc8cd0aac1.png">  
적은 수의 데이터를 가지고도 정확한 이미지 분류를 수행하는 U-Net Model을 사용했습니다.  

[이미지 출처](https://medium.com/@msmapark2/u-net-%EB%85%BC%EB%AC%B8-%EB%A6%AC%EB%B7%B0-u-net-convolutional-networks-for-biomedical-image-segmentation-456d6901b28a)

## 3. Demo
<img width="500" alt="demo" src="https://user-images.githubusercontent.com/75603262/124211573-4b187180-db28-11eb-9e7e-14ad13cc475b.png">

## 4. Reference
* https://github.com/bckenstler/TheresWaldo
* https://www.flickr.com/photos/153621475@N06/albums/72157684946674930/with/36420949126/
* https://www.kaggle.com/kairess/find-waldo
