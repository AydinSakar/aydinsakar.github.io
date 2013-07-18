---
layout: post
title: "Code Blocks Options with Octopress"
date: 2013-07-17 17:11
comments: true
categories: 
- Octopress
- Markdown
---

I actually figured out several different options that we can use to insert code blocks with [Octopress][]


### 1. Markdown codeblocks:

We have to use 4 spaces or 1 tab to designate that this is a codeblock.

        var respond = function(response, data, err) {
            var responseObj = {data: data, error: err};
            response.writeHead(200, {"Content-Type":"application/json"});
            response.write(JSON.stringify(responseObj));
            response.end();
        };
        var arr1 = new Array(arrayLength);
        var arr2 = new Array(element0, element1, ..., elementN);

And this is what we get with the 4 spaces, or the tabs removed from the start of the line.

    var respond = function(response, data, err) {
        var responseObj = {data: data, error: err};
        response.writeHead(200, {"Content-Type":"application/json"});
        response.write(JSON.stringify(responseObj));
        response.end();
    };
    var arr1 = new Array(arrayLength);
    var arr2 = new Array(element0, element1, ..., elementN);

And this is the HTML that is written for you:

{% codeblock HTML Result lang:html %}
<pre><code>var respond = function(response, data, err) {
    var responseObj = {data: data, error: err};
    response.writeHead(200, {"Content-Type":"application/json"});
    response.write(JSON.stringify(responseObj));
    response.end();
};
var arr1 = new Array(arrayLength);
var arr2 = new Array(element0, element1, ..., elementN);
</code></pre>
{% endcodeblock %}

### 2. Backtick Code Blocks (GitHub Flavored Markdown):
    ``` [language] [title] [url] [link text]
    var respond = function(response, data, err) {
        var responseObj = {data: data, error: err};
        response.writeHead(200, {"Content-Type":"application/json"});
        response.write(JSON.stringify(responseObj));
        response.end();
    };
    var arr1 = new Array(arrayLength);
    var arr2 = new Array(element0, element1, ..., elementN);
    ```    

``` javascript Backtick Code Blocks (GitHub Flavored Markdown)
var respond = function(response, data, err) {
    var responseObj = {data: data, error: err};
    response.writeHead(200, {"Content-Type":"application/json"});
    response.write(JSON.stringify(responseObj));
    response.end();
};
var arr1 = new Array(arrayLength);
var arr2 = new Array(element0, element1, ..., elementN);
```

### 3. Codeblocks

{% raw %}
    {% codeblock [title] [lang:language] [url] [link text] %}
    var respond = function(response, data, err) {
        var responseObj = {data: data, error: err};
        response.writeHead(200, {"Content-Type":"application/json"});
        response.write(JSON.stringify(responseObj));
        response.end();
    };
    {% endcodeblock %}
{% endraw %}

{% codeblock  Javascript Example lang:js %}
var respond = function(response, data, err) {
    var responseObj = {data: data, error: err};
    response.writeHead(200, {"Content-Type":"application/json"});
    response.write(JSON.stringify(responseObj));
    response.end();
};
var arr1 = new Array(arrayLength);
var arr2 = new Array(element0, element1, ..., elementN);
{% endcodeblock %}

#### Note:
For code-coloring to work, be sure you have Python27 at your Path.

[Octopress]:  http://octopress.org/ "Octopress"
