# study-note

$(function(){
	//alert(document.getElementById(‘box’));	
//[object HTMLDivElement],原生DOM对象
Alert($(‘#box’).get(0));
	//[object HTMLDivElement],原生DOM对象

});
jQuery.noConflict();	//自行了断，把自己的$所有权剔除
alert($('*').length);	‘求’所有DOM节点
alert($('*')[0].nodeName);	‘求’第一个DOM节点
.class1.class2{	//多个class选择器}
.class1,class2{	//群组选择器}
选择器越复杂，那么字符串解析就越慢，只追求必要的确定性。
$('#box p').css('color','orange');		下一行，是等价的find()方法
$('#box').find('p').css('color','orange');
$('#inbox+p').css('color','pink');		下一行，是等价的next()方法
 $('#inbox').next('p').css('color','pink');
nextAll()		children() 		prev() 		prevAll()	
siblings()同级上下所有元素选定
nextUntil()		prevUntil()
