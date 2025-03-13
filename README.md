# main 함수
이름이 main인 함수는 C 프로그램을 시작할 때 실행됩니다. 
main 함수의 실행이 끝나면 C 프로그램이 종료됩니다. 

#### 코드 예시:
```c
/* 프로그램의 시작과 끝인 main 함수 */
int main() {
   return 0;
}
```

#### 관련 C89 표준

2.1.2.2 Hosted environment

>"Program startup"
>
>The function called at program startup is named main.
>The implementation declares no prototype for this function.
>It can be defined with no parameters: `int main(void) { /*...*/ }
>
>...
>
>"Program termination"
>
>A return from the initial call to the main function is equivalent to calling the exit function
>with the value returned by the main function as its argument.
>If the main function executes a return that specifies no value, the termination status
>returnted to the host environment is undefined. 
