# Operators and Loops

## Comparison Operators

==      is equal to
- Compares two values, are they the same

!=      is not equal to
- Compares two values, sees if they are *not* the same

===     strict equal to
- Compares two values *and data types* - are they the same

!==     strict not equal to
- Compares two values *and data types* - are they *not* the same

'>'     greater than
- Between two numbers

'<'     less than
- Between two numbmers

'>='    greater or equal
- Between two numbers

'<='    less or equal
- Between two numbers

## Logical Operators

Return single values **True** or **False**

&&      And

||      Or

!       Not

## Loops

Loops check a condition. If it returns **true**, a code block will run. Then, the condition will be checked again and if it still returns **true**, the code block will run again. It repeats until the condition returns **false**.

### Types of Loops

**For**
- Condition is usually a counter which is used to tell how many times the loop should run.

```
for (var i = 0; i < 10; i++) {
    documents.write(i);
}
```

This is a **for** loop. if variable (i) is less than 10, the code inside the curly braces is run. Then the counter is incremented by 1, and if i is still less than 10, it runs again.

**While**
- If you do not know how many times the loop should run, usually use a **while** loop.
- Condition is something other than a counter, and as long as the condition evaluates to **True**, the loop runs.
- A ***Do While*** loop is similar to a ***While*** loop, except that it will always run the code inside the curly braces at least once, even if the condition evaluates to *false*.

### Loop Counters

Initialization

```
var i = 0;
```

Condition

```
i < 10;
```

Update
```
i++
```