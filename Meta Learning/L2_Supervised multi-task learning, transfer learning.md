## [📔 L2_Supervised multi-task learning, transfer learning]

#### 'Task'?
> Definition: <img src="https://user-images.githubusercontent.com/33504288/124423334-dfd8d480-dd9f-11eb-862b-45f6ef9d8db6.png" width="200" height="30">
> > **p(x)**: input의 distribution, **p(y|x)**: x의 label distribution, **L**: loss

<br>

#### Multi-task classification vs. Multi-label learning
> - **Multi-task classification**: 모든 task의 loss function(**L**)이 같음 (e.g. per-language handwriting recognition)
> - **Multi-label learning**: 모든 task의 loss function(**L**)과 input data(**p(x)**)가 같음 (e.g. scene understanding)

> 그럼 loss function이 같은 경우는?
> <br>: 이산/연속 label이 섞여있을 때, 다른 task보다 특정 task 하나에 더 집중할 때

<br>

#### Task Descriptor
 <img src="https://user-images.githubusercontent.com/33504288/124550449-9e156000-de6b-11eb-8f9c-d46bb4e73b0e.png" width="480" height="220"> <img src="https://user-images.githubusercontent.com/33504288/124551325-eaad6b00-de6c-11eb-87a9-2fe201f71e0d.png" width="200" height="60">


> - Basic structure: input x와 **task descriptor인 Zi**가 같이 주어짐
> > **task descriptor**란?<br>
> > : 단순히 task index를 one-hot encoding한 것<br>
> > : 또는! **meta data**를 제공하는 것 (e.g. personalization(user features/attributes), language description of the task, formal specifications of the task)
> <br>
> 💡 자, 그럼 Multi-task learning에서 우리의 목표는 두 가지!<br>
> Q1. **task descriptor Zi**를 어떻게 정할 것인가?<br>
> Q2. **objective**를 어떻게 optimize할 것인가?

<br>

#### 
