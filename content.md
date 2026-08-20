# What Loop Control Means

Loop control statements change the normal flow of a loop. They let you stop early or skip part of an iteration when certain conditions are met. This can be important for structuring the logic of a piece of code, or to speed up execution by eliminating unnecessary iterations.

# Exiting the Loop Early

In most languages, the word `break` immediately terminates the current loop.

```
FOR each item IN collection:
    IF stop_condition:
        BREAK
    process(item)
```

This is useful for cases like:

* When searching data for the first item that matches a condition, so no further processing is needed.
* When a certain threshold in a calculation is reached, and continuing would be inefficient or irrelevant.

# Skipping to the Next Iteration

In most languages, the word `continue` skips the rest of the current iteration and moves directly to the next one.

```
FOR each item IN collection:
    IF skip_condition:
        CONTINUE
    process(item)
```

This is useful for cases like:

* When you want to ignore certain items that don't meet criteria, but still want to process the rest.
* When you want to skip over items that would cause errors or are irrelevant for the current processing step.
