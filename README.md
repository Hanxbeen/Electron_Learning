# Electron_Learning
Electron tutorial for proficiency

2021.08.12
ERP Desktop Application 개발을 위한 Electron 학습 시작

Electron 개발을 위해서는 Node 및 NPM이 설치되어 있어야합니다.

## Electron 개발환경 설정
* node --version
* npm --version

이미 설치돼있다면 버전을 확인하고 없다면 설치를 합니다.

$ node --version
v14.17.4

$ npm --version
6.14.14

npm을 사용해서 프로젝트를 생성할 때마다 프로젝트에 대한 모든 세부정보가 포함된 package.json 파일을 제공해야 합니다.
npm을 통해서 쉽게 설정해봅시다

* npm init

패키지 이름부터, 버전, 설명, 레포지토리, 작성자 등 다양한 정보들을 입력할 수 있습니다.

John@DESKTOP-DLNQO69 MINGW64 /c/SynologyDrive/Electron_Learning/Electron_Learning 
(feature/tutorial)
$ npm init
This utility will walk you through creating a package.json file.
It only covers the most common items, and tries to guess sensible defaults.

See `npm help init` for definitive documentation on these fields
and exactly what they do.

Use `npm install <pkg>` afterwards to install a package and
save it as a dependency in the package.json file.

Press ^C at any time to quit.
package name: (electron_learning)
version: (1.0.0)
description: tutorial
entry point: (index.js)
test command: test
git repository: (https://github.com/Hanxbeen/Electron_Learning.git)
keywords: study
author: hanxbeen
license: (ISC) MIT
About to write to C:\SynologyDrive\Electron_Learning\Electron_Learning\package.json:

{
  "name": "electron_learning",
  "version": "1.0.0",
  "description": "tutorial",
  "main": "index.js",
  "scripts": {
    "test": "test"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/Hanxbeen/Electron_Learning.git"
  },
  "keywords": [
    "study"
  ],
  "author": "hanxbeen",
  "license": "MIT",
  "bugs": {
    "url": "https://github.com/Hanxbeen/Electron_Learning/issues"
  },
  "homepage": "https://github.com/Hanxbeen/Electron_Learning#readme"
}


Is this OK? (yes) yes
## Electron 설치
이제 일렉트론을 전역에 설치하겠습니다.

* npm install -g electron

실행 후 설치가 완료되면 다음 명령을 실행하여 올바르게 설치되었는지 확인할 수 있습니다.

* electron --version
$ electron --version

v1.4.13

## Electron 작동원리

Electron은 package.json 파일에 정의된 기본 파일을 가져와 실행하게됩니다.

이 기본 파일은 Rendering된 웹 페이지와 운영체제의 기본 GUI와의 상호작용을 포함하는 응용프로그램 창을 생성합니다

Elcetron을 사용하여 애플리케이션을 시작하면 Main Process가 생성됩니다.
이 Main Process는 운영체제의 기본 GUI와 상호작용하는 역할을 하며, 애플리케이션의 GUI를 생성합니다.
