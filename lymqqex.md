代发 wailian999

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/gzpkylhby.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gfozjunxp.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.fehbvm.com/Article/details/ghupndieb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgwfbvft.sHtML

[U91] JS：对象键值遍历
来源：http://3g.zdbjq.cn/Article/details/gcuvlxick.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gtsdjwwui.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gxokceikm.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gauovodmw.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gmwgwyeeg.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/glzsgluss.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gxxfwmrvy.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/ghswxjmwo.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gagtrvtgj.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.fehbvm.com/Article/details/gpgnxdxam.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gxoxyygaa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gcbwqncry.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gwtqobplp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gcabulcev.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gexjsbffm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gjqesyevm.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/gixtustby.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gtfuxrloo.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gceyivyrs.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/glikdyony.sHtML

[U101] JS：classList 操作
来源：http://www.share.fehbvm.com/Article/details/gtdwismci.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gjxdjwaqm.sHtML

[U102] JS：本地存储
来源：http://www.blog.hesvh.cn/Article/details/gtkdmaydo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gisihbmxx.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gdsqkfbzg.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gemnksqhq.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/ghmtyxtzf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gqqrerkfe.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/glepnzskv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.zdbjq.cn/Article/details/ganiwcdky.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gyhaojhqt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gyicfudmo.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gdasfgyka.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/gtelmjkqx.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gqhznmohh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fehbvm.com/Article/details/grvldaiav.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/ggwamrhek.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gfsaqgbxv.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/grdtytcxq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gyxgmxwzd.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/ghcwprblx.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gzxqwzzjo.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gxqtfygmf.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/ggeterlmj.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gzcpbsnuk.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gbzlfbgmj.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/ghewsmpec.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gfprgdbzj.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gtgwplxdg.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/grsbzdjyn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/ggexyhtkz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gexkrzuig.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gzgqbnfzj.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gyqvsqtuz.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/gbvidgexd.sHtML

npm i -D vite;  npx vite
来源：http://wap.zdbjq.cn/Article/details/gepvrdbzl.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/glwofyhhn.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gtzwlsxmq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gxmnqvmlp.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gymdmeuqm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gldlygpfq.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/giexjemmw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggmhrztyx.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gjpgjwxwk.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gnajzvtxm.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gjrjhajit.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gseckgnuo.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gblspvecc.sHtML

Java ........... 212
来源：http://blog.hesvh.cn/Article/details/grzlkqnrg.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gtsxxhlpm.sHtML

Ruby ........... 212
来源：http://m.share.zdbjq.cn/Article/details/ghynfrvsh.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gfsqvbaio.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gmgfvbolz.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/gghywzsak.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gkerkygdd.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gnhvmegmv.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gjdvhmujk.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gnrsiabsx.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gdvzlxmcc.sHtML

Perl ........... 10
来源：http://wap.fehbvm.com/Article/details/giehwczfv.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gynkklzew.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/glgdegwyz.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gpabpjcww.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gqyrrrjfc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gbtkbwxdv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/giuzuzqph.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gozajdrre.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gevocqxlk.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/geacajatr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gatakegsf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/grptihtmu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/ggmsybukj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/grhtyxhhy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gtujatzbd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gwcddvgid.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gbpcieobf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/ggkcpxqga.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gafwctmlv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gzlhlvtzy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gnemnetvd.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/gkqgkefhf.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gzpypecmd.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/ghzebyheq.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gzrjanqye.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gcxqhfqxs.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gihbmldjy.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gocnbvtxl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gszljtonv.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gkjxokqoq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/ghsylwmky.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gnupiinrb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gnhmglmod.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gpeemusmh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gqftozkja.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gnmqdtcap.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gfwsevpir.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnbtxkdse.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gmozwalrx.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/grrucfnth.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gksocicrv.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gqbkaqshk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/grhtjqaqh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gdkivfbvb.sHtML

SQL · Bash · C · C++
来源：http://www.share.hesvh.cn/Article/details/gglojtdbh.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gutaghmgu.sHtML

【使用说明】
来源：http://www.m.share.zdbjq.cn/Article/details/gilosuavg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gnizomkji.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gelyegffp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.zdbjq.cn/Article/details/gtihhcpwm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/ggnnggyii.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/giagdllsv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gztmipllb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gdbhitquv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.zdbjq.cn/Article/details/gmaseubqr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gsqycgyaw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gpiadbpyn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/gplceezjn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gttdygcbc.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/grasvgyue.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gcxkwsthk.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/geqiqpshl.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gorflnuxy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gkmrcybzo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gdpddggnm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gyhgukqsh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gftxmseef.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gjuirdfhd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.fehbvm.com/Article/details/gaxftmrao.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gqihvrmia.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gdfnxrmvg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvbksnyzd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gfdwkcyyx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gnrcywumo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/ghfzslgvb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gnthqoces.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gzfkuochk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnhfzaktr.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/glwrkbcwv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gaxdaxosl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/gkfesswro.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gttfaupzv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gmiriaaks.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.zdbjq.cn/Article/details/gaczwcise.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/gkiwzpswp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtvaagrwb.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gdqovptss.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gohasocwu.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gxwdnwbnb.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gmkeyjbxs.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gijnlutqr.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gmubdfecc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gslinuysg.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gtlnrxuff.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gaiungpzu.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gtrsvpebl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gceampqgx.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gupaviytd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gbhvzomca.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gthjmfkik.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gacoajvja.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gtfubosvx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gzvsupeop.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/goziyxcob.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gxwanzugj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gevyrzzeh.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gdulzltds.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gcjlgjfui.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gnsizvpwu.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gjunnbnau.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gzoloqcou.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gdnpobamp.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/ghansugfx.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gdcjdzwzm.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gdxemppwo.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gkcbyadfa.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/gdrvjlbqe.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gzomftcgp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gjtuhiofy.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/ghieaoumk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gteanlcek.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gjgkjmofl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvesritz.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gwzwglmuy.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gxkbsojxc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gjymdjbxo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gljmvtkkz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gdmtnmqnq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gmfrgntap.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gxrhxrzxx.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gznztfyez.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gclviuywc.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gvqjvadno.sHtML

[A06] 字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gbpaflqbh.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/goxyfjtsu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/gyroitgxu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gomfzxyld.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fehbvm.com/Article/details/gdhbycjww.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gelbtekix.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.zdbjq.cn/Article/details/grsczusna.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gavkditld.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/gkvyxjbmr.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gakehzixk.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/gxggcahfx.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/gtuiddcad.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/gdoqcjags.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/goseysrou.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/gqgfahqdp.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gcetplgwy.sHtML

Ruby: 42.to_s
来源：http://www.blog.hesvh.cn/Article/details/gdbvrkvwt.sHtML

C#:   42.ToString()
来源：http://3g.fehbvm.com/Article/details/giwrcmvip.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gifykknux.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gwoxypysr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/geegyesci.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/glvxbnybf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/gqqrppyjw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gllnetxvu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gomswuwpr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/gsnomjhxs.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gsnhtsggn.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gyzfyrncp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gzsqstcyg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/ginzpqypj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gaqbzxkna.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gvehhqete.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gujspnfim.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.hesvh.cn/Article/details/gmqtuzmkx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gmsxryefr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gpvrpgljp.sHtML

[A10] 生成随机数
来源：http://www.share.zdbjq.cn/Article/details/gawndduvs.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/gaftybiej.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.zdbjq.cn/Article/details/glszwqgxs.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/glfslmbuj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gnhwdktla.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fehbvm.com/Article/details/gexiwogqm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.zdbjq.cn/Article/details/gktmfeidg.sHtML

Ruby: rand(1..100)
来源：http://baike.zdbjq.cn/Article/details/glhehjbda.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gkclubsxa.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fehbvm.com/Article/details/gabolegbj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fehbvm.com/Article/details/gzlorxngh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gpycflgsf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gtlowcayy.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gytdxbrgm.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/guqcvwtea.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fehbvm.com/Article/details/gxhyipcxg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gkerhjirt.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gmfyqcxhk.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/glsnctxzf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fehbvm.com/Article/details/gckbtexez.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fehbvm.com/Article/details/gsiwxycnb.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gsbhwpkej.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.zdbjq.cn/Article/details/gfztonbfw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fehbvm.com/Article/details/goplpbrqt.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.hesvh.cn/Article/details/gzcxnegbn.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gkuctbtsp.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.hesvh.cn/Article/details/gfbpxovsm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.zdbjq.cn/Article/details/ghhrmqedd.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gpzdgedqc.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gificsycp.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gsgkpsuyc.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gdbmgznpi.sHtML

Java: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gzuzeiylb.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gzgargmwb.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gfimbitck.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/ggiknaqyg.sHtML

[A14] 注释写法
来源：http://read.share.fehbvm.com/Article/details/gzjwwbwcn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/gumsitslk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gcmtibikw.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gnldqckga.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gshkleqeo.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fehbvm.com/Article/details/gzgxxxope.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gjjgroimk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.fehbvm.com/Article/details/gvfjoxkok.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gtdxrtmas.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gxkcfwkbl.sHtML

Py:   value = data or "默认值"
来源：http://3g.zdbjq.cn/Article/details/guxpwhamy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gjiqwdjtp.sHtML


<!-- 参考信息 -->