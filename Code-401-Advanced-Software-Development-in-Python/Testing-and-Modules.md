# Testing and Modules

## Test Driven Development (TDD) in Python

* The purpose of unit tests are to test the input, output and behavior of our code
* TDD is a strategy to think and write **tests first**
* Test name should be descriptive and say precisely what we are testing for
* The name of the file should follow the name of the module. For example, if the name of our file is sequences.py, our test file should be names test_sequences.py
* It's good practice to separate the test folder from the implementation
* A widely used convention for structuring our test folder is AAA (Arrange, Act, Assert)
    - Arrange: organize data needed to execute the input
    - Act: execute code being tested (behavior)
    - Assert: after executing the code, check if the output is the same as expected


example: 

```
import ZodiacDetector
class ZodiacDetector(object)
    
    def run (self, birthdate):
        result = requests.get('https://api.zodiacs.io/?birthdate={}'.format(birthdate)).json()
        return result('zodiac')

    def test_should_return_gemini_when_birthdate_is_5/25/1997():
        detector = ZodiacDetector()

        expected_zodiac = detector.run(‘5/25/1997’)

        assert expected_zodiac == ‘gemini’

```

## Modules in Python

In order to create a module in Python, we include the following snippet of code in our file:

`if __name__ == "__main__":`
    `main()`

if the name of our module file is `myscript.py`, this is how we would import it:

`import myscript`

`myscript.main()`

* Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.

* If you import this script as a module in another script, the __name__ is set to the name of the script/module.

* Python files can act as either reusable modules, or as standalone programs.
if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported

 














*Reading Sources:* [In-Tests-We-Trust—TDD-with-Python](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)
[What-Does-if__name__==__main__:do?](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)