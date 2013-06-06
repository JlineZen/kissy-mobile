
# Kissy Mobile 硬件测试基准

![](http://img01.taobaocdn.com/tps/i1/T1uGWxXx8hXXaZ8zjj-565-118.png)

说明： 

1，浏览器均为当前最新正式版
2，测试基准分为三级，A-级优先级最高，B-级次之（无功能性bug）
 
 ps：H5部分测试基准的制定原则是 

 1，基于浏览器的市场分布趋势
 2，基于淘宝用户的设备硬件情况

## 淘宝网移动硬件设备占有率

硬件设备

![](http://img03.taobaocdn.com/tps/i3/T1yg9tXCJhXXb7dhUe-420-376.png)

操作系统

![](http://img02.taobaocdn.com/tps/i2/T1XuewXrFaXXX53dHU-512-217.png)

PPS：UCWeb浏览器在国内市场占有率为50%，但内核和Safari以及Chrome一致，属于同类项，列为B级别，即在Safari/Chrome测试通过对功能在UC中基本可用，保持主功能ok即可

### 测试你的手机浏览器UA

![](http://img03.taobaocdn.com/tps/i3/T1dPCwXstbXXXwUNUD-222-215.png)

### 设备尺寸

此项为可选

- Android 320、480
- iphone 640（CSS尺寸以320为基准）
- ipad 768

### 浏览器内核、外壳、Webview

一个完整的浏览器由三部分组成，渲染引擎、JavaScript引擎、外壳，测试基准要尽可能的涵盖主流的内核，在移动领域情况稍微复杂，Webview成为另外一种形式的“外壳”。这在H5和Native相互交互的场景中较为常见。和PC环境不同，对页面功能兼容性影响最甚的因素不是内核差异，而是外壳对于内核的修改程度以及操作系统版本差异。因此，PC环境中的同类项归类原则不适用于移动端。因此GBS不能以内核来归类，而以操作系统来归类。
