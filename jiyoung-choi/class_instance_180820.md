# TWL_OOP_180820

객체지향프로그래밍(Object-Oriented Programming, OOP)의 개념

- 클래스(Class) : 상태와 연산에 대한 정의

- 인스턴스(Instance): 클래스에 의해 정의된 개념의 실제 사례들

| 클래스         | 인스턴스                                      |
| -------------- | --------------------------------------------- |
| pd.DataFrame   | df1 = pd.DataFrame(...)df2 = pd.read_csv(...) |
| int            | a = 1b = 2 + 3                                |
| list           | a = [1, 2, 3]b = [4, 5, 6]                    |
| VendingMachine | vm = VendingMachine()                         |

> 단! 변수 자체가 인스턴스는 아니다. 변수에는 인스턴스에 대한 **참조**가 담긴 것.

        

```python
# Kindle의 전원을 프로그래밍한다면!

class Kindle:
    def __int__(self):
        self.power = False
        self.page = 1

	def toggle_power(self):
    	self.power = not self.power
	
	def next_page(self):
    	self.page = self.page + 1

	def prev_page(init):
    	if self.page > 1:
    		self.page = self.page -1
```
