代发 wailian999

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gwdxxkopo.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.hesvh.cn/Article/details/gbduybuwq.sHtML

[U56] PHP：命名参数
来源：http://m.share.hesvh.cn/Article/details/gkpyumpyc.sHtML

f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gkikayrvm.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gtwhngixx.sHtML

"值: {$a}"
来源：http://m.share.fehbvm.com/Article/details/gtmrhfeyz.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/glezoywub.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gyrkvndws.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gamamtvut.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gbmbhxsbj.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.zdbjq.cn/Article/details/ggaueaeci.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.fehbvm.com/Article/details/gnspbyghp.sHtML

[U61] PHP：正则
来源：http://read.share.fehbvm.com/Article/details/gttfrdizq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/glmpdzvhh.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gxnhbydlj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.m.share.hesvh.cn/Article/details/gutxtysyr.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gpgjfffkt.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/glnwanqwc.sHtML

[U64] PHP：目录遍历
来源：http://wap.hesvh.cn/Article/details/gqfdfskxh.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://mobile.hesvh.cn/Article/details/gnqawfhgf.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/gjmmmhxhg.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gguqrbeeq.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gzpyixcgd.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.fehbvm.com/Article/details/gbxperjzy.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gqthbkyyl.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gyzhnpogk.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gyucwvlgn.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://mobile.fehbvm.com/Article/details/gljtsumve.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gvwbygupr.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.fehbvm.com/Article/details/gacmbjqca.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.fehbvm.com/Article/details/guwreihnj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.fehbvm.com/Article/details/gdpixgeey.sHtML

[U71] PHP：抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gvyseqipw.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fehbvm.com/Article/details/gulquvyhm.sHtML

[U72] PHP：写错误日志
来源：http://blog.hesvh.cn/Article/details/guktfohwv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/ggzhslxax.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/giyfhpzar.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gwylwpatt.sHtML

[U74] PHP：读取环境变量
来源：http://blog.fehbvm.com/Article/details/gbuuesdcw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gqshdibdy.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gwhxnfrtg.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/ghrnygtqq.sHtML

[U76] PHP：简单路由
来源：http://read.share.fehbvm.com/Article/details/gkskctaax.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gwatqgxyu.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gquopcafy.sHtML

composer require twig/twig
来源：http://mobile.zdbjq.cn/Article/details/gtqefmyzr.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gssdwwekw.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gosywvfsc.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gdwajwzkr.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gzibpsheb.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gcqwtpfvw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gvuukvize.sHtML

[U81] JS：初始化项目
来源：http://www.blog.zdbjq.cn/Article/details/gqodehrlm.sHtML

npm init -y;  npm i express
来源：http://read.share.hesvh.cn/Article/details/gmjxjdpjw.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gedrsuyes.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/gwfjponpl.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gsmiwfrbf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.hesvh.cn/Article/details/grqvabybw.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/ghcxysqtw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.fehbvm.com/Article/details/gmdwpfwmg.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gsjevalvl.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gjgnpjtle.sHtML

[U86] JS：空值合并
来源：http://www.share.fehbvm.com/Article/details/ghkvtpnpe.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gynxfvucy.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gfzvjvpjq.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gceypvacw.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gpzbgghlc.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gekmpmhcz.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/gdkwciawb.sHtML

[...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gsdcqwrpf.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gpdwvhwdk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gpyffxrpx.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/goppbhpca.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gtfofhlwp.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gzzqhrimz.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gkwuzwdtc.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gcnogjkkm.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gyxsknmvy.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/galdzthkd.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gxrcsfbwd.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gedjfesfq.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gsnkhqdyh.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gcleaxpli.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/grvhrlgzh.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/geryejmgf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gjyrtecmr.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gadxaxrlq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gucenbhtx.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/grrsmqtve.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gddfaqpcs.sHtML

[U100] JS：DOM 查询
来源：http://mobile.fehbvm.com/Article/details/glcbjmwdu.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gmgblfevq.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gwkvxlgau.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gnboeynmx.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/grvwqalqc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gexttafdl.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/glpnwkpqa.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gotdhgsjn.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gumqqrcoj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gqqhcsnzh.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/goneaaupn.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gbhcrcfxw.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/goqlyvgrw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/govvhdtun.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gfoabqzfy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gxrnkhgow.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gjgiiojpl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/gpnchaaca.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gflbbgbsr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gbwxltpkw.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gfqibolus.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gcxvkcnji.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gerorjrzj.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gkfbsxazt.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/ggdkouuxe.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gnfbthonx.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gddodrzfb.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gnljwrwhx.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fehbvm.com/Article/details/gtcuqgjyl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gqqtuzecs.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gepdebgin.sHtML

crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gwkaisilq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gbdhdirvm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gcqfynxzn.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/goazvbzdo.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/gvjwrcdqp.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/ghiyodgfl.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gyrjzooqk.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gcbdopzrj.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/goftdkpau.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gzqujvzci.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gusqtiwbr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gotygriov.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gigdbvkro.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gloqmqppj.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/grcgidzci.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gzswwyzhv.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gxzoilbts.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gejxhyxqa.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/giommovum.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/giplmgruv.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gchlfstvs.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gjrebwqox.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gsftjeihg.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gxmbnaupd.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gfxjdouoa.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gzwndwucu.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gyxvmsdrv.sHtML

Kotlin ......... 15
来源：http://read.share.zdbjq.cn/Article/details/gswjbvilz.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/glsqlokdf.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gnbsvscyp.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gbruaxofb.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gyeccapft.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gnmvlzwzr.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gvgmzlqfj.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/glvzrjiif.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gwadtjidg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gvcontskl.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gmrpphzie.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gwgmlcxuw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gcwlpbtfo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gzyurvmha.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gexgxtmew.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/guxnllifc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gqnelkdew.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gzwawuyak.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gfsunkvtt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/ggiiykcam.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gntfnjtwn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/giymcbkdl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gomvwqxfx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gguugtitn.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gqiwdvdwg.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/ggpaeioap.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gwkwqjdgm.sHtML

T 其他语言补充                          60
来源：http://mobile.hesvh.cn/Article/details/gtzmwdivv.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gezhxzavl.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gcemrakhn.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gyibbllnn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gbeudekdi.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gqzcpcbvf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/grvfkwnbl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gugjvesfl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gepydlhpc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gvdhizlco.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/ggsdohuhi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/grjbgxoox.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gdtlxjwah.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmtwwnotf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gqzxmzwfy.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/gptdelrkb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggeshofym.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gpyvnvits.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/glkrsdtwn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gyaruifrk.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/glifrqcnn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gkkliceqw.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gckasoyll.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gpkarxzox.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gwaigjuqv.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gzyarbadv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gjletakpm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gnzqcsett.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gdktzwqpi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gctnztobk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gtdggfeti.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gjpvnnzlh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gzrftbwdb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gjafkrxvq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gkxfmebhn.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gaufnrbww.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gpielovnv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/guicxqhzo.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gcicdrpbk.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gqdemgoge.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gcptdmpmt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/ggrrphggx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gccudovpy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gazsgansx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvgycxpir.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gozeeibco.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/grtbwznhx.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/ghiigpksj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gvgpscqhz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gzwonpelk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gydrvazsz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gxhtmkibo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gapkoxjub.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gyhbawybs.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gbhdgoikq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwbwaownm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gczzrdveu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/ggdeuphbu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gunjtmcwj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gbqshpxja.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gxgrqrlgu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnkuhpaix.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gldqukwlg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcmliunlv.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gawtwkslv.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gyhjwmeaf.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/gncvwqjxl.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gzmkajehk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fehbvm.com/Article/details/gyzaflhph.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/ghnwazkuc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gizjzlcpt.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/guyiyhsrv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/guysdlgwa.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gyicprfaj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gijvtsscx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gvguibqct.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/ghbcbznde.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/grgxdzfrf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gkqnfnyyv.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gxtaxxzlm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gztwvevag.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gyfxftkcc.sHtML

[A03] 常量定义
来源：http://www.m.share.zdbjq.cn/Article/details/ghbiaocww.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/guiwzdsob.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/givfksqpc.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gvifnvdtl.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gmogkuktd.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gbltcyxqp.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gezpbbdiz.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gceolibzc.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gigllcomw.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gwxihymds.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gdefrhfvp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fehbvm.com/Article/details/gzfllqxno.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gjxdwqlre.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/geayfkfuy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gtxkfemvl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gfoxnqrhf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.hesvh.cn/Article/details/gkyuuecnd.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/glubgszra.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/gewrznlbr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gyiloqjdx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gdkwazrln.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gucskjibg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gjrzrtrlh.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gojyaxdkw.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gqdwmrjwo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gbvcyypsv.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gelovjlrr.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gzbqtrenu.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/ghpajstuu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gljhdutrq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fehbvm.com/Article/details/gaeghmhje.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gwlnhbpjp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.hesvh.cn/Article/details/guqgoypyp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/genaookbu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/gdjwaypep.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gagohadwm.sHtML

[A07] 数字转字符串
来源：http://www.blog.zdbjq.cn/Article/details/grkptxedk.sHtML

Py:   str(42)
来源：http://m.share.hesvh.cn/Article/details/ghrftxzxi.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.hesvh.cn/Article/details/gqcemlslf.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gsuibkeqc.sHtML

TS:   String(42)
来源：http://read.share.hesvh.cn/Article/details/gcwojzodg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gvvpexvfp.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.hesvh.cn/Article/details/goiisvrun.sHtML


<!-- 参考信息 -->