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

아래 명령으로 local에서 오류 확인 후에 단순히 commit & push 하면 됨. 

```
bundle exe jekyll serve
```

***

## freq command

```bash
mogrify -format png **/*.jpg
```

***

## Log

2022-05-30
* Github Actions을 이용하여 배포 과정을 자동화 하였음
* updated ruby & gem version 