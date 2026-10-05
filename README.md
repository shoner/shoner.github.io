# Shoner's It Blog

[Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) Jekyll 테마 기반 개인 블로그입니다. → <https://shoner.github.io>

[Chirpy Starter](https://github.com/cotes2020/chirpy-starter) 구조를 따르며, 테마 파일은 `jekyll-theme-chirpy` gem에서 가져옵니다.

## 글 쓰기

`_posts/YYYY-MM-DD-제목.md` 파일을 만들고 맨 위에 front matter를 넣습니다.

```yaml
---
title: 글 제목
date: 2026-10-05 21:00:00 +0900
categories: [대분류, 소분류]
tags: [태그1, 태그2]
---
```

## 로컬에서 미리보기

```shell
bundle install
bash tools/run.sh      # http://127.0.0.1:4000
bash tools/test.sh     # 프로덕션 빌드 + 링크 검사
```

## 배포

`main` 브랜치에 push하면 GitHub Actions(`.github/workflows/pages-deploy.yml`)가 빌드해서 GitHub Pages로 배포합니다.
저장소 **Settings → Pages → Source** 가 **GitHub Actions** 로 설정되어 있어야 합니다.

## 문서

- [Chirpy 테마 문서](https://github.com/cotes2020/jekyll-theme-chirpy/wiki)
