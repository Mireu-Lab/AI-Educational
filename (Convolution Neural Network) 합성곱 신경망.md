### (Convolution Neural Network) 합성곱 신경망

CNN신경망은 데이터의 특징을 추출해서 특징의 패턴을 파악하는 구조로 되어있는 모델입니다

해당 네트워크는 이미지의 픽셀 단위로 뜯어 맛보는 미친 모델입니다

CNN을 사진으로 구현했을때 아래와 같습니다

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/49a6eb32-16d7-45ff-9af6-fb1d79d0a009/Untitled.png)

네트워크는 Convolution필터, Pooling필터을 이용해서 머신러닝을 진행합니다

### **Convolution**

**Convolution은 이미지에있는 픽셀을 뜯어 또하나의 곱으로 만드는 필터 입니다**

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9a6ba828-fb30-4684-b2e1-b16a463a9148/Untitled.png)

```jsx
데이터의 특징을 추출하는 과정으로 데이터에 각 성분의 인접 성분들을 조사해 특징을 파악하고 
파악한 특징을 한장으로 도출시키는 과정이다. 

여기서 도출된 장을 Convolution Layer라고 한다. 
이 과정은 하나의 압축 과정이며 파라미터의갯수를 효과적으로 줄여주는 역할을 합니다.

출처: https://ebbnflow.tistory.com/119 [삶은 확률의 구름]
```

해당 뜻은 각 픽셀마다 성분들을 조사해서 특징을 분석하고 그 분석한걸 한장으로 변환 하는 방식이다

### **Pooling**

Pooling은 Convolution에서 나온 데이터값을 더 줄어주는 과정을 해주는 필터입니다

```jsx
이는 Convolution 과정을 거친 레이어의 사이즈를 줄여주는 과정입니다.
단순히 데이터의 사이즈를 줄여주고, 노이즈를 상쇄시키고 미세한 부분에서 일관적인 특징을 제공합니다.

출처: https://ebbnflow.tistory.com/119 [삶은 확률의 구름]
```

해당 말의뜻은 이미지에있는 노이즈을 상쇄시키는 필터입니다

이제 보통 CNN는 이미지 분류, 분석, 문장 분류등에서 영상 이미지 처리 부분쪽에서 많이 사용하고있습니다