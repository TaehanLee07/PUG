# 설치 전에

## Node JS
- [Node.js 공식 웹사이트](https://nodejs.org/)
- PUG를 사용하기 위해서는 Node.js 설치가 필수입니다. 설치법은 공식 문서 또는 구글링을 참고하세요.

## VS Code
- [VS Code 공식 웹사이트](https://code.visualstudio.com/)
- 본 문서는 에디터로 VS Code를 사용합니다.

## 시작

### Doctype 선언
1. ROOT 폴더(현재 프로젝트 내에서 최상위 폴더) 안에 `html` 폴더를 생성합니다.
2. ROOT 폴더 안에 `index.pug` 파일을 생성합니다.
3. `index.pug` 파일에 아래와 같이 작성 후 저장합니다. 이는 Doctype 선언입니다.

    ```pug
    doctype html
    ```

### PUG 컴파일
PUG 파일은 브라우저가 인식하지 못하므로 컴파일이 필요합니다. 아래의 명령어를 터미널에 입력합니다.

```sh
pug -w ./ -o ./html -P
```
Enter를 눌러 위 명령어를 실행한 후, html 폴더에서 자동 생성된 index.html 파일을 확인할 수 있습니다.

## 오류 발생시 
1. Windows PowerShell을 관리자 권한으로 실행합니다.
- get-help Set-ExecutionPolicy [Y] 누르고 대기
- Set-ExecutionPolicy RemoteSigned [다시 Y 누르기]
