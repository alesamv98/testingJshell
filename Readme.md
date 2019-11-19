#Repository for testing jshell

Errors

jshell> char = 'B';
|  Error:
|  '.class' expected
|  char = 'B';
|       ^
|  Error:
|  unexpected type
|    required: variable
|    found:    class
|  char = 'B';
|  ^---^

jshell> b = n;
|  Error:
|  incompatible types: possible lossy conversion from int to byte
|  b = n;
|      ^

jshell> C = n;
|  Error:
|  cannot find symbol
|    symbol:   variable C
|  C = n;
|  ^

### “After errors fixed:”
int n = 68;
byte b = 127;
char c = 'B';
b = (byte)n;
b ==> 68
c = (char)n;
char = 'D';