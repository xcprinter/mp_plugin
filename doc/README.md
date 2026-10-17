# 蓝牙硬件插件

## 支持硬件
* 蓝牙打印机
* 蓝牙秤

## 如何使用

* [代码示例](https://github.com/xcprinter/mp_plugin/tree/main/miniprogram)
* [代码示例2](https://github.com/one-work/mp/tree/main/pages/print)

* 引用
```js
const bluetooth = requirePlugin('bluetooth')
const printer = new bluetooth.BluetoothPrinter(wx, this)
```

* 打印
```js
printer.getState({
  success: res => {
    if (res.printable) {
      printer.writeValue(data) // data 为打印内容
    }
  }
})
```
