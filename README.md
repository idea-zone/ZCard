# BWLabels

基于 [mini-vlook](https://github.com/idea-zone/mini-vlook) 主题的一组标准化卡片模板：目的是更方便的记录卡片笔记。



可基于 mini-vlook 的彩虹标签功能自定义：

###### `#功能|微章#(theme1!)`

* 添加内容块 `#自定义属性|f=wz#` ,  当前块不会渲染微章，具有层级关系时，会影响到当前块的所有子块内。

  * `#微章标题|微章内容#(颜色)` 或者 `#微章标题#(颜色)` 仅渲染标题

  * 其中 `(颜色)` 可以省略，即仅写为 `#微章标题|微章内容#` ，省略颜色时，渲染为内置的 `theme2`

  * 颜色可以写选择预定义的颜色名, 或者 `#ffffff` 格式的颜色值（*建议用预定的颜色名称*）

    ``` ts
    // 支持的颜色名称
    'red', 'orange', 'yellow', 'lime', 'green', 
    'aqua', 'cyan', 'blue', 'sea', 'steel', 'purple', 
    'magenta', 'pink', 'gold', 'brown', 'gray', 'black', 
    'theme1', 'theme2'
    ```

  * 可以在颜色后添加 `!` 强调微章内容。即写为 `#微章标题|微章内容#(red!)`

    `#微章标题|微章内容#` `#状态|未完成#(theme1)` `#对外公开|V1.0.0#(green)`  `#💡|提示#(orange)`

* 也可以仅有微章标题：`#微章标题#` `#状态#(theme1)` `#对外公开#(green)` `#💡#(orange)`

