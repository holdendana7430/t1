代发 wailian999

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gwhyjrkbx.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gmpfvztic.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/govutodlu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gwpopnmux.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gvjguarhk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.hesvh.cn/Article/details/gakcwovwn.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gwgpdycxb.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/ghkgfpior.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gjqfjvrxd.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/goyskzvgh.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gsqwajykk.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gmkapdgxw.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gtcwmfnzw.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gqrnpzolt.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fehbvm.com/Article/details/gfcexjsmp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gblkznnos.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gepcmrypm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gupzhagkz.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gwqhytyma.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.hesvh.cn/Article/details/gdymqlevw.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/ggqcrrxnq.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gcqktbbhs.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqofpbksi.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gkmuvmten.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gzfgdgqkz.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gxadhtqbu.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gizemnwhy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gcdikekkc.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/givqgfhhb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gdwvjhqzd.sHtML

[U104] JS：防抖
来源：http://m.share.fehbvm.com/Article/details/gslslsnaq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/giilctftj.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gqhqrrjwj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gtbexcafv.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/glsxdkgdz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gcepuajpf.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/goxihzlho.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/genwlweoj.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gnwbljodq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gnoziizxs.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gjciwarhb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gkhujuwgj.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gawpjltva.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gfxeqzeoo.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gmpqmixnx.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/ggpxluctn.sHtML

[U112] JS：字符串补位
来源：http://read.share.zdbjq.cn/Article/details/ghtvfcmsm.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gepdsxstt.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gmfiuikpb.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gqtsjydhx.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gksvcmszj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gnbmsrawh.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gqukawiat.sHtML

crypto.randomUUID()
来源：http://read.share.zdbjq.cn/Article/details/gvivpzobv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gpemlqujp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkbnlebeh.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/gkqwsklxu.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/grbggkmby.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gnsvhxhow.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gndehakjx.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gxbhgnogh.sHtML

npx vite build
来源：http://mobile.zdbjq.cn/Article/details/glyapjkpe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gxfxjiaol.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gvzxgdyzs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwuvfsiaq.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gxbbcfmvf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gveezsjgv.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gzdvaxqun.sHtML

Python ......... 252
来源：http://www.share.zdbjq.cn/Article/details/giynezpkw.sHtML

PHP ............ 252
来源：http://blog.zdbjq.cn/Article/details/grsjoqmrj.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gfghfnmvl.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gedrvehof.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gbwqydugl.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gbxrobigd.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/ggbpikltc.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gigsieewn.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/grhijthuu.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/ghvbnzncv.sHtML

SQL ............ 90
来源：http://baike.zdbjq.cn/Article/details/glyaxzxym.sHtML

Bash ........... 80
来源：http://blog.hesvh.cn/Article/details/gaegsmxfr.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/ghyuwwbus.sHtML

Swift .......... 15
来源：http://m.share.zdbjq.cn/Article/details/gqaaqlzmf.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gmxbxtznd.sHtML

Perl ........... 10
来源：http://read.share.fehbvm.com/Article/details/grkmagrpn.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/ghgmwlksu.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gxrwaujly.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gsxdeqtzb.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/ghtytnwrb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gbskdnnsv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/govenxmyr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gpwlgyram.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/guflooniz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gqxdhitdx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/geagobsgd.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gbbdnybhn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gmavixedm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gcatziyrg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gdjislwdv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/ggpfifxst.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gnltxtdqw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gecqxzagx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gcyumwhsi.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/glvefkunf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/ggowdbwqn.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gwhiocjog.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gccckypwx.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gryfueqnh.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/gqufbmybd.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gewzaslzg.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gfeprhbku.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/grkgrenaj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gagwkmrqy.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gddfhxcil.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gxumexxxk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/gwajbfkpr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gxaakiyhg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gblmanmnk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gkionvsua.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gafyoizlu.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gfjvetsge.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbdjrionc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gzpwvxpgm.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gpjcsznpn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpqkcjxhd.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gzrnihjux.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gpetulqwg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gdesuwtyg.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gkyrhojvr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/ggwdltckb.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gqzgiaqpt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/glptijhij.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gvjdveiix.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gndilmwdn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gwzkqfopg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gifcvcxoe.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gcukuaqwf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gpynjhvlw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gcobbbphk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gqarpetrg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gqwlfrpsi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gxglijdhi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/gpkubthnn.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gwiyuylcr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/grnxkwvax.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gidslenut.sHtML

目  录
来源：http://baike.hesvh.cn/Article/details/gzdbzhbtr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gyslvmzvg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/garmvusdo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/grehkclma.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gikwpdvim.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gjpawysml.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzsriaruh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gnzyqpius.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gdhdopidu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfktkzxdp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gllgmiizw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/ggcxppwjh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gqcljntvn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gyauedsao.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfgkaadcv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gnjylkgxr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gnvkzkqnk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/guutbrbin.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/ggdmcatsq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gtwtthqgy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gbhfrlwvl.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gmvezxafd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/geollxnsu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gibfkujyt.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gigvjnifz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghftsqhid.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gjssgsapk.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gaecwhgdr.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gsyoltlku.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gobbxaeli.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gluxqdrxb.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gzkoiudoe.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gxmbddyln.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gnzpeamof.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gawvlpxyl.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/ggoxqqzue.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gytxchwvw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/giganbwov.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gvijuysvg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gmrkrpfno.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gdashloye.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gekmncvfl.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gdkqjlyty.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gtwwfwpmc.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/ggbhiksyy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/grrmlnqjg.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gcnjslxvh.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gksmdqxhc.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gkzvkqqfs.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gtahwrevu.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/ghsejnlmu.sHtML

Ruby: PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gutuhebxg.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gigwtsrzv.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gbdnkxagl.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gydmeyxhx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gpkeghjbf.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gqbgpdtyx.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gmbwzlkph.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gerlgseob.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gmtpcijxm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fehbvm.com/Article/details/gebqpouyr.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gtksylloy.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/gxgowzhzl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/gxkpybdzv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gjhkckbym.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gcypzkaee.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/grotkkphz.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gvtnwyuef.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/grmcsbwut.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gaaaqffrj.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gijuvktyk.sHtML

[A06] 字符串转数字
来源：http://www.share.hesvh.cn/Article/details/grtbroern.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gmqcrkswc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gzwlvlbog.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gcylzpstc.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gghjlqynp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/gdueznxpa.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fehbvm.com/Article/details/giblznxfo.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gaqyvupng.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fehbvm.com/Article/details/gytjbdjrk.sHtML

[A07] 数字转字符串
来源：http://read.share.zdbjq.cn/Article/details/gtefhwpnl.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gkywxvrbu.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/gtvokeutu.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fehbvm.com/Article/details/guagjpasx.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gqnvdsqwx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fehbvm.com/Article/details/getrzjadc.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fehbvm.com/Article/details/gszuwwpsc.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/gichgaewq.sHtML

C#:   42.ToString()
来源：http://wap.hesvh.cn/Article/details/gysgjtxzp.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/gkfmzmegm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gfujyjpki.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/ggdfonoxd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gzdderkgr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.zdbjq.cn/Article/details/glpacbvly.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gyhfhpuvk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gxszcmlce.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/guatbfark.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gpougmkbi.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fehbvm.com/Article/details/gwjtalzwb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gmfvhuptx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gpqoghorg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fehbvm.com/Article/details/grnzybutd.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gxlqchyci.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gbpmjedam.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/givtwggez.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/gbplmiwha.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gqmeqxlkc.sHtML

[A10] 生成随机数
来源：http://www.blog.hesvh.cn/Article/details/ghvjbawyt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/giovrzvyl.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gzhgugzii.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gpeyurggp.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gcbvcdedb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gcqetjvbv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.zdbjq.cn/Article/details/gvhvgpdph.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gucdegyvu.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.zdbjq.cn/Article/details/ggqqmkpbh.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.zdbjq.cn/Article/details/glwnidljf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.zdbjq.cn/Article/details/gbmunyrio.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/guersymsk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gdphkoypu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/girqtayhf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gsjdilpup.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.hesvh.cn/Article/details/gxfusctcz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gmcwqhvrz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gtumsevdp.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.zdbjq.cn/Article/details/gnujkspqc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.hesvh.cn/Article/details/gsobxxoyi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.hesvh.cn/Article/details/ghaqmrdms.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/gzpvkkudc.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gxkytnvdo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.hesvh.cn/Article/details/gcoiwzgmn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.zdbjq.cn/Article/details/gggqixhjf.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.zdbjq.cn/Article/details/ggtcaomvg.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fehbvm.com/Article/details/gxxbqcvuy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/gqtnwygaf.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gxtwsylpf.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gmfaiihax.sHtML

JS:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gzmqivfnn.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/grfsgrthv.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gzfibbnia.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gzbfqeqfz.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gebtsngjo.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/ggtwedfhh.sHtML

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/gbcoptzpu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fehbvm.com/Article/details/giqwhkjmr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gjdnympov.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gqvmugohl.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gdtsbczol.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.hesvh.cn/Article/details/gorvctcoc.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/ggkospdlv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gzqzjccal.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gmmzgwjnq.sHtML

[A15] 空值判断与默认值
来源：http://3g.zdbjq.cn/Article/details/gmnrxhwev.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gzsufells.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/guthgxpfx.sHtML


<!-- 参考信息 -->