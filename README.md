Task Requirements
Create a function def pascal_triangle(n): that returns a list of lists of integers representing the Pascal’s triangle of n:

Returns an empty list if n <= 0
You can assume n will be always an integer
guillaume@ubuntu:~/0x00$ cat 0-main.py
#!/usr/bin/python3
"""
0-main
"""
pascal_triangle = __import__('0-pascal_triangle').pascal_triangle

def print_triangle(triangle):
    """
    Print the triangle
    """
    for row in triangle:
        print("[{}]".format(",".join([str(x) for x in row])))


if __name__ == "__main__":
    print_triangle(pascal_triangle(5))

guillaume@ubuntu:~/0x00$ 
guillaume@ubuntu:~/0x00$ ./0-main.py
[1]
[1,1]
[1,2,1]
[1,3,3,1]
[1,4,6,4,1]
guillaume@ubuntu:~/0x00$ 
🔧 Task setup.
 Create task file and set write permission.
touch ./0-pascal_triangle.py
chmod +x ./0-pascal_triangle.py
./0-pascal_triangle.py

pycodestyle ./0-pascal_triangle.py
pep8 ./0-pascal_triangle.py

 Create test file
touch ./0-main.py
chmod +x ./0-main.py
./0-main.py
