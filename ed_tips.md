---
layout: page
title: Debugging tips and Ed posting norms 
nav_exclude: true
---

# Debugging tips and Ed posting norms 

Please be sure to follow this hierarchy when debugging your code.

Starting steps:

*   Open a new jupyter cell and print each variable that you use in the code that doesn't work. Check the type and the value is what you expect.
*   Restart your jupyter kernel and re-run your code from the top. 
*   Review your code line by line using the [Duck method](https://en.wikipedia.org/wiki/Rubber_duck_debugging#:~:text=In%20software%20engineering%2C%20rubber%20duck,%2Dline%2C%20to%20the%20duck.). 
*   Copy and paste your error into Google search, as Stack Overflow very likely has at least one relevant post about your bug, making sure to exclude any object names that are specific to your code. 
*   **Read all prior Ed posts,** as someone may have already asked your question.
*   To learn a new technique, 
    * search `TECHNIQUE_DESCRIPTION python PACKAGE_NAME` on Google. For example, `how to make a bar graph python seaborn`. Feel free to share your findings in a public Ed post! 
    * alternatively, kindly request that ChatGPT write you a tutorial on how to use the technique. For example, `Please write a tutorial on how to make a bar graph of my data in python using seaborn."

Follow-up step:

*   If the steps above do not resolve your bug or answer your question, we strongly encourage you to **make a public Ed post**. Many other students likely have the same question. You are encouraged to paste error messages in Ed posts, and thoroughly describe the code that generated the error. **Please use the `code editing fonts`** as they make Ed posts a lot easier to read (see below).

**Hard to read:**

── Attaching packages ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────── tidyverse 1.3.0 ── ✓ ggplot2 3.3.2 ✓ purrr 0.3.4 ✓ tibble 3.0.3 ✓ dplyr 1.0.2 ✓ tidyr 1.1.2 ✓ stringr 1.4.0 ✓ readr 1.3.1 ✓ forcats 0.5.0 ── Conflicts ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────── tidyverse\_conflicts() ── x dplyr::filter() masks stats::filter() x dplyr::lag() masks stats::lag()

\# here's my plot code

x <- ggplot(df) + geom\_point(aes(x = year, y = count))

**Easy to read:**

```
── Attaching packages ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────── tidyverse 1.3.0 ──
✓ ggplot2 3.3.2     ✓ purrr   0.3.4
✓ tibble  3.0.3     ✓ dplyr   1.0.2
✓ tidyr   1.1.2     ✓ stringr 1.4.0
✓ readr   1.3.1     ✓ forcats 0.5.0
── Conflicts ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────── tidyverse_conflicts() ──
x dplyr::filter() masks stats::filter()
x dplyr::lag()    masks stats::lag()

# here's my plot code
x <- ggplot(df) + geom_point(aes(x = year, y = count))
```

If none of the steps above solve your issue, feel free to make a **private Ed post**.