### Create a file with sample data

```
mkdir word_count
cd word_count
touch data.txt
nano data.txt
cat data.txt
```

### Create mapper.py

```
touch mapper.py
nano mapper.py
cat mapper.py
```

### Run mapper.py

```
cat data.txt | python mapper.py
```

### Create reducer.py

```
touch reducer.py
nano reducer.py
```

### Run reducer.py

Sort the output of mapper.py in alphabetical order before passing it to reducer.py

```
cat data.txt | python mapper.py | sort -k1, 1 | python reducer.py
```