import random

class Encryptor: def init(self, numbers): self._numbers = numbers  # Приховуємо числа self._operation = random.choice(["+", "-", "", "/"])  # Випадкова операція

def _calculate(self):
    result = self._numbers[0]
    for num in self._numbers[1:]:
        if self._operation == "+":
            result += num
        elif self._operation == "-":
            result -= num
        elif self._operation == "*":
            result *= num
        elif self._operation == "/" and num != 0:
            result /= num
    return result

def str(self):
    return f"Operation: {self._operation}, Result: {self._calculate()}"

Приклад використання

enc = Encryptor(10, 5, 2) print(enc)
