# 23. [대화형 코딩 연습] 삶을 주(week)로 표현해보기

## 문제1) 현재 나이를 입력하면 90살 까지의 남은 며칠, 몇 주, 몇 달 남았는 지 표기되게 할 것. 
```py
# 🚨 Don't change the code below 👇
age = input("What is your current age?")
# 🚨 Don't change the code above 👆
```

# Write your code below this line 👇
## 내가 푼 방법
```py
age = int(age)
days = ((365 * 90) - (age * 365))
weeks = ((52 * 90) - (age * 52))
months = ((12 * 90) - (age * 12))
print (f"You have {days}, {weeks} weeks and {months} lest.")
```

## 정답
```py
age_as_int = int(age)
years_remaining = 90 - age_as_int
days_remaining = years_remaining * 365
weeks_remaining = years_remaining * 52
months_remaining = years_remaining * 12
message = f"You have {days_remaining}, {weeks_remaining} weeks and {months_remaining} lest."
print (message)
```