# MINST and how do we go about teaching computer to distinguish 3 and 7 (Numbers Recognition).

Food for thoughts: how do you know if 3 is 3 and 7 is 7? 
- Oh well, back in kindergarten my teacher had us drawn them on paper, 3 looks curvy, kind of like an 8 spit in half, while 7 is more similar to 1. Yes, the curves are what help me tell them apart!

## 1. Designing a decent baseline
Vocab: *Tensors* = PyTorch’s way to store and manipulate numeric data (like images, text embeddings, signals, etc.) on CPU or GPU.
- A decent baseline help you know if you have created a good model or a retarded one. A decent baseline in this context could be creating an ideal 3 and ideal 7 by taking average of a bunch of 3 images and 7 images, then we will compare a digit to see how close is it to the average 3 or 7 to make our decision.
- Let say after taking the average pixels value of all 200 images, I got a idea 3, how do I go about comparing a new img to this avr img?
  Easy, I can just take the mean square error of 2 pixel, one from the avr, one from the new img. If the error is small enough, accept, else reject. But what is small enough threshold though?
---

## Lists

Here's a list:

- item 1
- item 2

And a numbered list:

1. item 1
1. item 2

## Boxes and stuff

> This is a quotation

{% include alert.html text="You can include alert boxes" %}

...and...

{% include info.html text="You can include info boxes" %}

## Images

![](/images/logo.png "fast.ai's logo")

## Code

General preformatted text:

    # Do a thing
    do_thing()

Python code and output:

```python
# Prints '2'
print(1+1)
```

    2

## Tables

| Column 1 | Column 2 |
|-|-|
| A thing | Another thing |

## Footnotes

[^1]: This is the footnote.

