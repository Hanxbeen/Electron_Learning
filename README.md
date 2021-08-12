# Electron_Learning
Electron tutorial for proficiency

2021.08.12
ERP Desktop Application 개발을 위한 Electron 학습 시작

Electron 개발을 위해서는 Node 및 NPM이 설치되어 있어야합니다.

## Electron 개발환경 설정
* node --version
* npm --version

이미 설치돼있다면 버전을 확인하고 없다면 설치를 합니다.

npm을 사용해서 프로젝트를 생성할 때마다 프로젝트에 대한 모든 세부정보가 포함된 package.json 파일을 제공해야 합니다.
npm을 통해서 쉽게 설정해봅시다

* npm init

패키지 이름부터, 버전, 설명, 레포지토리, 작성자 등 다양한 정보들을 입력할 수 있습니다.

## Electron 설치
이제 일렉트론을 전역에 설치하겠습니다.

* npm install -g electron

실행 후 설치가 완료되면 다음 명령을 실행하여 올바르게 설치되었는지 확인할 수 있습니다.

* electron --version


이제 일렉트론을 사용해 첫 번째 앱을 개발해보겠습니다.
