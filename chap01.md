## chap01. 소개, 코드 포맷팅과 도구



코드를 짜다보면 어디선가는 클린 코드가 중요하다는얘기가 듣게 됩니다. 클린 코드가 도대체 뭘까요?

코드를 짜다보면 어디선가는 클린 코드가 중요하다는얘기가 듣게 됩니다. 클린 코드가 도대체 뭘까요?

#### 클린코드 소개

클린코드를 쉽게 설명하면, 쉽게 이해할 수 있는 코드입니다. 코드에 들어있는 내 아이디어를 다른 개발자가 쉽게 이해할 수 있게 만드는 코드를 짜는 것을 말해요. 왜일까요?

![clean](https://img.icons8.com/officel/16/100/code.png)

개발에서 유지보수는 굉장히 중요해요. 회사에서 코드를 짠 개발자가 평생 직장에 다니지도 않고, 게다가 ~~지난달에 내가 짠 코드는 남의 코드~~ 와 같은 일이 발생하죠. 그렇기 때문에, 이해하기 쉬운 코드를 작성하는 것이 중요해요.



#### 클린코드의 중요성 

이해하기 쉬운 코드를 작성한다는건 장기적으로 시간을 버는 일이에요. 코드의 가독성이 떨어지면, 다른 개발자가 이해하는데 시간이 오래걸려요..또한 클린하지 못한 코드 위에 쌓이는 엉망인 코드들은 이런 관리 시간을 증가 시키죠. 

이런 시간들은 결국 비용의 소모를 말하고, __기술 부채__ 라는 소프트웨어적 결함이 발생합니다.

##### 클린 코드를 위한 마인드

우리가 어떤 기술을 개발하다보면, 시간에 쫒겨 _"돌아가는데 그냥 낼까?"_ 하는 순간들을 직면합니다. 이러한 나쁜 유혹에 넘어가면이런 상황이 왔을 때 두가지 관점을 생각해보라고 해요. 

1. ##### 과거를 회상해보기 

   > 현재 내가 직면한 문제들이 과거에 잘못된 코드에서 기인된 것이 아닐까?

2. ##### 미래를 예측해보기

   > 현재 코드를 대충 짠다면 미래에 어떤 문제가 발생할까?



## 클린 코드를 도와주는 도구들 

클린 코드를 위해 python 에서 제공하는 도구들을 알아볼까요?

#### PEP-8

![pep-8](data:image/jpeg;base64,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)



파이썬에서는 PEP-8 이라는 코딩 스타일 가이드를 제공합니다. 또한 여기에는 코드 구조, 유지 보수성과 같은 기능들이 포함되어 있어요. 다른 언어 들도 존재하지만, PEP-8 은 파이썬 문법의 특수성을 고려하여 작성 되었습니다. 

PEP-8은 아래와 같은 특징이 있어요.

1. __검색효율성__ 

   코드에서 토큰을 grep 할 수 있는 기능을 제공합니다.

2. __일관성__

   코드가 일정한 포맷을 가지면 쉽게 읽을 수 있습니다

3. __코드 품질__ 

   한눈에 코드를 이해하고, 버그와 실수를 쉽게 찾을 수 있습니다.



#### Docstring 

##### Docstring?

파이썬은 인터프리터 언어이기 때문에, 동적으로 타입을 결정해요. 그래서 변수명을 작성 안해도 되죠. 코드를 짜기 편하다는 장점이 있지만, __함수나 메서드__를 거치면 변수나 객체의 값이 무엇인지 알기가 어려운 경우가 많아요. 이럴 때 __Docstring__ 을 통해 문서화 하는 것이 다른 개발자가 쉽게 이해하는게 도움이 됩니다.

docstring 은 특정 컴포넌트에 대한 _문서화_ 에요. 반환값, 매개변수 타입 정도이죠.

```python
# example
def my_func():
    """임의의 계산 수행"""
    return None
```

```shell
# result
>>> my_func().__doc__
'임의의 계산 수행'
```



##### 주석은 피하자

_엥 주석으로 쓸 수 있잖아요!_

클린한 코드를 위해서는 주석은 피하는 게 좋아요. 왜냐하면 주석은 코드에 작성하는 형태로 남기 때문에, 내가 짠 코드에 추가 설명이 필요하다는 것은 __내 아이디어를 코드로 제대로 설명 못했다는 것__ 을 의미합니다. 또한 코드 변경시 주석 업데이트를 깜빡하는 경우가 많기 때문에 주석 보다는 Docstirng 으로 대체하는게 좋습니다.



##### Sphinx library

Docstring 을 모아서 문서로 만들어주는 골격을 제공하는 라이브러리에요. autodoc 을 사용하면 문서화 된 페이지를 만들어줍니다!

<https://tech.ssut.me/start-python-documentation-using-sphinx/>



#### 어노테이션

어노테이션은 코드에 대한 타입 힌팅을 주는 기능입니다. __"코드 사용자에게 함수 인자로 어떤 값이 와야하는지 알려주자"__ 에서 시작합니다. 

자바 경험이 있는 사람들이라면, 어노테이션을 들어봤을 텐데요. 둘다 __데이터를 설명하는 기능__ 은 같지만, 문법적으로 차이가 있습니다.

java에서는 어노테이션을 사용할 때  `@~` 로 시작하는 필드를 사용해요.

```java
// java annotation
@Target(B)
@Retention(A)
public @interface TestAnnotation {
	boolean isCheck() default true;
}
```

python 에서는  `@` 이 들어간 내용은 데코레이터라는 다른 기능에 사용합니다! 

##### example

```python
class Point:  # pylint: disable=R0903
    """Example to be used as return type of locate"""
    def __init__(self, lat, long):
        self.lat = lat
        self.long = long

def locate(latitude: float, longitude: float) -> Point:
    """맵에서 좌표에 해당하는 객체를 검색"""
    
# python~=3.6 부터는 변수에도 주석을 달 수 있습니다.
class Point:
    lat: float
    long: float
```

이렇게 type hinting 을 붙히면 python 에서 자동으로 `__annotation__` 이라는 특수한 속성을 만들어 줍니다.

```shell
>>> locate.__annotations__
{'latitude': <class 'float'>, 'longitude': <class 'float'>, 'return': <class '__main__.Point'>}
```



##### Mypy library

타입 검사하는 linter 라이브러리입니다. type hint 같은 자동화된 검증을 실행할 수 있어요.

```python
$ pip install mypy
$ mypy add.py
add.py:6: error: Argument 1 to "add" has incompatible type "str"; expected "int"
add.py:6: error: Argument 2 to "add" has incompatible type "str"; expected "int".
```



#### 어노테이션으로 Docstring 을 대체할 수 있을 것 같은데요?

docstring과 어노테이션은 서로 보완적인 개념이에요. 보다 나은 문서화를 위해 둘다 사용하는게 좋습니다.

요 함수를 볼게요. `dict` 을 받아 `dict`  을 리턴하는 함수입니다. 하지만,

- response 의 올바른 인스턴스 형태는 어떤가
- 결과의 리스폰스의 형태는 어떤가

에 대한 내용이 부족하죠. 이런 내용을 Docstring 을 사용하면 좋습니다.

```python
# annotation 만 적용한 함수
def data_from_response(response: dict) -> dict:
    if response["status"] != 200:
        raise ValueError
    return {"data": response["payload"]}
```

##### docstring 을 사용한 예제 

```python
# docstring 을 추가한 함수
def data_from_response(response: dict) -> dict:
""" response 에 문제가 없다면 response 의 payload 를 반환

	- response 의 사전 예제:
    {
    	"status": 200, # <int>
    	"timestamp": "..", # 현재 시간의 format string
    	"payload" : { ... }
    }
    
    - return 값의 사전 예제
    {"data": {..}}
    
    - 발생 가능 예외
    - HTTP status가 200이 아닌 경우 ValueError 발생 
"""
    if response["status"] != 200:
        raise ValueError
    return {"data": response["payload"]}
```

반환 값의 형태를 확실히 알 수 있죠? 또한 이런 내용들은 단위 테스트에서도 유용한 정보로 사용됩니다!



#### 기본 품질 향상을 위한 도구 설정

클린 코드를 위해서 반복적으로 확인하고 고치는 작업이 필요한데요. 이런 반복을 줄여주는 __코드 검사 실행도구__ 를 소개합니다. 

##### 또한 동료가 작성한 코드를 살펴볼 때 아래와 같은 내용을 고민해야합니다.

- 동료 개발자가 쉽게 이해하고 따라갈 수 있을까?
- 업무 도메인에 대해서 말하고 있는가?
- 팀에 새로 합류하는 사람도 쉽게 이해하고 효과적으로 작업할 수 있을까?



또한 클린 코드는 포맷팅, 일관된 레이아웃, 들여쓰기로는 충분하지 않아요. 더 넘는 패턴을 사용하고 정교한 작업이 필요하죠. 기본적인 내용들은 자동화 해서 시간을 효율적으로 사용하는게 좋습니다. 



이런 도구들을 알아봅시다!



#### 1. MyPy를 사용한 타입 힌팅

mypy 를 설치하면 프로젝트의 모든 파일을 분석하여 타입 불일치를 검사해 줍니다. 

```python
$ pip install mypy
```

가상환경에 mypy를 설치하고 `mypy {filename}`  을 입력해보면, 해당 파일의 타입 검사 결과를 제공해줍니. 

잘못된 탐지를 할 경우, 문장 끝에 `type: ignore` 라는 주석을 추가하면 무시합니다.

```
type_to_ignore = "something" # type: ignore
```



#### 

#### 2. Pylint 를 사용한 코드 검사

Pylint 는 기본적으로 PEP-8을 준수했는지 여부를 검사해 줍니다. 이건 에디터에 익스텐션으로도 제공됩니다!

```python
$ pip install pylint
```

를 입력하고 명령어 창에 `pylint ` 를 입력하면 된다. 



#### 3. Black 

자동으로 코드를 포맷팅 해주는 도구입니다. Black 은 다른 PEP-8 보다 엄격한 규칙을 적용하기 때문에 자잘한 코드 포맷팅의 걱정 필요 없이 문제의 핵심에만 집중할 수 있는게 장점입니다.

###### example

- 문자열에 항상 쌍따옴표를 사용한다.
- 파라미터 형태는 같은 구조를 사용한다. 



mypy, pylint, black 와 같은 도구들은 IDE 에 통합하여 작업할 수 있어요. 



##### 요약

클린 코드는 타인의 이해도를 높이는 효과적인 코드 작성방법입니다. 

이를 위해 코딩스타일, 포맷팅을 지키는 것이 중요합니다. 

이런 검사들을 자동화하는 도구들을 사용해 코드를 효과적으로 작성할 수 있습니다.

다음장에서는 python 코드에 초점을 맞춰 작고 효율적인 코드 사용을 알아봅시다.