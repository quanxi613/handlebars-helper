# handlebars-helper
常用的handlebars helper总结


## help列表

1. eq
  用法: `{{#eq left right}} block {{else}} inverse {{/eq}}` else为可选
  含义: 如果left严格等于right, 渲染block, 否则渲染inverse

2. noteq
  用法: `{{#noteq left right}} block {{else}} inverse {{/noteq}}` else为可选
  含义: 如果left不严格等于right, 渲染block, 否则渲染inverse

3. gt
  用法: `{{#gt left right}} block {{else}} inverse {{/gt}}` else为可选
  含义: 如果left大于right, 渲染block, 否则渲染inverse

4. gte
  用法: `{{#gte left right}} block {{else}} inverse {{/gte}}` else为可选
  含义: 如果left大于等于right, 渲染block, 否则渲染inverse

5. lt
  用法: `{{#lt left right}} block {{else}} inverse {{/lt}}` else为可选
  含义: 如果left小于right, 渲染block, 否则渲染inverse

6. lte
  用法: `{{#lte left right}} block {{else}} inverse {{/lte}}` else为可选
  含义: 如果left小于等于right, 渲染block, 否则渲染inverse

7. even
  用法: `{{#even num}} block {{else}} inverse {{/even}}` else为可选
  含义: 如果num为偶数, 渲染block, 否则渲染inverse

8. odd
  用法: `{{#odd num}} block {{else}} inverse {{/odd}}` else为可选
  含义: 如果num为奇数, 渲染block, 否则渲染inverse

9. multiple
  用法: `{{#multiple num base}} block {{else}} inverse {{/multiple}}` else为可选
  含义: 如果num为base的倍数, 渲染block, 否则渲染inverse

10. and
  用法: `{{#and item1 item2 ...}} block {{else}} inverse {{/and}}` else为可选
  含义: 多个值求并 &&, 参数可变长,如果结果true渲染block, 否则渲染inverse

11. or
  用法: `{{#or item1 item2 ...}} block {{else}} inverse {{/or}}` else为可选
  含义: 多个值求或 ||, 参数可变长,如果结果true渲染block, 否则渲染inverse

12. stringify
  用法: `{{stringify obj}}`
  含义: 将obj序列号为字符串,并执行HTML特俗字符转换, 如", <, >, &这样
        就可以直接将对象设置到DOM属性上,或者输出对象
