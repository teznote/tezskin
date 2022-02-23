# tezskin

## 사용법

Github Pages 를 생성하고, _config.yaml 파일에 아래 내용을 포함합니다.

```
title: # 사이트 이름
desc: # 사이트 설명
footer: # Footer 설명
url: # 사이트 주소
cats: # Nav 에 표시되는 순서, docs 폴더 하위의 폴더 이름을 표시되고자 하는 순서대로 나열한다 ex) ["cat_1", "cat2", "another cat"]

markdown: kramdown # highlight JS 를 쓰기로 했다. 기본 하이라이터를 사용하면 style 이 제대로 먹히지 않는다.
kramdown:
    syntax_highlighter_opts:
        disable: true
```

docs 폴더는 아래와 같은 구조로 page 를 나열해야 한다.

```plaintext
/docs
  + cat_1
    + 0001_page.md
    + 0002_page.md
    + 0003_page.md
    + 0004_page.md
  + cat_2
    + 0001_another.md
    + 0002_another.md
```

그리고 page 가 되는 md 파일의 formatter 는 아래 내용이 들어가야 한다.

```yaml
layout: default            # 고정값
title: "원하는 타이틀"      # 따옴표 안에 page title 기입
updated: 2021-02-12        # 날짜 형식 텍스트
permalink: /cat0010-0010   # 이 페이지의 url 경로
```

## 2022-02-13 - 2

Highlight JS 를 cdn 으로 붙였다.

## 2022-02-13

nav 를 만들어 붙이고, liquid 템플릿으로 적절히 전체 구조를 묶어주었다.

어느정도 디자인도 적절히 입혀보았다. 이정도면 일단은 테마로써 최소한의 기능은 갖춘 것 같다.

## 2022-02-12 - 2

main contents 스타일을 만들어 붙였다.

지금 운영하고 있는 style 을 그대로 옮기되, 누더기 처럼 되어 있는 코드 정리도 했다.

## 2022-02-12

Github Pages 에서 사용할 수 있는 Jekyll 테마를 제작해보고 있습니다.

현재까지는 Layout 과 Button 을 만들어서 적용시켜 보았습니다.

나중에는 개인블로그에 적용시켜 볼 예정입니다.