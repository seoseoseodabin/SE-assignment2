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
    