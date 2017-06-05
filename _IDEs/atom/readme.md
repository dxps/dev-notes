

These are my custom settings related to `tab-bar` with `tab` and `close-icon`, plus `status-bar`:

```less
/* ------- vision8 custom styles : begin ------- */

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

// atom-brackets-glow settings

@bright-color: fade(#D11B24, 25%);
@dim-color: fade(#D11B24, 5%);

@keyframes glow {
  to {
    background: @dim-color;
    box-shadow: 0 0 16px 2px @dim-color;
  }
}

atom-text-editor .bracket-matcher .region {
  background: @bright-color;
  box-shadow: 0 0 0 2px @bright-color;
  border-radius: 64px;
  padding: 4px 4px 13px 4px;
  animation: glow 1.5s steps(10, start) infinite alternate;
}

/* ------- vision8 custom styles : end ------- */
```

And that's the result (with UI Theme = 'One Light' and Syntax Theme = 'Solarized Light'):
![](https://github.com/vision8tech/dev-notes/raw/master/_IDEs/atom/images/tabbar-statusbar-result.png)
