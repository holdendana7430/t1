代发 wailian999

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/geelhofqj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gryfhtazz.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gvkslsycc.sHtML

f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gqgotknze.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/glylhgkji.sHtML

"值: {$a}"
来源：http://read.share.zdbjq.cn/Article/details/gawcldmju.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gjxpcibrx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gfwcwehtn.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gkocllrpx.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gblumucdk.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gfbovhckq.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.fehbvm.com/Article/details/grwaliija.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gesezqkuu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gsygppdph.sHtML

[U62] PHP：日期对象
来源：http://blog.zdbjq.cn/Article/details/gcxgjtoeq.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.zdbjq.cn/Article/details/ggfjlxxml.sHtML

[U63] PHP：文件读写
来源：http://mobile.zdbjq.cn/Article/details/guptnnwui.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://blog.fehbvm.com/Article/details/gckzjpiwi.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/grmrmnsnt.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.blog.fehbvm.com/Article/details/gymivksbx.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gxzotxyzs.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gxzlfjrxg.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.hesvh.cn/Article/details/gqdqbwtaw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gjqkfjawi.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gnpftfitd.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gviqogxsp.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gamoeznlf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gaccvunqs.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gzxmdlrlw.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/glluwxode.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fehbvm.com/Article/details/gnyxearyq.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.zdbjq.cn/Article/details/gqhmqrgzu.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/glewkhull.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/gqcfhayng.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gxgsalizh.sHtML

error_log("失败: " . $e->getMessage());
来源：http://baike.hesvh.cn/Article/details/gkaiwdbcy.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gtiehftcs.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/gipvvdlyr.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gqvjnvwrx.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gfndowvae.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gycbrnjhk.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gxebzdtsm.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gizqdbcba.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.zdbjq.cn/Article/details/gmdehzqmw.sHtML

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gpdfcjknz.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gypxakcqg.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gyalvtrog.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gwxaorxbc.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gucqjomkr.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gxsdevamg.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/gnhnxarxn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/ggppwgpiz.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/ghxzpwxrn.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gdzzkfhwq.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gfroxdozk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gqjsnkvyu.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gmniqtcan.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gqhntzwpa.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.zdbjq.cn/Article/details/gmntxygbq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.zdbjq.cn/Article/details/ggpfrpjel.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gehuasxud.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/ghdnfrjwd.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gmmeopgto.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gjgffaobz.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gfnnxogql.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gidlufrdj.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gdpqbtyld.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gmrtyuvee.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/ggiggvvcz.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gjcptccvw.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.zdbjq.cn/Article/details/givtjyqdl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gmqrggouc.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gwynzoozr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.fehbvm.com/Article/details/gueesxhhu.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.hesvh.cn/Article/details/guyjjepml.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gzjjfdgaj.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gdvmkzwrx.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gltsuerya.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/giahyvmom.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/giwzuiays.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fehbvm.com/Article/details/giuclexxy.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gdzdixvaj.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gxwmdeykr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gcewzdztk.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/ggdeziiwv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gkmwjleds.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/gsonglqjg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gbscvupgv.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/gbmlaarpx.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gvqaspxzr.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gyycjktok.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gpoxkzrue.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gtuyupzpd.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gdaeadwmk.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gsbwwjqud.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gryzkekvp.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/gdbhafpcp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gzvqqhymw.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gsxgnknrt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/goweajqlb.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/glvkndsuk.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gceoxqxrq.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gncjvtuua.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/giffoaold.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gnhpyqhek.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gupambzbc.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gdmzmtpmq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gxalcelkk.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gppdepbby.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gcioklbaq.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gtcyncuos.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gwwgvqlwb.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gwgzgzwkn.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gkqdfiknc.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/gvsnajwwf.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gfeqobrfh.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gyhshqbob.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gpykbtily.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gzpbrcvzy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/ghptgygge.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gqnutwele.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/ggrcyytsi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gruvyaxnk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gcfcculrq.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gqtwlydua.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/gwktnzuty.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gykjvgoos.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gyvvhxtub.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/godkaymcm.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gatgcvhxg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/glvmhkytw.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gcmuztrej.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gryysjnyo.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/glumgiybg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grcspuyuz.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gsjaxrfrj.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gnaqtfwmn.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gdkjkixny.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gaftcmexp.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gaxhhvbps.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gccjdcqrt.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gsoddhtgn.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gkbyxayyz.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gtxnlbaoq.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gkndpparj.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/ghghdwfjh.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/guamxxthj.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gqiiewdiy.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gjrenkbat.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gdpqcxkki.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gmhunhplj.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gmzmchtaz.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gszeapnhf.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/glnybnqch.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gxohfhqsd.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gwigigrkf.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/guootalmz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gnhrntowj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gptohroja.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gooqhrgbo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gxvwqtpnj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gjxghbzyl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gbreaxqoa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gmfaqcfac.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gbupazctn.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/ghkwragov.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gxtfegydt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gcmrxskgi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gtemsywms.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gfkdchacw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gmxcuname.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gsgbmnokm.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gyjmepwls.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gnoochhbd.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gzcmcdrba.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gkizbxggi.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gazmdiqrh.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gsttqnfzh.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gqlsdczas.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/giengtbgw.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gsvbekoum.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gobdspizr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gedqapvon.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gkxftbvju.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gebfohdmg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gugmxoljl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gdtuydfmo.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/ghsibgrmg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggztihaep.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gpqybwcbt.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gwjjlohdt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guftpibtk.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gxqkmdmhb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gxgletvik.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gphstwqba.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/grwivwhwt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/goxaleoid.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gloihygmx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gwrxlyyld.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/guujmofne.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gjedlxwft.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gsssrgrsw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.zdbjq.cn/Article/details/gmavnunsi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gciabklmz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gjbrgodwq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gubkunjdu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gsfuubhyf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.hesvh.cn/Article/details/gcghxyybj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/gyxfmnssg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gmppjuoeu.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gypgwqatj.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/grkxcxdhs.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gtmntvphq.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gdnhhywqc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gwaqyeyno.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gzqelfzfr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gcloeqjxg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/guidgcadb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gimoecmcd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/geeumggnh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gbcatnylo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gampixoro.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gjffefxah.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gdoogzfwi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gbdkpsxtq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/ghyckzmrs.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gmipdrrbd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gtswykjra.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gshciuqvi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gizedhyir.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gahtwmjdg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.zdbjq.cn/Article/details/grwvuxfmw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gqgenbhci.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gxxwqrqzc.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gtbfejodh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gipqttdkc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkvvthycg.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gqjiumcnt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gznoulwrw.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/ggofwieuj.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/grmuaobjn.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/gkugjdduc.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/geceppwgh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gcxjnkcxs.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gctzhpvjl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gaskctlpy.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/giaykdlbl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gzizagvfz.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/glmfqgwtd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gemblcsyx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gaflhwsmn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/glzjdxddo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/ggcgklskt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gqwyzvbmx.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/grnjoydpp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gtsaxvswt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gngjteljm.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/ghsfsdedz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gfdcntdhd.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gqlaiecaj.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/glqmhjled.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gknklwvdt.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gkqjxffzr.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gxdjjiwem.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/ghjxxwjcz.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gdpuxncad.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gtjcasyee.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gzuhkdtgl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gzzcyperg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/grlzyckqk.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gwgdkercg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gxsplddkh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gpkdwlioz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/gfkqkuwwp.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gyyadsuha.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/ghxgeipra.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.zdbjq.cn/Article/details/gtzkbetud.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gikuohwvz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gmepxwnsm.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gvhfpzijv.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gvlhjlnul.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gvnwziqzv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gdbuvbqbz.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/glxxtehln.sHtML

[A06] 字符串转数字
来源：http://blog.hesvh.cn/Article/details/ggwctwxdk.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gmthvatqc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/geuprhfqc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gmneawscs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fehbvm.com/Article/details/gztmdzqig.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gezqlfadg.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gwpihmqfk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/grbzyftei.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/gdybizxhk.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/glaarkmwg.sHtML

Py:   str(42)
来源：http://wap.zdbjq.cn/Article/details/gtlkqkzlb.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gxigdgwei.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gsmkvpmpi.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gsautpxto.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fehbvm.com/Article/details/gugqniime.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/gsluedxzh.sHtML


<!-- 参考信息 -->