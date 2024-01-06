# mypy-bug-reproducer

Repository that reproduces what to me seems like a bug in mypy.

To reproduce:

```sh-session
$ poetry install --with dev
$ poetry run mypy reproducer-main.py
```

This should in my mind report an error given that the code makes a blatant type
error in reproducer_import.py. However, if you follow these instructions, you
will find that no error is reported, which is strange to me..
