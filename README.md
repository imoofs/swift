# Swift 프로그래밍 언어

이 문서는 **Swift 프로그래밍 언어**(TSPL, *The Swift Programming Language*)의 원본 소스를 포함하는 저장소에 대한 설명입니다.
Swift 문서를 [docs.swift.org][published]에서 확인할 수 있으며,
본 문서는 [Swift-DocC][docc]를 사용하여 작성되었습니다.

## 기여 방법 (Contributing)

작은 변경 사항,
오타 수정 및 몇 개의 문단만 변경하는 소규모 수정은 **포크(fork) 후 PR(Pull Request)** 을 생성하면 됩니다..

큰 변경 사항,
더 큰 수정이 필요할 경우, 공식적인 기여 프로세스가 **아직 개발 중** 입니다.
**많은 시간을 들여 작성하기 전에**, [Swift forums][forum]에 *pitch thread* 를 시작하여 접근 방식과 잠재적인 문제를 논의하세요.

이 문서는 [Apple Style Guide][asg] 및 **TSPL 스타일 가이드**([this book’s style guide][tspl-style])를 따릅니다..

내용과 관련된 문제는 [GitHub Issues][bugs]에 보고할 수 있습니다.

Swift 프로젝트의 모든 논의 및 기여는 [Swift Code of Conduct][conduct]를 준수해야 합니다.

**자세한 기여 방법은** [Contributing to The Swift Programming Language][contributing] **문서를 참고하세요.**.

[asg]: https://help.apple.com/applestyleguide/
[bugs]: https://github.com/apple/swift-book/issues
[conduct]: https://www.swift.org/code-of-conduct
[contributing]: /CONTRIBUTING.md
[forum]: https://forums.swift.org/c/swift-documentation/92
[tspl-style]: /Style.md
[published]: https://docs.swift.org/swift-book/documentation/the-swift-programming-language/
[docc]: https://github.com/apple/swift-docc
  
---

## 빌드 및 미리보기 (Building & Previewing)  

**Swift-DocC를 사용하여 Swift 문서를 로컬에서 미리 볼 수 있습니다.**  

1️⃣ 저장소의 루트 디렉터리에서 다음 명령을 실행합니다.  
```sh
docc preview TSPL.docc
```

2️⃣ 실행이 완료되면 `docc` 출력에서 제공하는 링크를 열어 **로컬 미리보기** 를 확인할 수 있습니다.  

> 💡 **참고 사항**  
> - **Swift.org에서 툴체인을 다운로드하여 DocC를 설치한 경우**, `docc`는 **툴체인 설치 경로의 `usr/bin/`** 에 위치합니다.  
>   - 따라서 `PATH` 환경 변수를 해당 디렉터리가 포함되도록 설정해야 합니다.  
> - **Xcode를 통해 DocC를 설치한 경우**, 아래 명령어를 대신 사용하세요.  
>   ```sh
>   xcrun docc preview TSPL.docc
>   ```

---

**Swift 문서를 직접 수정하고 기여하는 데 관심이 있다면, 이 가이드를 참고하여 적절한 방식으로 참여하세요!** 🚀  

[published]: https://docs.swift.org/swift-book/documentation/the-swift-programming-language/  
[docc]: https://github.com/apple/swift-docc  
[asg]: https://help.apple.com/applestyleguide/  
[bugs]: https://github.com/apple/swift-book/issues  
[conduct]: https://www.swift.org/code-of-conduct  
[contributing]: /CONTRIBUTING.md  
[forum]: https://forums.swift.org/c/swift-documentation/92  
[tspl-style]: /Style.md  

## Building

Run `docc preview TSPL.docc`
in this repository's root directory.

After running DocC, open the link that `docc` outputs
to display a local preview in your browser.

> Note:
>
> If you installed DocC by downloading a toolchain from Swift.org,
> `docc` is located in `usr/bin/`,
> relative to the installation path of the toolchain.
> Make sure your shell's `PATH` environment variable
> includes that directory.
>
> If you installed DocC by downloading Xcode,
> run `xcrun docc preview TSPL.docc` instead.

