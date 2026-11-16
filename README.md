# R Comp Tech Homepage

정적 HTML 홈페이지입니다. GitHub Pages로 배포합니다.

## 파일 구성
| 파일 | 역할 |
|---|---|
| `index.html` | 메인 페이지 (R Comp Tech 타이틀 + 공지사항 링크) |
| `notice.html` | 공지사항 · 공고 목록 페이지 |
| `style.css` | 공통 스타일 |

## 배포 (GitHub Pages)
1. 파일들을 저장소 최상위(root)에 올립니다.
2. 저장소 **Settings → Pages** 로 이동합니다.
3. **Source: Deploy from a branch**, Branch: `main` / `/ (root)` 선택 후 Save.
4. 1~2분 뒤 `https://<아이디>.github.io/<저장소명>/` 에서 확인합니다.

## 공지 추가 방법
`notice.html` 안의 `notices` 배열 맨 위에 항목을 추가하면 됩니다.

```js
{
  type: "공지",            // "공지" 또는 "공고"
  title: "제목",
  date: "2026-12-01",
  body: "본문 내용 (줄바꿈은 \n)"
},
```

## 커스텀 도메인
보유한 도메인을 연결하려면 Settings → Pages → Custom domain에 입력하고,
도메인 업체 DNS에 GitHub Pages용 레코드(CNAME 또는 A 레코드)를 추가하세요.
