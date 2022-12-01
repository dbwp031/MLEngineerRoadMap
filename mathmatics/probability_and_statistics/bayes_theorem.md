# Bayes Theorem

## 순서

# 베이스 설명 케이스
## 영상 설명 기준 [링크](https://www.youtube.com/watch?time_continue=9&v=HZGCoVF3YvM&feature=emb_logo)
* 전세계에 #사서:#농부 = 1:20 (라는 통계 혹은 사실이 주어져있다고 하자.)
### Case 1
* steve가 있다. 사서일까? 농부일까?
  * H: steve는 사서다.
  * $P(H)=\frac{1}{20}$, 사전 확률
### Case 2
* steve가 있다. steve는 소심하다. 사서일까? 농부일까?
  * H: steve는 사서이다.
  * E: steve는 소심하다.
  * 사서 중 소심한 사람 40%, 농부 중 소심한 사람 10% 일꺼라는 **주어진 조건 (혹은 사실, 혹은 빅데이터를 통한 통계, 즉 이미 알고 있는 정보)**
  * $P(H|E)=\frac{P(H\cap E) \text{-> 소심한 사람 중 사서인 사람}}{P(E)\text{-> 소심한 사람}} = \frac{1 * 0.4}{1 * 0.4 + 20 * 0.6}$ 
  * 관측값이 주어졌을 때의 확률 (조건부 확률): 우도liklihood
  * 따라서 만약에 최고값으로 판단해야 한다면 Max Liklihood 혹은 Max A Posteriori로 판단.
  * Maximum Liklihood
    * $P(H\text{사서}|E) = \frac{1 * 0.4}{1 * 0.4 + 20 * 0.6} $
    * $P(H\text{농부}|E) = \frac{20 * 0.6}{1 * 0.4 + 20 * 0.6} $
    * 따라서 농부일 가능성이 더 높다.
   * Maximum A Posterori
     * $P(H\text{사서}|E)P(\text{사서})$
     * $P(H\text{농부}|E)P(\text{사서})$
# 기계학습 수업 예시 기준
* 개:고양이:호랑이=5,4,1 (라는 통계가 있다 하자.)
### Case 1
* 물체가 있다. 개일까? 고양이일까? 호랑이일까?
  * A: 물체는 개이다.
  * $P(A)=\frac{5}{10}$, 사전 확률
### Case 2
* 물체가 있다. 물체는 꼬리가 10cm이다. 개? 고양이? 호랑이?
  * A: 물체는 개이다.
  * B: 물체는 꼬리 길이가 10cm이다.
  *  
 
