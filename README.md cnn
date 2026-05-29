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

