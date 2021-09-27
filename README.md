# Revolution2

## #1. 부정보험금청구탐지(Insurance Fraud Claims Detection) 데이터 

<pre>- months_as_customer : <i>int</i> 보험금 납입 기간(누적, 개월)
- age	: <i>int</i> 연령
- policy_number :  <i>int</i> 보험 가입번호
- policy_bind_date : <i>str</i> 보험 계약일
- policy_state : <i>str</i> 보험 계약자 주
- policy_csl : 보험한도  : <i>str</i> 사고 발생 시 1인당 보험금 한도액 / 전체 보험금 한도액 (단위 :  천달러)
- policy_deductable :  <i>int</i> 보험의 자기부담금
- policy_annual_premium	: <i>float</i> 연간보험료
- umbrella_limit	: <i>int</i> 보험금 한도
- insured_zip : <i>int</i>피보험자 우편번호
- insured_sex  : <i>str</i>피보험자  성별
- insured_education_level	:<i>str</i>   피보험자  교육수준
- insured_occupation	insured_hobbies :<i>str</i>  피보험자의 취미
- insured_relationship :<i>str</i> 피보험자 와 보험계약자의 관계
- capital-gains : <i>int</i> 자본이득
- capital-loss :  <i>int</i> 자본손실
- incident_date	: <i>str</i> 보험 사고 일자
- incident_type	: <i>str</i> 보험 사고의 종류
- collision_type	: <i>str</i> 충돌 유형
- incident_severity : <i>str</i> 손상정도
- authorities_contacted :  <i>str</i> 보험사고 발생 당시 연락기관(경찰서, 소방서 등)
- incident_state :  <i>str</i> 사고 발생 지역
- incident_city : 	<i>str</i> 사고 발생 도시
- incident_location : 	<i>str</i> 사고 발생 위치
- incident_hour_of_the_day : <i>int </i> 사고 발생 시각 (예: 20시 경)
- number_of_vehicles_involved	: <i>int </i> 총 사고 발생 차량 수
- property_damage : <i>str </i> 재산 피해 여부
- bodily_injuries	: <i>int </i> 신체 피해 정도( 0 : 없음, 1: 경상 2: 중상)
- witnesses	: <i>int </i> 사고 목격자 수
- police_report_available : <i>str </i> 	경찰 보고서 확인 가능 여부
- total_claim_amount : <i>int </i> 총 보험금 청구금액
- injury_claim : <i>int </i> 상해 청구금액
- property_claim :<i>int </i> 재산 피해 청구 금액
- vehicle_claim :<i>int </i> 차량 피해 청구금액
- auto_make :<i>str </i> 자동차 제조사
- auto_model :<i>str </i> 자동차 모델
- auto_year :<i>int </i> 자동차 연식
- fraud_reported :<i>str </i> 허위 청구여부 (허위청구 :  Y / 정상청구 : N)
</pre>

#### 데이터 불러오기
<pre><code>insurance_claim = pd.read_csv("https://raw.githubusercontent.com/fintech-data/Revolution2/main/data/insurance_claims.csv")
</code></pre>


## #2. 피싱탐지(Phishing Detection) 데이터 

<pre>- SFH	: <i>int</i> Server Form Handler(서버 폼 핸들러)의 이상여부
- popUpWidnow : <i>int</i> 윈도우 팝업 여부
- SSLfinal_State	:<i>int</i>   https의 이상 여부
- Request_URL	:<i>int</i> 요청 url의 이상여부
- URL_of_Anchor :<i>int</i>  <a>테그의 이상여부
- web_traffic :<i>int</i>  웹사이트 트래픽의 이상여부
- URL_Length :<i>int</i>	의심스러운 부분을 숨기기 위한 긴 url 여부
- age_of_domain :<i>int</i>  도메인의 수명 이상여부
- having_IP_Address :<i>int</i> ip 주소의 사용여부
- Result :<i>int</i>  피싱사이트 여부
</pre>


#### **데이터 불러오기**
<pre><code>website_phishing = pd.read_csv('https://raw.githubusercontent.com/fintech-data/Revolution2/main/data/Website%20Phishing.csv')
</code></pre>

## #3 보험료 결정 데이터 


<pre>- age: <i>int</i>, 나이
- sex: <i>str</i>, 성별 
- bmi: <i>float</i>, BMI지수
- children: <i>int</i>, 자녀 수
- smoker: <i>str</i>, 흡연여부
- region: <i>str</i>, 사는 지역
- charges: <i>float</i>, 보험료
</pre>

#### 데이터 불러오기
<pre><code>insurance = pd.read_csv('https://raw.githubusercontent.com/fintech-data/Revolution2/main/data/insurance.csv')
</code></pre>

## #4 여행자 보험  데이터 

<pre><code>- Agency: <i>str</i>, 보험 판매점
- Agency Type: <i>str</i>, 판매점 형태
- Distribution Channel: <i>str</i>, 판매 채널
- Product Name : <i>str</i>,  판매 상품 종류
- Duration: <i>str</i>, 보험기간
- Destination: <i>str</i>,  여행국가
- Net Sales: <i>int</i>, 순마진
- Commision (in value): <i>float</i>, 수수료
- Gender: <i>str</i>, 성별
- Age: <i>int</i>, 나이
- Claim : 보험금 청구
</code></pre>

#### **데이터 불러오기**
<pre><code>travel_insurance = pd.read_csv("https://raw.githubusercontent.com/fintech-data/Revolution2/main/data/travel%20insurance.csv")
</code></pre>
