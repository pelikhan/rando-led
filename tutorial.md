# Random lights

## Step 1

Add a ``||led:toggle||`` block under the ``||basic:forever||``
event.

```blocks
basic.forever(function () {
    led.toggle(0, 0)
})
```
## Step 2

Insert a block to generate a random ``x`` LED position to toggle,
a nubmer between ``0`` and ``4``.

```blocks
basic.forever(function () {
    led.toggle(Math.randomRange(0, 4), 0)
})
```

## Step 3

Insert a another block to generate a random ``y`` LED position to toggle,
a nubmer between ``0`` and ``4``.

```blocks
basic.forever(function () {
    led.toggle(Math.randomRange(0, 4), Math.randomRange(0, 4))
})
```

<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
