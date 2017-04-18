# jquery each()详细介绍

##### each 方法能使DOM循环结构简单，不容易出错。each()函数封装了十分强大的遍历功能。使用方便，它可以遍历一维数组，多维数组，DOM,JSON等等。

* 在javaScript开发过程中使用$each可以大大的减轻我们的工作量。

  ##### 下面提一下each的几种常用的用法
  
   each处理一维数组

        var arr1 = [ "aaa", "bbb", "ccc" ];      
        $.each(arr1, function(i,val){      
            alert(i);   
            alert(val);
        }); 

   alert(i)将输出0，1，2

   alert(val)将输出aaa，bbb，ccc

  
   each处理二维数组
 
        
        var arr2 = [['a', 'aa', 'aaa'], ['b', 'bb', 'bbb'], ['c', 'cc', 'ccc']]; 
        $.each(arr2, function(i, item){
            alert(i);
            alert(item);
        });  
      
  
   arr2为一个二维数组，item相当于取这二维数组中的每一个数组。

   item[0]相对于取每一个一维数组里的第一个值   

   alert(i)将输出为0，1，2，因为这二维数组含有3个数组元素

   alert(item)将输出为  ['a', 'aa', 'aaa']，['b', 'bb', 'bbb']，['c', 'cc', 'ccc']
