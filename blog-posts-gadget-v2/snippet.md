# Snippet

Snippet of the post's content.

`data:posts[i].snippets`

## Short

```html
<!-- Snippet -->
<data:post.snippets.short/>
```

Support for *jump break*:

```html
<!-- Snippet -->
<b:if cond='data:post.hasJumpLink'>
  <data:post.body/>
<b:else/>
  <data:post.snippets.short/>
</b:if>
```

## Long

```html
<!-- Snippet -->
<data:post.snippets.long/>
```

Support for *jump break*:

```html
<!-- Snippet -->
<b:if cond='data:post.hasJumpLink'>
  <data:post.body/>
<b:else/>
  <data:post.snippets.long/>
</b:if>
```

## Custom

```html
<!-- Snippet -->
<b:eval expr='snippet(data:post.snippets.long, { length: 150, links: false, linebreaks: false, ellipsis: true })'/>
```

Support for *jump break*:

```html
<!-- Snippet -->
<b:if cond='data:post.hasJumpLink'>
  <data:post.body/>
<b:else/>
  <b:eval expr='snippet(data:post.snippets.long, { length: 150, links: false, linebreaks: false, ellipsis: true })'/>
</b:if>
```
