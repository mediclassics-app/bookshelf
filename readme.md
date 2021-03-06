# 사용 설명

## 서적 편집

### 서적이 추가된 경우

#### 서적 데이터 편집

`_data/distBook.yml`, `_data/eBook.yml`, `_data/paperBook.yml` 가운데 알맞은 파일에 원하는 서적의 정보를 추가한다.

이때 bookid는 서적의 주소가 되므로 영문과 숫자로 정한다.

#### 서적 파일 추가

`books/distBook`, `books/eBook`, `books/paperBook` 가운데 알맞은 폴더 아래 bookid와 동일한 폴더를 만든다. 그런 다음 아래 파일을 추가한다. 이때 파일 이름을 아래와 같이 맞춰 주어야 한다.

* 책의 표지 : `cover_small.png`
* 배포할 책의 파일 : `book.epub`, `book.pdf`


### 서적이 삭제되거나 변경된 경우

#### 서적 데이터 편집

편집하거나 삭제하고자 하는 서적의 정보를 `_data/distBook.yml`, `_data/eBook.yml`, `_data/paperBook.yml` 가운데에서 수정하거나 삭제한다.


#### 서적 파일 편집

편집하거나 삭제하고자 하는 파일을 `books/distBook`, `books/eBook`, `books/paperBook` 가운데에서 찾아 수정하거나 삭제한다.


***

## deploy

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

***

## freq command

```bash
mogrify -format png **/*.jpg
```
