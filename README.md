# config-parser-flex

A tiny parser to read content of a own config file using pure c and flex library.

## Compile

```bash
$ flex myscanner.l
$ cc myscanner.c lex.yy.c 
$ ls
a.out  config.in  lex.yy.c  myscanner.c  myscanner.h  myscanner.l
```

## Using

Run parser and get contents from `config.in` file via linux/unix command:

```bash
$ ./a.out  < config.in 
1
db_type is set to mysql
2
db_name is set to testdata
3
db_table_prefix is set to test_
4
db_port is set to 1099
```

### TODO

- Adding `fopen()` to read yyinput from file

Feel free to participate and develop.

### Acknowledgment

I saw an video from Jonathan Engelsma and It's encouraged me to do this project myself.

© Copyright Max Base
