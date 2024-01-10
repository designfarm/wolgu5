# 주의사항
- 네이버 서치 어드바이저의 경우 사이트당 하루 50회까지 가능합니다.
- 구글 색인의 경우 서치 콘솔당 하루 200회까지 가능합니다.
- **프로그램 실행전 info.txt 파일 먼저 작성하세요.**
- 네이버 색인을 넣을때는 2차 비밀번호 인증이 해제되어 있어야 합니다.
- 구글 색인을 넣을때는 instant indexing api 실행 및 json 파일이 필요합니다. 어떻게 하는지 해당 설명서에 나와 있으니 그대로 따라하시면 됩니다.
- 구글 색인은 사이트에 맞는 json 파일이 필요합니다. 만약 관리사이트가 5개의 경우 5개의 json 파일이 있어야 합니다.
<br><br><br>

------
<br><br>

# 파일구성
![파일 트리구조](https://github.com/designfarm/wolgu5/assets/52616957/2c08838b-14f2-436d-a02d-6be712777ae9 "파일 구성")
<br><br><br>

------
<br><br>
# 실행시 PC보호 발생할 경우
![window_defence_ignore](https://github.com/designfarm/wolgu5/assets/52616957/a4ef1ab8-344f-4ebd-8b81-85bb11f128d8 "실행시 PC보호 발생할 경우")
<br><br><br>

------
<br><br>
# info.txt 작성방법
![info_file_help](https://github.com/designfarm/wolgu5/assets/52616957/9c754a57-d129-44f8-be23-6f250ea37f16)
<br><br>
- 각 행 ‘:’ 옆에 띄어쓰기 하지말고 필요 정보를 넣습니다.
<br><br>
- Site:에는 색인 넣을 대상 주소를 입력합니다.
이때 ‘https://’는제외한 주소를 넣습니다.
<br><br>
**옳바른 예시**
- aa.tistory.com
- naver.com
<br><br>
**틀린 예시**
- https://aa.tistory.com
<br><br>
- Code:에는 개발자에게 전달 받은 패스코드를 입력합니다.
티스토리 비밀번호 아닙니다.
<br><br><br>

------
<br><br>
# 네이버 색인 (파일명 : NaverInstantIndexing.exe)
![indexing_naver_tool_help](https://github.com/designfarm/wolgu5/assets/52616957/8f91a3d0-7133-489f-9a6f-b33937095a14)
<br><br>
- Info.txt 에 정보를 기입하였다면, 각 정보가 자동으로 호출 됩니다.
- 네이버에 색인을 넣을때는 좌측에 있는 4가지 정보가 모두 필요합니다
<br><br><br>

------
<br><br>
# 네이버 색인 실행
![indexing_Complate_Used_Help](https://github.com/designfarm/wolgu5/assets/52616957/ada84d77-b4cb-426a-9d4a-143af1f6365b)
<br><br>
**https://tt.tistory.com의 경우 프로그램을 실행 후**
- tt_sitemap.txt, tt_used_sitemap.txt 2개의 파일이 생성 됩니다.
  - _sitemap의 경우 색인을 넣지 않은 url
  - _used_sitemap의 경우 색인을 넣은 url
<br><br>
- 프로그램을 껐다 켜도 색인 넣지 않은 url에 대해서만 색인이 시작됩니다.
- 새로운 글이 발행 될경우 해당 링크 역시 _sitemap에 추가됩니다.
- 만약 색인을 전부 다 하였을 경우, 최신 글부터 다시 시작하게 됩니다.
