# 작업 6: Microsoft Defender 파일 검사 활성화

일부 파일 정책은 보호된 파일의 내용을 검사하기 위해 접근 권한을 요구합니다. 이 작업에서는 Microsoft Defender가 OneDrive와 SharePoint 파일 내용을 스캔하여 민감한 정보를 찾을 수 있도록 필요한 권한을 부여해야 합니다.

<br>
1.	https://security.microsoft.com 로 이동해 Microsoft Defender XDR 관리 사이트에 접속합니다. (admin계정)
<br>

<br>
2.	왼쪽 사이드바에서 [시스템(system)] – [설정]을 클릭합니다.
<br>

<br>
3.	[설정]을 선택한 후 [클라우드 앱(Cloud Apps)]를 클릭합니다.
<br>
 
 ![](Task06%20_Enable_file_inspection_in_MicrosoftDefender.assets/2026-07-06-20-06-58.png)
<br>
4.	Cloud Apps 창 내 왼쪽 창에서 [정보 보호 섹션(information Protection)] – [Microsoft Information Protection]]를 클릭합니다.
<br>


<br>
5.	보호 파일 검사(Inspect protected files) 항목에서 파일 검사를 활성화하기 위해 [권한 부여(grant permission)]를 클릭합니다.
 <br>

 ![](Task06%20_Enable_file_inspection_in_MicrosoftDefender.assets/2026-07-06-20-07-07.png)
 
 <br>

![](Task06%20_Enable_file_inspection_in_MicrosoftDefender.assets/2026-07-06-20-07-16.png)
<br>
6.	Microsoft Entra ID에서 필요한 권한을 허용하는 안내를 따라가면, Microsoft Defender for Cloud Apps에서 파일 검사가 활성화된 것을 확인할 수 있을 것입니다. 이제 Defender에서 파일 검사가 활성화되어 파일 정책이 민감한 콘텐츠를 스캔할 수 있습니다.
 <br>
![](Task06%20_Enable_file_inspection_in_MicrosoftDefender.assets/2026-07-06-20-07-23.png)
