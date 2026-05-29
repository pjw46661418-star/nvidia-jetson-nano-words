# nvidia-jetson-nano-words
# Convolutional Neural Network (CNN)

## 1. What is CNN?

Convolutional Neural Network (CNN)은 이미지 처리와 분류에 특화된 딥러닝 모델이다.

CNN은 Artificial Neural Network(ANN)의 한 종류이며,
Convolution Layer(합성곱 계층)를 사용하여 이미지의 중요한 특징을 추출한다.

주로 사용되는 분야:

* Image Classification
* Object Detection
* Face Recognition
* Medical Imaging
* Autonomous Driving

---

# 2. Artificial Neural Network (ANN)

Artificial Neural Network(ANN)는 인간의 뇌 신경망 구조를 모방한 계산 모델이다.

신경망은:

1. 입력값(Input)
2. 가중치(Weight)
3. 활성화 함수(Activation Function)

를 사용하여 데이터를 변환한다.

각 Layer의 출력은 다음 Layer의 입력으로 전달된다.

반복적인 학습을 통해:

* Edge
* Shape
* Pattern

과 같은 특징을 학습한다.

---

# 3. Convolution Operation

CNN의 핵심 연산은 Convolution(합성곱)이다.

Convolution은:

* 입력 이미지(Input Image)
* Filter(Kernel)

를 결합하여 새로운 Feature Map을 생성한다.

```text id="dxp7xv"
Input Image + Filter → Feature Map
```

---

# 4. Convolution Layer

Convolution Layer는 이미지의 중요한 특징을 추출한다.

예시:

* Edge
* Corner
* Texture
* Shape

필터(Filter)는 이미지 위를 이동하면서 계산을 수행한다.

예를 들어:

* 5×5 Filter
* 3×3 Filter

등이 자주 사용된다.

---

# 5. Feature Map

Convolution 결과 생성되는 출력 데이터를 Feature Map이라고 한다.

Feature Map은:

* 특정 패턴
* 특정 특징

이 얼마나 강하게 존재하는지를 나타낸다.

---

# 6. Pooling Layer

Pooling은 Feature Map의 크기를 줄이는 과정이다.

대표적으로:

* Max Pooling
* Average Pooling

이 사용된다.

---

## Max Pooling

가장 큰 값만 선택하여 중요한 특징만 유지한다.

### Advantages

* 계산량 감소
* Overfitting 감소
* 중요한 특징 유지

---

# 7. Fully Connected Layer

CNN 마지막 단계에서는 Fully Connected Layer를 사용한다.

모든 특징 정보를 결합하여 최종 분류를 수행한다.

예시:

* Cat
* Dog
* Traffic Sign

등의 클래스를 예측한다.

---

# 8. CNN Structure

일반적인 CNN 구조:

```text id="3pwf8s"
Input Image
    ↓
Convolution Layer
    ↓
Activation Function (ReLU)
    ↓
Pooling Layer
    ↓
Fully Connected Layer
    ↓
Output
```

---

# 9. CNN Learning

CNN은 학습을 통해 자동으로 중요한 특징을 찾는다.

예시:

* 일반 물체 인식 → Shape 정보 중요
* 새(Bird) 분류 → Color 정보 중요

훈련 데이터에 따라 필요한 특징을 자동으로 학습한다.

---

# 10. Why CNN is Powerful

CNN은 이미지의 공간적 특징을 매우 효과적으로 학습할 수 있다.

### Advantages

* 이미지 특징 자동 추출
* 높은 정확도
* Parameter 공유로 효율적 학습
* 이미지 처리에 최적화

---

# 11. GPU Acceleration

CNN은 매우 많은 연산을 필요로 한다.

특히:

* 대규모 이미지 데이터
* 수백만 개 파라미터
* 반복적인 학습

때문에 GPU 사용이 필수적이다.

GPU는 병렬 연산을 통해:

* Training 속도 향상
* Inference 속도 향상

을 제공한다.

---

# 12. Deep Learning Frameworks

대표적인 딥러닝 프레임워크:

| Framework  | Description       |
| ---------- | ----------------- |
| TensorFlow | Google의 딥러닝 프레임워크 |
| PyTorch    | Meta의 딥러닝 프레임워크   |
| Caffe      | 이미지 처리 중심 프레임워크   |

---

# 13. CNN Applications

CNN은 다양한 분야에서 사용된다.

### Applications

* Self-Driving Car
* Face Recognition
* Medical Diagnosis
* OCR
* Security System
* Image Search

---

# 14. Summary

* CNN은 이미지 처리에 특화된 딥러닝 모델이다.
* Convolution Layer를 사용하여 특징을 추출한다.
* Pooling은 Feature Map 크기를 줄인다.
* Fully Connected Layer가 최종 분류를 수행한다.
* GPU는 CNN 학습 속도를 크게 향상시킨다.
* CNN은 현대 컴퓨터 비전의 핵심 기술이다.

---

# References

* Deep Learning - Ian Goodfellow
* Stanford CS231n
* TensorFlow Documentation
* PyTorch Documentation
* NVIDIA Deep Learning Docs








​1. 핵심 개념 용어
​컴퓨터 비전 (Computer Vision): 컴퓨터가 사람처럼 이미지나 영상을 보고, 그것이 무엇인지 '이해하고 해석'하게 만드는 기술입니다.
​일반화 (Generalize): 훈련할 때 보지 못했던 새로운 데이터(예: 다른 각도, 다른 배경의 엄지손가락)가 들어와도 정확하게 정답을 맞히는 능력을 말합니다. AI의 성능을 평가하는 가장 중요한 기준 중 하나입니다.
​2. AI의 두 가지 단계
​AI 프로젝트는 크게 '공부하는 단계'와 '시험을 치는 단계'로 나뉩니다.
​훈련 / 학습 (Train): AI에게 문제(이미지)와 정답(레이블)을 주며 공부를 시키는 과정입니다. 틀리면 정답을 맞힐 때까지 반복해서 학습합니다.
​추론 (Inference): 학습을 마친 AI 모델을 현장(실시간 카메라 등)에 배치하여, 새로운 데이터를 입력받았을 때 실시간으로 정답을 예측(판단)하는 과정입니다.
​3. 모델의 내부 구성 요소
​파라미터 / 가중치 (Parameter / Weight): AI의 두뇌 세포들 사이에 연결된 '회로의 조절 나사' 같은 것입니다. 처음에는 이 나사들이 엉망으로 조여져 있어서 틀린 답을 내지만, 학습을 거듭할수록 정답을 맞히도록 정교하게 조여집니다.
​범주 / 클래스 (Category / Class): AI가 분류해야 하는 **'정답의 선택지'**입니다. 예를 들어 '행복', '슬픔' 두 가지만 맞히는 모델이라면 클래스는 2개가 됩니다.
​4. 학습 과정 관련 용어
​노이지한 (Noisy): 데이터에 섞여 있는 **'불필요한 방해 요소'**들을 뜻합니다. 엄지손가락을 찍었는데 배경에 지나가는 고양이나 어두운 조명이 찍혔다면, 이는 AI 학습을 방해하는 '노이즈'가 됩니다.
​에포크 (Epoch): 준비한 **전체 데이터세트를 AI가 처음부터 끝까지 '한 번 다 공부한 횟수'**를 뜻합니다. "10 에포크를 돌렸다"는 것은 교과서를 처음부터 끝까지 총 10번 반복해서 정독했다는 의미입니다.
