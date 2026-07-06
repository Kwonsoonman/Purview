# Lab05 - DLP 정책을 구현하고 관리
Microsoft 365 전반에 걸쳐 민감한 고객 데이터를 보호하기 위해 데이터 손실 방지(DLP) 정책을 설정하도록 요청받았습니다. 이 실습에서는 Microsoft Purview와 Microsoft Defender를 사용하여 신용카드 번호나 직원 ID와 같은 민감한 정보 공유를 탐지하고 제한하는 DLP 정책을 만들고 관리할 것입니다.


## 작업 1: 시뮬레이션 모드에서 DLP 정책 생성
이 작업에서는 시뮬레이션 모드에서 Teams 메시지의 신용카드 번호를 대상으로 하는 DLP 정책을 만듭니다. 이 정책은 사용자가 민감한 콘텐츠를 공유하려 할 때 알림을 주고, 정당한 사유로 무효화할 수 있도록 허용합니다.

<br>
1.	Microsoft Edge에서 https://purview.microsoft.com 로 이동하여 Joni Sherman으로 Microsoft Purview 포털에 로그인 합니다.<br>


<br>
2.	[솔루션(solution)] – [데이터 손실 방지(Data Loss Prevention)]을 클릭합니다.
 <br>

![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-46-47.png)
<br>
3.	데이터 손실 방지 화면에서 [정책(Policies)]를 클릭합니다.<br>


<br>
4.	정책 페이지에서 [+ 정책 생성(create Policy)]를 클릭합니다.<br>
 

![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-46-54.png)
<br>
5.	'무엇을 보호하고 싶은가?' 페이지에서 [Enterprise 애플리케이션 및 장치]를 선택한 후 다음을 클릭합니다.<br>
 
 ![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-47-01.png)

<br>
6.	템플릿으로 시작하거나 맞춤 정책 생성 페이지에서 카테고리로 [Custom]을 선택한 후 Regulations 항목에서 [Custom 정책]을 선택한 후 [다음(Next)]을 클릭합니다.
 <br>


![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-47-08.png)
<br>
7.	'DLP 정책 이름 지정' 페이지에서 다음을 입력하세요:

+ 이름: DLP - Credit Card Protection
+ 설명: Detect and restrict sharing of credit card numbers in Teams messages.
[다음(Next)]을 클릭합니다.
 <br>


![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-47-15.png)
<br>
8.	관리자 단위 할당 페이지에서 [다음]을 클릭합니다.
 <br>

![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-47-29.png)
<br>
9.	'정책 적용 위치 선택' 페이지에서 [Teams 채팅과 채널 메시지]만 사용할 위치를 활성화하세요. 다른 위치가 선택되어 있으면 해당 위치를 해제하세요. [다음(Next)]을 클릭합니다.
 <br>

![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-47-38.png)

<br>
10.	'정책 설정 정의' 페이지에서 [고급 DLP 규칙 생성 또는 커스터마이즈(Create or customize advanced DLP rules)]를 선택한 후 [다음]을 클릭합니다.
 <br>

![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-47-45.png)
<br>
11.	고급 DLP 규칙 사용자 지정 페이지에서 [+ 규칙 만들기]를 클릭합니다.
 <br>


![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-47-52.png)
<br>
12.	Create 규칙 플라이아웃에서 이름 필드 : Credit card information을 입력합니다.
 <br>


![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-47-58.png)
<br>
13.	Microsoft 365에서 콘텐츠 공유(Restrict access or encrypt the content in Microsoft 365 locations)]을 클릭합니다.
<br>

<br>
14.	내용은 Microsoft 365 섹션에서 공유에서 [조직 외부인과 함께하는 옵션(Block only people outside your organization)]을 클릭합니다.
 <br>


![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-48-04.png)

<br>
15.	조건 항목에서 [+ 추가 조건(add condition)] – [컨텐츠 포함(Content contains)]를 클릭합니다.
<br>
 
 ![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-48-11.png)

<br>
16.	[추가(add)] – [민감한 정보 유형(Sensitive info types)]를 클릭합니다.
 <br>

 ![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-48-18.png)

<br>
17.	민감 정보 유형 페이지에서 [Credit Card Number]를 입력하고 검색한 결과에서 선택하고 [추가(add)]를 클릭합니다.
 <br>


![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-48-24.png)
<br>
18.	[Actions] – [Add an action]에서 [Microsoft 365 위치의 접근 제한 또는 콘텐츠 암호화(Restrict access or encrypt the content in Microsoft 365 locations)]를 클릭합니다.
 <br>


![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-48-32.png)
<br>
19.	접근 제한 또는 콘텐츠 암호화 섹션에서 [조직 외부인만 차단(Block only people outside your organization)]를 클릭합니다.
 <br>

![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-48-40.png)
<br>
20.	사용자 알림 항목에서 [사용 알림] 토글을 켜서 사용자에게 정보를 알리고 민감한 정보의 올바른 사용법을 알리는 메시지가 나타나게 하고, [Office 365 서비스에서 정책 팁과 함께 사용자 알림( Notify users in Office 365 service with a policy tip)] 체크박스를 클릭합니다.
 <br>

![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-48-46.png)

<br>
21.	사용자 덮어쓰기에서는 [정책 제한 변경 허용 체크박스를 선택하고, (Fabric, Exchange, SharePoint, OneDrive, Teams 사용자)( Allow users to override policy restrictions)]
<br>

<br>
22.	[사업 정당화 필요(Require a business justification to override)] 체크박스를 클릭합니다.
 <br>

![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-48-53.png)


<br>
23.	사고 보고서 항목에서, 관리자 알림 및 보고서에서 이 심각도 수준 사용하기(Use this severity level) 드롭다운에서 [Low]를 클릭하고, 규칙 만들기 플라이아웃 패널 하단에서 [저장(save)]를 클릭합니다.
<br>

 ![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-49-00.png)

<br>
24.	'고급 DLP 규칙 맞춤'에서 [다음(Next)]을 클릭합니다.
 <br>


![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-49-07.png)
 <br>
25.	정책 모드 페이지에서 [시뮬레이션 모드에서 정책을 실행하기(Run the policy in simulation mode)]를 선택하고, [시뮬레이션 모드에서 정책 팁 표시(Show policy tips while in simulation mode)] 체크박스를 선택한 후 [다음(Next)]을 클릭합니다.
<br>

![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-49-15.png)
 
<br>
26.	검토 및 완료 페이지에서 설정을 검토한 후 [제출]를 클릭합니다.
 <br>

 ![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-49-23.png)

<br>
27.	새 정책 생성 페이지에서 [완료]를 클릭하여 DLP 정책을 만들어 Teams 콘텐츠를 신용카드 번호를 검색하고, 비즈니스 정당성을 이유로 덮어쓰는 것을 허용는 정책을 생성하였습니다.
 <br>

 ![](Task01_Create_DLP_policy_in_simulation%20mode.assets/2026-07-06-19-49-30.png)

