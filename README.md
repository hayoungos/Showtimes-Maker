# 나만의 상영시간표

정적 사이트(HTML 1개 + 폰트 2개)라서 빌드 설정이 필요 없어요.

## Vercel 배포 (택1)

A. GitHub로 배포
1. 이 폴더를 GitHub 저장소에 올리기
2. vercel.com → Add New → Project → 저장소 Import
3. Framework Preset: Other, Build Command / Output Directory 비워두고 Deploy

B. 터미널로 배포
```
cd vercel-deploy
npx vercel        # 처음엔 로그인/프로젝트 설정 질문에 답하기
npx vercel --prod # 실제 주소로 배포
```

## 저장 방식
- 시간표는 브라우저 localStorage, 스틸컷 이미지는 IndexedDB에 저장돼요.
- 서버로 아무것도 보내지 않아요. 같은 기기·같은 브라우저에서만 이어서 볼 수 있어요.
