# jQuery_ajax
JQ的ajax方法
<pre>
$.ajax({
  url:'www.baidu.com',             //必填
  type:'post',              //传输方式post 默认为get  get时将数据转换成字符串格式并添加到URL的后面  如果不想转换成字符串需设置processData为false
  data:{city:'shanghai'},  //发送到服务器的数据
  processData:false,  //默认为true     如果不想把数据转换成字符串只要设置为false，比如传输XML对象给服务器时用false
  dataType:'json',    //数据类型json
  cache:true,         //缓存 如果多次通过ajax请求同一个地址  true只有第一次从服务器请求 后面的会在缓存中获取（缓存中存在）
  crossDomain:true,  //跨域
  async:false,         //异步  默认true; 默认情况下都是异步传输
  success:function(){}  //连接服务器成功后 执行的函数
    })
</pre>
