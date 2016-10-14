
# jsFeeder by Gojira

## What can you do with jsFeeder?

It will replace the content of your elements with test content. So you can see the when your layout breaks.
This is to check if your layout doesn't break. For example: check if your navigation doesn't break with menu items with more than 2 words.

## How to use jsFeeder

Simple add data-feed to your element with value the type and number of words or sentences.
Refresh your page and new content will be inserted in your elements.

### How to use jsFeeder

#### Words

```
<a href="#" data-feed="w=2">Nav item 1</a>
```

The content "Nav item 1" will be replaced with 2 random words


#### Sentences

```
<div data-feed="s=5">
    Lorem ipsum dolor sit amet, consectetur adipisicing elit.
</div>
```

The content between the div will be replaced with 5 sentences.