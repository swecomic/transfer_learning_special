# Continuous Learning

Continuous Learning의 주요 요소인 Feature Extraction, Finetuning, Knowledge Distillation(KD), Learning Without Forgetting(LWF)기법으로 cifiar10 성능 실험결과에 대해서 다룬다. 코드는 Pytorch 기반으로 작성 되었다.

## 개념
Continuous Learning은 널리 알려진 Transfer learning의 상위 개념이라고 이해하면 된다. Transfer learning은 주로 기존 잘 훌련된 pre-trained network를 가져와 new task에 일부 레이어를 finetuning 하는 방식인데, 이 경우 original task에 대한 성능은 저하된다. 그 이유는, new task에 모델이 다시 fitting 되었기 때문이다.
본 실험에서는 편의를 위해 Teacher Network(Pre-trained)로 VGG16 모델을 사용하였고, Student Network은 VGG16보다 얕은 layer와 channel를 가진 모델을 임의로 생성을 하였다. 모델에 대한 코드는 model.py에서 확인 가능하다.

1. Feature Extraction

2. Finetuning

3. Knowledge Distillation(KD) 

4. Learning Without Forgetting(LWF)


