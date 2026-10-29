代发 wailian999

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gbbtikksl.sHtML

"值: {$a}"
来源：http://baike.hesvh.cn/Article/details/gsyyyjhga.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gqyflbruc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://read.share.hesvh.cn/Article/details/gulvkzllh.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.hesvh.cn/Article/details/gndqdzlrm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gcaifxjfc.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.zdbjq.cn/Article/details/gnsymloqr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.zdbjq.cn/Article/details/gcuuupghg.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/ghqfylbhy.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gunmillnx.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gknmemdyo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gohwwebbk.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gdcjcgliy.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gehkpcznj.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.hesvh.cn/Article/details/geffztwcf.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.zdbjq.cn/Article/details/gcwijkzcg.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/gvxlinusw.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gsutgrtif.sHtML

[U66] PHP：设置 Cookie
来源：http://blog.hesvh.cn/Article/details/gotpgeiff.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.fehbvm.com/Article/details/gwisotobn.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.hesvh.cn/Article/details/gtgksqdny.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.hesvh.cn/Article/details/gnauewfpn.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/guwuozhri.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gaefgnfcl.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gnjzcxabj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.fehbvm.com/Article/details/gqytxnukx.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.fehbvm.com/Article/details/gimjsqtjp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/grgmihxpk.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gxysmumww.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/guhrqwjdr.sHtML

[U72] PHP：写错误日志
来源：http://www.share.hesvh.cn/Article/details/glydylonl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/glucsijjt.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/ghmczcaxp.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdxrqeen.sHtML

[U74] PHP：读取环境变量
来源：http://wap.hesvh.cn/Article/details/gidrxqyqy.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.fehbvm.com/Article/details/gtiwcphpj.sHtML

[U75] PHP：依赖注入
来源：http://baike.zdbjq.cn/Article/details/gurmsekwz.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/gdawmstih.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gkvnefhba.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gfmcinncl.sHtML

[U77] PHP：模板渲染
来源：http://www.share.hesvh.cn/Article/details/guzwduhuw.sHtML

composer require twig/twig
来源：http://www.blog.fehbvm.com/Article/details/gmvyttdkg.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gjgrjwgik.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/glmttbhfd.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gujzdjsqc.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.hesvh.cn/Article/details/govexzqsp.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gyvdjrvvp.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gjnlgsnjm.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gzdhyvnow.sHtML

npm init -y;  npm i express
来源：http://3g.fehbvm.com/Article/details/gflvnzmim.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gpojldxqg.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gkkxrvmnp.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.hesvh.cn/Article/details/gmaegctmf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gnzpmpiqr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.zdbjq.cn/Article/details/gqaiogzok.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gswbevtzx.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gcnesoyta.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gjldqfvzo.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/garrhxqmv.sHtML

a ?? b
来源：http://www.m.share.hesvh.cn/Article/details/gewmmnobv.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gjhxhhwtp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.hesvh.cn/Article/details/gaqhtmwdn.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gayxdytmz.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gdrdatgvf.sHtML

[U89] JS：数组去重
来源：http://mobile.fehbvm.com/Article/details/gvlnqinyd.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gturlydlb.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gzlhofgpn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gcznfcojn.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gurpowbtn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/gryynbnjx.sHtML

[U92] JS：深拷贝
来源：http://wap.fehbvm.com/Article/details/gmigdhtpx.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gofgjcysl.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gmqtukgpr.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gkatfzndt.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gunzbzaxg.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gaqcwqevu.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gegyzqejd.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gmljbhncp.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/grnnvfcff.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gjgoaomqt.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gkcntqnxy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gexjmxdns.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/gapkvpdvm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.fehbvm.com/Article/details/ghhatasbq.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gzybhilnx.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gzbmiwrpv.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/givyfavuz.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/guxcluvys.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gjpygqwcw.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/gzjyzbyte.sHtML

[U102] JS：本地存储
来源：http://baike.zdbjq.cn/Article/details/gyzbmrcmw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gkrcahawl.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gmmtmmdmz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gxrydzaab.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gzywiilds.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gidpintbm.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gkrlbjedi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gyyqbyjlw.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gyzmjmkjr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gazfslodf.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gssixhwow.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gmontzseh.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/giaikiirw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gmqakbibh.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/ghxqsqeuk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/ghhauhemv.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gyrtsgqhm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gicqigoba.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gpzoftoon.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/ggqfshatv.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gljlxguvo.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gfeymxmqm.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gkxmzdjdc.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/grwjpdopy.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/grgtrumos.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/goryghjxe.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gfeqkgyxn.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gkaxaszrv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/ggbbsvpku.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/ggrmnhxvl.sHtML

[U117] JS：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/gfpbyihds.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gxdrgfhdi.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gkjmyjvip.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gxmbvtlqo.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/ggadpllnf.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gwgwraiap.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/gtplmlalj.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gzdbgacfw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gttrerzvq.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gwbxxtwff.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvywhycrf.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/ghjcnautj.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gupicyyhs.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gevdifuek.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gddodlrrb.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/geqssisjk.sHtML

Java ........... 212
来源：http://wap.fehbvm.com/Article/details/gxkgnkiue.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gpuwflosq.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gtxsfzxrj.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gdhpyjslv.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gtnkvlfdj.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gxnfsimrz.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gnswzvvei.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gbtitilbm.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/grrgmfnlq.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gscvpskjz.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/goqeufwqr.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/ggndaxbep.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gnogwqbbh.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gksfwkqvd.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gojxusxrq.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gptgkgfhy.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gfwswsdnl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gfiqgootz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/ghyhovrec.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/genuhfhfo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gqxiylqtg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/guzhzbxjc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gifydczus.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gboddltzw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gdvrwyxai.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gldejxlvv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gjkkevdvq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/ghxnkesep.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gtxrampkv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gekeznakm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gkoppahmx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gwwaxkqmf.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/ggmoesdhx.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gxnevoasf.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gzsrbysco.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gyuxpihwf.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/gsrkordha.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gizursyba.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/gdwlntniq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gyxwtnkpe.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gkkzxowtq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gnhrgpbuw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fehbvm.com/Article/details/gixsuryaj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gjvpvbxje.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gxdxppoih.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gttnygeqx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fehbvm.com/Article/details/grhczzwzg.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gjygqmrhz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqgzaxkwa.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/giqwupyoc.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gpeabqcll.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcmwzyixs.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/guewdaiig.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/geqgrfdsb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gnfnnhfra.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gmbodmwzo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gmnowbade.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gsoktdmsz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/gevazatwh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/ghmmkfnlv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gauuxoewm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gbksejxrs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.zdbjq.cn/Article/details/giprjlhxo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gbenrpqmv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gdtwkiokt.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gbyizdpjz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gpjhykuce.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gaaqsbkir.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gcjsabbta.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gxmmcgapf.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gbxlkrgmz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gjhtshtld.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gjztzepfx.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gmsdrtllx.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gezbslulz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/grimdomfe.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gujkmlrct.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gbcnosurw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gqbfhexnk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/glyjrklmu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gxjmhkwpm.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gjwyknzvi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gjdhndkoq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/ggbcyhjwc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/ghbrpabbb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gnrcnjgok.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gndpoxprg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gczzclsqw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gfoldyohx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gbxjrmzrs.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gfdtfjwyu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gxgxncupr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gsikewsrs.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/gbauqjdph.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gxsybwpod.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/ghdwzhbkx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcayswoar.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gftiaybtj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guseucwpw.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gqrgwckxq.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gkaeoctwb.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gcdtwkock.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gkgmdqvdx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gvuujffkl.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gxukfugrc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gyuowucqn.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gmavyttwf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gxjvpvikq.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gmwuslsri.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gptlfxbbq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gxvcovllx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gfylcqhrb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gwxqdybkx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gthestvzq.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gaejlkmvi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gcgoxlhdc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gyklikfht.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/gjqbdvwjk.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gwgqoxqdl.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gjosjctmj.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gnoqdktzi.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gnosyinyc.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/grloripyz.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gjzywluai.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gciokkeel.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/glztebfyu.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gdkzunfmf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gnxotprwu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/gbjoaougb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gntlwglqs.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gqvgbgxxs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gmxyzzodb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/gkwtyrgdn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/gttlmbpfs.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gdhuucsqr.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gmidlksez.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/gaqyljcfa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gdsahbvma.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gonhyevmq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/grpvnmorw.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gfrfapowx.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gjzwfwpdt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gfuvnmvqf.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gfchgeejo.sHtML

[A06] 字符串转数字
来源：http://www.share.fehbvm.com/Article/details/ggzgbuitm.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/geovvcsfz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/gikgscidj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/ghkiegyvz.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/garxvjcpd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gmurclipf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gvhlhzxpq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/gycgofgmz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.hesvh.cn/Article/details/gxnegoyxo.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/grrosnhhd.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gxoejktxo.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gzzmldlfy.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fehbvm.com/Article/details/gfffyzdls.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/gzsxpkych.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.zdbjq.cn/Article/details/gpzwxycao.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.hesvh.cn/Article/details/gstdwcegj.sHtML

Ruby: 42.to_s
来源：http://www.m.share.hesvh.cn/Article/details/gvphmzyyp.sHtML

C#:   42.ToString()
来源：http://www.share.zdbjq.cn/Article/details/gfqtbqjtb.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/ggfzjsfge.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gtvvcvfkj.sHtML


<!-- 参考信息 -->