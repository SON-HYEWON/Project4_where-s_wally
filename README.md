# 🔍 Where's Wally? with U-Net
`Image Segmentation`을 통해 Wally의 위치를 찾아내고,  
새로운 이미지가 들어와도 Wally를 찾아낼 수 있는 `U-Net Model`을 구축하였습니다.

## 1. DataSet
[해당 링크](https://www.kaggle.com/kairess/find-waldo)의 데이터 셋을 사용했습니다.  

데이터 셋은 다음과 같이 분류되어 있습니다.
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
모델 평가 결과, 0.99의 높은 정확도를 확인할 수 있었습니다.  

새로운 이미지가 들어왔을 때에도 모델은 Wally를 성공적으로 찾아내었습니다!

## 4. 프로젝트 정리
- [프로젝트 발표자료 링크](https://github.com/hyewonsonn/Project4_where-s_wally/blob/main/AI_02_%E1%84%89%E1%85%A9%E1%86%AB%E1%84%92%E1%85%A8%E1%84%8B%E1%85%AF%E1%86%AB_Section4(%E1%84%89%E1%85%AE%E1%84%8C%E1%85%A5%E1%86%BC).pdf)
- [프로젝트 발표 영상 링크](https://youtu.be/kNREu3zikb4)

## 5. Reference
* https://github.com/bckenstler/TheresWaldo
* https://www.flickr.com/photos/153621475@N06/albums/72157684946674930/with/36420949126/
* https://www.kaggle.com/kairess/find-waldo
