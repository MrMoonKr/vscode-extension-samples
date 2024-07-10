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

## tsc 명령행 옵션들

### 기본 옵션들

- --help, -h: 도움말을 출력합니다.
- --version: TypeScript의 버전을 출력합니다.
- --init: 기본 설정 파일(tsconfig.json)을 생성합니다.
- --project, -p <디렉토리/파일>: 특정 tsconfig.json 파일을 사용합니다.
- --watch, -w: 파일을 감시하여 변경 시 자동으로 다시 컴파일합니다.
- --build, -b: 프로젝트를 빌드합니다.

### 파일 관련 옵션들

- --outFile <파일>: 모든 입력 파일을 하나의 파일로 합칩니다.
- --outDir <디렉토리>: 컴파일된 파일이 저장될 디렉토리를 지정합니다.
- --rootDir <디렉토리>: 입력 파일의 기본 디렉토리를 지정합니다.
- --sourceRoot <디렉토리>: 디버거가 사용할 소스 루트를 지정합니다.
- --mapRoot <디렉토리>: 디버거가 사용할 소스 맵 파일의 위치를 지정합니다.

### 컴파일러 동작 제어 옵션들

- --target <버전>: ECMAScript 타겟 버전을 설정합니다 (ES3, ES5, ES6/ES2015, ES2016, ES2017, ES2018, ES2019, ES2020, ES2021, ES2022, ESNext).
- --module <타입>: 모듈 시스템을 지정합니다 (CommonJS, AMD, System, UMD, ES6/ES2015, ESNext, None).
- --lib <라이브러리>: 컴파일에 포함할 라이브러리를 설정합니다 (예: ES6, DOM).
- --jsx <모드>: JSX 코드의 변환 모드를 설정합니다 (Preserve, React, React-native).
- --declaration, --d: .d.ts 파일을 생성합니다.
- --sourceMap, --sourcemap: 소스 맵 파일을 생성합니다.
- --removeComments: 출력 파일에서 주석을 제거합니다.
- --noEmit: 출력 파일을 생성하지 않습니다.
- --noEmitOnError: 오류가 있을 경우 출력 파일을 생성하지 않습니다.
- --strict: 모든 엄격한 타입 검사를 활성화합니다.

### 디버깅 및 로깅 옵션

- --diagnostics: 컴파일 시간을 출력합니다.
- --extendedDiagnostics: 상세 컴파일 시간을 출력합니다.
- --listFiles: 컴파일할 파일 목록을 출력합니다.
- --traceResolution: 모듈 해상도 로그를 출력합니다.


## 추가 및 갱신해야할 내용들

- from scratch 버전 업데이트 필요
- 디버깅 관련 내용

