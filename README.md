본 저장소는 패스트캠퍼스 Coding the Mathematics 강의에 필요한 소스코드 및 필요한 자료를 업로드하기 위한 저장소입니다. Coding the Mathematics 수업은 
저장소에는 크게 3개의 디렉토리가 있습니다. 

1. curriculum 

본 강의의 커리큘럼과 필요한 선수지식에 대한 내용이 들어 있습니다. 

1.1 syllabus - mathematics2.pdf 

본 강의의 실라버스입니다. 대략적인 강의 스케쥴과 소개가 나와 있습니다. 

1.2 pre-req

본 강의에서 필요한 선수지식을 자체적으로 테스트하기 위한 문제가 들어 있습니다. 문제는 각각 pre-req1.py, pre-req2.py에 들어 있으며, 답은 solution1.py, solution2.py에 들어 있습니다. 
pre-req1.py는 수강에 필요한 최소한의 필요지식을, pre-req2.py는 수강하는데 충분한 지식을 테스트하는 문제입니다. 

pre-req1.py에는 두 문제가 있습니다. 

- look-and-say 수열 
look-and-say 수열은 한국에서는 베르나르 베르베르의 소설 '개미'에서 나온 것으로 유명합니다. 이 수열은 다음과 같이 만들어집니다. 

1번째 항 : 1 
2번째 항 : 전 항에 '1'개의 '1'이 있었으므로 11 
3번째 항 : 전 항에 '2'개의 '1'이 있었으므로 21 
4번째 항 : 전 항에 '1'개의 '2', '1'개의 '1'이 있었으므로 1211

이런 식으로 진행됩니다. 본 문제에서는 초항이 first_element일 때, n번째 look-and-say 수열을 출력하는 함수 look_and_say를 구현하시면 됩니다. 위키피디아(https://ko.wikipedia.org/wiki/%EC%9D%BD%EA%B3%A0_%EB%A7%90%ED%95%98%EA%B8%B0_%EC%88%98%EC%97%B4)를 참고하시면 문제 이해에 도움이 될 것입니다. 

- 하노이의 탑 
하노이의 탑은 재귀를 공부하기 위한 전통적인 예시입니다. 고대 인도 베나레스에 있는 한 사원에는 다이아몬드로 이루어진 3개의 기둥이 있고, 그 기둥 중 하나에 가운데에 구멍이 나 기둥에 끼울 수 있게 된 n개의 크기가 각각 다른 황금 원반이 꽂혀 있다고 합니다. 황금 원반은 가장 아래쪽에 있는 것이 가장 크고 위로 갈수록 점차 작아져 전체적으로 원추형의 탑을 이루고 있는데, 원반은 한번에 하나씩만 옮길 수 있으며 작은 원반 위에 그보다 더 큰 원반을 옮길 수 없습니다. 이 때, 처음 놓여있던 기둥에서 다른 기둥으로 모든 원반을 옮기는 방법을 출력하면 됩니다. 

나무위키(https://namu.wiki/w/%ED%95%98%EB%85%B8%EC%9D%B4%EC%9D%98%20%ED%83%91)를 참고하시면 문제 이해에 도움이 될 것입니다. 답안이 나와 있으므로 문제를 푸신 후에 보는 것을 권장드립니다. 

pre-req1.py에 있는 문제는 본 강의를 수강하기 위해서 필수적으로 요구되는 코딩 기술을 테스트하는 문제로, 적어도 solution1.py에 있는 답안을 이해할 수 있어야 본 수업 수강에 무리가 없을 것입니다. 
해답을 이해하기 어렵다면 재귀(recursion)이나 파이썬 문법에 대해서 공부하신 후 수강할 것을 권장드립니다. 

pre-req2.py에는 한 문제가 있습니다. 
- 수식 parser 만들기 
수식에는 사칙연산과 지수연산(^), 그리고 괄호가 포함됩니다. 일반적인 연산에 준해서 계산할 수 있게 calculate 함수를 작성하면 됩니다. 테스트로 33개의 예제가 주어져 있습니다만, 필요한 경우 예제를 더 만드셔도 좋습니다. 기본적으로는 파이썬의 수식 문법을 따라가지만, 몇몇 예제에서는 편의를 위해서 파이썬의 수식과 조금 다릅니다. 예를 들어서 eq30의 경우, 파이썬에서는 불가능한 문법이지만('3*(2*2+1)'이 맞는 문법이며, 저 문법의 경우 3이라는 함수에 (2*2+1)을 대입하는 것으로 인식하므로 TypeError가 납니다.) 일반적으로 수식에서 곱셈의 경우 제외하는 경우가 많으므로 저렇게 쓰는 것을 허용하도록 하였습니다. 

본 문제는 있는 문제는 정해진 답이 없는 open problem으로, 꼭 solution2.py에 있는 방법대로 풀 필요는 없으며 solution2.py에 있는 방법은 하나의 방법일 뿐입니다. 스택을 이용한 풀이가 일반적이므로 궁금하시다면 이를 검색해 보는 것을 추천드립니다. 

2. documentation 

본 강의에서 설명할 개념에 대한 교재입니다. LaTeX 코드와 pdf가 같이 올라갈 예정입니다. 

3. src

구현된 pymath 모듈과 스켈레톤, 그리고 실습의 소스코드가 있는 디렉토리입니다. 

3.1 pymath 

주로 구현할 모듈이 있는 디렉토리입니다. 집합, 벡터/행렬/텐서, 함수, 방정식, 극한/미분/적분, 확률분포 등을 여기서 구현합니다. 

3.2 skeleton 

수강하실 때 클론하여 실습할 수 있도록 만든 스켈레톤 코드입니다. 빈 부분을 채우시면서 테스트하고, 실습할 수 있도록 구성하였습니다. 

3.3 recitation 

실습에서 쓸 데이터와 코드가 있는 디렉토리입니다. 




오타나 에러, 적절하지 못한 구현에 대한 조언은 principia_12@kaist.ac.kr로 메일 보내주시면 감사하겠습니다. 

