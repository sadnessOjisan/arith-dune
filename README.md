# arith-dune

TaPL の 4 章のサンプルコードを dune でビルドする

元のサンプルコード: https://www.cis.upenn.edu/~bcpierce/tapl/

## dev

```sh
# 実行

dune exec -- ./arith.exe
```

```
❯ dune exec -- ./main.exe
File "syntax.ml", line 2, characters 0-18:
2 | open Support.Error
    ^^^^^^^^^^^^^^^^^^
Error (warning 33): unused open Dune__exe.Support.Error.
File "syntax.ml", line 54, characters 9-11:
54 |     TmIf(fi, t1, t2, t3) ->
              ^^
Error (warning 27): unused variable fi.
File "syntax.ml", line 77, characters 10-14:
77 |   | TmZero(fi) ->
               ^^^^
Error (warning 27): unused variable fi.
```

```
File "lexer.mll", line 96, characters 24-37:
Alert deprecated: Stdlib.String.create
Use Bytes.create instead.
File "lexer.mll", line 105, characters 23-29:
Error: This expression has type bytes but an expression was expected of type
         string
```
