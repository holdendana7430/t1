代发 wailian999

[U69] PHP：PDO 预处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gohlwwrlm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggegzfpia.sHtML

[U70] PHP：PDO 事务
来源：http://3g.fanxiaobao.xyz/Article/details/gybrvfkvp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcgpsmra.sHtML

[U71] PHP：抛出异常
来源：http://baike.fanxiaobao.xyz/Article/details/ggyhjpylp.sHtML

throw new RuntimeException("失败", 500);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvasjdsa.sHtML

[U72] PHP：写错误日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gmubefxbc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fanxiaobao.xyz/Article/details/gmbdxqkxm.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fanxiaobao.xyz/Article/details/gtafwveqv.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkklnikem.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gaulodajz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmmpyces.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsmqkpzl.sHtML

composer require psr/container
来源：http://blog.fanxiaobao.xyz/Article/details/gedcsbkfq.sHtML

[U76] PHP：简单路由
来源：http://blog.fanxiaobao.xyz/Article/details/gcindbtck.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcawdvufz.sHtML

[U77] PHP：模板渲染
来源：http://blog.fanxiaobao.xyz/Article/details/gfcoyzhaa.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhbewgty.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gmquwpisp.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fanxiaobao.xyz/Article/details/gsuvxqdzf.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gjidqtboq.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbhokjfq.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusnohapw.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfjezjok.sHtML

[U81] JS：初始化项目
来源：http://3g.fanxiaobao.xyz/Article/details/guxmcyajc.sHtML

npm init -y;  npm i express
来源：http://3g.fanxiaobao.xyz/Article/details/gayfinjeo.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fanxiaobao.xyz/Article/details/gfbhjogal.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhibmboj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/guureyszz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gwkvkomfw.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gweusyskp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwrumjiy.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtejsbznh.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gdjbxiihe.sHtML

[U86] JS：空值合并
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrhgubmc.sHtML

a ?? b
来源：http://mobile.fanxiaobao.xyz/Article/details/gqekquhfx.sHtML

[U87] JS：解构默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkaolkvn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fanxiaobao.xyz/Article/details/gohpsonmw.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fanxiaobao.xyz/Article/details/goqrubocj.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gliurlnfx.sHtML

[U89] JS：数组去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gciabcdoa.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gpwkhgrdt.sHtML

[U90] JS：数字数组排序
来源：http://baike.fanxiaobao.xyz/Article/details/gooxavzsi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gvxveboil.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gaefgihad.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.fanxiaobao.xyz/Article/details/gcydawfwe.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/glvmbpiic.sHtML

structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/geyrbjclp.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqtykuay.sHtML

`共 ${n} 条`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajfegfgw.sHtML

[U94] JS：箭头函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnjgixtf.sHtML

const double = x => x * 2;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdvenkoe.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcefxhexe.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fanxiaobao.xyz/Article/details/gzzuuvach.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gofnegqvz.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/grvqoagfj.sHtML

[U97] JS：并发请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geerecpyv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/goinxsget.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfqhtspr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrxigphm.sHtML

[U99] JS：事件监听
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdabmhmt.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjelusuo.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsmodyva.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gardizzpo.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmrikadn.sHtML

el.classList.toggle("active")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfprqqjo.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/gxugrewrw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxbbnhdj.sHtML

[U103] JS：定时器
来源：http://read.share.fanxiaobao.xyz/Article/details/gbihuqdrn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgkeaakp.sHtML

[U104] JS：防抖
来源：http://3g.fanxiaobao.xyz/Article/details/gvheuqrkg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/grpjoxmtj.sHtML

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfexfmfds.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fanxiaobao.xyz/Article/details/glvhbtuge.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqazucwen.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fanxiaobao.xyz/Article/details/gwquutvxd.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaebistl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggujowblx.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/grtlrhfny.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvlffied.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfbuqeaw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gxhwokxtx.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gjlffmrcz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gjpuxqxzq.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdblggufv.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gffkapjvu.sHtML

[U112] JS：字符串补位
来源：http://3g.fanxiaobao.xyz/Article/details/gijruotlj.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gurgtuhsu.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhttjahj.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gspzyefzl.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gduhydbms.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gugbpdvlz.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmyqtldg.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwxpptng.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscpzwajo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/guwgckgnt.sHtML

[U117] JS：单元测试
来源：http://read.share.fanxiaobao.xyz/Article/details/gkojjzlrc.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhygjzzg.sHtML

[U118] JS：开发服务器
来源：http://www.share.fanxiaobao.xyz/Article/details/gwenwbgul.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fanxiaobao.xyz/Article/details/ghupkeuch.sHtML

[U119] JS：生产构建
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehirbjbs.sHtML

npx vite build
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkktgrsr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gphwaftzj.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/glipgrcqv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckdeaprz.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/glcsjmjeg.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaolcotw.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuvaaxum.sHtML

Python ......... 252
来源：http://3g.fanxiaobao.xyz/Article/details/glczltsbj.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gygvzsopj.sHtML

JavaScript ..... 252
来源：http://blog.fanxiaobao.xyz/Article/details/glqygdwlj.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgbvkndy.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gqawlfjcv.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumpchpad.sHtML

Ruby ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gafkgltau.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxwjtlfr.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqwyjerm.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gcnlvewxt.sHtML

SQL ............ 90
来源：http://baike.fanxiaobao.xyz/Article/details/gatjzilyy.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgunlaex.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgxclbey.sHtML

Swift .......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvvatfdv.sHtML

Lua ............ 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlkbbhjl.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gadbpspjn.sHtML

Scala .......... 10
来源：http://3g.fanxiaobao.xyz/Article/details/gduqoglla.sHtML

------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozoqdsso.sHtML

合计 ........... 2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gfjrrbgap.sHtML

按章节统计：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpdzyzfg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeycqslh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gcapxbcui.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gijsdvpwa.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/glybzppop.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/guszbwqgj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gmfszpojg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gfyvaphwf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gkukeybin.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fanxiaobao.xyz/Article/details/gqpuawgjs.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrrzinve.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gspdgdxxg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbesjcbm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gcdpdjpjp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqnvtawt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeprtzry.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gkpipojyu.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gjesvqojf.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucjpzfhf.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyzuusir.sHtML

T 其他语言补充                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gvivmxwbf.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gccmgmblv.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwiondvn.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gposvrmxy.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiyfexdl.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuvxbgsh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdjizpat.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fanxiaobao.xyz/Article/details/gbasjjtas.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgardihn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/gbyjzfkya.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fanxiaobao.xyz/Article/details/ghodqikdj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsateveq.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gxjdrfqzc.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrcuugmd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guneundvs.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/gaygsqhxq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgnlnkjn.sHtML

【收录内容】
来源：http://3g.fanxiaobao.xyz/Article/details/gbvpqcyin.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/grrtklmjb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/gyujbseaw.sHtML

SQL · Bash · C · C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsetgqdn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgokohub.sHtML

【使用说明】
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaizqbab.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fanxiaobao.xyz/Article/details/gikiusbvj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fanxiaobao.xyz/Article/details/garsgnytl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginkjeftd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/gfzlitrwl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhvznnei.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/gkbcprdlz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fanxiaobao.xyz/Article/details/gikekmrkd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getzhztrh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyvbnias.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fanxiaobao.xyz/Article/details/gsjnrrrea.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gdepiiemj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fanxiaobao.xyz/Article/details/gxebxisni.sHtML

【文件统计】
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuvsrtpx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fanxiaobao.xyz/Article/details/gdoacobpd.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfamhlctv.sHtML

目  录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejsfngfv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fanxiaobao.xyz/Article/details/gyisolnjf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gcfudfmlu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/getgbeftz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gljremnjz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gkpxesghb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhdgbkxv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/greyphzjl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmapwdsd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxsukedn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxrxczgw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpmpeirh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gvzxlyidg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnqwgmjd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuzyaeia.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvyocwrw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeeejvlw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmwamscl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/glmolmamu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqsbzwdus.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fanxiaobao.xyz/Article/details/ggttoanlk.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeuiznnk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlvzgjft.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geejzwlzn.sHtML

A. 基础语法与类型
来源：http://baike.fanxiaobao.xyz/Article/details/gghjuhnob.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvuzotksy.sHtML

[A01] Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gmolveqrg.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfiyuzok.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fanxiaobao.xyz/Article/details/glmtdmrfm.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gnodvivcs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/gicbmvoxw.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpkkklrq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fanxiaobao.xyz/Article/details/gcoryznrx.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gepckxupp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfpasmrw.sHtML

[A02] 变量声明与赋值
来源：http://3g.fanxiaobao.xyz/Article/details/gtrmynqdz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqeiksnf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gfedfmooh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gqdwxishg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggejliqoo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/ggbtmynfs.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxvlcfdy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fanxiaobao.xyz/Article/details/gyjdwjago.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gomroansm.sHtML

[A03] 常量定义
来源：http://baike.fanxiaobao.xyz/Article/details/gmhgesago.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisifuqsz.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gosyqvirs.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/ghgmzagqs.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnunlvymp.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gisbquyas.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmcpcxik.sHtML

Ruby: PI = 3.14159
来源：http://baike.fanxiaobao.xyz/Article/details/gglcizvam.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gkryurbdb.sHtML

[A04] 判断变量类型
来源：http://www.share.fanxiaobao.xyz/Article/details/grnvgqtzo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fanxiaobao.xyz/Article/details/gguguidfu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fanxiaobao.xyz/Article/details/ghtdkuyhe.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fanxiaobao.xyz/Article/details/gzxmamhep.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/glhwrzgnh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fanxiaobao.xyz/Article/details/ghxoudahi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fanxiaobao.xyz/Article/details/guppkqwis.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.fanxiaobao.xyz/Article/details/guumvxlij.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fanxiaobao.xyz/Article/details/gvfnzokye.sHtML

[A05] 整数除法与取模
来源：http://baike.fanxiaobao.xyz/Article/details/ggqbentvj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gjefqjlud.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/geklbztju.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcurfnwp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gajajpyqv.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/getotexij.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gpoblawzv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrqdscku.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/ghshiadhy.sHtML

[A06] 字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/gaxezqfca.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/ghvkmwrqr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdckykxto.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/girxoqcst.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gtznjltoj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdvrtyou.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdywfhemb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fanxiaobao.xyz/Article/details/gglhttlde.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsgnjzti.sHtML

[A07] 数字转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsliscbk.sHtML

Py:   str(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/guutqfiso.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdwzojbq.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjauqmudd.sHtML

TS:   String(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gjbnomjuo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhttigyp.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgxxcvef.sHtML

Ruby: 42.to_s
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqqubydc.sHtML

C#:   42.ToString()
来源：http://3g.fanxiaobao.xyz/Article/details/gamxyhngh.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfitosij.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmwmyiae.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelgmwhev.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gcqnsvzfp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngfeqosp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/goufjmuxk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwkfywbv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfnhgzbn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwndymgb.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihlbzgno.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwslrlxo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gcbovdcoh.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/giqwgsqeq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvqbknzh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gvmbngzrj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmqqqylt.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fanxiaobao.xyz/Article/details/giobqmkld.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxgiknti.sHtML

[A10] 生成随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvbrsxvg.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwuyojou.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fanxiaobao.xyz/Article/details/gyagrszsz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gojjbrgeh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujzbaltj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzyoordd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fanxiaobao.xyz/Article/details/gqmzrpjqh.sHtML

Ruby: rand(1..100)
来源：http://read.share.fanxiaobao.xyz/Article/details/gowysxnhj.sHtML


<!-- 参考信息 -->