# 우현호 포트폴리오

백엔드 개발자 우현호의 정적 포트폴리오 사이트입니다. 별도의 빌드 단계나 런타임 의존성 없이 GitHub Pages에서 배포됩니다.

## 로컬 확인

저장소 루트에서 다음 명령을 실행합니다.

```bash
python -m http.server 8080
```

브라우저에서 `http://localhost:8080`을 엽니다. 파일을 직접 열 수도 있지만, 실제 배포 환경과 비슷하게 확인하려면 로컬 HTTP 서버 사용을 권장합니다.

## 배포

`main` 브랜치에 변경이 병합되면 `.github/workflows/deploy-pages.yml`이 다음 절차를 수행합니다.

1. 정적 파일 검증
2. GitHub Pages 아티팩트 업로드
3. 프로덕션 Pages 배포

저장소의 **Settings → Pages → Build and deployment → Source**가 **GitHub Actions**로 설정되어 있어야 합니다.

## 운영 점검

- 모든 링크와 연락처가 최신인지 확인
- 모바일과 다크 모드에서 시각 확인
- JavaScript 비활성화 상태에서도 본문이 표시되는지 확인
- PR의 Pages 워크플로 검증 통과 여부 확인
