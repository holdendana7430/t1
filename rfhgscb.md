代发 wailian999

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/gtfvehzjx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gvhrxiezb.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gjntyfghq.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/genbnmthq.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gailxccxe.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gilubgcpt.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/ghxwqywqg.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/ghvhkwugt.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gddaditqo.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/glgiuaynj.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gajcibuuk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/ghzqghqdy.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gtypgduuw.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gikkmpcgs.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gyuibbdgv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gbvxlboyt.sHtML

[U99] JS：事件监听
来源：http://3g.zdbjq.cn/Article/details/glcvuafjk.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gadkqhhkg.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/giucjzchp.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gswfdksys.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gvefempvq.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gdwjcudbu.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gcmrzyffy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gdrarwikc.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/ggkflvapj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gpltxfdna.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/ghxkrrgvu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gxvorxwto.sHtML

[U105] JS：节流
来源：http://wap.zdbjq.cn/Article/details/gjyedpavz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gfxfggpik.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/godqitgst.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gqegqfcbz.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/gdbteksil.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gvylgjkcq.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/glrjjtcou.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gmmxjnyfd.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gwdtiubdh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gfodvppjc.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gtykwltxi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gbwyvoobw.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gtmowzcoq.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gjppishaq.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/ggdkryrgd.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gstprucad.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gytwrfdgh.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gfkyypjkn.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gkptjfjax.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gaesrzfqc.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gfthgzpnv.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gpwpgjdsd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/ggvsxzruy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gpvetioay.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/ghhhdferi.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gnmnzxblz.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gwfzqnzdb.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gxbsxlomw.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/ghtjcadtz.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/geccnoqnt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/grtztynjc.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/goeyqivhx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzokbqvku.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gvlfqzaza.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxtryukyk.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gcsqfamub.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gryarvwfp.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gcuhrjswa.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gpnxcalws.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gslmfdwfk.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/ggyjrqdhp.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/giwwcfgos.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/ggiubgygn.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gackbhxex.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gwtcqpivo.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gkqkleubo.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/ggrsxlrxp.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/glyeepvgg.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gjxslymri.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gwmkbignw.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gudsawwqq.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/grplfvdmt.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/ggzkehtzd.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gkeywixiz.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/ghmgollbl.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gynseawih.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gzsleifee.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gbrqdurtc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gijgdasvq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gdiaxkeyf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/ghivacelo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gbvbttxnf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gcdsgdtlu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gffexbsfj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gxfyerdhk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gazswgneu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gsfexrgud.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gddrjtjta.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gqhrabvgo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gjzmquusz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gmasdsaja.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/giglclraw.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gegnjcfqn.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/glyuqjdin.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gmjouhnza.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/glprvequu.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/gqcsqpmjg.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gtwimsjdt.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gjwgqureo.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/ghruzuecl.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gbovpplqx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gkjtxshqq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gjhlwobch.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gbxdrsdiu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gshpqeyxm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gmnicnffs.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.hesvh.cn/Article/details/gslrbeicn.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gdpwgpyhv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gifadlmoj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gdwxiguri.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gccgtxdyy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gypfelamc.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gesnkdwvb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gafgxdwxx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gvpazyjae.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gvmjvsmwd.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gwfbcyjql.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gitwxdaoj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/gemmrwqdi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gpcasysmb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gggcegxke.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.hesvh.cn/Article/details/gelccoibo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gnytxltvo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gixlgagzo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/girbpzdhm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gicpboefh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/gsckyeqot.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gzkoxaqsh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.zdbjq.cn/Article/details/gejldqrwr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gjeucclut.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/ghjrddgar.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gnhxdxqjj.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gmbjnbsho.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/gpwmazwve.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gmuyzjxyw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gxexblgsb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gdlvvkyyo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gukuwbjzg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/grymfinrs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gfsecrmbj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gygzmxncr.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gpetesmsd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gcpkhffho.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/geajcemmz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghfbvcler.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/geretaqhu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/glhixlatp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gxxdjmteg.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/glxlhqjpu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/ggtjwnupk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gxguqewdh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gvmtqdorr.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/ggazpliob.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/glqwpthgh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gdbdjwtnv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/grsovwbgl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqffqrlaf.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gjfaoldob.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwkpnxhdx.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gnhmwqzvj.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gmrxvwetu.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gjysyditj.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/grsbgfsga.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gxqrghjwb.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/grhnclgjm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gpgkebjld.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/ggyobwibg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/ghxxgizaq.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gsdpjeszx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gnteatkwq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gpbsyqhaq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.hesvh.cn/Article/details/glofdnwqd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gdxitouif.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gcwpoflaq.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/goginhajw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gmwmjhoqx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/glcwnscdd.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/gidzywatf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.hesvh.cn/Article/details/gqixpxbro.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gesnmapzd.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gjpdtzclb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/glutwxjth.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gkopiokec.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gsuvnbkso.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gdkbsldlc.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ghrzxhhab.sHtML

[A04] 判断变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gxuyqfidi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gtlvsyqnd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gkkjapgyo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gyotwaodx.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gqorllsca.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gdqponrlh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/ggvepoxbp.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gxcqgxoxd.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gyzfgxtxk.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.hesvh.cn/Article/details/gdtvsrwnb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.zdbjq.cn/Article/details/gcmmzzjcq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gyllqivwn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gwkiozvtw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gyfxjozpu.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gevyxiqlo.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gwcklnleu.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gzpbomxlt.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/glgifnjvi.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/ghrvugqwj.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gkvqumnaq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gvxxfdyes.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gffxcqqqa.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gqzzlayud.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gxxuektou.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/gblskcack.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/gqxvxtjhl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/galxsjwgr.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/gsvwexrhu.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gjvcwigvi.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/gkctnblga.sHtML

JS:   String(42); (42).toString()
来源：http://blog.hesvh.cn/Article/details/ggecglkno.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/gndonsohx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/govxnajut.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.hesvh.cn/Article/details/gzjtmbriq.sHtML

Ruby: 42.to_s
来源：http://m.share.zdbjq.cn/Article/details/gmjiloeqv.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gavfgmlgc.sHtML

[A08] 取整与四舍五入
来源：http://wap.hesvh.cn/Article/details/gcoxilxdn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gdfcvbkoy.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.zdbjq.cn/Article/details/gdfqsejkg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gyfpwinbn.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/gtqbfgrzp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/guyjkusgr.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gawmbwhsh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/gwctpycmk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gsdqflzue.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/ginbfcxpz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gnlhiptif.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gdajummae.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gcfzbwlnx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gwsdlpzfk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gycyvdlbn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/gwocuukhf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/gjvcwkiyf.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghxvatxju.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gsygjpogw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/gboesfnpy.sHtML

PHP:  random_int(1, 100);
来源：http://wap.hesvh.cn/Article/details/gvqfhtnfh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gfnrhkkcc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/gtjiqvuqy.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gljiaaeic.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/gqdpemuld.sHtML

Ruby: rand(1..100)
来源：http://blog.zdbjq.cn/Article/details/gqhdzikqn.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.zdbjq.cn/Article/details/grbsmlhlu.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fehbvm.com/Article/details/gtgwvwmun.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/gmmdxcgmc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gptsljvjg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/goveoclhn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gfwpnawka.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gipioorhi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.hesvh.cn/Article/details/gbpsamwod.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gnrpmmkan.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/ggwdoegcv.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.zdbjq.cn/Article/details/gyotrzxwc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gofivlmsi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/gsyhhcpzc.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gagffssaf.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gcqrmgggv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzvxgswr.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gurbfhznz.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.zdbjq.cn/Article/details/gjkduhicx.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.zdbjq.cn/Article/details/gcmpwwlxm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fehbvm.com/Article/details/gcycsdidz.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gsykutcrk.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gpnaeygcp.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gbutgszum.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gamspzqux.sHtML

Java: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gtlllaghs.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gvlahmmgq.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gbqdkjxey.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gqmugoiwv.sHtML

[A14] 注释写法
来源：http://wap.hesvh.cn/Article/details/gbqckuepv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gzorutxte.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gwwotcnmy.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/ggmbyikjv.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/grpdbgzym.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fehbvm.com/Article/details/gcwkvwpkk.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gniznrnsm.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/gahqnydmq.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/glawacfgs.sHtML

[A15] 空值判断与默认值
来源：http://3g.zdbjq.cn/Article/details/gfxnehahc.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/gldqloybw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/galjptbpi.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/ghyfzvusg.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/grvhmdmpa.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.zdbjq.cn/Article/details/gufantada.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/gchnarmep.sHtML


<!-- 参考信息 -->