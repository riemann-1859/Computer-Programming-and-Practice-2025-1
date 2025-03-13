# 함수호출식 (매개변수 있는 함수)

매개변수가 있는 함수를 호출할 때는 매개변수들을 어떤 값들로 초기화한 후에 실행할지를 정해줘야 합니다.
함수 호출할 때 전달하는 값을 인수 또는 인자라고 합니다. 
인자의 개수는 호출하려는 함수의 매개변수 개수와 같아야 합니다. 

`식` `(` `인자리스트` `)` 형태로 씁니다. 

`인자리스트`는 `식` 또는 `식` `,` `인자리스트` 입니다.

#### 코드 예시:
```c
int value(int x) {
   return x;
}
int main() {
   return value(5); /* value 함수에 인자 5를 전달해서 호출하고, 반환값을 그대로 반환합니다. */
}
```

#### 관련 C 표준
3.3.2.2 Function calls
> Constraints
>
> ... the number of arguments shall agree with the number of parameters.
> Each argument shall have a type such that its value may be assigned to an object with the ...
> type of its corresponding parameter.
>
> Semantics
>
> ... The list of expressions specifies the arguments to the function
>
> An argument may be an expression of any object type.
> In preparing for the call to a function, the arguments are evaluated,
> and each parameter is assigned the value of the corresponding argument. ...
>
> ... the arguments are implicitly converted, as if by assignment,
> to the types of the corresponding parameters. ...
> If the function is defined with a type that is not compatible with the type (of the expression)
> pointed to by the expression that denote the called function, the behavior is undefined. 
>
> The order of evaluation of the function designator, the arguments,
> and subexpressions within the arguments is unspecified, but there is a sequence point
> before the actual call.
