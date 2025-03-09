# 🎯 Battle Game Result Prediction using Heterogeneous Graph
### 📌 프로젝트 개요
본 프로젝트는 Graph Mining 기법을 활용하여 멀티플레이어 배틀 게임의 승패 및 점수를 예측하는 프로젝트입니다.
특히 승패 여부(Task 1) 와 점수 예측(Task 2) 두 가지 문제를 해결하는 것이 목표였습니다.

#### 🏆 Task 1: 승리 예측
🔹 방법론
- 이종 그래프 생성: 게임과 플레이어를 노드로 하는 그래프 구축
- GraphSAGE 모델 학습: 그래프 구조를 활용한 예측
- PageRank & 평균 점수 활용: 노드 중요도를 반영하여 성능 향상
  
📊 결과 (Validation Accuracy)
| Method                             | Accuracy (%) |
|------------------------------------|-------------|
| Random                             | 50.48       |
| Counting                           | 67.33       |
| **Heterogeneous Graph + GraphSAGE** | **79.70**   |

#### 🏆 Task 2: 점수 예측
🔹 방법론
- 이종 그래프 생성 (Task 1과 동일)
- GraphSAGE 학습
- PageRank & 평균 점수 적용

📊 결과 (Validation Accuracy)
| Method                             | Accuracy (%) |
|------------------------------------|-------------|
| Random                             | 50.48       |
| Average Score                      | 80.08       |
| PageRank & Average Score*          | 84.55       |
| **Heterogeneous Graph + GraphSAGE** | **86.79**   |

#### 🚀 결론 및 성과
- GraphSAGE 기반 이종 그래프 모델이 기존 방법 대비 우수한 성능을 보임
- 승리 예측(Task 1): 79.70%, 점수 예측(Task 2): 86.79%
- PageRank와 평균 점수를 함께 사용할 경우 예측 성능이 향상됨
- **최우수 프로젝트 선정(1팀)**
