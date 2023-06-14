# Reproduce issue as llhttp pull-225 description

Step:
```sh
# first time is ok
cmake -B build

# after first time, always fail until delete libllhttp.pc manually
cmake -B build
```
