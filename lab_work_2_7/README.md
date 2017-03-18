##Laboratory Work 2.7

####Description:

Write the code to do following:

- Write a script that creates a new output file called myfile.txt
- writes the string "Hello file world!" into it
- write another code that opens myfile.txt in w+ mode
- read and print its contents
- write into “Hello file” string new value “my” – “Hello my file”
- Save changes without file object close

####Here is its solution code:

*solution_2_7.py*
```python
"""Write a script that creates a new output file called myfile.txt
"""
create = open('files/myfile', 'w')

"""writes the string "Hello file world!" into it
"""
create.write('Hello file world')

"""write another code that opens myfile.txt in r+ mode
"""
create.close()
another = open('files/myfile', 'r+')

"""read and print its contents
"""
print(another.read())

"""write into “Hello file” string new value “my” – “Hello my file”
"""
another.seek(len('Hello '))
another.write('my file world!')

"""Save changes without file object close
"""
another.flush()
another.close()

printer = open('files/myfile')
print(printer.read())
printer.close()

```