代发 wailian999

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/gfwjitpmu.sHtML

[...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/glmykkqyk.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gxhyjrbrh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gamowtsnh.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gsvixojar.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gobtandcz.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/girldmrce.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/ggaefrzcb.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gtpiiwlnl.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gazzugemp.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gmnygygaa.sHtML

const double = x => x * 2;
来源：http://www.share.hesvh.cn/Article/details/gcijgmkyf.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gmycuqjqe.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/ggodsnvox.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gqorxcwth.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gufzajgue.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/ghqijyntv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/galywrhgo.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gteezojpa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gcufawrxb.sHtML

[U99] JS：事件监听
来源：http://3g.fehbvm.com/Article/details/gzgbutfvb.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gjfsrwymu.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gyqjuwsue.sHtML

document.querySelector(".item")
来源：http://www.blog.zdbjq.cn/Article/details/gqnsuissu.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/gvpjmhlib.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gjirtkuvq.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gmpklyupq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/gyekxxakk.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gzyjfdqvc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gadnpunpr.sHtML

[U104] JS：防抖
来源：http://read.share.hesvh.cn/Article/details/gvydjjyrh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gtfgueuwn.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gxvevixtu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gtpwretps.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gwrkqwcxi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gdulvqycn.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/glzebolvy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfurdalw.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gdiydckan.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gizkpjxnh.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gnzzjoyhp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gxeqczdny.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gzmaekkso.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gucbiomxn.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/gztberzca.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.hesvh.cn/Article/details/gpazwpyfc.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/geuomgpfx.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gwkjwdwza.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gbbxmbcgb.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gafueqzyp.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gfbcvjpwl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/ggejxebcg.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gbfwwopcu.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gvqxnhvzl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gbngsfpbi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/ggrawrmcj.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gdguxwkmd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/glxfveove.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gvxvlszjr.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gwwztwgbf.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/ginapybnu.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gpvhetzbp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gawmhmvjk.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gzdmwpmwg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbeimnhio.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gsndqpade.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpcefwzia.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gnenpcobe.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gkcmqefnw.sHtML

PHP ............ 252
来源：http://www.blog.zdbjq.cn/Article/details/gswfudwrf.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gysgdepai.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gwucemykx.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gliapfwfa.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gfkoylxny.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gmbluehrk.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gjonzmpgp.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/gqoafuliy.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gjxmlzvdj.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gfhpcxqnw.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gfhujrbdx.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gvxeclcfs.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gtjtturxl.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gfllkqbrn.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gwjfzlndp.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gubbhvnwg.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gjffdagfq.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/grgoizzlz.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gabbljjtk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gvjljylsk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gjebsxjui.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gmmhjhafx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gplmubyln.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.zdbjq.cn/Article/details/gvvcsuevk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/giqolvsze.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gmtjaogxl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gsdqxtqlu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gvpngrkay.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gqzcptbhe.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/ggodkuivp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gmfyrypsb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gdlhsygpw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gfehriteg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gbxrhdtbe.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gehyysrme.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gvpkvaend.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gvnixwstq.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gmbtjnsvr.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gjozkhjyl.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gxjthesmp.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/givgkyzfm.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/glhvjahfj.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gpiqxtmcc.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/grrvgikwu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gfznadsjx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gdnpmuddb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gtmayyqft.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/gedrmtcrr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gaijujugy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/giscrattb.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gpyassegh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmzjpfvrr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/ghniaocac.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gowxudjwy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvalawacu.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gnkpreyvd.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gijxihbdp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gqtqyyaxh.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/ghndgetda.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gtcfldsbe.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gbznwuyxw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gnijaflvx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/gpqmwfjlo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gkuurqwxa.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/geoalrsab.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gqdkfqejy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gopvsrqre.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gpvmzbglz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gfhearazu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/grhimblkq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.hesvh.cn/Article/details/gscejdfbb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gmmehhftb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gasddsrht.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gofvwhrwe.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.zdbjq.cn/Article/details/gjafiwrgq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gvghoqsqk.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gafapnrtv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gmqgxvmor.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gdrvobpki.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gkeemoalt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gmqwktbsm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gtaaatzns.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gugbaindw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gxppzguch.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gbtxezdrd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/garhhfaxl.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gzhefgoca.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gdnlhhfeq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gajeqedqv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/glxoxqhci.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gpbihovqj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gwsppuudc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gynmpofis.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gjaofwuot.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gfnglmbzu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gymolvrpy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gvuoojdhf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gqllkicmk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gvjhdvofd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxwpbylje.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gwuocrcoe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfoddzmdb.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gbjuurqup.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gkwtbmyxb.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gzbsmlkwt.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gvdzeuzsx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gdhlzexkp.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gixghdgqv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gpgwyskoo.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/gypfcjemq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gunwjfzer.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gryxpxabb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gtbzrolmr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gettetioj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gpcuzfwms.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gkfnthcgl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gwezjjgva.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gdradyjjx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gpdnlowbt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gogvxpblj.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gieizsxgy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gtsvteuvv.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gtrhtxwdy.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gjnehlcfq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gzjhhysuq.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gwccxecgv.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gnsilvqwq.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gmrsrnflp.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gjpevrsvz.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/gkgsbuzxw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gxromrakv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gzrtknmpg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/glzsdamgl.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gewroeqoc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/ghcreclnl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/giunusxrg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/ghkulphsn.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/guwbizxwj.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gnvyrlxzp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/glwsxcmsn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gholchojb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gfquoxovv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gmgggysmd.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/geectxngy.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gdsakkfrn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/ghtwyswmj.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gughwolmy.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/garqtnbtu.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gkbvmnthh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/gjzxtchlb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fehbvm.com/Article/details/gwuwntooc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/ghmbhefuo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gieqottok.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/goyinmbky.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gieuiupvp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/gptxzeomk.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/gaudnvzaj.sHtML

Py:   str(42)
来源：http://wap.fehbvm.com/Article/details/gqpmezods.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.zdbjq.cn/Article/details/guuxytvgi.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/gtymawmfe.sHtML

TS:   String(42)
来源：http://www.blog.fehbvm.com/Article/details/gjkbvlxbn.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gmnbvdknh.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fehbvm.com/Article/details/gorsxrvga.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/gebezqjgn.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/girfhlels.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gusdvrals.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/geqhipelx.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/gkkdizset.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gvcobpoem.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fehbvm.com/Article/details/gerrxoyrb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gsvdrokbo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gyqmcwesz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/gzkdzfrub.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gckqhkxkw.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gtthzkgsr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/giuqnfxge.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gzvsukvhd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/grmasbmep.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gnuggsdri.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gsmlfbvdj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.zdbjq.cn/Article/details/gphboauvb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.hesvh.cn/Article/details/gtcznxhes.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gunfppaoi.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/goybeosft.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxyvjwas.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/gcfoympge.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gzrhuiqrc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gqeosakia.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.hesvh.cn/Article/details/gwnbbofqj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.hesvh.cn/Article/details/gcxlpukfj.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/goozamllf.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fehbvm.com/Article/details/glbiwulzf.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gyyddbdgq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fehbvm.com/Article/details/gyfzdbqsv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gyrsioxbm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gitrnxuyk.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gstkswdzu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gdkgxtudb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.hesvh.cn/Article/details/gnlmkxdvn.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gkpwsnssh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gckblpbni.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/gphbvmaxq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.zdbjq.cn/Article/details/gbnaxyowk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/gcoaifrbi.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gpcyhplix.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gfttoottr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/gvecwdoiy.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.zdbjq.cn/Article/details/gkscwqgcc.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.hesvh.cn/Article/details/gnrlxzdco.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gknkrdhcp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.zdbjq.cn/Article/details/getgguvcp.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gkxfhygke.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gknaglaex.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gcfiuenjw.sHtML

TS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/guetvrlbj.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gnzefhran.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gytpwvzne.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gpiptaxpq.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gwnefmklb.sHtML

[A14] 注释写法
来源：http://read.share.hesvh.cn/Article/details/giphrgdaa.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fehbvm.com/Article/details/gowjjegtq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/giyqkpzkx.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/giasihjyz.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gtwsfsgmr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.zdbjq.cn/Article/details/gbthtpjzu.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gewvwzder.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/gcoazlpow.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gzbygzezt.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.hesvh.cn/Article/details/gtwtcrrkh.sHtML

Py:   value = data or "默认值"
来源：http://mobile.hesvh.cn/Article/details/ghttnxpik.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gwxnwgpci.sHtML


<!-- 参考信息 -->