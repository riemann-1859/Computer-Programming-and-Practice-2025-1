# include 지시어
전처리 지시어는 C 소스 파일을 기계어로 번역하기 전에 어떤 텍스트 작업을 할지 정합니다.
include 지시어는 특정 파일의 내용을 모두 소스파일의 해당 위치에 포함시키는 작업을 지시합니다. 
주로 함수 선언, 다른 전처리 지시어들을 모아놓은 헤더파일이라는 파일을 포함시킵니다. 
C 소스 파일의 확장자는 c고, 헤더 파일의 확장자는 h입니다. 

`#` `include` `"` `파일이름` `"` `엔터` 형태로 쓰면 현재 폴더, 지정된 폴더, 라이브러리 헤더 폴더 순으로 파일을 찾습니다.

`#` `include` `<` `파일이름` `>` `엔터` 형태로 쓰면 라이브러리 헤더 폴더에서 파일을 찾습니다.

#### 코드 예시:
```c
#include "value.h" /* value.h 파일의 모든 내용을 현재 위치에 포함시킵니다. */
```

#### 관련 C89 표준
3.8.2 Source file inclusion
> Semantics
>
> A preprocessing directive of the form
>
> `# include <h-char-sequence> new-line`
>
> searches a sequence of implementation-defined places for a header identified uniquely by the
> specified sequence between the < and > delimiters, and cause the replacement of that directive
> by the entire contents of the header. How the places are specified or the header identified is
> implementation-defined.
>
> A preprocessing directive of the form
>
> `# include "q-char-sequence" new-line`
>
> causes the replacement of that directive by the entire contents of the source file identified by
> the specified sequence between the delimiters. The named source file is searched for in an
> implementation-defined manner. If this search is not supported, or if the search fails, the directive
> is reprocessed as if it read
>
> `# include <h-char-sequence> new-line`
>
> with the identical contained sequence ... from the original directive. 
