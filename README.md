# css笔记
> * 外层设置border-radius，内层设置背景，如果外出没有内边距，内层会遮挡外层的圆角

## 打印 去掉 页眉，页脚
```css
<style media="print">
    @page {
      size: auto;  /* auto is the initial value */
      margin: 0mm; /* this affects the margin in the printer settings */
    }
</style>
```

## img 底边空白      
> * vertical-align: bottom;

## Url icon 尺寸
> * 32 * 32

## <!DOCTYPE html>
> * 全称为Document Type HyperText Mark-up Language
> * 意思为文档种类为超文本标记性语言
> * 此标签可告知浏览器文档使用哪种 HTML 或 XHTML 规范解析
> * 避免出现怪异模式，按统一标准解析html


## vw vh
> * vw vh是视窗单位，也是相对单位，由视窗（Viewport）大小决定，单位1，代表1%，1vw = 视窗宽度的1%


## calc()
> * 使用“+”、“-”、“*” 和 “/”四则运算
> * 可以使用百分比、px、em、rem等单位
> * 可以混合使用各种单位进行计算
> * 表达式中有“+”和“-”时，其前后必须要有空格，如”widht: calc(12%+5em)”这种没有空格的写法是错误的
> * 表达式中有“*”和“/”时，其前后可以没有空格，但建议留有空格
> * less 中使用 calc(~"100% - 80px")
兼容性
```css
width: 208px; /* Fallback for browsers that don't support the calc() function */ 
width: -moz-calc(25% - 10px * 2 - 8px * 2 - 20px); 
width: -webkit-calc(25% - 10px * 2 - 8px * 2 - 20px); 
width: calc(25% - 10px * 2 - 8px * 2 - 20px);
```
