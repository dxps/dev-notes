

These are my custom settings related to `tab-bar` with `tab` and `close-icon`, plus `status-bar`:

```less
/* ------- visvadw custom styles : begin ------- */

@font-size: 15px;
@tab-height: 28px;
@line-height: @tab-height;

atom-workspace {
    font-family: 'Sys-Light', sans-serif;
    font-size: @font-size;
}

.tab-bar {
  height: @tab-height + 1;
  line-height: @tab-height;
  .tab {
    height: @tab-height + 1;
    line-height: @tab-height;
    max-width: 170px;
    .close-icon {
      top: 8px;
      right: 6px;
      font-size: 11px;
    }
  }
}

.status-bar {
  font-size: 14px;
  height: 26px;
  line-height: 26px;
}

/* ------- visvadw custom styles : end ------- */
```

And that's the result (with UI Theme = 'One Light' and Syntax Theme = 'Solarized Light'):
![](https://github.com/visvadw/dev-notes/raw/master/atom/images/tabbar-statusbar-result.png)
