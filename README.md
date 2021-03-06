<a href="https://github.com/hanakim120/e-book-text-mining"><img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fhanakim120%2Fe-book-text-mining&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false"/></a>
<p>
<h1 align="center">π Text mining project π<br>
: λ νΈμ e-book dataμ κ°μ λΆμ κ²°κ³Όμ<br> μ±μ κ²°λ§ μ¬μ΄ κ΄κ³ μ°κ΅¬ </h1>
</p>

## π Quick overview
<p  align="center">
<strong>Text mining μ ν΅ν΄ μ±μ μ λ°μ μΈ κ°μ λΆμ κ²°κ³Όμ μ±μ κ²°λ§ μ¬μ΄μλ μ΄λ€ κ΄κ³κ° μλμ§ μμλ³΄κ³ μ νλ€.</strong><br>
λ³΄ν΅ μ±μ κ²°λ§μ μ±μ λ§¨ λ§μ§λ§ λ¬Έλ¨ νΉμ λ§μ§λ§ λ¬Έμ₯μ λ³΄λ©΄ μ μ μλ€κ³  κ°μ νλ€.
</p>

<p  align="center">
<img  src="./image/μ°κ΅¬λ°°κ²½.png"  width="60%"  align="middle"/>
</p>

1) **νμ€νΈ λ°μ΄ν° μμ§**
> νμ€νΈ λ°μ΄ν°λ Project Gutenberg μμ λ¬΄λ£λ‘ μ κ³΅νλ e-book λ°μ΄ν°λ₯Ό μ¬μ©.<br>
λΉκ΅λ₯Ό μν΄ λνμ μΈ ν΄νΌμλ©κ³Ό μλμλ©μ κ°μ§ μ± 2κΆμ νμ€νΈ λ°μ΄ν°λ₯Ό μ¬μ©νμλ€.

2) **Data Preprocessing**
>  μ«μ νν, κ³ μ  λͺμ¬, νΉμλ¬Έμ μ¬μ© μ νμ λ¨μ΄ μ΄νΌκΈ° λ± 

3) **EDA**
>  DTM κ΅¬μΆ, λΉλν, λμ  λΉλ κ³μ°, WordCloud κ·Έλ¦¬κΈ°

4) **κ°μ  λΆμ**
 > `textdata` λΌμ΄λΈλ¬λ¦¬μ λ΄μ₯λμ΄ μλ μ¬μ  λ°μ΄ν°(dictionary-based)λ₯Ό νμ©νμ¬ κ°μ λΆμ

- μμΈν λ΄μ©μ μλ μ΅μ’ λ°ν μλ£λ₯Ό μ°Έκ³ ν΄μ£ΌμΈμ

  
## ππ»ββοΈ λ°ν μλ£


- μ΅μ’ λ°ν μλ£ ([link](https://github.com/hanakim120/e-book-text-mining/blob/main/Text_mining_project.pdf))

## π οΈ Skills
- R 3.6.1 

- μ¬μ©ν library 
	- tm, tidyverse, stringr, topicmodels, wordcloud, RColorBrewer, tidytext, dplyr


## ποΈ μ¬μ©ν λ°μ΄ν°

### Raw λ°μ΄ν° μμ§ κ²½λ‘ 

-   Project Gutenberg μμ λ¬΄λ£λ‘ μ κ³΅νλ e-book λ°μ΄ν°λ₯Ό μ¬μ©. ([project gutenberg](https://www.gutenberg.org/))
1) The Strange Case of Dr. Jekyll and Mr. Hyde by Robert Louis Stevenson
2) Cinderella by Henry W. Hewet
<p  align="center">
<img  src="./image/project_gutenberg.png"  width="60%"  align="middle"/>
</p>


## π  Data preprocessing

1. λ§λ­μΉμ λ±μ₯ν μ«μννλ€μ λͺ¨λ μ­μ .  
2. λ§λ­μΉμ μ¬μ©λ νΉμλ¬Έμλ€μ κ²½μ° λ λ¨κ³λ₯Ό ν΅ν΄ μ¬μ μ²λ¦¬.
	- α. νμ λ°λΌ λͺλͺ ννλ€μ κ΅μ²΄.
	- α. 2-αμ ν΄λΉλμ§ μλ νΉμλ¬Έμλ€μ μΌκ΄ μ­μ .  
	
	
|jekyll data|Cinderella data|
|:-:|:-:|
|![firstimage](./image/jekyll_after.png)|![Second Image](./image/cinderella.png)|
	

3. 2λ² μ΄μ μ°μ΄μ΄ λνλ κ³΅λλ€μ νλμ μ€νμ΄μ€ κ³΅λ(β β)μΌλ‘ λ°κΏ. 
5. λλ¬Έμλ‘ λνλ νμ€νΈλ λͺ¨λ μλ¬Έμλ‘ μ ν.  
6. tm λΌμ΄λΈλ¬λ¦¬μ νμ¬λ SMART λΆμ©λ¬Έμ λͺ©λ‘μ ν¬ν¨λμ΄ μλ λ¨μ΄λ€μ λͺ¨λ μ­μ .  
7. μ΄κ·Όμ΄ λμΌνμ§λ§ λ¬Έλ²μ μΌλ‘ λ³μ©λ λ¨μ΄λ€μ ν΅ν©νλ μ΄κ·Ό λμΌν μκ³ λ¦¬μ¦μ μ μ©.


## π EDA
### WordCloud
DTM μ κ΅¬μΆνκ³  λμ  λΉλμλ₯Ό κ³μ°νμ¬ κ°μ₯ μμ£Ό λ±μ₯νλ¨μ΄λ₯Ό 1~20λ± μ΄ν΄λ³Έλ€. 

|jekyll DTM|Cinderella DTM|
|:-:|:-:|
|![firstimage](./image/jekyll_dtm.png)|![Second Image](./image/cinderella_dtm.png)|
	

|jekyll λ°μ΄ν°μ WordCloud|Cinderella λ°μ΄ν°μ WordCloud|
|:-:|:-:|
|![firstimage](./image/jekyll_wordcloud.png)|![Second Image](./image/cinderella_wordcloud.png)|	


## π€ κ°μ λΆμ 
	
|jekyll λ°μ΄ν°μ κ°μ λΆμ κ²°κ³Ό<br> κΈμ μ μΈ λ¨μ΄λ³΄λ€ λΆμ μ μΈ λ¨μ΄κ° 237κ° λ λ§μ΄ λμ΄|cinderella λ°μ΄ν°μ κ°μ λΆμ κ²°κ³Ό<br> λΆμ μ μΈ λ¨μ΄λ³΄λ€ κΈμ μ μΈ λ¨μ΄κ° 97κ° λ λ§μ΄ λμ΄|
|:-:|:-:|
|![firstimage](./image/jekyll_sentiment.png)|![Second Image](./image/cinderella_sentiment.png)|
	

## π» Results 

- μλμλ©μΈ μ±μ μ λ°μ μΌλ‘ λΆμ μ μΈ λ¨μ΄κ° λ§μ΄ λ±μ₯  
- ν΄νΌμλ©μΈ μ±μ μ λ°μ μΌλ‘ κΈμ μ μΈ λ¨μ΄κ° λ§μ΄ λ±μ₯

> νμ€νΈ λ°μ΄ν°λ₯Ό λ κΆμΌλ‘λ§ λΆμνκΈ° λλ¬Έμ λ λ§μ λ°μ΄ν°λ‘ λΆμν΄ λ΄μΌ ν  νμμ±μ΄ μκ³ , μ€κ°μ λ°μ μ΄ μλ μ±μμλ κ°μ κ²°κ³Όκ° λμ¬μ§, μ±ν° λ³ λ‘ κ°μ λΆμμ μ€μνλ©΄ κΈ°μΉμ κ²°μ ννΈ μ€ μ΄λ ννΈμ μ΄λ€ κ°μ  μ΄νκ° μλλμ λ°λΌ κ²°λ§μ΄ μ΄λ»κ² λλμ§ λν λΆμν΄ λ³΄κ³  μΆλ€.

## π Book References

-   λ°±μλ―Ό, γRμ μ΄μ©ν νμ€νΈ λ§μ΄λγ, νμΈμμΉ΄λ°λ―Έ(2017)
    
## License

[![License: LGPL v3](https://img.shields.io/badge/License-MIT-g.svg?style=flat-square)](https://tldrlegal.com/license/gnu-lesser-general-public-license-v3-(lgpl-3))

- Copyright Β© [Hana Kim](https://github.com/hanakim120).
