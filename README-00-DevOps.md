# VS Code Extension DevOps
VS Code 익스텐션 개발에 관련된 자료 모음집입니다.  
현재 자료를 모으고 문서화 중에 있습니다.  

## 개발환경

- VS Code
- nvm for Windows
- node
- npm 

## 의존모듈

- vscode ( depricated, use @types/vscode and vscode-test instead )
- @types/vscode
- vscode-test
- typescript
- @types/node

## 프로젝트 생성 ( Yeoman 버전 )

- [Yeoman](https://yeoman.io) 을 이용해서 생성을 추천하고 있다

```
$ npm install --global yo 
$ npm install --global generator-code
$ yo code
```
```
# ? What type of extension do you want to create? New Extension (TypeScript)
# ? What's the name of your extension? HelloWorld
### Press <Enter> to choose default for all options below ###

# ? What's the identifier of your extension? helloworld (엔터)
# ? What's the description of your extension? (엔터)
# ? Initialize a git repository? No (엔터)
# ? Bundle the source code with webpack? Yes (엔터)
# ? Which package manager to use? npm (엔터)

# ? Do you want to open the new folder with Visual Studio Code? Open with `code`
```

## 프로젝트 생성 ( From Scratch 버전 )

- node 개발환경에서 시작
```
$ npm init --yes
...
```

## 설정파일들

- package.json
- ./vscode/tasks.json
- ./vscode/launch.json
- ./vscode/settings.json
- ./vscode/extensions.json

## 디버깅

-
- 


## 추가 및 갱신해야할 내용들

- from scratch 버전 업데이트 필요
- 디버깅 관련 내용

