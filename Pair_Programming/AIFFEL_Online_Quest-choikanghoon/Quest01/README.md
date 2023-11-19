# AIFFEL Campus Online 7th Code Peer Review Templete

- 코더 : 최강훈
- 리뷰어 : 김승순
  
📌 코멘트를 하이라이트 하여 작성하였습니다(김승순)


🔑 **PRT(Peer Review Template)**

- [✔️]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
    - 문제를 해결하는 완성된 코드란 프로젝트 루브릭 3개 중 2개, 
    퀘스트 문제 요구조건 등을 지칭
        - 해당 조건을 만족하는 부분의 코드 및 결과물을 근거로 첨부        
    ```python
    
    def reverse(text):
  reverse_text = text[::-1]
  print("뒤집힌 단어는 :",reverse_text)

  if text == reverse_text:
    return True
  else:
    return False
    input_text = input('입력값 : ')
    result = reverse(input_text)
    if result == True:
        print(f"입력된 단어 {input_text}는 회문입니다.")
    else:
        print(f"입력된 단어 {input_text}는 회문이 아닙니다.")
    ```

> - 문제를 요구하는 최종 결과물이 첨부되어 있음
> - 다만, 퀘스트 요구조건이 지칭되지 않은 것이 아쉬움

<br>

- [✔️]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**
    - 해당 코드 블럭에 doc string/annotation이 달려 있는지 확인
    - 해당 코드가 무슨 기능을 하는지, 왜 그렇게 짜여진건지, 작동 메커니즘이 뭔지 기술.
    - 주석을 보고 코드 이해가 잘 되었는지 확인
        - 잘 작성되었다고 생각되는 부분을 근거로 첨부합니다.

> 아래의 코드와 같이 정답으로 제출한 코드에 주석을 달아 상세한 풀이 과정을 설명함

```python
def reverse(text):
  reverse_text = text[::-1] # [::-1]은 거꾸로 간격을 1로하는 슬라이싱
  print("뒤집힌 단어는 :",reverse_text)

  if text == reverse_text: # 내가 적은 text와 거꾸로 출력된 text의 인덱스와 문자열이 같을 경우
    print(f"입력된 단어 {input_text}는 회문입니다.")
  else: # 반대되는 경우
    print(f"입력된 단어 {input_text}는 회문이 아닙니다.")

input_text = input('입력값 : ') # 내가 입력하는 단어, 문장
result = reverse(input_text) # 사용자 지정함수 만든것을 활용?
# 조건문을 굳이 2번을 써서 출력하지 않아도 된다는 생각에 함수 조건문에 바로 print()을 적용 해봤다.
# 그 결과 동일한 출력을 얻어낼 수 있었다.

# if result == True:
#     print(f"입력된 단어 {input_text}는 회문입니다.")
# else:
#     print(f"입력된 단어 {input_text}는 회문이 아닙니다.")

```
<br>


- [🔺]  **3. 에러가 난 부분을 디버깅하여 문제를 “해결한 기록을 남겼거나” 
”새로운 시도 또는 추가 실험을 수행”해봤나요?**
    - 문제 원인 및 해결 과정을 잘 기록하였는지 확인 또는
    - 문제에서 요구하는 조건에 더해 추가적으로 수행한 나만의 시도, 
    실험이 기록되어 있는지 확인
        - 잘 작성되었다고 생각되는 부분을 근거로 첨부합니다.

> - 에러가 난 부분에 대한 디버깅 없음
> - 문제풀이의 결과를 출력하는 부분에서 return에서 print로 시도한 점

- [✔️]  **4. 회고를 잘 작성했나요?**
    - 주어진 문제를 해결하는 완성된 코드 내지 프로젝트 결과물에 대해
    배운점과 아쉬운점, 느낀점 등이 상세히 기록되어 있는지 확인
        - 딥러닝 모델의 경우,
        인풋이 들어가 최종적으로 아웃풋이 나오기까지의 전체 흐름을 도식화하여 
        모델 아키텍쳐에 대한 이해를 돕고 있는지 확인

> - 회고를 잘 작성하고 특히 KPT로 작성한 부분이 좋았습니다.

- [✔️]  **5. 코드가 간결하고 효율적인가요?**
    - 파이썬 스타일 가이드 (PEP8) 를 준수하였는지 확인
    - 코드 중복을 최소화하고 범용적으로 사용할 수 있도록 모듈화(함수화) 했는지
        - 잘 작성되었다고 생각되는 부분을 근거로 첨부합니다.
     
    ---

[Review]
Comment[김승순] :
- 배운개념과 요구사항을 명확하게 정의를 하고, 그 개념에 맞게 코드를 작성해서 깔끔하다고 느꼈습니다.
- 요구사항이 명시되지 않은 것은 다소 아쉽습니다.(하지만 설명할때는 구두로 잘 설명해주셔서 코드를 이해하는데 어려움이 전혀 없었음!)