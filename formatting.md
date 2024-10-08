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
