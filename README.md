# Supertamer

혼자 제품을 만드는 사람의 제품 빌딩 동반자 — macOS 네이티브 앱입니다.

이 저장소는 베타 빌드 배포용입니다. 최신 빌드는 [Releases](https://github.com/secondstagehq/supertamer/releases)에서 받으세요.

## 설치

1. 최신 릴리즈에서 `Supertamer.zip`을 내려받아 압축을 풉니다.
2. `Supertamer.app`을 `/Applications`로 옮깁니다.
3. 이 베타는 공증(notarization)되지 않았습니다. 첫 실행이 차단되면 다음 중 하나로 엽니다.
   - 시스템 설정 → 개인정보 보호 및 보안 → "확인 없이 열기"
   - 또는 터미널에서:

     ```bash
     xattr -dr com.apple.quarantine /Applications/Supertamer.app
     ```

## 요구 사항

- macOS (Apple Silicon / Intel universal 바이너리)
