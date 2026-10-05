# 중기메니저 Windows 배포

이 저장소는 **설치파일과 자동 업데이트용 Release만 관리**합니다.

## 현재 최신 버전

**v1.2.14**

- 최신 Release: https://github.com/fqhdtn-lgtm/junggi-manager-releases/releases/latest
- 설치파일: `JunggiManager-Setup-1.2.14.exe`
- 자동 업데이트 정보: `update.json`
- 이전 버전 Release는 롤백/기록용이며 새 설치에는 사용하지 않습니다.

## 소스 기준

개발 소스는 `fqhdtn-lgtm/junggi_manager`에서 관리합니다.

현재 v1.2.14 기준 소스는 **PR #47 `[CURRENT] 중기메니저 v1.2.14 기준 소스`**로 표시해 두었습니다.
이전 버전용 임시 배포 워크플로는 모두 제거했습니다.

## 배포 원칙

1. 실제 사용할 소스 상태를 먼저 GitHub에 보존합니다.
2. `pubspec.yaml` 버전과 `lib/app_version.dart` 버전을 동일하게 맞춥니다.
3. Windows Release 설치파일을 빌드하고 해시를 검증합니다.
4. Release에는 설치파일, `SHA256SUMS.txt`, `update.json` 세 파일만 올립니다.
5. 배포 완료 후 `releases/latest`가 새 버전을 가리키는지 확인합니다.

설치 후 프로그램의 **업데이트 확인** 버튼으로 새 버전을 받을 수 있습니다.
