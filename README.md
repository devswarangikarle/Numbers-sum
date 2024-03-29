# Numbers-sum
You're given a 3 digit number abc, digits are a, b and c. Find the sum of numbers- abc, bca and cab i.e. abc+bca+cab.  Input Given an integer- abc.  Constraints abc is a 3- digit integer, none of whose digits is 0. Output Print an integer.


def sum_of_numbers(abc):
    a = abc // 100
    b = (abc % 100) // 10
    c = abc % 10

    return abc + (b * 100 + c * 10 + a) + (c * 100 + a * 10 + b)

abc = int(input())

print(sum_of_numbers(abc))
