# Git Commands
## # ".gitignore" file
> ### syntax 
- 특정파일 thisfile 제외하기 : `thisfile.txt`
- 특정 디렉토리의 특정파일을 제외하기 : `fileDirectory/thisfile.txt`
- 특정 디렉토리의 모든파일 제외하기 : `fileDirectory/`
- 특정 확정자를 가진 모든 파일 제외하기 : `*.exe`
- 현재경로의 파일 제외하기 : `/thisfile.txt`
- 에외 처리 : `!thisfile.txt`

> ### .gitignore이 적용이 안될 때 

1. 이미 커밋된 파일이 있을 때 .gitignore가 제대로 작동하지 않을 수 있음. 
    - 만약 `*.exe` 의 적용이 안된다면,

   ```
    git rm --cached *.exe
    git commit -m "Remove already committed files"
    ```
    
 3. 스테이징 영역에 이전에 캐시된 정보가 남아있을 수 있음
     - 스테이징 명령에서 파일을 제거하고 그 후에 변경된 .gitignore 을 반영해 다시 스테이징하고 커밋하는 과정이 필요함.

    ```
     git rm -r --cached .
     git add .
     git commit -m "Update .gitignore"
     ```
    
