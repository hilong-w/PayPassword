# PayPassword
6位数字支付密码设置插件

在使用的位置注册插件。

注册插件的confirm事件，在事件中可以获取设置的密码。
onConfirm(e) {
  let password = e.value;
}

注册input事件，可以输入事件进行控制。
onInput(e) {
  //e.cancel = true;
}
