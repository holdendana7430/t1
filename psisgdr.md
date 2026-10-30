代发 wailian999

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gnqywdkab.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gqgermbau.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gsarqrfye.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gbsungmsb.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fehbvm.com/Article/details/gnprxwwre.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/glhrbrcjv.sHtML

[U92] JS：深拷贝
来源：http://blog.hesvh.cn/Article/details/gjrtvnwxf.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gkdabnaym.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gwwmvmrsb.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gnvhxkvkj.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gvwbfgjae.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/grtlcfuog.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gjqrxxqbk.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gssxeqdsf.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gkznhqskb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gxgrwbyqf.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gtznoytcr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gbothyjdi.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.hesvh.cn/Article/details/ghxohvnoc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gsrmzteug.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gxekvewud.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/ghscujjkb.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fehbvm.com/Article/details/gbswvvkyg.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/ghuyjwrdw.sHtML

[U101] JS：classList 操作
来源：http://blog.zdbjq.cn/Article/details/gqdrrnkiy.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/ggtxrvrzv.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gxncgulwc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gvrdqcarl.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/gtnhjxral.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gpqdenvbs.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/genhcfhfm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gfsrkhchl.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gpuofbiaq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/guwrsxuav.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gthffgvzg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.hesvh.cn/Article/details/gfkvusoqu.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gkfzvybdd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gxpqdbouw.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gpybprbxw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gtommttjj.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gyvuoajro.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gnjswcukz.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gvyecsdjx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gnusijlme.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gbxqoqnjf.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/givjrvfbb.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gyhcpvypo.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gysiddyho.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gifdyblwf.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbtcdublc.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gjrbezrlc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/ghqqfsmij.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/guoybrtap.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gthbjfssw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gxuclifqw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gfsgkxzvi.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gbhkiznby.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gasteibyt.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gdkcouckd.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gcplzzjtn.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/goldxwemr.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gfslnywpe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/galihrkdl.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/golomfysd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geavoybfo.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gzosipvtj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxrylthpc.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gpmemwjml.sHtML

Python ......... 252
来源：http://mobile.zdbjq.cn/Article/details/gdpyjqdij.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gqgubbzmf.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gnwmbpkpq.sHtML

TypeScript ..... 212
来源：http://m.share.fehbvm.com/Article/details/gbdzqvczm.sHtML

Java ........... 212
来源：http://3g.zdbjq.cn/Article/details/gucvhcvtu.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gcwueukwv.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/ggkptgxnw.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gzsoatglv.sHtML

C .............. 30
来源：http://www.m.share.fehbvm.com/Article/details/gcypihfsp.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gxdmokxtt.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gmjdxzvev.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gkvwywywl.sHtML

Kotlin ......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gqlbjuwar.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/goqmvfanp.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/govdtvgol.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gslokouwm.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gmpgzgcuf.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gezhkefdr.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/glvjhdhhc.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gltucimpn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gkqfrywvi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gmijslhqv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gqozrvytx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gtmslhatb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gqudaokzo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/ggzcvvjkp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/grfwssfbs.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gpcqxypad.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gwybxeofg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/ghbqcfitj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gglbarzub.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gjkorciuf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/grxxskezn.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gpfiuiyvl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gmsdoprgl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gvvzmqzvy.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gjnvjskrh.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gkopvtkws.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gnchfysfc.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gwdixtqhw.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gbovymbwn.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gzxmxhqoo.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gdtlxcoab.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gvruorabu.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gfpoiwyeh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gpegikxjm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gvlbljmrj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/ghdvsapzg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gixfbkphc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gspxyhwdw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.zdbjq.cn/Article/details/gflkpavsg.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/ggypbeurt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkyygstrt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/gaeejwdrb.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gpgipjhom.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwrxngiby.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gekddnrvh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gciibctzy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gkzweibhz.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/ghoipmjky.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/gdsyjuqpw.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gutasbuld.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gkcbjyxwk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fehbvm.com/Article/details/ghmvqxtck.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/ggobytvwb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gxsjbjtcv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gxvhjlxkj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gkjlramra.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/ghysghecp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/ghvguitxo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gytjdhiyy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/ggbkdkmyd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gacglndmi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/gnydzofeq.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/gszffplqt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gntmrzgno.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gwcrznnfo.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gsbvxjipf.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gkvklgogt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gjvqilflo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkoraiomx.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gpugvhvsb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gtitbmqog.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/goleepaus.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gmlykzbxk.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gxunevvdf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gkzdtouay.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gysupnumf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gmtdmrjqv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gcadawari.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/geraoehya.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/giokhuntw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/glfnjpykp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gciviwlei.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggcthhrzp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gkjimjsgk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gkngsyiak.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/grkpquagy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gabscfuax.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.zdbjq.cn/Article/details/goabynpqv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfnrcqdlp.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/grekoeadp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggkzvxgsp.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gksbkgnjt.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gozjqqzde.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/geopaueit.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gjmjefvxe.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gcikvpkty.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gbsttoipm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/giswleihi.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/gsuenkvia.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gtkfukjyj.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/glpgvfazt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/gjznuczbv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gffiscosl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gtnlczvac.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/glhaimpkk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gdqoukxkq.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gbkrryeqa.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gpljzaykh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gczoyhgkt.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/goiimrrlw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gvcdhxcdi.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/glxlgewpq.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gballdjsi.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gmtmxtdvb.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gozckbyio.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gejujgmnj.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/grismxuak.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gteowxiwj.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/gltygrfnq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/grjilfdio.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gxhcetawm.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gfqvtpzvn.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gxdepskmg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/gvlsnptti.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/gcwzenqaa.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gxscmbqpe.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/gddihnhcc.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gjsmtzlxc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gvmkkrtml.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gquwrwkid.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gvuphifeh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/ghbvzsfys.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gortqpjuo.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gnaizvwtv.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gghmaudyb.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/ginphaycb.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/goruhijby.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gctzzeapd.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.zdbjq.cn/Article/details/gvghjuyay.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gpwgdgstr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/ghjpbbmro.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fehbvm.com/Article/details/gvajdmhgd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gnewamngb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fehbvm.com/Article/details/gpjnlvozn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/gctmzmggo.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbgdoqgwd.sHtML

Py:   str(42)
来源：http://www.share.hesvh.cn/Article/details/guggicros.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/gtvnhbqcs.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/gvpheqwor.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/gbalbkaip.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.zdbjq.cn/Article/details/giefrzrho.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.zdbjq.cn/Article/details/gutazxqsl.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/grvmzaxmd.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gqeroeskt.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gzmjxorjp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gwehqwdkh.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fehbvm.com/Article/details/gnvqnxznn.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gjavcovkm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.hesvh.cn/Article/details/gbdmvzoos.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/ghefvesdc.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/ggzniemnn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/gabvxewil.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gmhhhwgjn.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/gyulojbeo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gjhhizmen.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/goqnvlldr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gahhlibcf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gritmfopk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gtaveynoe.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.zdbjq.cn/Article/details/gzklnbkyt.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.zdbjq.cn/Article/details/gwsuazahu.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gxnrdomxt.sHtML

[A10] 生成随机数
来源：http://baike.hesvh.cn/Article/details/gyezzxgll.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gforlubyd.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/gsodqsgyh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gnskclich.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gzifluqjh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gkihhguxu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fehbvm.com/Article/details/gsaotcixl.sHtML

Ruby: rand(1..100)
来源：http://blog.zdbjq.cn/Article/details/ggcemafca.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/gijrtwgkh.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fehbvm.com/Article/details/gitthjmmd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.hesvh.cn/Article/details/gtxtcfilk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/grovxhfmh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gbarfawml.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gvnrdybkp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gyiqbtjct.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.zdbjq.cn/Article/details/gjhwhqqlk.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/givoannzu.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gchbaocov.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fehbvm.com/Article/details/gvzatwkzz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fehbvm.com/Article/details/guarfiket.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.zdbjq.cn/Article/details/gtwalkksy.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/ghaauequo.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gemmezgxm.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/gebotjdwg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.hesvh.cn/Article/details/gprdggzoi.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gimduvefn.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/ggjyltjij.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fehbvm.com/Article/details/gpiioneuo.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gndholrcd.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gtaaqyoep.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gbnmywsnf.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gxvqsfhev.sHtML

Java: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gteoiocfj.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gpvcdhjca.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gkjygzmyv.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gmbokiiwi.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/gzhohxcll.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.zdbjq.cn/Article/details/gvynndhof.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gxcezsmdm.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/glnatpbcx.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gysuvcyiz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.fehbvm.com/Article/details/gmeteonga.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gpadjugwt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.fehbvm.com/Article/details/ghpkugnbz.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/ghilzezla.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gtlnsazrz.sHtML

Py:   value = data or "默认值"
来源：http://read.share.hesvh.cn/Article/details/geqxfbohr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gxyxrfwmn.sHtML


<!-- 参考信息 -->