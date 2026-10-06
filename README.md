# Python Print Statement Examples

이 저장소는 Python에서 다양한 출력 방법을 소개하는 간단한 예제 코드입니다.

변수 선언부터 여러 가지 출력 형식과 옵션을 포함한 다양한 출력 방식을 보여줍니다.

---

## 코드 설명

### 변수 선언

    name = "Alice"
    age = 25
    score = 95.5

Python에서 변수를 선언하고 값을 저장하는 방법을 보여줍니다.

### 1. 기본 출력

    print("Hello, Python!")

print() 함수를 사용하여 문자열을 출력합니다.

### 2. 여러 값 출력

    print("Name:", name, "Age:", age, "Score:", score)

콤마를 사용하여 여러 값을 한 번에 출력할 수 있습니다.

### 3. f-string

    print(f"My name is {name}, I am {age} years old, score: {score}")

f-string을 사용하여 문자열 안에 변수의 값을 넣어 출력할 수 있습니다.

### 4. format() 함수

    print("My name is {}, I am {} years old, score: {}".format(name, age, score))
    print("My name is {0}, age {1}, score {2}".format(name, age, score))
    print("Score with 2 decimals: {:.2f}".format(score))

format() 함수를 이용하여 문자열에 변수의 값을 넣어 출력할 수 있습니다.

### 5. % 포맷팅

    print("Name: %s, Age: %d, Score: %.1f" % (name, age, score))

% 기호를 이용하여 문자열을 형식에 맞게 출력할 수 있습니다.

### 6. 여러 줄 출력

    print("This is line 1\nThis is line 2")

\n을 사용하여 출력 내용을 여러 줄로 나눌 수 있습니다.

### 7. end 옵션

    print("Hello", end=" ")
    print("World!")

end 옵션을 사용하여 출력이 끝난 후 들어갈 문자를 지정할 수 있습니다.

### 8. sep 옵션

    print("2025", "09", "23", sep="-")

sep 옵션을 사용하여 여러 값 사이에 들어갈 구분자를 지정할 수 있습니다.

### 9. 딕셔너리 출력

    data = {"name": name, "age": age, "score": score}
    print("Data:", data)

딕셔너리와 같은 자료형도 print() 함수를 이용하여 출력할 수 있습니다.

### 10. f-string에서 계산식과 함수 사용

    print(f"Next year age: {age + 1}")
    print(f"Score (rounded): {round(score)}")

f-string 안에서 계산식이나 함수를 사용할 수 있습니다.

### 11. 멀티라인 f-string

    print(f"""
    Student Info:
     - Name : {name}
     - Age  : {age}
     - Score: {score:.2f}
    """)

멀티라인 f-string을 이용하여 여러 줄의 정보를 출력할 수 있습니다.

---

## Rich를 이용한 출력

main_print_v2.py에서는 rich 라이브러리를 사용하여 다양한 형태의 출력을 구현했습니다.

### Rich Print

    from rich import print as rprint

rich.print()를 사용하여 색상과 스타일을 적용한 출력을 할 수 있습니다.

### Panel

    from rich.panel import Panel

Panel을 이용하여 정보를 박스 형태로 출력할 수 있습니다.

### Table

    from rich.table import Table

Table을 이용하여 데이터를 표 형태로 출력할 수 있습니다.

### 반복문을 이용한 데이터 출력

    for k, v in data.items():
        table.add_row(k, str(v))

딕셔너리의 데이터를 반복문을 이용하여 표에 추가할 수 있습니다.

---

## 파일 설명

- main_print_v1.py : Python의 다양한 print 출력 방법을 보여주는 예제
- main_print_v1.ipynb : Python 출력 관련 Jupyter Notebook 예제
- main_print_v2.py : Rich 라이브러리를 이용한 출력 예제
- requirements.txt : 프로젝트에 필요한 Python 패키지 목록
- .gitignore : Git에서 제외할 파일과 폴더를 설정하는 파일

---

## 사용한 기술

- Python
- Jupyter Notebook
- Rich
- Git
- GitHub
- Git branch practice