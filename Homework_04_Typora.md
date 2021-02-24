***Caitlin Jeffrey***  

***Bio 381***  

***Homework 4***



# First level header

## Second level header

### Third level header

#### Fourth level header

##### Fifth  level header

###### Sixth level header



## Unordered lists

* Item 1

* Item 2

  + Item 2a
  + Item 2b

  

## Ordered list

1. Item 1
2. Item 2
3. Item 3
   + Item 3a
   + Item 3b

# Links

http://example.com

[linked phrase](http:example.com)

A [linked phrase][id]. 



Adding text and doing so with *markdown* codes. **Bold** text and all other font enhancements. Command/forward slash changes view to markdown.

## 

```
This is a box of literal plain test. Just like I **type it**
```

```{r}
#here is a comment
x <- 3
y <- "character string"
```



Add text here. Just use it like a typewriter, and add as much or as little as you like.

New text appears here in a separate paragraph. 

Nick Gotelli  
Dept Bio  
UVM  

Use two or more blank spaces at the end of a single-spaced line.

###### 

#Basic text formatting

italic *text* like this

bold **text** like this

subscript~text~ like this

superscript^text^ like this

strikethough ~~text~~ like this



#Fencing

inline fencing with a backtick `to show anything in plain text with *no* formatting` which can be useful for many things. 

in line execution of r inside the backticks by inserting r as the first element `r 3 + pi`

in line execution of r inside the backticks by inserting r as the first element `3 + pi`

3 backticks for a whole section of plain text

```
everything in here is in plain text.
even single lines.

useful especially when showing others coding instructions.
```

#Block quotes with `>` 

> To be or not to be, that is the question. Whether tis nobler... blah blah blah

# Spacer line with 3 or more underscores

___

Adds a line between text






# Images

`!["rplot.tiff"]`

<img src="rplot.TIFF" width = "200" height ="200" />

At the bottom of the document:

`[id]: figures/img.png "Title"`

# Tables

| First Header | Second Header    |
| ------------ | ---------------- |
| Content Cell | Content Cell     |
| Content Cell | *formatted text* |

# LaTeX code for equations

We set off equations with `$` for brackets.

## In-line equations

These equations such as $a = 3 + 4$ will appear inside of a single line of text.

These equations such as $$a = 3 + 4$$ will appear in a separate line of their own. 

##Subscripts

$$H_0 = Z_{a + b}$$

## Superscripts

$$S = cA^z$$

Elements can be coupled and nested

$$S=cA^z_1 +z_{2 + x}$$

## Fractions and Greek symbols

$$\alpha = \frac{\beta}{\delta + \gamma_x}$$

## Summation signs

$$z= \sum_{i=1}^X{K}$$

## Escape the backslash with a custom term

$$\backslash \alpha \le b \backslash$$

## Rendering plain text in a LaTeX equation
$$P(Ocurrence of Species A) = Z$$

$$P(\mbox{Occurrence of Species A}) =Z$$


```{r,echo=TRUE,eval=FALSE}
# Don't forget to start with comments!
# Prelimimaries
library(ggplot2)

pred <- 1:10 # vector of ten integers
res <- runif(10) # random uniform values

# print the random numbers
print(res)

# plot the graph
qplot(x=pred,y=res)
```


Now back to writing text in our markdown document, including LaTeX equations if we need then as such $a + b$ inserted in the middle of my sentence.

