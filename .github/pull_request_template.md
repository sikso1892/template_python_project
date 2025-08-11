# PR 제목 규칙
* 형식: `<type>: <subject>` 혹은 `<type>: <issueID>, <subject>`
* `type`은 소문자 시작, 브랜치 타입과 일치.
* 예시:

  * `feat: DD-185, optimize image processing engine`
  * `fix: handle empty payload in webhook`

# 리뷰/PR 운영 원칙

* **Draft PR**: 추가 작업 필요 시 리뷰어 지정 없이 Draft로 생성.
* **근거 제시**: 취향성 변경 지양. 요청 시 구체·명확한 근거 첨부.
* **\[nitpick]**: 중요도 낮은 제안에만 사용. 작성자가 반영 여부 결정 후 resolve.
* **Approve**: 더 이상 리뷰 불필요하고 devel 병합 가능하면 승인.

# PR 템플릿 (복사해 사용)

```markdown
## What has changed
1. <무엇을 했다 한 줄 요약>
2. <예: Optimize LID inference using batch processing>
3. <...>

## Additional info
- <맥락/설계 결정/참고 링크>

## Checklist
- [ ] Target branch: devel
- [ ] Tests: 작성/수행 완료 (pytest 등)
- [ ] Lint/Format: 통과 (black/isort/flake8 or ruff)
- [ ] Docs/Changelog: 필요한 경우 업데이트
- [ ] Dependencies: 변경 시 명시

## Changelog (선택)
- Added:
- Changed:
- Fixed:
- Deprecated/Removed:
- Security:
- Breaking Changes: (필수 시) `BREAKING CHANGE: ...`
```

# Type(제목 prefix) 목록

* `feat` 새 기능
* `fix` 버그 수정
* `perf` 성능 개선
* `refactor` 리팩토링(기능 변화 없음)
* `style` 포맷/스타일(의미 변화 없음)
* `test` 테스트 추가/수정
* `docs` 문서
* `build` 빌드/의존성
* `ci` CI 워크플로우
* `chore` 잡무/정리
* `i18n` 다국어/현지화
* `BREAKING CHANGE` 호환성 깨짐(제목 맨 앞 태그)
* `WIP` 진행 중(임시 라벨/제목 접두)

# 자주 쓰는 리뷰 코멘트 약어 (영어; 한글)
* **LGTM** (Looks good to me; 좋아 보입니다)
* **PTAL** (Please take a look; 확인 부탁드립니다)
* **WDYT** (What do you think?; 의견 어떠신가요?)
* **IMO/IMHO** (In my (humble) opinion; 개인적 의견입니다)
* **FYI** (For your information; 참고용입니다)
* **WIP** (Work in progress; 작업 중)
* **DNM** (Do not merge; 병합 금지)
* **RFC** (Request for comments; 의견 요청)
* **ACK / NACK** (승인 / 반대)
* **SGTM** (Sounds good to me; 좋아 보입니다)
* **TBD/TBA** (결정/공지 예정)
* **ETA** (Estimated time of arrival; 예상 완료 시점)
* **QoL** (Quality of Life; 사용성 개선)
* **NFC** (No functional change; 기능 변화 없음)
* **nit / nitpick** (사소한 제안; 중요도 낮음)
* **opt** (Optional; 선택 사항)
* **q:** (Question; 질문)
* **blk:** (Blocking; 병합 전 반드시 반영 필요)
* **suggest:** (수정 제안)
* **note / nb:** (참고 메모)
