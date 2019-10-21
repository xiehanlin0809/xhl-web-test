10.21日测验
在本地创建一个文件夹叫test10.21 ,文件夹中应含有5个html文件,分别命名为1.html等.再创建一个readme.txt文件,将这几个问题贴如其中,最后将html中的js代码贴到答的下方.

1.将两个字符利用字符串对象的方法变成一个字符,显示在页面id为h1的元素中
答:<h1 id="h1"></h1>
		<script type="text/javascript">
			var a = '123';
			var b = 'nihao';
			document.getElementById('h1').innerHTML=a.concat(b);
		</script>

2.一个富豪想存87万,给理财顾问写了87w,请自动生成存储870000的方法,显示在页面id为h2的元素中
答:<h2 id="h2"></h2>
        <script>
             var str = '87';
             var estr = str.padEnd(6,'0');
             document.getElementById('h2').innerHTML= estr;
        </script>

3.一个数字79387.348的工程款,保留两位小数存入,显示在页面id为h3的元素中
答:<h3 id="h3"></h3>
		<script type="text/javascript">
			var num = new Number(79387.348);
			document.getElementById('h3').innerHTML = num.toFixed(2);
		</script>

4.一张图片是一个相对路径img/head/,icon/1.jpg,我只需要拿到它的文件夹目录后显示在页面id为h4的元素中
答:<h4 id="h4"></h4>
		<script type="text/javascript">
			var h4 = document.getElementById('h4');
			var img = 'img/head/icon/1.jpg';
			h4.innerHTML = img.substr(-5,5);
		</script>

5.用户输入验证码,无论大小写输入都会正确的方法,显示在页面id为h1的元素中,显示在页面id为h4的元素中
答:<h4 id="h4"></h4>
		<script type="text/javascript">
			var str = prompt('输入验证码');
            var h4 = document.getElementById('h4');
            h4.innerHTML = str.toLocaleUpperCase();
		</script>