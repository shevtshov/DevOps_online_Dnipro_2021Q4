## Module Python Essentials


solv_square_equation:
```
import math


def main():
    print('Введите a,b,c')
    valid_param = validate_param()
    a = valid_param[0]
    b = valid_param[1]
    c = valid_param[2]
    d = discriminant(a, b, c)
    root(d, a, b)
    square_print(a, b, c)


def discriminant(a, b, c):
    d: float = b ** 2 - 4 * a * c
    return d


def root(d, a, b):
    if d > 0:
        x1 = (-b + math.sqrt(d)) / (2 * a)
        x2 = (-b - math.sqrt(d)) / (2 * a)
        print(f'x1 = {x1:.2f}', f'x2 = {x2:.2f}')
    elif d == 0:
        x = -b / (2 * a)
        print('x = {x1:.2f}', x)
    else:
        print('No roots ')


def square_print(a, b, c):
    print('a = ', a)
    print('b = ', b)
    print('c = ', c)
    print('square: ', a, 'x^2 + ', b, 'x + (', c, ")")


def validate_param():
    attemts = 3
    while attemts > 0:
        try:
            print(f'{attemts} attemts left')
            a = int(input('a number: '))
            b = int(input('b number: '))
            c = int(input('c number: '))
        except ValueError:
            print('its not int')
            attemts -= 1
            continue
        else:
            return a, b, c


if __name__ == '__main__':
    main()
```

unit-test:
```
import unittest
import solv_square_equation


class MyTest(unittest.TestCase):
    def test_discriminant(self):
        self.assertEqual(solv_square_equation.discriminant(2, 4, -7), 72)


if __name__ == '__main__':
    unittest.main()

```
