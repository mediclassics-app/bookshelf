# Read me Legacy

Github Actions를 이용하여 자동 배포 하기 전 설명. 기록으로 남겨 놓음.

local에서 수동으로 build하여 "/docs" folder에 최종 파일을 넣고 push하였음.

## Deploy

```bash
# git master branch (bookshelf 폴더애서 bash 해야함)
bundle exe jekyll build
# Site located /docs
```

then, `git` `commit` and `push`

build 결과는 `docs` folder 아래 저장됨.

## development

If you want to test pages, you can run this command

```bash
bundle exe jekyll serve
# serve를 하면 build도 됨.
# git push 하기전에도 결과물을 로컬 브라우저에서 미리 확인 할 수 있음
#permission 에러가 날 때는 열려있는 파일이나 폴더를 닫고 다시 시도
```
