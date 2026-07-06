
# 작업 6 : 키워드 사전 만들기
이메일에서 개인 정보 유출을 방지하기 위한 키워드 사전을 만듭니다.

<br>
1.	Microsoft Purview 포털은 왼쪽 사이드바에서 분류기를 펼친 후 [민감한 정보 유형(Sensitive info types)]을 클릭합니다.<br>


<br>
2.	[+민감 정보 유형 만들기]를 클릭합니다.
<br>
 
![](Task06%20_Create_keyword_%20dictionary.assets/2026-07-06-18-52-57.png)
 <br>
3.	 새로운 민감한 정보 유형 구성을 진행합니다. '민감한 정보 이름 지정' 페이지에 다음을 입력합니다.

+ 이름: Contoso Diseases List
+ 설명: List of possible diseases of employees.
[다음(Next)]을 클릭합니다. 
 <br>

![](Task06%20_Create_keyword_%20dictionary.assets/2026-07-06-18-53-05.png)

<br>
4.	이 민감한 정보 유형 패턴 정의 페이지에서 [+패턴 만들기]를 클릭합니다. 
 <br>

![](Task06%20_Create_keyword_%20dictionary.assets/2026-07-06-18-53-25.png)
<br>
5.	오른쪽의 New pattern flyout 패널에서 기본 요소 아래에서 [+기본 요소 추가(Add primary element)]를 선택한 후 [키워드 사전(keyword dictionary)]를 클릭합니다.
 <br>

![](Task06%20_Create_keyword_%20dictionary.assets/2026-07-06-18-53-33.png)
<br>
6.	키워드 사전 추가(Add a keyword dictionary) 페이지에서 다음을 입력하세요:

+ 이름: Diseases Dictionary
+ 키워드:
  -  flu
  - influenza
  - cold
  - bronchitis
  - otitis
플라이아웃 패널 하단에서 [완료(Done)]를 클릭하세요.
 <br>

![](Task06%20_Create_keyword_%20dictionary.assets/2026-07-06-18-53-43.png)

<br>
7.	새 패턴 페이지로 돌아가 지원 요소 아래에서 [+추가 요소 또는 요소 그룹 항목(+ Add supporting elements or group of elements)을 선택한 후, [키워드 리스트(Keywork list)]를 선택하여 키워드 사전에 추가 지원을 추가합니다.
 <br>

![](Task06%20_Create_keyword_%20dictionary.assets/2026-07-06-18-54-58.png)

<br>
8.	키워드 리스트 추가(Add a keyword) 페이지에서 다음을 입력합니다.

+ 명칭: absence reason terms
+ 대문자 구분 없음:
  - employee
  - absence
  - reason
플라이아웃 패널 하단에서 [완료(Done)]를 클릭합니다.
<br>


![](Task06%20_Create_keyword_%20dictionary.assets/2026-07-06-18-55-07.png)

<br>
9.	새 패턴 페이지로 돌아가 구성을 검토한 후 [생성(Create)]을 클릭합니다. 
<br>


<br>
10.	이 민감한 정보 유형에 대한 패턴 정의 항목에서 [다음(Next)]을 클릭합니다.
 <br>

![](Task06%20_Create_keyword_%20dictionary.assets/2026-07-06-18-55-54.png)
<br>
11.	컴플라이언스 정책에 표시할 권장 신뢰 수준 선택 후 기본 값을 그대로 둔 후 [다음]을 클릭합니다.
 <br>

![](Task06%20_Create_keyword_%20dictionary.assets/2026-07-06-18-56-02.png)

<br>
12.	설정 검토 및 완료 페이지에서 설정을 검토한 후 [생성]을 선택하세요. 
 <br>

![](Task06%20_Create_keyword_%20dictionary.assets/2026-07-06-18-56-09.png)
<br>
13.	민감한 정보 유형이 생성되면, '민감한 정보 유형 생성됨' 페이지에서 [완료(Done)]을 클릭합니다. 키워드 사전을 기반으로 새로운 민감 정보 유형을 성공적으로 만들었고, 오탐률을 줄이기 위해 더 많은 키워드를 추가하였습니다.
<br>

![](Task06%20_Create_keyword_%20dictionary.assets/2026-07-06-18-56-17.png)
 

