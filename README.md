
# FeedEm - test your design's tolerance for dynamic content

## What can you do with FeedEm?

It will test your layout to its maximum by testing its tolerance by dynamic content. This way you can see if your layout breaks. If it breaks, fix it! For example: check if your navigation doesn't break with menu items with more than 2 words. Or you can use it to insert test content if you don't have your final copy yet.

## How to use FeedEm

FeedEm is available via `npm install feedem` or `bower install feedem`


Include the script right above the closing body tag.

```
<script src="path/feedem.js"></script>
```


Simple add data-feed attribute to your element to feed 'em random content.
Refresh your page and new content will be feeded to your elements.

### Words

```
<a href="#" data-feed="w=2">Nav item 1</a>
```

The content "Nav item 1" will be replaced with 2 random words

### Sentences

```
<div data-feed="s=5">
    Lorem ipsum dolor sit amet, consectetur adipisicing elit.
</div>
```

The content between the div will be replaced with 5 sentences.

### Paragraphs

Sometimes you want to insert paragraphs, jsFeed can do that for you by adding the p value

```
<div data-feed="p=2">
</div>
```

2 random paragraphs are added inside the div

## Options
There is only 1 option at the moment. You can highlight the feeded elements on by adding the option `highlight` and `highlightColour`. Hightlight is default on false.

```
$(function(){
    site.feedEm({
        highlight: true,
        highlightColour: '#eeeeff'
    })
});
```

## F5 the shit out of it!
Keep pressing ctrl + f5 or cmd + f5 to test your layout.


# To do
- Got any ideas for other options?

# License
MIT License

Copyright (c) 2016 Dennis Perremans

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.