# Team Members

* [Alexia Newgord](https://github.com/alne4294)
* [Austin Wood](https://github.com/indiesquidge)
* [Ian K.](https://github.com/ianks)
* [Daniel Nolan](https://github.com/dano8957)
* [Alex Tsankov](https://github.com/antsankov)

# Promotional campaign

## Description
Our promotional campagin will be based on graphing different actions over time for different products. We can take the HTTP requests for the different products and judge customer interest. 

Some of the data point that we might pay attention to are: 

1. Products that me might be gaining in popularity, but are still relatively unpopular.

## Rationale 1

```
{{sourcetype=access_* action = "purchase" OR "addtocart" | timechart count(action) by productId useother=f usenull=f limit=16}}
```
![Rational 1](http://i.imgur.com/7gY7AHb.png)
This shows products that are added to the cart and actually pruchased, which can show us broad interest in a product.

## Rationale 2

```
sourcetype=access_* productId=* action="purchase" | timechart count by categoryId limit=16 useother=false
```
Strategy games are wildly popular in our stores, let's focus more resources on that.

![screenshot of a data table or a graph or both](https://www.dropbox.com/s/s1jjwbsvue5u4fs/Screenshot%202014-09-08%2018.20.03.png?dl=1) 
{{write-an-one-sentence-caption}}

## Rationale 3

```
{{splunk query producing the table or graph below}}
```
![screenshot of a data table or a graph or both](image.png?raw=true) 
{{write-an-one-sentence-caption}}

## Rationale N

{{more if desired, use-the-same-template-structure-as-before}}

# Loyalty program

## Description
{{an-one-paragraph-description}}

## Rationale 1

```
{{splunk query producing the table or graph below}}
```
![screenshot of a data table or a graph or both](image.png?raw=true) 
{{write-an-one-sentence-caption}}

## Rationale 2

{{one more, use-the-same-template-structure-as-before}}

## Rationale 3

{{at least three, use-the-same-template-structure-as-before}}

## Rationale N

{{more if desired, use-the-same-template-structure-as-before}}
