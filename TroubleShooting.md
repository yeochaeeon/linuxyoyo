

## linux trouble shooting

### #1. 리눅스 서버시간 동기화 

1. ``` sudo apt-get install rdate``` # rdate 설치

2. ```  password  ``` 입력 
   
3. ``` rdate -s time.bora.net``` 말고 ``` sudo rdate -s time.bora.net``` 으로!! #time.bora.net으로 부터 시간을 받아옴
   
4. 혹은 ``` rdate -s time.bora.net && hwclock -w``` # 시간을 받아와서 하드웨어 시간을 해당 시간으로 설정 .
   
* root 권한으로 실행: "rdate" 명령을 실행할 때 sudo 명령을 사용하여 관리자 권한으로 실행해야함

