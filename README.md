# spec-diff

Testing Python's difflib to look at html output for a spec, both with
json and text.

## Generation
```bash
spack spec --json python@2.7 > spec1.json
spack spec --json python@3.9 > spec2.json

spack spec python@2.7 > spec1.txt
spack spec python@3.9 > spec2.txt
```

## Html Output

```bash
python diff.py -m spec1.txt spec2.txt > index.html 
python diff.py -m spec1.json spec2.json > json.html 
```


## View

 - [txt](https://vsoch.github.io/spec-diff/)
 - [json](https://vsoch.github.io/spec-diff/json.html)
 
The json is nice!
