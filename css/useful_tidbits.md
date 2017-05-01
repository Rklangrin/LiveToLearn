# Useful Tidbits

* Set a specific height for divs and use `overflow: scroll` in order to prevent text not contained within the specified height from just displaying right after the end of the div.

```sass
  div
    height: 200px
    overflow: scroll
```

* If you don't want text to wrap
```sass
  div
    white-space: nowrap
```

## Sneaky Tricks
- For responsiveness and uniform height
  * Set div height to 0 and padding-bottom to 50%. Padding-bottom is measured in terms of it's width. Setting it to 50% means it should be 50% of whatever it's max-width is. 