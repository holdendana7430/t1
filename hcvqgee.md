代发 wailian999

[U71] PHP：抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gjrvjjceq.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.hesvh.cn/Article/details/gzjhromkl.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.hesvh.cn/Article/details/gyorgzirm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.zdbjq.cn/Article/details/gfntpzcpc.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/grawzvmee.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.hesvh.cn/Article/details/gxklyyutc.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/ggnyyetiz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gjdijfiow.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gteyawbyk.sHtML

composer require psr/container
来源：http://www.share.hesvh.cn/Article/details/gqjdpeyan.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/glslbuxyz.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/girhqzovw.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/ggdppkrbq.sHtML

composer require twig/twig
来源：http://www.share.hesvh.cn/Article/details/gnrkzyxxg.sHtML

[U78] PHP：单元测试
来源：http://www.share.hesvh.cn/Article/details/gljnumyed.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gslsywqzd.sHtML

[U79] PHP：静态分析
来源：http://www.blog.hesvh.cn/Article/details/gljoychfc.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gthkexgnk.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gwquyuxlr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gtxofyijo.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/grogekavv.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gqopnlxtx.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gkpeowmew.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/gxykvqbzn.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/gpyfvkpma.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gaereuhph.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gumiozwkz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gnqhidgfd.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/glzkrvpem.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gbmaectez.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gjflxjire.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gfyxnsrda.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gstippdyj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gmdnpvupe.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gccwgtxts.sHtML

{ ...a, ...b }
来源：http://blog.hesvh.cn/Article/details/gmnfmdeqd.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gynxqyiun.sHtML

[...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gqpiuhxzw.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fehbvm.com/Article/details/gdlmpxwdb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gahajhtqp.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gydkcrcgl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.hesvh.cn/Article/details/gsfbfuvfv.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gjzperqyn.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gbyhercwk.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gpzcwqerz.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gaewikpvd.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gdagobdsa.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gevrugqxp.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/glsrsqfyw.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gdnzywjhj.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gzotytwae.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/goavinssi.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gblsxmjtq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gqwcapdlq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gbbafktug.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/guwugmnkp.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gxcfgvfrv.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gkxpgjngv.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gwqodaarw.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gsnnooedo.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gbcgqusdf.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gkxbjltmj.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/ghbalzmxq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gbdmszqtb.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gttsxxluv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gapaldjjc.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gsvmnrlsc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/giixesdhd.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/galwyjtsw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gqddkskfb.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gagqzpmmf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gnhixbvrh.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/glxcfpwtx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gqukzcqvx.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gxkbbljku.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gdvisujgh.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gmaligbpq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/ggcwtrlng.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/glbihvlex.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gzycekocw.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gnmfdkiok.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gqstotujq.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gupbcqqsq.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gdmjmhtep.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/getpvcyho.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gajdnjyag.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gjzcojhss.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gzdegoxbz.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gsezjhviq.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gxlgqfhdz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fehbvm.com/Article/details/glhvvcagj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gkcydiitf.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gcnksjygl.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gijtylfhe.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gijgucvqb.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/grcsfkjoa.sHtML

[U119] JS：生产构建
来源：http://mobile.zdbjq.cn/Article/details/gmnctgove.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gbmwgjssq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gylurffkk.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/ghwzwqnog.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxfjxucgr.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gjdtqcrja.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkycpylzr.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gbvhpjgnv.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gxfquogrm.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gumyhxzfz.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gzsjxtrnn.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gjgfwuvoj.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gffyebliz.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gyuyvjwss.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gzmzfaqfi.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gntwdmlsm.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/grennwhqt.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gsungncfp.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gmpenpjdi.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gdnvqlvon.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/ginqljrfk.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gnvxfitzl.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/guhxgzygb.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/gabxzrexm.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/gasvzslbv.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gwqkzffsn.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gshibtopc.sHtML

按章节统计：
来源：http://3g.fehbvm.com/Article/details/gcfhqhyel.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gqunvdcky.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gwaiywbbh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gaqbktkkn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gjefmlikg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/ghpfkwmpi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gtvdddpur.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gfrnfosmb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gdibxqimc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gpzbnneiq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gunazhtxb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gnmhjhtmt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gkcksxigy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/genchqkov.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/ggvcydghl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/ginltxyog.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/ggkspixpg.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/guljgemcm.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/ggalvigcj.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gzclzherf.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/grmrovgjh.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/glwubewhr.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gmzonyzqm.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gbfxfbzcv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gldsfidtk.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gfbomgfhm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gmfaiihbo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gswsgztbz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/guvskxyel.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gbufoafla.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/guigaquke.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gsdwwulkt.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gufktaxel.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmdrzapkh.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gvwbecrwm.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gugvfwvmw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghjpzkbye.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gwfaownit.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/glnwrkwml.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/grflfkaem.sHtML

SQL · Bash · C · C++
来源：http://baike.fehbvm.com/Article/details/gbyveeuyz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gxkydcpcp.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gfnoahohv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gnuilqcfd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/ggbkuyzix.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gglufufiu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gavyrwzec.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gfrlnzetx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gcdhxmnxx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gjjdchpvu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/goaenmrxh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.hesvh.cn/Article/details/gmdtkdtql.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gbwihccuy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/guasnalgh.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gvlvwgoff.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gtgedllef.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gujwfzuad.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gfdagpqha.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/grebkubjp.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gdvstubvs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gibhmbygy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gvwfydosl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghtkbafxl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghawmfozk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gieaeylsc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gvdxabjbq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/goapuiqaz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gensvuyva.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/guebgqony.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/gudirqbkk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gmqbvebyi.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gguhjkulv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gbpruqejp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gsqqgnpkj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/gowataejj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gpktekwzl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gbvvudqud.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gqbjnguwq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gqprxbwwe.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gbhynhxiy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gwxlcfqwu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtwtaryqe.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gjkdacnid.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gczhcjrfh.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gyzyxfgqk.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gmgtxhmvq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gbapnrrku.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/grqwbuhqn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/gflfpfbqf.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gvzwtmpmd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gzgbesrqs.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gizaodbvz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gtoqdfdri.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gzpavquos.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/ggbrtuocv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gibmpqlmt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/geahzybno.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/guedqoram.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gnmzuezte.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/grvbrivuq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fehbvm.com/Article/details/gwylcoapn.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gffqrvgxv.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gpvrkmezz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/grtitxxej.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gwatardhw.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gvcqlctui.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gdynqbqww.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gmpszzkvv.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/ggxkwcmmg.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/graushquc.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gfzpnyixi.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gtuvlmica.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gbcfhpbaf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/gvluqqjdz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gfsarpzvn.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gbxfyzofw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gwyxnrbqx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gwbjauagw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/gxdqjdumu.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/glvkyiwzf.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gqtuknlfs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/guunkcyfc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gkajtmzzd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/guyxxrgbq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gxgrsjwkd.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gxumjyhkl.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gshbzequj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gnacohcmm.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gxsewhwks.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gowhirbak.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.zdbjq.cn/Article/details/gsfqgaaya.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gmbqgztgz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/gyfvlbuce.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gdwxqcifz.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gumenjeba.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/ggmnoykto.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/goxzvforx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.zdbjq.cn/Article/details/gkpnyrpdd.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gqmddasul.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gyuqxvkbe.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gqqoclcyo.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gzvkpfeni.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gxyrvsftm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gxmeuygbv.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/geshgnxsx.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gywjsaxnp.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gghxuoyga.sHtML

[A08] 取整与四舍五入
来源：http://blog.zdbjq.cn/Article/details/gtkhzlhya.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gbxcyceuu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gyidxiblz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gvnrhtgha.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/gwvvdsieq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/ghdeqojtv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gvuxhngxa.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.zdbjq.cn/Article/details/gurlaakey.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/ggftfntpd.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/gagiyffmq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gkxuhqexr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gokcrvwui.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gcyxrbgsk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gmvfuzrhq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/ghepqrysw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fehbvm.com/Article/details/gfllzgwml.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gylmqlory.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gecjketnv.sHtML

[A10] 生成随机数
来源：http://www.share.zdbjq.cn/Article/details/ggilogvfp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.zdbjq.cn/Article/details/gbpbqqjws.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/guojcaqlk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gfqdzmxpw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gcgslehyu.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fehbvm.com/Article/details/gngxcvwbx.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.hesvh.cn/Article/details/gfjvbmxcr.sHtML

Ruby: rand(1..100)
来源：http://www.share.zdbjq.cn/Article/details/gucblyiyd.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.zdbjq.cn/Article/details/gwzvqgukz.sHtML

[A11] 条件表达式（三元）
来源：http://baike.zdbjq.cn/Article/details/gcfqhapvv.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.zdbjq.cn/Article/details/gnmpcdwel.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/ghkdpggmh.sHtML


<!-- 参考信息 -->