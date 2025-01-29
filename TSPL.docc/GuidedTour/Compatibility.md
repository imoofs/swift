# 버전 호환성

이전 언어 모드에서 사용할 수 있는 기능을 알아보기.

이 문서는 **Swift 6**에 대해 설명하며, 이는 **Xcode 16**에 포함된 기본 Swift 버전입니다.  
Swift 6 컴파일러를 사용하면 **Swift 6, Swift 5, Swift 4.2, Swift 4**로 작성된 코드를 빌드할 수 있습니다.

Swift 6 컴파일러를 사용하여 **Swift 5 언어 모드**로 코드를 빌드할 경우,  
Swift 6의 새로운 기능을 일부 활용할 수 있습니다.  
이 기능들은 기본적으로 활성화되어 있거나, 향후 기능 플래그를 통해 사용할 수 있습니다.  
그러나 **엄격한 동시성 검사(strict concurrency checking)** 를 활성화하려면 **Swift 6 언어 모드**로 업그레이드해야 합니다.

추가적으로, **Xcode 15.3**을 사용하여 **Swift 4 및 Swift 4.2** 코드를 빌드할 경우,  
대부분의 **Swift 5 기능**을 여전히 사용할 수 있습니다.  
하지만, 다음과 같은 변경 사항은 **Swift 5 언어 모드**에서만 적용됩니다.  

- **불투명 반환 타입(opaque type)** 을 반환하는 함수는 **Swift 5.1 런타임**이 필요합니다.  
- `try?` 표현식은 이미 옵셔널을 반환하는 경우, **추가적인 옵셔널 레벨을 생성하지 않습니다**.  
- **큰 정수 literal(리터럴) 초기화 표현식**이 올바른 정수 타입으로 자동 추론됩니다.  
  예를 들어, `UInt64(0xffff_ffff_ffff_ffff)`는 올바르게 평가되며 **오버플로우되지 않습니다**.

또한, **동시성(Concurrency)** 기능을 사용하려면 **Swift 5 언어 모드**가 필요하며,  
해당 동시성 타입을 제공하는 **Swift 표준 라이브러리 버전**이 있어야 합니다.  
Apple 플랫폼에서는 다음 최소 **배포 대상(deployment target)** 을 설정해야 합니다.  

- **iOS 13** 이상  
- **macOS 10.15** 이상  
- **tvOS 13** 이상  
- **watchOS 6** 이상  
- **visionOS 1** 이상

Swift 6로 작성된 대상(Target)은 **Swift 5, Swift 4.2, Swift 4**로 작성된 대상과 **상호 의존 가능** 합니다.  
즉, 대규모 프로젝트에서 여러 개의 프레임워크를 사용하고 있다면,  
한 번에 **하나의 프레임워크씩** 새 언어 버전으로 점진적으로 마이그레이션할 수 있습니다.

<!--
This source file is part of the Swift.org open source project

Copyright (c) 2014 - 2022 Apple Inc. and the Swift project authors
Licensed under Apache License v2.0 with Runtime Library Exception

See https://swift.org/LICENSE.txt for license information
See https://swift.org/CONTRIBUTORS.txt for the list of Swift project authors
-->
