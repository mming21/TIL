# [markdown]

가능한 읽을 수 있도록 최소한의 문법으로 구조화한 마크업 언어

ex. README.md, 기술 블로그 등


## Heading

1. 문서의 제목이나 소제목으로 사용
2. #의 개수에 따라 대응되는 수준(Heading level)이 있으며, h1~h6까지 표현 가능
3. 문서의 구조를 위해 작성되며 글자크기를 조절하기 위해 사용되어서는 안됨


## List

1. 순서가 있는 리스트(ol)(앞에 번호가 뜸)와 순서가 없는 리스트(ul)(순서가 없음)로 구성

2. #의 개수에 따라 대응되는 수준(Heading level)이 있으며, h1~h6까지 표현 가능


## Fenced Code Block

1. 코드 블록은 backtick 기호 3개를 활용하여 작성(``` ```)

2. 코드 블록에 특정언어를 명시하면 Syntax Highlighting 적용 가능

3. 일부 환경에서는 적용이 되지 않을 수 있음

  ```java
 class MySumTest {
    public static void main(String args[]){
        int i = 10;
        int j = 20;
        
        MySum ms1 = new MySum(i, j);
        MySum ms2 = new MySum(j, i);

        System.out.println(ms1);//30
        System.out.println(ms2);//30

        if(ms1.equals(ms2)) {
            System.out.println("ms1과 ms2의 합계는 동일합니다.");
	}
    }
}
  ```

## Inline Code Block

backtick 기호 1개를 인라인에 활용하여 작성
`class MySumTest`


## Link 

* url을 통해 링크 작성가능

* 특정파일들 포함하여 연결시킬 수도 있음

  https://youtu.be/xdzKVzMuzUs


## Image

![문자열](url)을 통해 이미지를 사용가능
![문자열](https://cgeimage.commutil.kr/phpwas/restmb_allidxmake.php?idx=3&simg=20210215161822074978a9710824910624586229.jpg)


## Blockquotes

>학교라는 감옥에 갇혀 

ex. > blah blah

## Table

| 사과 | 복숭아 |
| :---: | :---: |


## text 강조

굵게(__굵게__), 기울임(*기울임*)을 통해 특정 글자들을 강조

__여름이었다.__
*피사의 사탑*


## 수평선

3개 이상의 asterisks*** dashes--- underscores___ 선 작성

ex. 구분선

-------------------------





