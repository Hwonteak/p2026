# 이원택 후보 캠페인 홈페이지

전북특별자치도지사 후보 이원택 (제9회 전국동시지방선거) 캠페인 홈페이지 소스코드입니다.

## 📁 파일 구조

```
이원택_홈페이지/
├── README.md           ← 이 파일 (GitHub에 업로드 불필요)
├── index.html          ← 메인 페이지
└── images/
    ├── hero.jpg        ← 메인 포스터 ("기회를 주십시오")
    ├── share.jpg       ← 카카오톡·SNS 공유 미리보기
    └── together.png    ← 이재명·이원택 사진 (민주당 원팀 카드)
```

## 🚀 GitHub 업로드 방법 (반드시 이 구조대로)

### 권장 방법: GitHub Desktop 사용

가장 확실하고 실수가 없는 방법입니다.

1. [https://desktop.github.com](https://desktop.github.com) 다운로드 및 설치
2. GitHub 계정 로그인
3. **File → Clone repository** → 본인 저장소 (1taek) 클론
4. 클론된 폴더 열기 (Windows: 파일 탐색기 / Mac: Finder)
5. 압축 해제한 이 폴더의 **모든 내용물을 복사**해서 클론 폴더에 **붙여넣기** (덮어쓰기)
   - `index.html` 파일
   - `images` 폴더
   - (README.md는 굳이 안 올려도 됨)
6. GitHub Desktop에 돌아오면 변경사항이 자동으로 감지됨
7. 하단 **Summary** 칸에 "사이트 업데이트" 같은 메시지 입력
8. **Commit to main** 클릭
9. 우상단 **Push origin** 클릭
10. 1분 정도 후 Vercel이 자동 재배포

### 대체 방법: GitHub 웹사이트에서 직접 업로드

1. 본인 GitHub 저장소 페이지 접속 (예: github.com/leewontaek/1taek)
2. 우상단 **Add file → Upload files** 클릭
3. **드래그앤드롭 영역에**:
   - `index.html` 파일을 드래그
   - **그리고 `images` 폴더 전체를 폴더째로 드래그**
4. 하단 파일 목록에서 다음과 같이 보여야 함:
   ```
   index.html
   images/hero.jpg
   images/share.jpg
   images/together.png
   ```
   ⚠️ 만약 `hero.jpg`처럼 `images/` 없이 보이면 잘못된 것 → 취소하고 다시 시도
5. 페이지 하단 **Commit changes** 클릭

## ✅ 배포 후 점검 (필수)

업로드 1분 후 브라우저에서:

| 점검 URL | 정상 결과 |
|---------|----------|
| https://1taek.vercel.app/ | 메인 페이지가 정상 표시 |
| https://1taek.vercel.app/images/hero.jpg | 메인 포스터 이미지 단독 표시 |
| https://1taek.vercel.app/images/share.jpg | 공유용 이미지 단독 표시 |
| https://1taek.vercel.app/images/together.png | 이재명·이원택 사진 단독 표시 |

위 4개 URL 모두 정상이면 배포 성공입니다.

## 💬 카카오톡 미리보기 활성화

배포 후, 카카오톡에 사이트 링크를 붙여넣을 때 미리보기 이미지가 보이게 하려면:

1. [https://developers.kakao.com/tool/clear/og](https://developers.kakao.com/tool/clear/og) 접속
2. URL 입력: `https://1taek.vercel.app/`
3. **캐시 초기화** 버튼 클릭
4. 1~2분 후 카카오톡에 사이트 링크 보내보기 → 미리보기 정상 표시

> ⚠️ 이미지 점검(위 단계)이 먼저 성공해야 카톡 미리보기도 작동합니다.

## 🔧 자주 발생하는 문제

### 이미지가 안 나옴

**원인**: GitHub에 `images/` 폴더가 누락 또는 잘못된 위치에 업로드됨

**해결**:
1. GitHub 저장소 페이지에서 `images/` 폴더가 보이는지 확인
2. 폴더 클릭해서 안에 hero.jpg, share.jpg, together.png 3개 파일이 있는지 확인
3. 없으면 GitHub Desktop 사용해서 다시 업로드

### 사이트가 옛날 버전으로 보임

**원인**: 브라우저 캐시

**해결**: 강제 새로고침
- PC: `Ctrl + Shift + R` (Mac: `Cmd + Shift + R`)
- 모바일: 시크릿/프라이빗 모드로 접속

### 카톡에 옛날 미리보기 이미지가 뜸

**원인**: 카카오톡 서버의 OG 캐시

**해결**: 위 "카카오톡 미리보기 활성화" 단계에서 캐시 초기화

## 📝 페이지에 포함된 기능

- ✅ 핵심 메시지 (민주당 원팀 vs 무소속 비교)
- ✅ 3대 핵심 약속 (원팀의 힘 · 100년 먹거리 · 농민수당)
- ✅ 14개 시·군별 공약 (선거공보 기준)
- ✅ 6개 세대·계층별 공약 (청년·여성·어르신·농어민·장애인·문화)
- ✅ 사전투표 안내 (5월 29~30일)
- ✅ 우리집 주소 → 가장 가까운 사전투표소 찾기 (전북 243개 데이터)
- ✅ Open Graph 메타태그 (SNS 공유 미리보기)
- ✅ 모바일 최적화 (40-50대 친화 큰 폰트)

## 📞 캠프 정보

- 선거사무소: 전북특별자치도 전주시 완산구 백제대로 336
- 전화: 063-224-0036
- 팩스: 063-254-8258

## 📜 데이터 출처

- 지역별/세대별 공약: 「제9회 전국동시지방선거 책자형선거공보」(2026.05.06)
- 사전투표소 정보: 중앙선거관리위원회 공식 자료
