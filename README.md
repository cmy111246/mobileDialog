# mobileDialog
mobile dialog

##options
```c
 var defaultOptions = {
      title: '',
      content: '<p>暂无数据</p>',
      canDisnoLayer: true, //点击遮罩层是否关闭弹窗
      showLayer: true, //是否显示遮罩
      buttons:[],//按钮
      ok:null,
      cancel: null,
      speed: 310 //动画时间
  }
  

##buttons
  ```b
  buttons:[
      {
          id: 'ok',
          className: 'btn-green mr10',
          value: "确定",
          callback: function(){
              alert("a")
          }
      },
      {
          id: 'cancel',
          className: 'btn-green',
          value: "取消",
          callback: function(){
              
          }
      }
  ]


###调用
```a
$(".a").on('click', function(){
    var a = new dialog({
        title:"1",
        content:$(".J_template").html()
    });
    a.open();
});
