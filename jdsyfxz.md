代发 wailian999

[U51] PHP：数组解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbxagnuw.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwrjrzpf.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxosrxcbd.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbqewidq.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxwopwqw.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.fanxiaobao.xyz/Article/details/glyhglrmv.sHtML

[U54] PHP：空安全调用
来源：http://3g.fanxiaobao.xyz/Article/details/gxakpttxc.sHtML

$obj?->method()
来源：http://m.share.fanxiaobao.xyz/Article/details/grycifoby.sHtML

[U55] PHP：match 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gtozgoztf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.fanxiaobao.xyz/Article/details/gtubfmjrh.sHtML

[U56] PHP：命名参数
来源：http://mobile.fanxiaobao.xyz/Article/details/guiolbgdr.sHtML

f(a: 1, b: 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gyaxraghh.sHtML

[U57] PHP：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcydlfih.sHtML

"值: {$a}"
来源：http://blog.fanxiaobao.xyz/Article/details/goayipvfc.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvmktjyi.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gwenfzyvj.sHtML

[U59] PHP：自定义排序
来源：http://3g.fanxiaobao.xyz/Article/details/grtouehhc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gloyypehs.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fanxiaobao.xyz/Article/details/gwwxrrqxb.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gegeoaeak.sHtML

[U61] PHP：正则
来源：http://baike.fanxiaobao.xyz/Article/details/gtwptgiql.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gehdznqan.sHtML

[U62] PHP：日期对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gglcuktkg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://3g.fanxiaobao.xyz/Article/details/geshvlsjn.sHtML

[U63] PHP：文件读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gstmvrgqu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.fanxiaobao.xyz/Article/details/gajnwydrp.sHtML

[U64] PHP：目录遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyznabgc.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://blog.fanxiaobao.xyz/Article/details/gffgxmcia.sHtML

[U65] PHP：会话
来源：http://read.share.fanxiaobao.xyz/Article/details/gqktzkjau.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gwtytqeie.sHtML

[U66] PHP：设置 Cookie
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlzwlnkd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurlaxlua.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fanxiaobao.xyz/Article/details/gbdiduuog.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkoiooik.sHtML

[U68] PHP：PDO 连接
来源：http://3g.fanxiaobao.xyz/Article/details/gzdhwzsqg.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxizugkvr.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fanxiaobao.xyz/Article/details/gekyenzqn.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gptorcapm.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fanxiaobao.xyz/Article/details/grbwzzkbv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fanxiaobao.xyz/Article/details/gxpvxbjmm.sHtML

[U71] PHP：抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzsgboyy.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/geiteqywz.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/grsymvzkx.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gituklked.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtprvenk.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyipinwam.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/guvyeotsj.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtendnqel.sHtML

[U75] PHP：依赖注入
来源：http://blog.fanxiaobao.xyz/Article/details/gfbapiaes.sHtML

composer require psr/container
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlmsiarg.sHtML

[U76] PHP：简单路由
来源：http://m.share.fanxiaobao.xyz/Article/details/gylwazgot.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gbrnoauch.sHtML

[U77] PHP：模板渲染
来源：http://mobile.fanxiaobao.xyz/Article/details/grekxzctj.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvgzdcqx.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbvpolmr.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmgnytnc.sHtML

[U79] PHP：静态分析
来源：http://3g.fanxiaobao.xyz/Article/details/gkcftqoqs.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/gimlvetbb.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fanxiaobao.xyz/Article/details/goeishdof.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gicnbeely.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/gsweqhnzd.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgoovods.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/geqomoncy.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaahxxur.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfpfrpcf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fanxiaobao.xyz/Article/details/gnzkynevx.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/giukfwvrf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fanxiaobao.xyz/Article/details/guxakbpjn.sHtML

[U85] JS：可选链
来源：http://www.share.fanxiaobao.xyz/Article/details/guguoqsfo.sHtML

a?.b?.c
来源：http://www.share.fanxiaobao.xyz/Article/details/grghyrzfl.sHtML

[U86] JS：空值合并
来源：http://www.blog.fanxiaobao.xyz/Article/details/gantssryr.sHtML

a ?? b
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyrnsldq.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gudwzxbkn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fanxiaobao.xyz/Article/details/gckqiuivx.sHtML

[U88] JS：对象展开合并
来源：http://baike.fanxiaobao.xyz/Article/details/gppasggzu.sHtML

{ ...a, ...b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gufcpzmxi.sHtML

[U89] JS：数组去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbgcwapl.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gymqulqhe.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gcaoxdesj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpyccnzf.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzepzxba.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/gjwwbvjqf.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gcqatneza.sHtML

structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfuhqalo.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/givlolubh.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypgcuitn.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gprkbewvk.sHtML

const double = x => x * 2;
来源：http://3g.fanxiaobao.xyz/Article/details/gjufzxndw.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgscfdhh.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwwdlpsw.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/guxmrcpxl.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzrwgsnf.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gfbxlwhgt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gmbqlupnv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiufpbgg.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnhszhjr.sHtML

[U99] JS：事件监听
来源：http://3g.fanxiaobao.xyz/Article/details/gouvruhvt.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fanxiaobao.xyz/Article/details/gmvnfyayy.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gdhpnbhti.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/grlpwcvdd.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrtxqwej.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdouvfepq.sHtML

[U102] JS：本地存储
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwoktqqx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fanxiaobao.xyz/Article/details/gtrzorfxm.sHtML

[U103] JS：定时器
来源：http://wap.fanxiaobao.xyz/Article/details/gokaoquga.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gktybsrdn.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/grvviqsea.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gaibvekke.sHtML

[U105] JS：节流
来源：http://3g.fanxiaobao.xyz/Article/details/glfozaxzq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/geomgixuu.sHtML

[U106] JS：日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gissfxjno.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/ggtanlcgf.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/geotjoihk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fanxiaobao.xyz/Article/details/gycrtmlnz.sHtML

[U108] JS：随机整数
来源：http://3g.fanxiaobao.xyz/Article/details/gooogazpx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gojijyzfu.sHtML

[U109] JS：数组分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gigbuqooq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdqcvdzc.sHtML

[U110] JS：数组分块
来源：http://read.share.fanxiaobao.xyz/Article/details/gpylqmusg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fanxiaobao.xyz/Article/details/genxoekfs.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhmmuzcc.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvzstizi.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gjapzreid.sHtML

"7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjecnozoo.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrhqtvvj.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmfhtnmx.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gszejwtis.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdfjhmus.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gnqkkchby.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gqezlgtiv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkrzaahg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgvsycia.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/goyzhmypx.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvvynqjk.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gbzhnsfjk.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkicetljh.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gayyabuhh.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmwqarhb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpscfxxsg.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkubjnjd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeranxrt.sHtML

统计汇总
来源：http://3g.fanxiaobao.xyz/Article/details/gihynkqqa.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhzithpi.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxlktguy.sHtML

Python ......... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gtfwftocn.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/giqxsezmu.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gfdrqpvmn.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gpxxfutjg.sHtML

Java ........... 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhxzcjdi.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gwlifinkz.sHtML

Ruby ........... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gssifinit.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garnfngcx.sHtML

C .............. 30
来源：http://wap.fanxiaobao.xyz/Article/details/gmepbdrcp.sHtML

C++ ............ 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdczvcji.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvzglbtq.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwodvxbqg.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/graudyjsd.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvqruhzw.sHtML

Lua ............ 10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqwvgwpa.sHtML

Perl ........... 10
来源：http://baike.fanxiaobao.xyz/Article/details/gvgqbmooc.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gfmvcvwfk.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gddbovevw.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gtdkvvunk.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gjhpojtvg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gdgfodyig.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaitihjh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicqaarhs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gmfquswgx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbvhxrgh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpaqjqst.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmogrquh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gsotckaqn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwdwfrri.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gbmhzslpr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/geeenrthz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdofikug.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvynxafe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlttnmlu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fanxiaobao.xyz/Article/details/gvbhxyjjn.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gzksxlplo.sHtML

Q SQL 专题                              90
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlfsavqe.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbwfdpxc.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gqdyjfiqq.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gbkfsamva.sHtML

U 高频实用片段                         120
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzwvjymb.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gwadtjgvg.sHtML

合计                                  2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gfyjhwgyi.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlpclooz.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbtvprzw.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gglbsrhgr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/glabztmlz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fanxiaobao.xyz/Article/details/gporqhcma.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fanxiaobao.xyz/Article/details/gsabncnef.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyopcytxv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakpcykzu.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gwugalgtj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdiqfnks.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnccedbo.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrehyllw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gpxtfkanz.sHtML

【收录内容】
来源：http://wap.fanxiaobao.xyz/Article/details/gglbaewiv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/goqqpxqak.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbbacrrv.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoishjwx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gecsrodsk.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcleefvp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fanxiaobao.xyz/Article/details/gouekctpa.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtwcmxds.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fanxiaobao.xyz/Article/details/guhoqofmn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/girlnlvek.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gszihvouh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/grvhhzkba.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezpgtkgd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fanxiaobao.xyz/Article/details/gvbrwtxwu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeazbfql.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fanxiaobao.xyz/Article/details/gusrmqciu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fanxiaobao.xyz/Article/details/gnvnovqbp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fanxiaobao.xyz/Article/details/gflqpgpvw.sHtML

【文件统计】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgaogpjl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fanxiaobao.xyz/Article/details/gngjapclf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthrzexmc.sHtML

目  录
来源：http://wap.fanxiaobao.xyz/Article/details/glrdqonng.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbnsmkcf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzuqkrbp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqmxwiht.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gflocccsj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gnvipgwzh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjgdfdjj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gykmaoxhm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/givfkyfqt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjgmaeya.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gvsaspjke.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gourwbvhx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gawqpepzp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gbqzxjnoi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gyurovlrd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxlyrrsk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/guwlqraby.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzvjnyvg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fanxiaobao.xyz/Article/details/goyjqqfwg.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grelvsiie.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlopyetl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fanxiaobao.xyz/Article/details/gszocdlik.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijkfubjq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyvesqqq.sHtML

A. 基础语法与类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gegyhwrpw.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgbksavw.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrxwvizl.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvbnfgen.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fanxiaobao.xyz/Article/details/gdeissnrc.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtgsblnl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrnfumap.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gigybrvjo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpuonwgyd.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fanxiaobao.xyz/Article/details/gpifqkexa.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/giymxsnyx.sHtML

[A02] 变量声明与赋值
来源：http://blog.fanxiaobao.xyz/Article/details/giqpsqbfg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gwudknbyo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gobaccwkx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gticdefuf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/geuoxuprh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrgvhufa.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gssqklrux.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fanxiaobao.xyz/Article/details/gzbfbvbyk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmfetcvx.sHtML

[A03] 常量定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefkrgfyc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fanxiaobao.xyz/Article/details/govkzixhb.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giamdsfqm.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/grukxoxzx.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gwmlhenkz.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzmlvowm.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyehamwf.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwlsbzkv.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/ghjlyqyds.sHtML

[A04] 判断变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gyevrnrsk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhdexmqh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggebzbpzp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gsztnakjr.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbkxdlfa.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnktsxaf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fanxiaobao.xyz/Article/details/ghsrtxhtd.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fanxiaobao.xyz/Article/details/gdtvcyufk.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.fanxiaobao.xyz/Article/details/gcdgctwtk.sHtML

[A05] 整数除法与取模
来源：http://blog.fanxiaobao.xyz/Article/details/gnlxhbnsd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebslinqp.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfvxsdcx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqtienoi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnktkmkgq.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxqgqnytz.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/glzmdhxrl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/glpdlwbcr.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gqcndjggd.sHtML

[A06] 字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gdnjskvyr.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdfmuxzg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fanxiaobao.xyz/Article/details/gwbhorkha.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwsjdjdb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/ghalfgpwn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gttaaialv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkfipndh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmxnvnjw.sHtML


<!-- 参考信息 -->