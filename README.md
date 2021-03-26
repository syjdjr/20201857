# 20201857
## 1. table extention 
- 설명 : table이란 데이터를 행,열에 맞추어 배열하는 것. 
> 
>> #### [표현 방법] : | 사용하기 
>> 1. 행과 열에 맞게 원하는 텍스트 데이터를 기입한다.  
>> 2. line 제일 앞과 뒤, 그리고 데이터들 사이에 |를 넣어 cell을 구분시킨다.  
>> 3. 이때, table은 무조건 **-** *(hyphen)* 을 포함한 **delimiter row**가 있어야 한다. 
> - 주의점 : block 수준의 요소들은 table에 넣을 수 없다. 
> - 주의점 : cell끼리 길이를 맞추지 않아도 된다. 
>
    >> delimiter row 구성 
    >> **[방법1]** : **-** *(hyphen)* 사용하기 
    >> **[방법2]** : **:** *(colon)* 사용하기 
    >> **[방법3]** : 좌 , 우, 가운데,를 각각 할당하여 나타낸다. ???

### 2. task list extention 
- 설명 : 추가적인 수행 단계를 list item들로 나타낼 수 있으며 이는 check box 형태로 표현 된다.  
> #### [표현 방법] : - [ ] 사용하기 
>> 1. **-** 사용하여 task list 임을 알린다. 
>> 2. [ ] 을 사용하는데, 이때 [ ] 안에 space 혹은 글자 **x**를 넣어준다. 이는 checkbox 형태에서 unchecking 혹은 checking 형태로 나타날 것이다.
>> 3. [ ] 뒤에 기입하고자 하는 내용을 넣는다. 
>> 4. 들여쓰기하여 새로운 task list를 만들 수 있다. 

### 3. strike through extention
- 설명 : 추가적인 강조를 할 수 있다. 
> #### [표현 방법] : **~~** 사용하기 
>> 1. 원하는 단어나 구절 앞과 뒤에 ~~를 붙여준다. 

### 4. Autolinks extention
- 설명 : 기존 링크를 더 단순하게 나타내고 hyperlink 해준다. 
> ### [주소의 유형] 
>>  #### 1. www로 시작하는 주소 
>> - www. 은 autolink로 자동 인식 된다.
>> - paragraph 내에서 autolink를 활용할 수 있다. 
>> #### 2. ) 로 끝나는 주소 
>> - )로 끝나는 주소일 경우 삽입 어구의 total number를 이용하여 인지한다. 
>> - autolink 안에 있는 삽입어구는 신경쓰지 않는다. 
>> #### 3. ; 로 끝나는 주소 
>> - &를 이용하여 뒤에 1개 이상의 알파벳 character가 있는 경우 entity reference와 비슷한지 확인해야 한다. 
>> - entity reference는 autolink에서 제외 된다. 
> 주의 : 주소에는 space 와 -< character가 없어야 한다. 

### [ URL ]
> - http:// 혹은 https:// 중 하나일때 URL이 인식된다. 
> - URL에는 space 와 -< character가 없어야 한다. 

#### [email]
> - text node 1개 이상 있을 때 인지된다. 
*text node : alphanumeric 혹은 . - _ + @*
** alphanumeric과 - _ 는 한개 이상의 .을 가지고 있어야 인지된다** 
> - 이때, text node 중  - 와 _ 는 맨 끝의 character가 되서는 안된다.  

>> - Trailing punctiation 은 autolink로 고려되지 않는다. 
    >>> * trailing punctiation: . ? ! , : * _ ~
>> 

### 5. Disallowed Raw HTML extention
- 설명 : HTML 태그를 이용하여 HTML 산출물들을 제공할 수 있다. 
> #### [표현 방법] : < > 사용하기
>> 1. < >를 사용하여 태그를 나타낸다. 
