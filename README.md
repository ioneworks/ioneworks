# IONEWORKS

------------------------------------------------------------------------------------

### 시작하기 (JDK 21 이상 준비)
+ H2DB 파일모드 기본 설정
+ DBMS 변경 시 /configuration/application.properties에서 DATABASE.conn.root의 DB 연결정보 수정
+ statup.bat 수정 및 실행 (JAVA_HOME 설정)
+ 브라우져에서 http://localhost 접속 (포트가 8080의 경우 http://localhost:8080)
+ root 계정으로 접속 아이디 : ioneworks , 초기 패스워드 : 111111

------------
### Standalone
 + 실행파일 다운로드 : https://drive.google.com/file/d/1d0mdGjZ7lps7Vv91G6DSq3To-_yLuVMn/view?usp=sharing
 
------------

### VM 옵션 JAVA_OPTS

```
-Dio.env="dev"
를 추가하면 application.properties 가 아닌 application.dev.properties 를 사용한다.
application.dev.properties는 application.properties에서 변경된 부분만 설정하면 된다.

아래와 같이 옵션을 설정하면
-Dio.fileupload:flag="false" 는
fileupload.properties의 flag 값을 대체한다.

컨테이너 환경의 경우 IP가 유동적이기 때문에 아래와 같이 서비스네임을 지정한다.
-Dio.servicename="ioneworks"

config file path 수동 지정 (미 지정시 /WEB-INF/configuration 를 사용)
-Dioneworks.configuration=/home/ioneworks/configuration
```
```
개발 환경 예시
-Dio.env="dev"
-Dio.servicename="ioneworks"
-Djava.net.preferIPv4Stack="true"
```
<br />
------------
이 소프트웨어는 소유자의 저작권으로 보호받고 있습니다. 무단으로의 복제, 배포, 수정, 판매, 그리고 허가되지 않은 상업적 이용은 저작권법 및 계약 위반이 될 수 있으며, 이로 인해 법적 문제가 발생할 수 있습니다.<br />

사용 문의 : one@ioneworks.com
```
라이선스 키 요청 : 아래 양식으로 one@ioneworks.com 으로 이메일을 보내주시면, 라이선스 키를 발급해 드립니다.
양식)
- 회사/개인 명 : (주)우리회사이름 
- 담당자 성명 : 홍길동
- 담당자 연락처(핸드폰) : 010-0000-0000
- 담당자 이메일 : email@mycompany.com
- 사용 도메인 : mycompnay.com
```
