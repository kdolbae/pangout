# 팡아웃 · PANG OUT

팡아웃 디자인 브리프를 바탕으로 제작한 반응형 홈페이지 시안입니다. 벽 단면을 중심으로 슬레이트와 앰버 색상을 사용합니다.

## 파일 구성

- `dist/index.html`: 홈페이지 전체(스타일·스크립트 포함, 한 파일)
- `dist/photos/`: 시공 사진. 지금은 AI로 만든 연출 이미지이며, 실제 현장 사진이 생기면 같은 파일 이름으로 교체
- `dist/jd-logo.png`: 집대리 협력업체 배너 로고
- `wrangler.jsonc`: Cloudflare Workers 정적 배포 설정

## 실행

```sh
python -m http.server 8000 --directory dist
```

## 배포 (Cloudflare)

```sh
npx wrangler deploy
```

`wrangler.jsonc`의 routes로 pangout.kr, www.pangout.kr 에 연결됩니다(도메인은 같은 Cloudflare 계정에 있어야 함).

## 운영 메모

- 상담은 카카오톡 채널(https://pf.kakao.com/_jxhyZX/chat)로 연결합니다. 문의 폼은 메모를 만들어 복사만 하고 서버로 보내지 않습니다.
- 열화상 온도 수치는 설명용 예시입니다.
- 단열 기본 55,000원/㎡(VAT 별도, 최소 450,000원), 단열 강화와 탄성 코팅·곰팡이 제거는 현장 견적입니다.
