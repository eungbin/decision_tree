# decision_tree
decision_tree with sklearn

Root_node - Intermediate node - Terminal/Leaf node

가지치기(Pruning) => Overfitting을 막기 위한 전략
트리에 가지가 너무 많을 경우 오버피팅이라 볼 수 있음
최대 깊이, 터미널 노드의 최대 개수, 한 노드가 분할하기 위한 최소 데이터의 수 제한

불순도(Impurity) => 해당 범주 안에 서로 다른 데이터가 얼마나 섞여있는지
결정트리는 불순도를 최소화하는 방향으로 학습을 진행

엔트로피(Entropy) => 불순도를 수치적으로 나타낸 척도

정보획득(Information gain) => 분기 이전의 엔트로피에서 분기 이후의 엔트로피를 뺀 수치
Information gain = entropy(parent) - [weighted average]entropy(children)
결정트리 알고리즘은 정보 획득을 최대화하는 방향으로 학습을 진행한다.