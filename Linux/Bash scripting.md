

#### A bash script always starts with the following line of code at the top of the script.

```

#!/bin/bash

```


We write this so the shell knows that this is a bash file and it needs to run using bash in terminal.

> [!info] In Bash , scripts are ran in a step by step order which is called a procedural script



---

### Variables

```
name="jammy"

```

To access variable we use echo $name which will give output : jammy

---

2. Conditionals (If/Else)

- **Syntax**: Use `[[ ]]` for modern Bash tests. Ensure spaces exist inside the brackets. 

bash

```
if [[ $AGE -ge 18 ]]; then
    echo "Access granted."
elif [[ $AGE -gt 13 ]]; then
    echo "Limited access."
else
    echo "Access denied."
fi
```

Use code with caution.

Common Operators:

- `-eq` (equal), `-ne` (not equal), `-gt` (greater than), `-lt` (less than).
- `-f file` (exists), `-d dir` (is directory), `-z str` (is empty string). 

3. Loops

- **For Loop**: Iterate over a range or list.
- **While Loop**: Run while a condition is true. 

bash

```
# Range loop
for i in {1..5}; do
    echo "Iteration $i"
done

# While loop
COUNT=1
while [[ $COUNT -le 3 ]]; do
    echo "Count: $COUNT"
    ((COUNT++))
done
```

Use code with caution.

4. Functions

- **Definition**: Group commands to reuse them.
- **Arguments**: Use `$1`, `$2`, etc., to access parameters passed to the function. 

bash

```
greet_user() {
    echo "Welcome to Linux, $1!"
}

greet_user "Admin" # Call function
```

---
