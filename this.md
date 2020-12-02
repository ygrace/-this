# 关于this的知识点（假设fn是一个普通函数，arrow是一个箭头函数）
1. 在new fn()调用的时候，fn里的this指向新生成的对象，这是new决定的
2. 在fn()调用中，this默认指向window，这是浏览器决定的
3. 在obj.fn()调用中，this默认指向obj，这是js的隐式传this
4. 在fn.call(xxx)调用中，this就是xxx,这是开发者通过call显示指定的this
5. 在arrow()的调用中，arrow里面的this就是arrow外面的this，因为箭头函数里面没有自己的this
6. 在arrow.call(xxx)调用中，arrow里面的this还是arrow外面的this，因为箭头函数里面没有自己的this