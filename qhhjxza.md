代发 wailian999

[U65] PHP：会话
来源：http://wap.zdbjq.cn/Article/details/gecyucmnl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gqpuppmcf.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gvvsoklqx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/glksreqtr.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gwxbdybsa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.zdbjq.cn/Article/details/gqmbthpay.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.zdbjq.cn/Article/details/gquyidmrl.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.hesvh.cn/Article/details/gkscrmnng.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.fehbvm.com/Article/details/glffnesbd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gfivnsaij.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gsoiattqv.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gbofkfnpw.sHtML

[U71] PHP：抛出异常
来源：http://read.share.fehbvm.com/Article/details/gjsbjkkqa.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/gzeoctxuj.sHtML

[U72] PHP：写错误日志
来源：http://www.share.fehbvm.com/Article/details/gwlnlbclz.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.zdbjq.cn/Article/details/grxkkygtq.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/ghpupibyu.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gtkdhphbb.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gqjafkxod.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gsrrahguj.sHtML

[U75] PHP：依赖注入
来源：http://wap.hesvh.cn/Article/details/gqkusqqgb.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gcsotmbyz.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gnlcbhzge.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gewjcwlid.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/ggpyrfavi.sHtML

composer require twig/twig
来源：http://read.share.zdbjq.cn/Article/details/gpsikkozd.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gagraphgv.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gmxsxtfps.sHtML

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gkrdahvhg.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gqsqaltix.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gkcxbgujy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/ghspbaswv.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gffbykwqo.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gbsmhwoyt.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.fehbvm.com/Article/details/gucwgfgev.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gogtngxiq.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gjwcgllrj.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gpodjdkgt.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gvldzbnmd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gyzkbqbrj.sHtML

[U85] JS：可选链
来源：http://wap.hesvh.cn/Article/details/ghcxxcqcg.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/geicytbmx.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gxzkjjgrh.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gntzwcuaw.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/ggojqnbqr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gkenfqxud.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gfhklilki.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gxdwxueau.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/ghrmcvfdk.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gbrbcupke.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/gzddxpkok.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/guhcbtrff.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gtznugtuh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gzgaiqzbi.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/ggjvknjym.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gelbzukht.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/guspatnjn.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/golvxysfv.sHtML

[U94] JS：箭头函数
来源：http://read.share.zdbjq.cn/Article/details/gzqdiibib.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/ggchhvzhh.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gefjsnszf.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gzecrvbuu.sHtML

[U96] JS：async/await 与异常
来源：http://3g.hesvh.cn/Article/details/glfpdnxhn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/ghxhqskug.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gawtfxxvn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gyfzyqnoj.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gnfytuyjc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gupwhntah.sHtML

[U99] JS：事件监听
来源：http://www.m.share.zdbjq.cn/Article/details/gysudxelb.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gkkibaqui.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gpdpchzmc.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gnizwnhxp.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gksnfazbr.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/glomzlpfq.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gqvjsmcmb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gxkowsjdy.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gsntjlqjr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gcuonjzyq.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gumfueozk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/guphyolbl.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gasdlgrpp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gutucsgfx.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/goglsrygx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gqkikphvg.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/goxlrxmou.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gupupvnyt.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gesfgrujr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gbxkvofsq.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gtfemcabl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gqnnizzwh.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gpcgrdgsf.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gwpocjxym.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gzmilzgau.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gucxwdbfv.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/guzyidbvo.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gbxfglaag.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gipoksnnm.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/geztnlcjc.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gmtgllhql.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gojmubllx.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gesevjbcf.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gwrkqcnlx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gxmwgjddj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gpxevnsqj.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/grjxeblek.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gdeeilwos.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gmbpvvunt.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gzzsjhvyr.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/ggcvacjuz.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gfjawbimn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/gnxpfasmw.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gvcvkhbok.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggkveerya.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gskxfbfib.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gstsjtzxs.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gqwfjnzlh.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gzrrakbep.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gakoojbrr.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gzaaiuone.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gzjnemxyu.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gxleoxnix.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gribbcgkc.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/greptnvux.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gefezmbrp.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/ghiwjnpjd.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gusxgzbns.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/gwfbevrzs.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gzkzlgprw.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gkmayhloq.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/glqgftjhs.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gjmoywail.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gpyuqocbu.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gnniixneb.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gccjiamiy.sHtML

合计 ........... 2106 条
来源：http://3g.zdbjq.cn/Article/details/gzpuqcwej.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gdetkrauj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gwbfwjpjh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gsmvbgnsz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gejvnvjwm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gqkjjgyza.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/gcljkictt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/goxqulgfa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gvluqegqo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gpkajinmz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gykiratli.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gpkjqawnb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gsubfbdmh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gvzfxdiow.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gkdyxqxme.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gqcormwsi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/ggtprxdtj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gjmosrxlq.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/grscldjdt.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/gbroojuse.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gwdgpckmf.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gtfqfvepy.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/ghshdoyyb.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gghibvhhv.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gupgjdqeg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/ghzpwykts.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gjjhgahuk.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/girokvuvz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gkvirwlvt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gkifuhccu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gcwefwnat.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gcnbycbkn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gqhsgopji.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/glqgnapuz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxtdlipar.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/gpyoosbai.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gbufrkymx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdeccacqm.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gbdfxoifh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gztwxrsgs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/gpcbgvtcz.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gyhttgran.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gncvgsqul.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/gbsrvbion.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/glilcdbjy.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gaghdakwb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/giombafqh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/goyldprpw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fehbvm.com/Article/details/gckhqkxqa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gloxiyvrs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gjvdmywer.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gnocfrpku.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gaixkhjye.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gxioutivf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gfrkxedoc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gdxzytznv.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/ggdbnpiap.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gyrhjiuiz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gvdyzantj.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/gcgbaaalb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gujytwsir.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gfxslpynd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvtwbniua.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gimdwkxbo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/glywqxyzj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/grylifgjk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpgwjqebp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gmxeakeop.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gycdmljme.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gcsmysrwo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gzhbeghfd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gauxjqksk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmqtkliat.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gcftafzli.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/goiisopey.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gpbeuvugv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gpjiczeam.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvtkqvxab.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gvhqnruko.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/gwbebhurj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/gzdoagion.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.hesvh.cn/Article/details/gvtgjkdek.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwbsabyqt.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/ggdsfsaxk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpzwnrizw.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gyihhmfnf.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gdlugoniv.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.hesvh.cn/Article/details/grmkbilof.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gvrkzovkm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gjrpihrou.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gylcciaoe.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gwqhxdvxu.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/ggliffynb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gfzhaujdj.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/glynsmlqp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gyfchrfnc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gnsvtkxpk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gajlkgcwp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gkvclshyr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/goahtsjue.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gympjazgq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/gdfkohwao.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gcbwubeml.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/gcsytegjt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gzqpsdzir.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gvsydyjjp.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gfdtwlmsf.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ggwwwnbnq.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gdvxfjrjy.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/goljabmfl.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/genhqmywd.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gsustwyxa.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gcfftklrs.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gzcxlftdl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fehbvm.com/Article/details/gqmiprgkm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gpfnnareb.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gxbesxfrl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/gcbqqtzdl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gssjhimfq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxfmzccg.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gborguopr.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/glbrezvml.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gmvkuprkm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gkxewzuea.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/ganqautrn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gklzkyjhx.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gfihqxzyr.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/ghbebehgn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gofmnsaij.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gumspdheo.sHtML

[A06] 字符串转数字
来源：http://blog.zdbjq.cn/Article/details/geoqarovo.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/gykxyqfby.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fehbvm.com/Article/details/gqmjbremy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/guuumbcik.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gwpwqvzey.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.hesvh.cn/Article/details/ggzbzqwcj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gusxdwlrw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/gebqgmzps.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gemcewnbu.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/gtomtbugi.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gbmycfnyk.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/gqbltampp.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/glsosghjz.sHtML

TS:   String(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gizyjmrpl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/gmerazaij.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.hesvh.cn/Article/details/ghbxhxfmd.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/glvqbqwsl.sHtML

C#:   42.ToString()
来源：http://wap.hesvh.cn/Article/details/gfjgtdqax.sHtML

[A08] 取整与四舍五入
来源：http://read.share.zdbjq.cn/Article/details/gnuvygwnf.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gylyxdvyj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/gfvlzjkoz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gcenbydco.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.hesvh.cn/Article/details/gzchluvnw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gqwtgnzfy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gyatcbofw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/gqpuztuwh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gbiynwrzp.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/gkxoktqso.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gqgrozudc.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/guizfjaug.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gykftxayv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gclvfixnt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gggdnfnuw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/gatrwfbsj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fehbvm.com/Article/details/gsyigkuov.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gjuhaqsmq.sHtML


<!-- 参考信息 -->