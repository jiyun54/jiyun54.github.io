---
title: "세번째 C감자"
layout: single
toc: true
toc_sticky: true
toc_label: "페이지 주요 목차"
categories: "C언어"
---
- 조건문 실습




 if 조건문에 관한 다양한 실습 예제와 그 해결 방안이다. 
 
 ### 01. 사주보기
 ![if 1][if 1 link]
 
 [if 1 link]: https://lh3.googleusercontent.com/25cLD-X4rZxy4n0Pl81NTSESprD_yI15By3c49GUzkAEcK0L7cfaDxvx1IepAxKvZXMAba5nMTtjZrE=w1213-h1319
 
 
 ~~~c
 #include <studio.h>
  int main(void){
  int year, month, day, result;
  
  printf("당신의 사주를 봐드립니다.\n");
  printf("연도, 월, 일을 차례대로 입력하세요 : ");
  scanf("%d, %d, %d", &year, &month, &day);
  
  result=(year-month+day)%10;
  if(result==0)
   printf("당신의 사주는 대박입니다.\n");
   
  else
   printf("당신의 사주는 그럭저럭입니다.\n");
   
  return 0;
  }
  
  ~~~
