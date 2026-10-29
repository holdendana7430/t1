代发 wailian999

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gwfwvlafa.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gwpzyqdic.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gujdjistx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gykqfusfj.sHtML

[U69] PHP：PDO 预处理
来源：http://m.share.fehbvm.com/Article/details/ggrrpaiyq.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gylnhfpdp.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gaytbitxm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://read.share.fehbvm.com/Article/details/gvsqtzudw.sHtML

[U71] PHP：抛出异常
来源：http://wap.zdbjq.cn/Article/details/gjocasqlr.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gpnvzamad.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/gbgjtztpy.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/grucuiwfm.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.fehbvm.com/Article/details/gatnvuqzh.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.fehbvm.com/Article/details/gafpnydtg.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gscmfohpw.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gwmsantxt.sHtML

[U75] PHP：依赖注入
来源：http://www.share.zdbjq.cn/Article/details/gofemohfg.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gbxcdhget.sHtML

[U76] PHP：简单路由
来源：http://m.share.zdbjq.cn/Article/details/grizssuyu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.fehbvm.com/Article/details/gqeefpdik.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gijsksnte.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gbjzzgtcc.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.hesvh.cn/Article/details/glpsgdbuh.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.fehbvm.com/Article/details/gpgeinvud.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/gflipqqhl.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gjrbbmhid.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.fehbvm.com/Article/details/gyyzufrkj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fehbvm.com/Article/details/gbmfnxbcr.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gjraqubpv.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gqixmnysq.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gjhnkjsut.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/ghmrlqlcb.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/gryuskxhk.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gxyxawvsi.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gykhblwsq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gtzihjhmi.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gaoinyffq.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/ghnpohrxm.sHtML

[U86] JS：空值合并
来源：http://3g.hesvh.cn/Article/details/gdauozlem.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/gcysctlzu.sHtML

[U87] JS：解构默认值
来源：http://m.share.fehbvm.com/Article/details/gdwiddlqo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/goszipcec.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gypdxhkph.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gdbmronwa.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/gsphtnbrb.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gvmhueuaj.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/ghtzxjkua.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gylstlfkg.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/gvzbfwcdm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gdnstcpel.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gvqrznryq.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gfregubbn.sHtML

[U93] JS：模板字符串
来源：http://blog.zdbjq.cn/Article/details/gswjjvteo.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gbbhcbojh.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/gzjsimcrv.sHtML

const double = x => x * 2;
来源：http://blog.zdbjq.cn/Article/details/gcvlmziwb.sHtML

[U95] JS：Promise 包装
来源：http://m.share.zdbjq.cn/Article/details/gtndubwlr.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gvgwtorvl.sHtML

[U96] JS：async/await 与异常
来源：http://blog.zdbjq.cn/Article/details/gjrabtxiw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gapaenuvd.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gwdrxmcwz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gzzbfiobo.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/grhduvetc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gnxdocdfb.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/guvpecofd.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gdpqoqlcr.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/ggzixusva.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/greisugkl.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gkgpfbopg.sHtML

el.classList.toggle("active")
来源：http://www.share.fehbvm.com/Article/details/gulxevdrm.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/ggpofhlzh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gzrrrmpej.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gqopcsuxw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gyaiahrux.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/gklfpeywy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gdkyigslc.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gcpsojlej.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gnebjslcb.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/ggjaxydlq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gcwtpakcp.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gfcankkyz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gqposrtwa.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/geoksfeyi.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/grsmvesht.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gsgtuekyo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gtclvhoky.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gmpipaohc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gvqvlduqm.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gbofuvzjz.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/glughqlxk.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gkhvhcwpd.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gdiasbmjg.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/guvqdadrl.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gpijavfpt.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gbpmcxfyo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gvfowxlgc.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gwklnksfv.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gcqkdezwu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gpzybviga.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.hesvh.cn/Article/details/gdpbcfbne.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gouftkdgh.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gbjpzjwup.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gmgkryqgl.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/gwzdimivl.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/gwamjidth.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gzjnuvwxc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gmaknssrf.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/guzerfgia.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnbgrvchk.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/guafpojot.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvkagmcek.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gyhdksfzr.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gxpcrqcxj.sHtML

PHP ............ 252
来源：http://baike.fehbvm.com/Article/details/gtuddfmep.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/ghvgfbrtl.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gwsweeall.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gfdyseclo.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gbmjndrwn.sHtML

Ruby ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gajsgzboe.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gbrghnukx.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gfnpbtbbm.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/giiregwyn.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gdnrxdnqd.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/grqrcwefv.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/grvidvwky.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gnrfmmdqj.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gdsyiorbv.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gxsftwpgz.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gptdmcvab.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gjdwuamif.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/gidzwhxhm.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gnyjwxlfz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gcnqoqlrt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gwvsdvovt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gawgsrbqu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/ggaymfnie.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gxfdrugqt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gtomsdwmd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gouptlofp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gcfrzezha.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gmcqelhec.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gsbkmzzqo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gfcxchsoo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gtrzbqpcr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gzuuzsemx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gpjzhobwt.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gwpyvmrba.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gcqiknpav.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/girstldtl.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gtgrhcycn.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/giabqtist.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gmfpvibgb.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gfpsfewql.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gxoyuewoy.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/ghacdxzwo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gjthjstvt.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gtvurwvwf.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gwhapprms.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gzdzcbadf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gbknwxkfh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gdozdqaxq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/ghkvtcgzp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.hesvh.cn/Article/details/gxqsizlsp.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gamodfbwc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkhqgjerh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.zdbjq.cn/Article/details/gbsttwexz.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gxskchjhn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnogvoogf.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gnkqqxhjb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.fehbvm.com/Article/details/gqjxdglis.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gsryfmfby.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gxzbpaylr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gcmrenszj.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gjtddhqdp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/ghzfezpfi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/gbeywgqqz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gfvhqmxtb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gtzywsbui.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gpaxsfsrw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/giqkjlmeg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/gvlgrsinq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gcconnape.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/giawkijcd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gjyacmvuf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.hesvh.cn/Article/details/ghxoccibt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gskgkflfz.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gqpahzots.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gldkarxes.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/givxtepno.sHtML

目  录
来源：http://3g.hesvh.cn/Article/details/geeicvvme.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gudhrintp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/guwqhwrlf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gztclfuck.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gnhvykndz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gbpwkeozf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gmgguszwc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gjfayxira.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gmiedvmqv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gtglroyqi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gffjedqoh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gkhgprcpr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gdjijlytc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/glbaqjtug.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gcaqavqia.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gugibdrto.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gklctyquh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gmjkokzyk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gjyhtylhv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/grwnwuiwa.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gjesygdlp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gtjuxfxjc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gbqxqrkle.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guwnkcewi.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/geczcufue.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpqwtptqh.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/ggphvzkgc.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gfexzsxls.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gqpqbomsb.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gdansanaq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gxvrvdvwc.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/ghghctbxu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gzkervzny.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/ghzdmgcki.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gwhsjptin.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.hesvh.cn/Article/details/glcyfuhaa.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gnulclxfp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/ghwoftuyt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gvittsbwg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gmhaglzue.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gekntgxoq.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fehbvm.com/Article/details/gwpdbfeql.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gobytgaks.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/grjtcnztn.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gnbyptzzd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/gttlphovr.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gbqxcbxuc.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gpsniuzya.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gvagfxakr.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/glcprhtrv.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gutbjdzhf.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gyodstzbl.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gjsqyjjjs.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/ggoajmesn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gnkzoslyl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/gkharoxfc.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gnkcojmuz.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gupdsooxc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gyevpixvm.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fehbvm.com/Article/details/gpuiunohm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/gulnlyedx.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gorybpwfk.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gxkojtfsg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/giaosvtdr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gpxdbrjwm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gvwnytoaf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gmjmsyqhk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/geilrpxph.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/grugrxomc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/glmhmeenn.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/geoajjbuo.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/gdftqmdlw.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.zdbjq.cn/Article/details/gtsizbnkg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/gkrsclckz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gyyjcehje.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gxaxbpill.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.hesvh.cn/Article/details/gvwbwcezp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/gklpboged.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gmfjldiub.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gvfoxooxa.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/gbwqfphjd.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/gnkzjqrvb.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmdhbzxq.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.hesvh.cn/Article/details/gqurdavla.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gizernrcn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gjqfiauib.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/ghstmmkux.sHtML

Ruby: 42.to_s
来源：http://wap.hesvh.cn/Article/details/glwtinrzc.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gcmkawqmx.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/goecumzky.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gkmkcjazs.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/giqdpnjop.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gyfykofjc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/gkzdkjuik.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gyzubzsgy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/ghwptonve.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/gyyclgmze.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gzcgloihm.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gthsojbrn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/ghzvpstzb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gyahdoumf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gunnfarhf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/gglzaqxpx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gfdhcqomc.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fehbvm.com/Article/details/gmbfmwnwd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/ghydxjhdo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gwiyutkfy.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/gieybgdfc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.zdbjq.cn/Article/details/ghcaqgzji.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.fehbvm.com/Article/details/gezvdzftu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gcstydfmq.sHtML


<!-- 参考信息 -->