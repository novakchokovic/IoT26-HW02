# IoT26-HW02
## 버튼 LED
### 1단계: Python 파일 만들기

- nano button_led.py

### 2단계: 코드 붙여넣기

```python
from gpiozero import Button, LED
from signal import pause

led = LED(14)
button = Button(4)

button.when_pressed = led.on
button.when_released = led.off

pause() 
```

### 3단계: 저장

- nano에서:
- Ctrl + O → 저장
- Enter
- Ctrl + X → 종료

### 4단계: 실행

- python3 button_led.py

### 5단계: 테스트

- 버튼 누름 → LED 켜짐
- 버튼 뗌 → LED 꺼짐

### 6단계: 종료

- Ctrl + C
