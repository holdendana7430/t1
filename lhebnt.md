代发 wailian999

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ndjtmhuc.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3colcgthr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ekqkkjqc.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3sagmdbpy.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3ukyugyrv.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3cxlzojgq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3oewfpphg.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3vofyikok.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mgijdlkr.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wmlpfwua.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3delqzjmc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3eiygtgfw.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3vkkrllci.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3fhspgtav.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3rufyroqi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wbqoalgd.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3jhjnpsra.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3blyfoeeu.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3qsngcfmj.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xsjqonub.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3koyndeht.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3pilpnwcv.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3xvnpzmtg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3wipkpopo.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3uqcaadki.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3frarrktq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rjoaukcx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3wdtymjzx.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3txejlxln.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gahsxnhd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3zzapgucn.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3pcqpkgqg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3mswusaqi.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3tvqpflka.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3wtooycaj.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3lshfmnqa.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3tkvcygnm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3zzknkbmi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3wmgjsbpr.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3hflbezcd.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wwfclept.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3nghewang.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ozvglyip.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3dcusbqmp.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rcietyzg.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3aqyalgvl.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wfnjowht.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3nafowhlh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3rbjqdsdx.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3qhvegqsz.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xgpngdjr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ruwhkddk.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3smrihadc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3gyavxblx.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qxsveudz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3bsjqmhtl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3pfeovnna.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3qmpqtrqv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3rwtfzhsg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3dtkafhdw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3cgajprqf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3igmwbpml.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3gsgknelk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3fnfptrbc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3rfiupknn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3trsnxocd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3rapuaegj.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3uqilzbby.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3mxnafsta.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3nzejenby.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3derujuhk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3ukhcnlbw.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3vatjgwyn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jodqzqbq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3pilctwpi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3vrofmpru.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3hevruaaj.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ddvwjjqq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3bnnalbjf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dyxcuedy.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ilatjwiv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3tjxjgiiq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kqjzojxf.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3daieqssh.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jegbkvvy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3wxhzwyjs.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ufxiiscn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3oxbaverh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3tykpsaip.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3gebnkdyf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3axvkntze.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kctylcqu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3qxispxyl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qdbeevrs.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ogxwprzb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3dcxjsofh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ofiljyzi.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uexeibor.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3zqrluwhl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3tfwwpbuw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3qzehlbqo.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3oihdofua.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3nqljnbhv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3kdajfjrf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3nrsqiyxc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3mefhgdpz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ldyvqqaa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qfhcukoc.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xnwwsuxe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bgzriyot.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3awwczfkz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3hjnqmbnt.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qtuazxrg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ubzhycxg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3cqvstkvy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3sjyqsmxi.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3rheznyvy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vxewqvrs.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3tnajsvqu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3nuaekkcc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vdyiiwqo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3tkkwuhzv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3pnhiicwz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tdgmtwry.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mwtryaor.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lnjtiaob.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3icfdiktr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mkuzypys.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zgkymlix.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3agjsfigw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3hvvvrnmq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3vyuinstf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3qrpiyvzf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3mbwmwhza.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3bkauilqi.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3kdjfxruk.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3cwflidzd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3wmkihand.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ctteuwpk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3kebiayso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3niciintf.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ypaiqslm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zecveuop.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3dhvrlcpc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kfywihgy.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3oehjoynt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3gqrchgyh.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3opjjvlaz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ztiyjxpk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nhtsmtct.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3heijykbq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xmhnwsgi.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3osdtzcyn.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3fnuwwyka.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3bihziulu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3kkcnciuf.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3daqxgtei.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3werqluro.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3yyxwmtcy.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3neabhgpt.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3glgdnjpq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vbrsmcvs.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ndeaiapa.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3jrfiolcw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jqyvrvht.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xbewzirg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uxgmcvtf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ycjcsxip.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3cnoldekk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wqqrfiit.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vuodyddj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ipsfmszi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lccgggiq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pxgbxnke.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ebyfyliu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3orudzypa.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pnsrfdmp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3aynhqxxe.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3wyftmgeg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tbzyovzy.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3rbbijlrv.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ucgxqwzw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3gaydsoyh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3jevuuxjm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3wafgmqbq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3phhquabg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ibnfxvwu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ijfjhepe.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3zmeylbty.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uglwlkdb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3dfswbgfi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3smbceugn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ywqvlsxx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qhoameae.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3xqeijwmd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3obcjirdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xetwozqr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3zcimjmet.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3jayofkpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ziyboloq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3lhntgdhq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ojdazasw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3fmcahacp.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3rtmagomt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3phiabukw.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3hqmfsttu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3szbiidlu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3slhvvxvh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3tnspzhow.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3eraruusi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jbiikzzz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ecrqpsla.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3apnejcin.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3fknaesxi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3efxgubsm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3pdugtfqc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3xzxrzjot.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3kibfplii.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3dfthlfiz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3xixngwpi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3znuzbtfh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3rfyskpea.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bgqejdzc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gqlhbxrm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jwzwcapn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vlxjyhzf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3pthluhyt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3qrmrkodd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jixxfzrx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ihyefzpg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3prdpxjtx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nizbqzhg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vzzvxzjv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wveyscye.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3oqbnburg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qunjyuje.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xealrzfn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yrcnfkdv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xpuvxktx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jbtvklhq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gmawbnuf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3gighuvkj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3htuxorhd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vtlgokbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nelnwgbe.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qovoeepq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qzuheiln.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3gcuqtgcf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3nscukawd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3emonezfs.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ynrrgwoe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3nndablvw.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dccmbepr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3yxqughsx.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3wzeyluhv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zvbbpmwb.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3myodfknq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3hnwgvjol.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3srybmlqh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cfmopiur.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3msudtlez.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ovdvgteu.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3xrvyfimv.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3vnvgjdcw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ignsmcje.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3henrorrw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3qpcwyyaz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xyujyasg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cmunbycw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xhlcgqal.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fjimlqgj.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ttfkucjw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3koeueoji.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3omrxmpvt.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3vaodfnjs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3wakqejlz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3avxlcoaq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fdevzbcq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3bciqyqeb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3vcysmaob.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3fikzjpgh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3mzyjqwjh.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3xhmepyfp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3rxqdkpvb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3vtfnbjtj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vqfjcjfv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yodhiwiz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gahbtgyw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3txsiloek.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xuswdavt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zbhjthrh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cmalbupk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gmsagmwv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mcbrarrd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3djxpltya.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vtqsuzxz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3scteesyp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ohegnqpx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tncjxanq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3uoegofwn.html


<!-- 参考信息 -->