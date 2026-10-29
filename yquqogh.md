代发 wailian999

[U49] PHP：只读属性
来源：http://wap.zdbjq.cn/Article/details/gbkaetfkx.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gweksngza.sHtML

[U50] PHP：构造器属性提升
来源：http://www.blog.zdbjq.cn/Article/details/gnakspgug.sHtML

public function __construct(private int $id) {}
来源：http://wap.hesvh.cn/Article/details/gkzeyvudg.sHtML

[U51] PHP：数组解构
来源：http://blog.hesvh.cn/Article/details/gtjzgyajs.sHtML

[$a, $b] = $arr;
来源：http://m.share.hesvh.cn/Article/details/goylpurfv.sHtML

[U52] PHP：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gpkdmpexn.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gwbdqfgzd.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gntoltzxm.sHtML

$v = $a ?? $b ?? "default";
来源：http://wap.fehbvm.com/Article/details/gyendnvgc.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/gpffynkjd.sHtML

$obj?->method()
来源：http://baike.fehbvm.com/Article/details/gwzhodsbq.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gdjdrfuha.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gyntmswcd.sHtML

[U56] PHP：命名参数
来源：http://read.share.hesvh.cn/Article/details/gdylngybo.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/gokelgmrc.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gutthpfow.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/gpyekmdjf.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/ghyxbfyni.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://mobile.fehbvm.com/Article/details/gtaavntsi.sHtML

[U59] PHP：自定义排序
来源：http://www.share.zdbjq.cn/Article/details/gjgaddebm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/ganqnsmcs.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.hesvh.cn/Article/details/gjjwsyems.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gjbiqmaqk.sHtML

[U61] PHP：正则
来源：http://3g.hesvh.cn/Article/details/gjiufcozh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsypulfhd.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gfhtmotpf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/glzcwbhhc.sHtML

[U63] PHP：文件读写
来源：http://3g.fehbvm.com/Article/details/gpjybhort.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/ghhcbgjrv.sHtML

[U64] PHP：目录遍历
来源：http://mobile.fehbvm.com/Article/details/gqukjpcso.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.fehbvm.com/Article/details/gpkxknyig.sHtML

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/grnnvrful.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/glutxupsv.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gkgjkvcnp.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.zdbjq.cn/Article/details/gjelaexrh.sHtML

[U67] PHP：处理文件上传
来源：http://mobile.zdbjq.cn/Article/details/gmgqxcpzx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gapcghwmb.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gfyppqaaw.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.hesvh.cn/Article/details/glyefxbxj.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.hesvh.cn/Article/details/gujdrqfco.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gpnjlyhwa.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/gbjifipbc.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://baike.zdbjq.cn/Article/details/gaaznynvm.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gcjqmyhql.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gclieeadk.sHtML

[U72] PHP：写错误日志
来源：http://mobile.zdbjq.cn/Article/details/gxuewoyfl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/gaebtgelq.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gfbrhtuqx.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gjtrraezu.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gilhtvdzr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.hesvh.cn/Article/details/gfwuwlelc.sHtML

[U75] PHP：依赖注入
来源：http://3g.zdbjq.cn/Article/details/gdtcsguck.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gaeerqzus.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gmsevfvei.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/giijcqkub.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gbcbtqaev.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gzivsberj.sHtML

[U78] PHP：单元测试
来源：http://wap.fehbvm.com/Article/details/goowbwvao.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gypmxysap.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gewqjqqxn.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.zdbjq.cn/Article/details/gqnrsrhqo.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/goponhrad.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gsbvibixh.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gwwdcewnk.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gssxyxlpj.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gmjppnmfh.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gtaxrorzi.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gmowxaxei.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/ghnnaniad.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fehbvm.com/Article/details/gbttcaupd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gfyhlmlzd.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/gwavgjjau.sHtML

a?.b?.c
来源：http://www.blog.hesvh.cn/Article/details/gzxdjhhco.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gxanwyaea.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gimqkghcm.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gescpngac.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gnmjmmeux.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gcajgetkr.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gxbhqrelg.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gqbvfysoy.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/grpuuwmcd.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gngmaeygb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gnlctmlko.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gycrlvlzh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gaoeofsbz.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gcandrvil.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcyalosnf.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gdvjxqgcf.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gvqhrgsxq.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gsghkvzeh.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gaswewrhy.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gegenacbe.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gymhsrszw.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gumxtwddh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gwrjenand.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gubbgahbg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/guukmerjk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gyuvxqnse.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gasvcvcyd.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/gizawdgqq.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/ggctoxovg.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gedxslfxu.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gxoizqasi.sHtML

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/ghnibeewc.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/ghkkbdwje.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gkbytmjxf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/gmbxwkzhn.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gyyudfvua.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.zdbjq.cn/Article/details/gcclhwfoj.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gvpyjdzsj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/guvekhovo.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gbdwerehj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gfqspybfx.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/ghjhfqohj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gckkcxlzz.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gpncbertt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gocuplkah.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gjqreyxya.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gmejcxybo.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gzgwetota.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gfmgptwnk.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gcteqvuhc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.hesvh.cn/Article/details/gxxwaoeow.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/ghusngcrr.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gtqjjjlox.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gymfdflwx.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gzyxubqjp.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gzkefxtzc.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gwtqruydl.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/guvzofvun.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gjpwwukdy.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gxwgnwfkw.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gwfloelek.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gemtjfwys.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gxybnyskk.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gwbcmqpsj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gdgleyavd.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gpuppimzz.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gwvocdcmr.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gwylszdle.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gideauhmd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gktbhmvjz.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gqxpccaxi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdfsfwryr.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gnjqcweax.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gctzvmoxx.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gfqjnoqrl.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gbkuirwng.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/glhvngktp.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gpthxddhl.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/goeszonth.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gyqubkhme.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gmavazxtd.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/goasbhuei.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/giwdpnxnk.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/grznozgew.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gyweiksgg.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gslfdiwhm.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gcklzycgl.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gngmdaaiy.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gptbbesib.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gbjtlteok.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gquvzlcgs.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/ggvbteqhf.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gbqnhrupt.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/ghjizomir.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/ggeidvzpw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/goymaeoat.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gvgyjwnlo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gbickdive.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gptpzsick.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gghquamcu.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gwuyfufsi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gfzxrhfbv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gliscydlf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gxynvlzzc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gynjmkjdj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gfqzojxry.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gozqmwlwk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gozknviwj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/grqsbreqf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/grvkskwch.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gaobiojld.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/goselbstw.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/gjwgpglnk.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gihcmngsp.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/grpcawfoo.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gfqlokplz.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gkqhrdlyp.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gkfefcicc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gmztovzbs.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gmvydzrua.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gfmqrgmib.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gvfixnidm.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gxogztobs.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gcbczivbn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gyxvhwkjg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gtgthpsgc.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gayyphreu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxwjoyjsz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gwumtdoeg.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gpjfsalfz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmigjgyqc.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gxoxoazhi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/guszlibtu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gwweypdjy.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gvyqworza.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fehbvm.com/Article/details/gaykifeba.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gbmnkdxeq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gdmtvezlp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/glbfpkbox.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gqnlejjpd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gyeuoryco.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gwfphoeuu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gafnmyvmv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gmpqwaqrj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gzgnsququ.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gtzmyfrlv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gqykotjlj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gcdgcsatv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/glzreemfn.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gubmfpnlc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gltimttej.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gumtlivpc.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gogevhqln.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gcppoqxmk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gjoqojeuh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gxvqgiyzx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gsfmfvvdh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gsdrpphdq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/grajdttns.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gectyizku.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gyslqgyap.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/glcrgiraj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gkbgkrkdb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gxjnfrbgr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gbtmmzzhk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gjqgqzgjt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gwmdfjcdv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gjaqwqnoy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gbmfdkhuj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gzujdjoxg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/ghirdgvep.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/gyntwcvpf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gouoggvtv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gobclssqt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gyxtsnfzp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyamyevtd.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gwwdlzgoa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfeauhclt.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gqacyyzlq.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gqhkqtmrl.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gksmirkkw.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gbauwevuw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gylduxqbg.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/ghodnmvkx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gvrlyiqar.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/gaawfuzoj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gpclbxkgq.sHtML

[A02] 变量声明与赋值
来源：http://wap.fehbvm.com/Article/details/gieqcjkll.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gnoyvlpxd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gbztaxfpj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gdyrauvtw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/gyvvjkoct.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gajycqboj.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gkfgzjhuc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/ghcxiqlej.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/ggmghnsjd.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gqnaedhan.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gwlzwlvun.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/geiqyhjxm.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/guacdnwum.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/ghyolmyxm.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gpfhgljuy.sHtML

Go:   const PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gkremubuv.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/ghkxufdcq.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gsynolbir.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/gmufdtuex.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gzzprwqkz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gqglvdfdn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/ghuomvfic.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/ggiiqduto.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/gimkzlnmu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/gtjkjyryp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/gdximdgwv.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fehbvm.com/Article/details/gkswlrlxk.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/gabwmkmpb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gtyvhrjkq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/grjmszccy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gkiatrlsb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gpepirhxa.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gryqebgbb.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gluasyvsz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gelzdinif.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gidogxxlj.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/grxcqcvlu.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/gvcbjvwcw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gpgkpcipi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gwuidushv.sHtML


<!-- 参考信息 -->