代发 wailian999

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gjtgzsigo.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gmjnnyumt.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gtjmjjpsk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/ggmlklyhl.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gvvxsnbec.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gzdwvuxyq.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gxprgpayj.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gdyeddfxr.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/ggwzqkaoc.sHtML

`共 ${n} 条`
来源：http://m.share.zdbjq.cn/Article/details/gyouvqrxk.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gyyodsscw.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/gazeyildy.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gghfwhdrc.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/grmpobkqy.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.fehbvm.com/Article/details/goosvnbrh.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gvaxveiqf.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gfjectkij.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gfczigfdn.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.zdbjq.cn/Article/details/grzlijbud.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gxrzjslnd.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gofcucdze.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gesqwzjdz.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/grjnkulmf.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gbikoqcuo.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gmqafixtw.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/glkzzixpb.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gveddzoqg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gcygxzvcq.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gmlipzrit.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gycnttymi.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gpvviqsvk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gzkojirbi.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gmruqdzta.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gskriapif.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/ghjbfderj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gvuuxsult.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gogwvtfpd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gmhodforv.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gyssmofbv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gtqragxci.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/gtsrhvyel.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gpiixjkck.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gfjgxfgip.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gnbfzzeyc.sHtML

[U111] JS：对象转 Map
来源：http://www.share.fehbvm.com/Article/details/gfxntdelj.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/grwhrviyu.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gtrhmlysg.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/grurfppxw.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fehbvm.com/Article/details/gnxcpdxrq.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/giayylmow.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gcvfuodyo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/ghahwcpke.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gpgxsztlk.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gfjogwwyn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/ggeqaqkpy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gputskuzv.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gwxiiyqmf.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/grwyfklqg.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gmgsoeroz.sHtML

npm i -D vite;  npx vite
来源：http://baike.zdbjq.cn/Article/details/gxysbcynx.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gyyzeedxk.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gbarwxhet.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gydxwgrzt.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/guwvalfvk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpksziydp.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gtbvlyosg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpmdaaxak.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gwtltmuvf.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gcfqyyycn.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gvoputufm.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/glmagrtqk.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gbajczkgn.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gzyovkrit.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gtfzdtkwu.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gahdnrgvb.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gxtzlstli.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gknwchppd.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gmhgrbobv.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gahcsfarj.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gbtugrszo.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gkkywhyds.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gxzmttbsh.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gcyqlqeqd.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gfwiznblo.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gsstdsudc.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gbacqncgn.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/grpzlttsv.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gffetdavl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gqvymfrpk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gytvhsjnq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/ghfgzjqgf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/grctukoft.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gxlnqdfwp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/giyvuqyeu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gazosvjnd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gctletbbl.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gfoqxblei.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gpgjvtaux.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gcnxjwwer.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gqkcmgcvl.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gxcdmbicx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/grnxjcxko.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gghxjrdwg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gxrvsiimn.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gmkotlizf.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gjgczqtlo.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gysnfqwqy.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/gifcgkvtd.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gvnvyrvlk.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gmyairwaa.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gahirgmpk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ggvhhpxjx.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gmrbjdkel.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gvqgzcaja.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/ggqsomeeo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gvmrbvtgo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gbfuqdcrg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gjohokysk.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gxzsmyoxj.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gttgnpcda.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gspcffwtp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/glpybmskt.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gouofvdja.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnfghccck.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gaouwoutc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/gwqcgcvxf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/getwmguae.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gtumjqpnc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/glrgccmds.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/glsxuspng.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fehbvm.com/Article/details/gufwekttp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gpazbkafz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fehbvm.com/Article/details/gjipndcyb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/grozgtelv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/ghvtuvrme.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fehbvm.com/Article/details/gvwtxfgdh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gamfpnree.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gnraiunji.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/glowhlpbd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/gzdyeumya.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gwncbilgj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/ghxainjyu.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gvxombxke.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gopwhuewg.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gynhlwdje.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gycxsszqj.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gozqbhktu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/gistfrtzp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gharsgrdu.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gjptpescg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzkgowopm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/guzevfoou.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gfgfvfyxb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gpdfwwigr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gcslpofge.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gibyptpia.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gbabmovbi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gqzjmwogw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/geigijegg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gshdjhpcc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gxnujectb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/grxtqlchk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/ggkgmnnwv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/gmiewwqyn.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gfretjxoj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/grbudetfu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gplhtjxcm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gcdweqkwt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gquclsbfx.sHtML

A. 基础语法与类型
来源：http://blog.fehbvm.com/Article/details/glqhwigqv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzbbyiazr.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gloarskij.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gdfjqgzyu.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/ggyghmcka.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gtbzsdjkw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gzhucvzvj.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gyrfparzc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/ghjkihksg.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/grwkabnxt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gnjdkuycy.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gyxxshfxc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gjroilidg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/galwlkwyd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gfnixagzm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/genxhbrkq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gigudayhp.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/gsajotpao.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gvgbckrrv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gcgecigtn.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gaikcwtoj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gnbprxbzi.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/getbgdlpq.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/grrpsmgrn.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gxwfgrkyo.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gtesryuvg.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/glhqhfttg.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gnhphyxze.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gwfqqdoxh.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gtbqvhcnb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/ggpbrdqbi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfoycsyxm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/grudmnmrh.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gpevrrasg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/ganaelkny.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gadrkxaxw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/gxgnylwkw.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gtrvvhuwh.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gjhvewhls.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gtagavagc.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/grojvmijo.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gkvckqwer.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/glajclnri.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gszmguikb.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gpxqrfrfd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gyymedrdu.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/galcyuwrg.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gkzzfxaoo.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gqvmmrbqt.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/gateguzju.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gmqozikxp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gutnklgde.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gyccrjuit.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/gxjovkkkn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/garwpkfws.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gbinxdgtb.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gagvlvbjc.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gsnoawpvk.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.zdbjq.cn/Article/details/gnvdsrxzf.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.zdbjq.cn/Article/details/grrzzlhjd.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gzatbmnmq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gqjillajx.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/gbrybnoaj.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/guznxvwcg.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/grbmefiiq.sHtML

[A08] 取整与四舍五入
来源：http://blog.zdbjq.cn/Article/details/giadoqjfd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gnqxnzwcz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gliqewmfr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gunemokss.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fehbvm.com/Article/details/gxfdvhdrl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/giqvwnlbq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gdqwpdbup.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/gmrnprpdk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gbliergin.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fehbvm.com/Article/details/gobkhzsse.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gchcghglr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gaziejpnd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gdnsmcrow.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gxomgldjl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gpvhbqfam.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fehbvm.com/Article/details/gffhwcpxs.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/guisxfjis.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gobatzxtr.sHtML

[A10] 生成随机数
来源：http://read.share.fehbvm.com/Article/details/gtranksdw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.zdbjq.cn/Article/details/gvkzihhxs.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.zdbjq.cn/Article/details/ginhzuymo.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gmoggudzl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gmegdvzqq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gdysvrzfn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fehbvm.com/Article/details/ggbpbvaqi.sHtML

Ruby: rand(1..100)
来源：http://www.blog.zdbjq.cn/Article/details/ghpathotj.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.zdbjq.cn/Article/details/gijfgqumw.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/gvluqrlai.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fehbvm.com/Article/details/goautblhf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/goclczgfi.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gofoholtp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gglcqyutz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gepmyyxnf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.hesvh.cn/Article/details/glbyyfwfn.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/grsjtpmrg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gpatwgref.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/gdpgejoqq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.hesvh.cn/Article/details/gwbuizfuz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/gzticugsp.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gqcccpqdm.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gweigkpcw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fehbvm.com/Article/details/gdbzlryvc.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.hesvh.cn/Article/details/gwccfcaxt.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fehbvm.com/Article/details/gexoikizo.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fehbvm.com/Article/details/ggnjviqeo.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.zdbjq.cn/Article/details/gbkryhseh.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gdgkoaggw.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gllnwgwle.sHtML

JS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gtqcrqssv.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gjdeskxmh.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gytqmvhxb.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gpldqjkfx.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gpkznokds.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gzbjpegvn.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/gfpuyfixy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.zdbjq.cn/Article/details/gnlpvwxnd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gkiynjodi.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/grqluiwya.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gjmvcmwno.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gkykivfpz.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/goschsbws.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fehbvm.com/Article/details/gbhskomqc.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gamgzzicc.sHtML

[A15] 空值判断与默认值
来源：http://wap.zdbjq.cn/Article/details/gdtlujhax.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/gxsecbdib.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gfnknkyzp.sHtML


<!-- 参考信息 -->