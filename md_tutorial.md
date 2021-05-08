# **Markdown Basic Syntax**

<br>

#### 읽기 전에)

- 각 문법마다 사용 예시를 넣어놨으니까 실제 어떻게 표현되는지는 복붙해서 확인해볼 것
- 아래 <간략히 살표보기> 표의 element들을 누르면 해당 문법이 있는 부분으로 이동됨

<br><br><br>

## ***1. Heading***

- **제목**을 나타낼 때 사용  
- **#의 개수**로 크기 조정. 적을수록 크기가 커지며, 레벨 1~6까지 있음  
- #과 제목 사이는 **한 칸 이상** 띄어있어야 함  

      # Heading level 1  
      ## Heading  level 2  
      ### Heading level 3  
      #### Hading level 4  
      ##### Heading level 5  
      ###### Heading level 6  

- **레벨 1과 2**는 **다음 줄에 각각 ==와 --를** 추가하는 방식으로도 사용 가능. 개수는 상관 없음  

      Heading level 1  
      ===============
      Heading level 2  
      ---------------

<br><br>

## ***2. Paragraph***

- **단락**을 나타낼 때 사용
- 단락과 단락 사이에 **빈 줄**을 넣음
- 단락이 리스트에 있지 않은 이상 스페이스나 탭으로 **들여쓰기 하면 안 됨**

      paragraph 1  
      
      paragraph 2  

<br><br>

## ***3. Line Break***

- **줄바꿈** 할 때 사용  
- **두 칸 이상** 띄어쓴 후 다음 줄로 넘어감  

      first line  
      second line

- **HTML의 \<br> 태그**도 대부분의 마크다운 어플리케이션에서 지원함

      first line<br>  
      second line

<br>
<br>

## ***4. Emphasis***

- ## *Bold*  

    - **굵은 글씨**로 강조할 때 사용  
    - 단어나 구의 **앞뒤에 \*\*이나 \_\_을** 붙임  
    - 단, **단어 사이**에 사용할 땐 **\*\*를** 사용하여야 함

        |markdown|rendered|
        |:---:|:---:|
        |\*\*Bold text\*\*|**Bold text**|
        |\_\_Bold text\_\_|__Bold text__|  
        |Thisis\*\*Bold\*\*text|Thisis**Bold**text|

<br>

- ## *Italic*

    - **이탤릭체**(글씨를 기울일 때)에 사용
    - 단어나 구의 **앞뒤에 \*이나 \_을** 붙임
    - 단, **단어 사이**에 사용할 땐 **\*를** 사용하여야 함

        |markdown|rendered|
        |:---:|:---:|
        |\*Italicized text\*|*Italicized text*|
        |\_Italicized text\_|_Italicized text_|
        |Thisis\*Italicized\*text|Thisis*Italicized*text|

<br>

- 두 개를 같이 사용할 땐 **안 쪽에 Italic 표시**가, **바깥 쪽에 Bold 표시**가 오도록 함
- 단, **단어 사이**에 사용할 땐 **\*\*\*만** 써야 함

    |markdown|rendered|
    |:---:|:---:|
    |\*\*\*Italicized bold text\*\*\*|***Italicized bold text***|
    |\_\_\_Italicized bold text\_\_\_|___Italicized bold text___|
    |\*\*\_Italicized bold text\_\*\*|**_Italicized bold text_**|
    |\_\_\*Italicized bold text\*\_\_|__*Italicized bold text*__|
    |Italicized\*\*\*bold\*\*\*text|Italicized***bold***text|
    
<br><br>

## ***5. Blockquote***

- **blockquote**를 표현하기 위해 사용  
- **단락 앞에 \>를** 붙임

      > I'm in blockquote  

- blockquote 안에서 **단락**을 표현할 땐 **단락 사이에 빈줄**을 넣고 **앞에 >을** 붙임

      > First paragraph in blockquote  
      >  
      > Second paragraph in blockquote  

- **중첩된 blockquote**를 사용할 땐 **중첩되는 블록 앞에 >>을** 붙여주면 됨

      > Blockquote  
      >> Nested blockquote  

- blockquote 안에는 **다양한 문법 요소들**이 사용될 수 있음
- 어떤 게 사용 가능한지는 **직접 확인**해봐야 함

      > ## Heading  
      >  
      > - list 1  
      > - list 2  
      >  
      > **Bold** and *Italicized*  

<br><br>

## ***6. List***

- ## *Ordered List*  

    - **순차적으로 번호가 붙은 목록**를 표현할 때 사용  
    - 각 아이템 **앞에 번호와 마침표**를 붙임
    - 앞에 붙는 번호가 꼭 순차적일 필요는 없지만, **반드시 1로 시작**해야 함  
    - 리스트 안에서 **4칸 스페이스나 탭 한 번** 하면 **indented list**도 표현할 수 있음  

          1. first item
          2. second item
              1. indented one
              2. indented two
          3. third item
        
          1. first item  
          4. second item  
          2. third item  
  
          1. first item  
          1. second item  
          1. third item  

<br>

- ## *Unordered List*

    - **순서가 없는 목록**을 표현할 때 사용
    - 각 아이템 앞에 **\-이나 \*, \+을** 붙임
    - 리스트 안에서 **4칸 스페이스나 탭 한 번** 하면 **indented list**도 표현할 수 있음  
    - 같은 리스트를 표현할 땐 **기호를 통일**시키는 것을 권장

          - first item
          - second item
              - indented one
              - indented two
          - third item
        
          * first item  
          * second item  
          * third item  
  
          + first item  
          + second item  
          + third item  

<br>

- **리스트 안에 다른 문법 요소**를 추가할 수 있음  
- **paragraph, blockquote, code block, image, nested list** 등
- 추가할 땐 스페이스나 탭으로 **4칸 들여써야** 함  
- **code block**을 사용할 땐 **보통 4칸** 들여쓰지만, **리스트 안에서는 8칸** 들여써야 함

      - first item
      - second item
      
          a paragraph
      
      - third item

          > a blockquote
      
      - fourth item  

              <html>
                <head>
                  <title>Test</title>
                </head>
      
      - fifth item

          ![What's Markdown?](https://d33wubrfki0l68.cloudfront.net/722f0d393d543949f94038accfbb3887ba9c318b/f6fc0/assets/images/atom.png)
      
      - sixth item  
          1. one
          2. two  
