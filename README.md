# 주석
주석은 실행 파일을 만들 때 제거되는 설명글입니다.

`/*` 이후로 처음 나오는 `*/`까지가 주석이 됩니다.

#### 코드 예시:
```c
/* 이것은 주석입니다 */
int main() {
  return 0; /* 이것도 주석입니다 */
}
```

#### 관련 C89 표준
3.1.9 Comments
> Except within a character constant, a string literal, or a comment, the characters /* introduce a comment.
> The contents of a comment are examined only to identify multibyte characters and to find the characters */ that terminate it. 
