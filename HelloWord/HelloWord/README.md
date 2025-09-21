//
// README.md
// HelloWord
//
// Created by otk on 9/21/25.
//

## 프로젝트 파일들 살펴보기

```
HelloWorld/                     <-- 프로젝트 루트 폴더
├── HelloWorld.xcodeproj/       <-- Xcode 프로젝트 설정 파일
│   └── project.pbxproj         <-- 빌드/구성 정보
│
├── HelloWorld/                 <-- 앱 소스 코드 폴더
│   ├── AppDelegate.swift       <-- (UIKit 기반일 때 주로 생성됨, SwiftUI는 보통 없음)
│   ├── ContentView.swift       <-- SwiftUI의 기본 뷰
│   ├── HelloWorldApp.swift     <-- 앱의 시작점 (@main, SwiftUI 진입)
│   └── Assets.xcassets/        <-- 앱 리소스 (아이콘, 이미지 등)
│       └── AppIcon.appiconset/ <-- 앱 아이콘
│
├── HelloWorldTests/            <-- 유닛 테스트 타겟
│   └── HelloWorldTests.swift
│
├── HelloWorldUITests/          <-- UI 테스트 타겟
│   └── HelloWorldUITests.swift
│
├── Preview Content/            <-- SwiftUI 미리보기 리소스
│   └── Preview Assets.xcassets/
│
├── README.md                   <-- 프로젝트 설명
├── .gitignore                  <-- Git 무시 규칙
└── Package.swift (옵션)        <-- Swift Package Manager 쓰는 경우



```

1. AppDelegate.swift
   > 앱의 실행 주기(Life Cycle)를 관리하는 내용의 스위프트 소스 코드가 들어 있는 클래스 파일

앱을 실행하거나 종료 또는 백그라운드를 실행할 때 하는 일들을 관리합니다. 일반적으로 초보 단계일 때는 프로그래머가 직접 코딩하지 않아도 됩니다.

2. SceneDelegate.swift

   > 사용자 인터페이스(Usr Interface; UI)의 실핼주기(Life Cycle) 관리하는 내용의 Swift 소스코드가 들어 있는 클래스 파일

3. ViewController.swift
   > 화면에 보이는 뷰에서 처리하는 내용의 Swift 소스 코드를 잠고 있는 클래스 파일

이 파일에서 코딩을 하게 되며 뷰 하나당 클래스 하나가 대응이 됩니다. 그러므로 스토리보드에서 여러 개의 뷰를 추가하면 뷰의 개수만큼 뷰 컨트롤러 클래스 파일이 필요하게 됩니다.

4. Assets.xcassets
   > 앱의 아이콘을 보관하는 저장소

이공ㅅ에서 앱 아이콘을 설정해야 원하는 앱 아이콘으로 표시할 수 있습니다.

5. LaunchScreen.storyboard

   > 앱이 실행될 때 잠시 나타나는 스플래시 화면을 만드는 `스토리보드`

6. Info.plist
   > 앱이 실행되는 데 필요한 정보를 저장하고 있는 파일
