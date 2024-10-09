# Add dot to end of a checkbox sentence

```md
- [ ] This is a sentence
  - [ ] This is another sentence
    - [ ] And again another sentence
```

`regex`: `^(\s+)?(-\s\[\s\]).+.*[^.\n]$`

`replaceBy`: `$0.`

```md
- [ ] This is a sentence.
  - [ ] This is another sentence.
    - [ ] And again another sentence.
```

# Add dot to all that do not start with `#` and do not end with `:;.`

```md
# Hello

- [ ] This is my test :
- [ ] This is another test
```

`regex`: `^(?!#)(\w\s)*.*[^;:.]$`

`replaceBy`: `$0.`

```md
# Hello

- [ ] This is my test :
- [ ] This is another test.
```
