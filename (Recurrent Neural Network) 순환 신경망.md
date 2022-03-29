### (Recurrent Neural Network) 순환 신경망

RNN 네트워크는 반복적이고 순차적인 데이터 학습에 특화된 모델입니다

한마디로 반복이 될수있는 데이터을 학습할수있는 모델입니다

예시로 NLP(자연어 처리)나 아니면 오디오에서 음성을 파악하는곳에서 사용하게 됩니다

RNN을 이미지로 표현했을때 아래와 같습니다

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/21f627e3-d6cf-49dd-882f-b7bfb3c722a8/Untitled.png)

RNN는 이렇게 구성이 되어있습니다

RNN은 X라는 데이터 값이 들어가면 H로 내보내는데 A를 둘러싼 반복은 다음 단계의 정보을 해석을 한다는것이다

그 문제을 이미지로 표현했을때는 아래와 같이 나옵니다

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/db2b8701-1192-466c-ae8d-60db4f7dce78/Untitled.png)

처음에 나왔던 이미지는 이렇게 풀어서 설명할수있습니다

 X에서 데이터값을 불러오고 H로 나가는데 텍스트나 아니면 오디오 인경우에서는 하나의 단어로 끝나는게 아니므로 이렇게 반복으로 표현하게 됐습니다

모든 RNN은 neural network 모듈을 반복시키는 체인과 같은 형태를 하고 있다. 

기본적인 RNN에서 이렇게 반복되는 모듈은 굉장히 단순한 구조를 가지고 있습니다.

우리가 X에다가 “Hello, World”라고 전송하게 되면

RNN에서는

```jsx
“Hello”, ”,”,  “World”
```

이렇게 짤라서 나오게 됩니다

이렇게 나온 데이터 결과 값은 H에 나오게 됩니다

RNN에서는 LSTM, GRU라는 필터을 이용해서 심층 분석을 합니다

### LSTM

LSTM Network은 긴 의존기간을 필요하는 학습에 사용됩니다