# Markdown使用

## 数学公式支持

		<script type="text/javascript" 									
		src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-
		MML_HTMLorMML"></script>


	    <script type="text/x-mathjax-config">
	        MathJax.Hub.Config({
	            tex2jax: {inlineMath: [['$', '$']]},
	            messageStyle: "none"
	        });
	    </script>


		行间公式：$$···$$
		行内公式：$···$


## 图片超链接

<a href="https://crash-database.readthedocs.io/en/master/"><img src="https://img1.wenhairu.com/images/2020/10/11/CkiRP.png"></a>

		<a href="[target-url]"><img src="[image-url]"></a>

## 页内跳转

[Index-name](#Crash)
<a name='Crash'>Target-name</a>

		[Index-name](#Crash)
		<a name='Crash'>Target-name</a>

## 表格形式

<table>
    <tr>
        <td><img src='Crash logo special.png'>
        <td><img src='Crash logo special.png'>
        </td>
    <tr>
        <td><img src='Crash logo special.png'>
        <td><img src='Crash logo special.png'>
        </td>
    </tr>
</table>

		<table>
			<tr>
			    <td><···>
			    </td><···>
			</tr>
		</table>