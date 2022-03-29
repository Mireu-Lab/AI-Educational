### (Artificial Neural Network) 인공 뉴런 네트워크

이 네트워크는 인간의 뇌 뉴런 네트워크 망을 인공으로 구현한 네트워크입니다

이 네트워크을 이용해서 DNN, CNN, RNN을 구현할수있는 한계로는 CPP같은 네트워크 이죠

```
인간의 뇌에서 뉴런들이 어떤 신호, 자극 등을 받고, 그 자극이 어떠한 임계값(threshold)을 넘어서면 결과 신호를 전달하는 과정에서 착안한 것입니다.

여기서 들어온 자극, 신호는 인공신경망에서 Input Data이며 임계값은 가중치(weight), 자극에 의해 어떤 행동을 하는 것은 Output데이터에 비교하면 됩니다.

출처: https://ebbnflow.tistory.com/119 [삶은 확률의 구름]
```

이걸 요약하자면 뉴런하나에서 자극을 주면 그 아래에있는 뉴런들을 거처 결과을 내놓는 방식입니다

그걸 이미지화 한 사진이 아래와 같습니다

![https://blog.kakaocdn.net/dn/k3IEn/btqAm4ga7mA/eINomW58l6k5kUcPToScCK/img.jpg](https://blog.kakaocdn.net/dn/k3IEn/btqAm4ga7mA/eINomW58l6k5kUcPToScCK/img.jpg)

대신 ANN은 문제점이 아래와 같습니다

1. 학습과정에서 파라미터 즉 필터의 최적값을 찾기 어렵다.
2. Overfitting (과한 학습하는 뜻)에 따른 문제
3. 학습시간이 너무 느리다.