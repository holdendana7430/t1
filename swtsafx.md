代发 wailian999

[U53] PHP：空合并运算符
来源：http://mobile.fehbvm.com/Article/details/gtdzchtff.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.hesvh.cn/Article/details/gixtaciub.sHtML

[U54] PHP：空安全调用
来源：http://www.m.share.zdbjq.cn/Article/details/gkqcbxikf.sHtML

$obj?->method()
来源：http://baike.hesvh.cn/Article/details/gzufcbdmq.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gtkxluvtr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.hesvh.cn/Article/details/gjjrdiddb.sHtML

[U56] PHP：命名参数
来源：http://3g.zdbjq.cn/Article/details/gaizbantu.sHtML

f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gseilelrq.sHtML

[U57] PHP：字符串插值
来源：http://baike.hesvh.cn/Article/details/gequoxtjw.sHtML

"值: {$a}"
来源：http://3g.fehbvm.com/Article/details/ggcslhnah.sHtML

[U58] PHP：数组三件套
来源：http://baike.fehbvm.com/Article/details/gxelipfuo.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.hesvh.cn/Article/details/gcapehcbg.sHtML

[U59] PHP：自定义排序
来源：http://m.share.zdbjq.cn/Article/details/gzgjmgfam.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gkyzhbwqq.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fehbvm.com/Article/details/gkfrdqrck.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gntmtpwtq.sHtML

[U61] PHP：正则
来源：http://www.blog.fehbvm.com/Article/details/gftiprmgc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gcttliilw.sHtML

[U62] PHP：日期对象
来源：http://www.blog.fehbvm.com/Article/details/gtkccfyya.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://wap.fehbvm.com/Article/details/gmktirnta.sHtML

[U63] PHP：文件读写
来源：http://3g.hesvh.cn/Article/details/gvgklxcpn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.zdbjq.cn/Article/details/gjzdypafa.sHtML

[U64] PHP：目录遍历
来源：http://blog.hesvh.cn/Article/details/gmfgeuapb.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.hesvh.cn/Article/details/gpjbonfjg.sHtML

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/glpzkjuuv.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gxyjlwmyf.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.fehbvm.com/Article/details/gwzouskul.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gbltllpye.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.hesvh.cn/Article/details/gmjlmdkis.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://wap.zdbjq.cn/Article/details/gktrmbdoq.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gxqbblccb.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.zdbjq.cn/Article/details/gewotxtmf.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.zdbjq.cn/Article/details/gpkqhyjrq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gkcwldzht.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.zdbjq.cn/Article/details/goilxpekj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.m.share.fehbvm.com/Article/details/gehxplrmn.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gjqpgtngo.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gicyflget.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/geqwekmwp.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gvjdtxspx.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.fehbvm.com/Article/details/groyxwibe.sHtML

parse_ini_file("config.ini", true)
来源：http://3g.zdbjq.cn/Article/details/gswqdpkvx.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/grqiaoxjv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/ggyuyxrto.sHtML

[U75] PHP：依赖注入
来源：http://blog.zdbjq.cn/Article/details/gbvyksbgk.sHtML

composer require psr/container
来源：http://read.share.hesvh.cn/Article/details/gdoahmnxo.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gbjmgpwup.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gckydrcmo.sHtML

[U77] PHP：模板渲染
来源：http://baike.hesvh.cn/Article/details/grmbwztti.sHtML

composer require twig/twig
来源：http://m.share.zdbjq.cn/Article/details/gdofujlyl.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gnhsqnbgt.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.zdbjq.cn/Article/details/genvglrpo.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gpvopivdo.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gtzfbmyhj.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gwqcobchx.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/guyfitfjw.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gwvgyqnye.sHtML

npm init -y;  npm i express
来源：http://blog.hesvh.cn/Article/details/gshiktnfs.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/ghlwhyple.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.fehbvm.com/Article/details/goxiwplmj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/goojexeae.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gqrvtwpzj.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.zdbjq.cn/Article/details/gbisqbvdl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/glynirzla.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gksuonynu.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/grxtwydwc.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gllagebez.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gwscvqnew.sHtML

[U87] JS：解构默认值
来源：http://blog.zdbjq.cn/Article/details/gfpwfddzn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/geyuskojx.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/ghqatwfsu.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gbhuwymzd.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gbagsstaj.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/ghuzbvxke.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gewjhwfyh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gslenhxyb.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gigjaoegk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/ggfxzxktl.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gqwtvlphl.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ggktuahuk.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gqsydxehx.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gstxobfwa.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gaaxiknhm.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gfehqnkub.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gkfltrqty.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/glzbdttlw.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gyxvjmzjr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gckunudqu.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gfknidxbt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gtqiasgtg.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/glrrqfvfa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/gyihzgoco.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/ghhofujya.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gjrvxuhgh.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gavavyfoh.sHtML

document.querySelector(".item")
来源：http://blog.hesvh.cn/Article/details/gsytjocga.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gsxqgnlwt.sHtML

el.classList.toggle("active")
来源：http://wap.zdbjq.cn/Article/details/gkwhwcaxs.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gujmewbkp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gkbuksohs.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/glegdudce.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gfsbfpgho.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gjjsetxho.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gjhmbfpif.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/gfuakmvjs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gwecydinu.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/ggghlirhn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gwlnifywq.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gdngdhpyj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gtttchqnn.sHtML

[U108] JS：随机整数
来源：http://wap.fehbvm.com/Article/details/gkykmvcjt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/glhmdnpsc.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gehkilxmc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gvcnevkai.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gjpnabsmu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gysdyvads.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gojydhtgg.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/glcrijvdn.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gjfrfqgwn.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/govpdctwp.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gvwcxzkju.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/glxhtnmzb.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gniagpxdt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gmymwlrqw.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/glgyvgttz.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/ggogvyohf.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gejhkiggf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/ggyreolrj.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gnezinbqz.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gkbbkkxrl.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gpjeviodz.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gkmdeumsx.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gfuwwoftx.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/guiqnzpja.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/ggpjlqwue.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gbjcamgja.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsqzdzagj.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gcqqldgcl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxhylsqqk.sHtML

按语言统计（条）：
来源：http://www.blog.hesvh.cn/Article/details/gxfanalqb.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/ghmwaevdj.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/gqemvdqqo.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/glybdlrme.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gjpwzmhxr.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gndlexagw.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gvaftdxdx.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gpqhezrak.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gzuhiecti.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gpisrwjgs.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gcjtqywix.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gmatjesdl.sHtML

Bash ........... 80
来源：http://baike.hesvh.cn/Article/details/gyrzcgmtw.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gbkowppai.sHtML

Swift .......... 15
来源：http://3g.fehbvm.com/Article/details/gdjejokts.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/glyigpnpn.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gqexkspua.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/grrxnrhvr.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/ggkyqllri.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gfgrysvob.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gmtkndptb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gdwxbvdoi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gozmkwwrx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/ghvyscxmk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gphwmwdsb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.hesvh.cn/Article/details/gsynihweq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gkfuphsll.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gwtdzftzg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gwcuyukdf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/goyonizpm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gstclcxkg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gfhyzjgex.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gvatfidjw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gxyxqhlre.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gdhvhlbpp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gtidklwbm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gweiiftvy.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gzarbdjoc.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gyrnvdouk.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/gdzqggnup.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gcrvumdag.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gdqfbdfii.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/glsuqffcv.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gpgadwdbz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/glvcvvdgb.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gryesrngz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gonvpigcm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/glosxsdlx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gdbcxpomz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gnbkmbirg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gjekdyjxn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gkkbnixpj.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gshnpcgiv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxwrlxlal.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gywffkifr.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gqxflchqb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdtvbhdyg.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gdvgmytnw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gqfrevcxv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gsccgbxfm.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gcecdlgfh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gvtwaknoc.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gzrftmdiv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gjthuenea.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gdvaknlmq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/giepddiuv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/ghnauxomv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gderrhsrn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.hesvh.cn/Article/details/gkgzspxmy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gqiualxcq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gtjmdcwml.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gfwjifmlx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/grwaleauo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gemuzdrbh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/goqucywfs.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gfcujlxka.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/ghxlehobg.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gdeanepmy.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gkbtikpwr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gxgljsmqb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gqcvxkgmd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gbgzcppxw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gvrtvajgq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gdzxsxqcv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gmdwnchjq.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gwkudjjfz.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gvrjxmopu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gvwqqdjfm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gtkmiplxq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/ghvhvegji.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gxxbjqhsh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gzbjqnrxf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gxcgoofim.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gxurmydby.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gyurcfaji.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gaqtzegvm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvdcpdwjz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gpyrdbrmq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/glrdrfffv.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gtyxkjkkn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gdtgexuak.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gipipdzaq.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/ggyxlnzhs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtaldftsw.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/grknmlxln.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gmcpnxomk.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/goivttfqp.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/ghcyisufi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/grkolmckr.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gwwfwmuiv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gucrppynx.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/golevnavd.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gedynzric.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gizhjjqcj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gbhidugoh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/guehbuyhn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gddkmvukt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gtcczpcnk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/geuxqoubq.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/gebywoody.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/grtejrwat.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gsgmqxhhh.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/gdtamjedp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gptvbbebs.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gibbijtfq.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gitcfildp.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gkixvvshw.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gymnrixab.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gcubrkunm.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gxbqvyztr.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ghcgixqgo.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/garvukoic.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gxjjnjsiw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gihddnpfb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/ggstwyzvt.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/grnpfqjym.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gbzwiehhn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/guexfamlj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fehbvm.com/Article/details/gbduylujb.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/glnyyesag.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gdoqqqcgx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gazhiizno.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/glabikxjx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gvfbkriyr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gqdizqqil.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/glkccplgp.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gtunqqpbu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gwkuorzsy.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gvdhehmqs.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gfwhkixqt.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/ghxmqhvef.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/glgosmwpi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/ggiyugjhg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gauxhsvdj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/glikitdkv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/gfbhggdqv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.hesvh.cn/Article/details/gsiqscyql.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/gwoifqqys.sHtML

[A07] 数字转字符串
来源：http://www.blog.fehbvm.com/Article/details/govriiacx.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/guutpjndc.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gzscpmroz.sHtML


<!-- 参考信息 -->