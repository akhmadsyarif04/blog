---
layout: post
title: Markdown Syntaxt
categories: markdown
tags:
  - markdown
published: true
---

## Headings  

| Markdown        | Html           | Output  |
| ------------- |:-------------:| -----:|
| # Heading level 1   | `<h1>Heading level 1</h1>` | <h1>Heading level 1</h1> |
| ## Heading level 2   | `<h2>Heading level 1</h2>` | <h2>Heading level 1</h2> |
| ### Heading level 3   | `<h3>Heading level 1</h3>` | <h3>Heading level 1</h3> |
| #### Heading level 4   | `<h4>Heading level 1</h4>` | <h4>Heading level 1</h4> |
| ##### Heading level 5   | `<h5>Heading level 1</h5>` | <h5>Heading level 1</h5> |
| #### Heading level 6   | `<h6>Heading level 1</h6>` | <h6>Heading level 1</h6> |


## Paragraphs  
| Markdown        | Html           | Output  |  
| ------------- |:-------------:| -----|  
| I really like using Markdown.   | `<p>I really like using Markdown.</p>` | <p>I really like using Markdown.</p>|
| I think I'll use it to format all of my documents from now on. | `<p>I think I'll use it to format all of my documents from now on.</p>` | <p>I think I'll use it to format all of my documents from now on.</p> |  


## Line Breaks  
gunakan 2 spasi diakhir kalimat dan enter.  


## Table  
```
| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |
```
```
:-------------: untuk align center
```
```
-------------: untuk align left
```
```
------------- untuk align right
```

## Bold  
| Markdown | Html | Output |
| ------------- |:-------------:| -----|
|  ```I just love **bold text**.```  | `I just love <b>bold text</b>.` | I just love <b>bold text</b>. |
|  ```I just love __bold text__.```  | `I just love <b>bold text</b>.` | I just love <b>bold text</b>. |
| ```Love**is**bold```| `Love<b>is</b>bold` | Love<b>is</b>bold |

## Italic  
| Markdown | Html | Output |
| ------------- |:-------------:| -----|
|  ```Italicized text is the *cat's meow*.```  | `Italicized text is the <i>cat's meow</i>.` | Italicized text is the <i>cat's meow</i>. |
|  ```Italicized text is the _cat's meow_.```  | `Italicized text is the <i>cat's meow</i>.` | Italicized text is the <i>cat's meow</i>. |
|  ```A*cat*meow```  | `A<i>cat</i>meow.` | A<i>cat</i>meow |

## Blockquotes  
Markdown :  
`` > Dorothy followed her through many of the beautiful rooms in her castle. ``  

Ouput :  
> Dorothy followed her through many of the beautiful rooms in her castle.

## Blockquotes with Other Elements
Markdown :  
```
> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.
```

Ouput :
> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.

## Ordered Lists
Markdown :
```
1. First item
2. Second item
3. Third item
4. Fourth item
```

Ouput :  
1. First item
2. Second item
3. Third item
4. Fourth item

Markdown :
```
1. First item
2. Second item
3. Third item
   1. Indented item
   2. Indented item
4. Fourth item
```

Ouput :  
1. First item
2. Second item
3. Third item
   1. Indented item
   2. Indented item
4. Fourth item

## Unordered Lists
Markdown :
```
- First item
- Second item
- Third item
- Fourth item
```

Ouput :  
- First item
- Second item
- Third item
- Fourth item

Markdown :
```
- First item
- Second item
- Third item
    - Indented item
    - Indented item
- Fourth item
```

Ouput :  
- First item
- Second item
- Third item
    - Indented item
    - Indented item
- Fourth item


Markdown :
```
*   This is the first list item.
*   Here's the second list item.

    I need to add another paragraph below the second list item.

*   And here's the third list item.
```

Ouput :  
*   This is the first list item.
*   Here's the second list item.

    I need to add another paragraph below the second list item.

*   And here's the third list item.


## Code Blocks
Markdown :
```
1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website.
```

Ouput :  
1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website.

## Code
Markdown :
```
At the command prompt, type `nano`.
```
Ouput :  
At the command prompt, type `nano`.

Markdown :
```
``Use `code` in your Markdown file.``
```
Ouput :  
``Use `code` in your Markdown file.``

javascript
var s = "JavaScript syntax highlighting";
alert(s);

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```

```python
s = "Python syntax highlighting"
print s
```

```
No language indicated, so no syntax highlighting.
But let's throw in a <b>tag</b>.
```


## Horizontal Rules
Markdown :
```
---
```

Ouput :  

---

## Links
Markdown :
```
My favorite search engine is [Duck Duck Go](https://duckduckgo.com).
```

Ouput :  

My favorite search engine is [Duck Duck Go](https://duckduckgo.com).

#### Adding Titles
Markdown :
```
My favorite search engine is [Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").
```

Ouput :  

My favorite search engine is [Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").  
 
#### URLs and Email Addresses
Markdown :
```
<https://www.markdownguide.org>  
<fake@example.com>
```

Ouput :  
<https://www.markdownguide.org>  
<fake@example.com>

## Images
Markdown :
```
![Killua so cool!](https://vignette.wikia.nocookie.net/hunter-x-hunter-fanon/images/a/a9/BABC6A23-98EF-498E-9D0E-3EBFC7ED8626.jpeg/revision/latest?cb=20170930221652 "Killua")
```

Ouput :  
![Killua so cool!](https://vignette.wikia.nocookie.net/hunter-x-hunter-fanon/images/a/a9/BABC6A23-98EF-498E-9D0E-3EBFC7ED8626.jpeg/revision/latest?cb=20170930221652 "Killua")

## Linking Images
Markdown :
```
[![Killua so cool!](https://vignette.wikia.nocookie.net/hunter-x-hunter-fanon/images/a/a9/BABC6A23-98EF-498E-9D0E-3EBFC7ED8626.jpeg/revision/latest?cb=20170930221652 "Killua")](https://vignette.wikia.nocookie.net/hunter-x-hunter-fanon/images/a/a9/BABC6A23-98EF-498E-9D0E-3EBFC7ED8626.jpeg/revision/latest?cb=20170930221652)
```

Ouput :  
[![Killua so cool!](https://vignette.wikia.nocookie.net/hunter-x-hunter-fanon/images/a/a9/BABC6A23-98EF-498E-9D0E-3EBFC7ED8626.jpeg/revision/latest?cb=20170930221652 "Killua")](https://vignette.wikia.nocookie.net/hunter-x-hunter-fanon/images/a/a9/BABC6A23-98EF-498E-9D0E-3EBFC7ED8626.jpeg/revision/latest?cb=20170930221652)


