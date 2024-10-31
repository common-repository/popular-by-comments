=== Popular-by-comments ===


Contributors: xinfuweng
Donate link: https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=Y5ECK2QA6R9PS&lc=C2&item_name=Popular%2dby%2dcomments&item_number=xinfuweng&currency_code=USD&bn=PP%2dDonationsBF%3abtn_donateCC_LG%2egif%3aNonHosted
Tags: popular,post
Plugin URI: http://www.juqng.com/wordpress-plugin/popular-by-comments/
Author URI: http://www.juqng.com/
Author: xinfuweng
Requires at least: 2.7.1
Tested up to: 2.7.1
Stable tag: 2.7.1
Description:Displays the popular posts based on comments, you can use Custom Fields.


== Description ==

Displays the popular posts based on comments, you can use Custom Fields.

本插件依据评论数量来评定热门程度，

Author URI: http://www.juqng.com/

Plugin URI: http://www.juqng.com/wordpress-plugin/popular-by-comments/



== Installation ==

使用方法：<br />
1.下载后解压上传至/wp-content/plugins/目录，<br />
 Upload this directory to your plugins directory to the /wp-content/plugins/ directory<br />
2.进入后台控制板，激活插件；<br />
Activate the Plugin via the Plugins section at your WordPress admin panel.<br />
3.在你的模板中使用插入inside your template.<br />

`<?php if(function_exists('popularbycomments')) { popularbycomments();};?> `

4.高级使用

`<?php if (function_exists('popularbycomments')) { 
	popularbycomments('<li><h5>Popular posts</h5><ul>',
	10,
	'no',
	'<li class="%No%"><a href="%post_url%"><img src="%post_meta%"/>%post_title%</a> %comments% comments</li>',
	'</ul><a href="%moreurl%">more popular</a></li>',
	'index_image',
	'http://localhost/juqng/wp-content/uploads/2009/03/il18.jpg',
	'http://localhost/juqng/index.php/popular-items/');
	} 
 ?>
`

参数含义依次为：<br />
1.热门文章列表前代码；<br />
2.显示文章数量；<br />
3.单个文章列表递曾类名如：no1,no2,no3...；<br />
4.每个列表输出格式；<br />
5.结尾更多页链接输出格式；<br />
6.自定义字段名称；<br />
7.自定义字段值默认替换；<br />
8.更多链接地址。
输出格式介绍：%No%为类名；%post_url%日志地址；%post_meta%自定义字段值（Custom Fields），%comments%评论数量；%moreurl%更多链接地址，%post_title%日志标题；