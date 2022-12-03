# ML & MAP Classification
## ML Classification (Maximum Liklihood)
* **조건부확률이다.** 
* 만약 `class conditional distributions`을 알고 있을 때 ( $c_k$ 에 대한 `liklihood, 가능도`) $P(x|c_i) \text{for all k = 1,..,K} $
* 위 조건부확률은 **liklihood (가능도)**, **class-conditional probability(distribution)** 이라고 부른다.

$$
\underset{k=1...K}{\operatorname{argmax}}P(x_{\text{new}}|c_k)
$$
* 각 동물들의 꼬리 분포에 대해서 알고 있을 때,
  * 개일 경우의 꼬리길이가 10cm일 확률: $P(x=\text{10cm}|c_\text{강아지})$

## MAP Classification (Maximum A Posteriori)
* **조건부확률에 사전확률을 곱한 값이다.**

$$
k^* = \underset{k=1...K}{\operatorname{argmax}}P(x_{\text{new}}|c_k)P(c_k) = P(c_k|x_{\text{new}})
$$
* 기존 조건부확률(ML Classification)에 사전확률(prior disdtribution)을 사용하여 구한 값이다.

## ML vs MAP Classification
* 만약 사전확룰을 안다면 MAP를 사용하고, 모른다면 ML을 써라.
  * 사전 확률 모르는 경우가 많음.
* 예시
  * 만약 각 동물에 대한 분포를 안다면 MAP를 써라. ex) P(c=강아지) = 0.4
