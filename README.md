# 졸업 작품 : 전동 킥보드 
<br>
첫 아이디어 회의 결과<br>
<br>
1. 4륜 전동 킥보드 <br>
2. 아두이노를 이용한 드론<br>
<br>
<br>
<br>
4륜 전동 킥보드로 주제 선정함. 기본적인 골자는 시중에 많이 나와있는 2륜 킥보드가 아닌 4륜 킥보드 제작<br>
사람이 서서 타는 곳은 스케이트 보드와 같은 형태지만 폭이 일반 스케이트 보다 더욱 넓은 형태.<br>
조향과 동력 전달을 위한 손잡이 부분이 올라와 있어야 한다. 또한 기존 핸들을 돌리거나 따로 버튼을 두어 속도를 조절하던 형태를 벗어나 <br>
손잡이를 밀고 당기는 행위를 통해 속도 조절을 할 수 있도록 제작!!<br>
<br>
동력장치는 허브모터를 사용해야 될 것으로 보임. <br> 배터리는 리튬이온 전지 혹은 납배터리를 사용!!<br>
재료비 어느정도인지 알아볼 것!<br>
허브모터 알아보기! <br>
허브 모터 : 바퀴와 모터가 결합된 형태. 바퀴 내부 디스크 부분에 모터가 있다.<br>
허브 모터 가격 대략 15만원 ~ 20 만원 선 (2개 필요할듯)<br>
24V-150W정도면 될것으로 예상 리튬이온 배터리 3.6V * 7 * 3 이라면 전류량이 대략 9000 mAh <br>
약 20분 정도 밖에 구동 안될것으로 예상,,, 배터리 용량을 증대해야됨,,<br>
<br>
<br>
<br>
# 졸업 작품 주제 변경<br>
<br>
<br>
처음 생각했던 사륜 전동 킥보드는 제작비가 너무 많이 들어갈 것으로 예상되어<br>
전동 킥보드가 아닌 전동 인라인 스케이트로 주제 변경 기존에 소장하고 있던 인라인 스케이트를 가지고 설계 <br>
모터의 가격이 생각보다 비쌈,,, <br>
한쪽 발에만 모터를 장착하는 방향으로,,<br>
<br>
<br>



![초기 컨셉도](https://github.com/jonghyunlee/Project/blob/master/%EC%B4%88%EA%B8%B0%20%EC%BB%A8%EC%85%89.jpg?raw=true)<br>
컨셉도<br><br>

기존에 가지고 있던 인라인 스케이트를 활용하여 제작을 하기 때문에<br>
인라인 스케이트 프레임에 장착할 수 있도록 하며 전동 스쿠터나 킥보드 처럼 <br>
큰 바퀴를 쓸 수가 없기에 보통 사용되는 허브모터를 사용할 수가 없는 제약 조건이 있다.<br>
또한 바퀴에 직접적으로 모터를 연결하여 사용할 수도 없기에 부득이 바퀴에 아래 사진과 같은 <br>
축을 설치하여 모터와 간접적으로 연결할 수 있도록 설계하였다.<br><br><br>
![바퀴 축 컨셉](https://github.com/jonghyunlee/Project/blob/master/%EA%B5%AC%EB%8F%99%20%EC%B6%95%20%EC%BB%A8%EC%85%89.jpg?raw=true)<br><br>
위의 사진처럼 바퀴에 가공물을 부착하여 축을 만들어 기어를 물릴 수 있도록 설계
<br>
<br>
<br>
<br>
기구물 설계 이후 모터의 간략적인 제어도를 생각해봄.<br>
<br>
![제어 컨셉도](https://github.com/jonghyunlee/Project/blob/master/%EC%A0%9C%EC%96%B4%20%EC%BB%A8%EC%85%89.jpg?raw=true)
<br>
<br>
일상생활에서 탈 수 있어야 하기 때문에 모터의 사양을 정할 때 AC 모터가 아닌 DC 모터를 사용<br>
그렇기 때문에 모터에 전원을 공급하기 위한 배터리가 필요!<br>
배터리는 리튬이온 배터리를 쓰는게 가장 좋은 조건일 거라고 생각이 듬.<br>
가격적인 면에서는 납배터리가 저렴하지만 크기와 내구성?, 보존성? 등을 생각하면 리튬이온!!<br>
<br>
<br>
모터를 컨트롤 하기 위한 컨트롤러는 아두이노를 이용하여 제작하기로 함<br>
또한 모터의 속도를 제어하기 위한 ESC(Electric Speed Controller)가 필요함!<br>
속도를 제어하기 위한 장치는 편의상 손에 쥘 수 있는 크기여야 할 것!<br>
<br>
<br>
<br>
<br>
# 사양 선정
<br>
<br>
모터 : 모터의 사양에서 가장 중요한 부분은 실제 탑승시에 과부화가 걸려 모터가 작동하지 않으면 안되기 때문에<br>
       알맞은 토크가 나오는 모터를 선정해야함!(전문가 조언이나 직접적인 실험이 필요할 것으로 예상)<br>
<br>
<br>
배터리 : 크기가 작아야 함. 리튬이온전지 따로 제작 필요<br>
18650 배터리를 연결하여 전압 맞추고 용량 맞춰서 사용하면 됨!<br>
<br>
<br>
모터 컨트롤러 : 아두이노를 이용해 제작 가능한 지 알아볼 것. <br>
어떤 기능을 넣어야되는지 자세히 알아보고 사용방법 숙지. Youtube에 많을 것으로 예상 <br>
<br>
<br>
ESC : 모터의 속도를 조절하기 위해 꼭 필요! 구로 공구상가나 세운상가에서 가격 및 사용법 알아보기.<br>
<br><br>
<br>
<br>
# 중간 보고서 작성
<br>
<br>
제안 작품 소개 부분 작성!!!
<br>
<br>
# 상세 설계
<br>
<br>
* 해야할 일 *
<br>
<br>
1. 인라인 스케이트 실치수 측정하기
<br>
2. 치수 맞춰서 설계 치수 변경
<br>
3. 모터 사양 선정하기!!!!
<br>
4. 상세 설계 및 도면 작성
<br>
5. 가공 업체 알아보기
<br>
<br>
<br>

![상세 1](https://raw.githubusercontent.com/jonghyunlee/Project/master/%EC%83%81%EC%84%B8%201.jpg)<br>
<br>
<br>
<br>
상세 1<br>
![상세 2](https://github.com/jonghyunlee/Project/blob/master/%EC%83%81%EC%84%B8%202.jpg?raw=true)<br>
<br>
<br>
<br>
상세 2<br>
![상세 3](https://raw.githubusercontent.com/jonghyunlee/Project/master/%EC%83%81%EC%84%B8%203.jpg)<br>
<br>
<br>
상세 3<br>
<br>
<br>
기존 설계에서 변경없이 결합 부위 마무리 함. <br>
스프라켓 사이즈에 제한사항이 생겨 기어비를 생각보다 크게 가져가지 못함 <br>
토크가 충분한지 확실치 않음 아무래도 테스트를 해봐야 할 것으로 예상<br>
모터는 DC 24V 100W BLDC 모터 사용 <br>
일반 DC 모터 사용을 하려 했으나 같은 100W급을 사용했을 시 크기 차이가 너무 심하다 <br>
DC 모터는 BLDC보다 높이가 약 100mm 정도 차이가 남(너무 크다) 일반 DC 모터를 사용하면<br>
인라인 스케이트를 타는 동안 반대발과 충돌이 예상되므로 BLDC사용 <br>
모터의 정격 회전 속도가 3000rpm 이므로 현재 설계상 기어비가 1 : 1.5 이므로 약 2000rpm으로 구동 가능
<br>
2000rpm 구동시 초당 33.3rps<br>
바퀴 크기가 110mm 이므로 초당 이동거리는 <br>
110mm * 3.14 * 33.3 = 11.5m/s 로 예상 <br>
생각보다 너무 빠르다 약 41km//h  안전상 문제가 예상됨<br>
별도의 속도 조절 장치가 필요!!! <br>
<br>
<br>
<br>
가공품 재질을 뭐로 할지 결정 필요!!<br>
1. 플라스틱류 : 가벼운 장점이 있음, 모터 회전시 나오는 진동에 영향을 많이 받을 것으로 예상 <br>
2. 알루미늄 : 철에 비해 가볍고 플라스틱류에 비해 단단하다, 진동에 큰 영향을 받진 않을 것으로 예상된다.<br>
3. SKD : 후보들 중 가장 단단하다, 안정성 면에서는 가장 좋음 하지만 무게가 너무 무겁다. <br>
프레임을 현재 약 15t 정도로 설계하였는데 그대로 할지 아니면 절곡품을 이용할지 결정 필요.<br>
절곡품으로 할 시 과연 모터 무게와 진동을 버틸 수 있을 지 의문,,,,,<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
현재 두께로 하기로 결정 지금 상태에서 도면 그리고 가공 맡겨야 함. <br>
<br>
<br>
<br>
<br>

![도면 1](https://github.com/jonghyunlee/Project/blob/master/%EB%8F%84%EB%A9%B4%201.jpg?raw=true)<br>
<br>
<br>
<br>
도면 1
<br>
<br>
<br>

![도면 2](https://github.com/jonghyunlee/Project/blob/master/%EB%8F%84%EB%A9%B4%202.jpg?raw=true)<br>
<br>
<br>
<br>
도면 2
<br><br>
<br>

![도면 3](https://github.com/jonghyunlee/Project/blob/master/%EB%8F%84%EB%A9%B4%203.jpg?raw=true)<br>
<br>
<br>
<br>
도면 3
<br>
<br>
<br>


![도면 4](https://github.com/jonghyunlee/Project/blob/master/%EB%8F%84%EB%A9%B4%204.jpg?raw=true)<br>
<br>
<br>
<br>
도면 4
<br>
<br>
<br>

베어링 결합 부 제외하곤 기본 공차로 맞춤 <br>
베어링 결합 부는 공차 확실히 넣기 <br>
<br>
<br>
<br>
가공 업체 미팅 결과 <br>
 2 업체에서 가능하다고 연락 줌. <br>
 한 업체는 아직 견적을 보내주지 않고 있다. 확인 후 더 저렴한 곳에서 추진.<br>
 가공품 제외한 나머지 재료들 구입하기!!<br>
 <br>
 <br>
구매품 List <br>
1. 베어링 : Thrust ball bearing 형번 51102 2개<br>
2. 스프라켓 : SP35B15-N-15 1개 , SP35B10-N-12 1개 <br>
3. 체인 : CHE35-U 1개 <br>
<br>
<br>
<br>
가공 중에 도면이 이상하다고 연락와서 수정 후 다시 보내드림!<br>
<br>
<br>
<br>

모터 테스트 <br>
<br>
<br>
<br>
배터리, 컨트롤러 연결해서 모터 구동 테스트 해봄.<br>
모터가 돌지 않음..... 원인 파악 시급 <br>
<br>
<br>
배터리 문제로 생각하고 배터리 Unplug 하고 바로 파워서플라이를 컨트롤러에 연결 후 테스트 <br>
다행히 모터가 정상 작동!! <br>
배터리 충전이 안되는 것으로 예상됨....<br>
충전 전압을 못 맞춰서 그런지 계속 충전이 되지 않음...<br>
다시 테스트 해볼 필요가 있다!!<br>
<br>
<br>
<br>
<br>
가공품 도착!! <br>
<br>
![가공품 1](https://github.com/jonghyunlee/Project/blob/master/%EA%B0%80%EA%B3%B5%ED%92%88%201.jpg?raw=true) <br>
가공품 1
<br>
<br>
<br>
<br>

![가공품 2](https://github.com/jonghyunlee/Project/blob/master/%EA%B0%80%EA%B3%B5%ED%92%88%202.jpg?raw=true) <br>
가공품 2
<br>
<br>
<br>
<br>

![가공품 3](https://github.com/jonghyunlee/Project/blob/master/%EA%B0%80%EA%B3%B5%ED%92%88%203.jpg?raw=true) <br>
가공품 3
<br>
<br>
<br>
<br>
가공품이 생각보다 너무 크다...<br>
그리고 두께를 15t로 할 필요가 없었을 것 같다.<br> 
너무너무 두껍다...<br>
<br>
<br>
<br>
가공품 도착하여 구매품과 함께 조립 
<br>


