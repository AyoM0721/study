#第五章 JavaScript语句
###5.1 分支语句
5.1.1 if语句

      var a = 10;
      //小括号里一定要是true
      if(a<20){
          alert('yes');
      }
  
5.1.2 if...else语句

      if(a<10){
          alert('yes');
      }else{
          alert('no');
      }

5.1.3 if...else if语句

        if(a<60){
            alert('D');
        }else if(a>=60 && a<75){
            alert('C');
        }
        }else if(a>=75 && a<85){
            alert('B');
        }
        }else if(a>=85 && a<=100){
            alert('A');
        }else {
            alert('缺考');
        }

5.1.4 switch 语句
switch小括号中一般情况是一个变量名,这个变量可能会有不同的取值.所有的case都是"或"的关系,case后面的值会与变量值作比对,满足后就执行case后面的代码.不写break就会将所有的比对进行一遍.
        var a = 10;
        //将判断的内容写在括号里
        switch(a){
            case 值1:
            //执行代码
            break;
            case 值2:
            //执行代码
            break;
            case 值3:
            //执行代码
            break;
            case 值n:
            //执行代码
            break;
            default:
            //执行代码
        }

###5.2 循环语句
5.2.1 while循环

while语句是一种前测试语句(先判断一下再执行),循环的目的是为了反复执行语句或代码块,只要表达式为true就循环执行,一旦为假的时候,循环退出.
	
	 var a = 1;
        var res = 0;
        while(a<=100){
            res += a;
            a++;
        }
        console.log(res);
        show.innerHTML = res;
5.2.2 do...while循环

do...while语句是一种后测试语句,就是在循环体中的代码执行之后,才开始判断条件.也就是说,在表达式判断之前,循环体内的代码至少会被执行一次.

	do {
            var say = confirm('我很丑，但是我很温柔，我们交往吧，你同意吗？');
            //返回值是true 或 false
            if(say){
                alert('现在拍婚纱打三折');
            }
        } while (!say);
5.2.3 for循环

for循环是一种前测试语句，一般情况下，有三个基础表达式语句，每一个要用分号隔开.

	//
	for(var )