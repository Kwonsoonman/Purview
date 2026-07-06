# 작업 4 : EDM 기반 분류 정보 유형 생성
이 작업에서는 직원 데이터의 데이터베이스 스키마를 사용하여 정확히 일치하는 데이터 매칭(EDM) 기반 분류를 생성합니다.

<br>
1.	Microsoft Edge에서는 여전히 Joni Sherman으로 Microsoft Purview에 로그인되어 있어야 합니다.
<br>



<br>
2.	왼쪽 사이드바에서 [솔루션] - [정보 보호]을 선택하여 정보 보호로 이동합니다.<br>


<br>
3.	정보 보호 페이지에서 [분류기(Classifiers)] – [EDM 분류기(EDM EDM classifiers)]를 클릭합니다.<br>

<br>
4.	EDM 분류기 페이지에서 [+EDM 분류기 만들기]를 클릭합니다.
<br>

![](Task04%20_CreateEDM_based_classification_information_type.assets/2026-07-06-18-44-23.png)

<br>
5.	스키마를 정의하는 방법에서 [수동(Manually define your data structure)]를 선택합니다. 

+ 이름과 EDM 분류기 설명 페이지에 다음과 같은 입력을 하면:
+ 이름: employeedb
+ 설명: Employee Database schema
[다음(Next)]을 클릭합니다.
<br>
![](Task04%20_CreateEDM_based_classification_information_type.assets/2026-07-06-18-44-45.png)
<br>
6.	스키마 정의 방법 선택 페이지에서 [수동으로 데이터 구조를 정의]를 선택한 후 [다음]을 클릭합니다.
<br>

![](Task04%20_CreateEDM_based_classification_information_type.assets/2026-07-06-18-44-54.png)

<br>
7.	감지하고자 하는 데이터를 포함하는 Define 열에 다음 열을 추가 입력합니다.

+ Name
+ BirthDate
+ StreetAddress
+ EmployeeID
[+ Add column]를 클릭하여 나머지 필드를 추가하여 총 4개의 열이 될 때까지 추가한 후 [다음(Next)]을 클릭합니다. 
 <br>

![](Task04%20_CreateEDM_based_classification_information_type.assets/2026-07-06-18-45-02.png)

<br>
8.	기본 요소 선택 페이지에서 EmployeeID 열을 찾으세요. 단일 토큰이 표시된 매치 모드 드롭다운 목록에서 SIT를 선택하려면 [+(플러스 기호)]를 클릭합니다.
 <br>

![](Task04%20_CreateEDM_based_classification_information_type.assets/2026-07-06-18-45-38.png)
<br>
9.	오른쪽의 "EmployeeID" 플라이아웃 패널에서 검색창에서 “Contoso”를 검색하여 이전 작업에서 생성된 Contoso 직원 ID의 민감한 정보 유형이 표시되어야 합니다. 이 민감한 정보 유형 왼쪽에 체크박스를 선택한 후 저장을 클릭합니다.
 <br>

![](Task04%20_CreateEDM_based_classification_information_type.assets/2026-07-06-18-45-48.png)

<br>
10.	기본 요소 선택 페이지에서 EmployeeID 오른쪽에 체크박스를 선택하여 이 필드를 [기본 요소(Primary element)]로 설정을 확인후 [다음(Next)]을 클릭합니다.
 <br>

![](Task04%20_CreateEDM_based_classification_information_type.assets/2026-07-06-18-45-56.png)

<br>
11.	선택한 열의 데이터 구성 설정에서 토글이 '예'로 설정되어 있는지 확인하세요. 모든 열에 동일한 설정을 사용하세요.
 <br>

 ![](Task04%20_CreateEDM_based_classification_information_type.assets/2026-07-06-18-46-06.png)


<br>
12.	모든 열의 데이터에 대해 구분자 및 구두점 무시(Ignore delimiters and punctuation for data in all columns) 하는 체크박스를 선택하고, 드롭다운에서 '구분자 및 구두점 선택'을 선택해 무시하고 다음을 선택합니다. 

+ 하이픈 ('-')
+ 마침표 ('.')
+ 공간 (' ')
+ 열괄호 ('(')
+ 괄호 (')')
드롭다운 밖 어디든 클릭한 후 [다음(Next)]을 클릭합니다.
 <br>

 ![](Task04%20_CreateEDM_based_classification_information_type.assets/2026-07-06-18-46-17.png)


<br>
13.	기본 요소에 대한 탐지 규칙 구성에서 기본 설정을 유지한 후 [다음]을 클릭합니다.
 <br>

![](Task04%20_CreateEDM_based_classification_information_type.assets/2026-07-06-18-46-48.png)

<br>
14.	리뷰 설정 및 완료 페이지에서 [제출(Summit)]을 클릭합니다.
 <br>

![](Task04%20_CreateEDM_based_classification_information_type.assets/2026-07-06-18-46-56.png)

<br>
15. 'You created the successful create a edm classifier' 페이지에서, 다음 작업에 사용할 스키마 이름을 꼭 복사합니다. 여기서는 “employeedb” 입니다. 스키마 이름을 복사한 후에는 [완료(Done)]를 클릭합니다. 데이터베이스 파일 소스에서 직원 데이터를 식별하기 위한 새로운 EDM 기반 분류 민감 정보 유형을 성공적으로 만들었습니다.
 <br>

![](Task04%20_CreateEDM_based_classification_information_type.assets/2026-07-06-18-47-03.png)