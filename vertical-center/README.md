# 水平垂直居中

## 仅居中元素定宽高适用：
- [absolute + 负margin]
- [absolute + margin auto]
- [absolute + calc]

## 居中元素不定宽高适用：
- [absolute + transform]
- [writing-mode]
- [lineheight]
- [table]
- [css-table]
- [flex]
- [grid]

## 总结

下面对比下各个方式的优缺点，肯定又双叒叕该有同学说回字的写法了，简单总结下

- PC端有兼容性要求，宽高固定，推荐absolute + 负margin
- PC端有兼容要求，宽高不固定，推荐css-table
- PC端无兼容性要求，推荐flex
- 移动端推荐使用flex

**小贴士：**

| 方法                     | 居中元素定宽高固定 | PC兼容性                        | 移动端兼容性          |
| ---------------------- | --------- | ---------------------------- | --------------- |
| absolute + 负margin     | 是         | ie6+, chrome4+, firefox2+    | 安卓2.3+, iOS6+   |
| absolute + margin auto | 是         | ie6+, chrome4+, firefox2+    | 安卓2.3+, iOS6+   |
| absolute + calc        | 是         | ie9+, chrome19+, firefox4+   | 安卓4.4+, iOS6+   |
| absolute + transform   | 否         | ie9+, chrome4+, firefox3.5+  | 安卓3+, iOS6+     |
| writing-mode           | 否         | ie6+, chrome4+, firefox3.5+  | 安卓2.3+, iOS5.1+ |
| lineheight             | 否         | ie6+, chrome4+, firefox2+    | 安卓2.3+, iOS6+   |
| table                  | 否         | ie6+, chrome4+, firefox2+    | 安卓2.3+, iOS6+   |
| css-table              | 否         | ie8+, chrome4+, firefox2+    | 安卓2.3+, iOS6+   |
| flex                   | 否         | ie10+, chrome4+, firefox2+   | 安卓2.3+, iOS6+   |
| grid                   | 否         | ie10+, chrome57+, firefox52+ | 安卓6+, iOS10.3+  |

