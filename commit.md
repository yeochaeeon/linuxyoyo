# linuxyoyo

## 리눅스 문제 해결 / git hub commit 문제 해결..

### #1. 리눅스 서버시간 동기화 
   1. ``` sudo apt-get install rdate```
   
   2. ```  password  ``` 입력
   
   3. ``` rdate -s time.bora.net``` 말고 
   
      ``` sudo rdate -s time.bora.net``` 으로!! 
   
   * root 권한으로 실행: "rdate" 명령을 실행할 때 sudo 명령을 사용하여 관리자 권한으로 실행해야함
