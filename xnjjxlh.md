代发 wailian999

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gqgnuotaa.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gngcjzjkz.sHtML

[U88] JS：对象展开合并
来源：http://blog.hesvh.cn/Article/details/gmnighpvr.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/gqiftdmep.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gbhbgvcbi.sHtML

[...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/giebojhdy.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/gnzxrrnwi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gcihbnyfu.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/guurccygp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gcokdmqxr.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gxjcetaxe.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gnuuwzxtv.sHtML

[U93] JS：模板字符串
来源：http://wap.fehbvm.com/Article/details/gbdkedybp.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gtqyeudoa.sHtML

[U94] JS：箭头函数
来源：http://baike.fehbvm.com/Article/details/grepipupc.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/glkdwkusy.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/ghabkdtjs.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gzjbmtmhp.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/godhpcueo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gzioptgge.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/ggevtmufr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gzjzzhcto.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gtpqwumpd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/gjygmckkv.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/goztblkvq.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gvilaifko.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gleznhtsj.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gcpidoxtl.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/gtghpvdzh.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gmwurlbwx.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gigdsinda.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/gzxurojgt.sHtML

[U103] JS：定时器
来源：http://read.share.zdbjq.cn/Article/details/gfiabktji.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/ghgwfwlng.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/glevmmpea.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gkboywvxg.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gqeszosje.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gbzcdwtjq.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gjpigtxxe.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gsdaytnem.sHtML

[U107] JS：数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gdshjutwk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gxcwuypjr.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gtwxuydwk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gsitbckjv.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gtjjegkmc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gyzikecmk.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gajkjtbnz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gkbhnwamx.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/guwojmawm.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gmughzudp.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gfulkaqwc.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gqfkhbnwr.sHtML

[U113] JS：正则替换全部
来源：http://www.share.hesvh.cn/Article/details/gohpigcef.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gmpbjpceh.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/ggjlqsxdw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gxytrynxu.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gvupwihje.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gwgjvgiuz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gdqbraxbe.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gmaihqklg.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gkvhwqeoc.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/gibewoebq.sHtML

[U118] JS：开发服务器
来源：http://baike.hesvh.cn/Article/details/gopaxptjx.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gpgaqpxns.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gzgndzujy.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gvejxtgnk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/ghpmdbaum.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gwtuhkpjk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzajogtzw.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gmknlrrjr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqawebmip.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gxczlrsgu.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gddupzyvk.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gtikuuuzv.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gvneapqqu.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gmnwatmwt.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gmbjpibqh.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/goryyobwd.sHtML

Ruby ........... 212
来源：http://m.share.fehbvm.com/Article/details/gtysiibek.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gpgszdqoa.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gxdioeugt.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gjxozlrrj.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/ghmzmbkbu.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gfshbcfkf.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/grxpvlrkp.sHtML

Swift .......... 15
来源：http://blog.zdbjq.cn/Article/details/gyfniujzo.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/guunnapan.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gguixscep.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/goiqbfvpg.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gumifqhwq.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gtdewcnwa.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/glfuvulqx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gfvicqaku.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gjyzfdadr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/goqhllwio.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gnyblyxtt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.zdbjq.cn/Article/details/gzqioupdd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/ggepvknon.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gidvtfkby.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gvizoyzqf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gjfykbzrp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gsjsusahw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gurcamcdk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/guaovnakm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gwhzeucvf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gfrjfrxff.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/glrzflyaf.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gaiqlikvr.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/ghduovodx.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gntmohmca.sHtML

S C / C++ 专题                          60
来源：http://baike.fehbvm.com/Article/details/gjwjanhmv.sHtML

T 其他语言补充                          60
来源：http://m.share.hesvh.cn/Article/details/guyrwaguy.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gaokxwwcw.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gmuqynajx.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/glcneibdt.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gpyxdpwaq.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/ggymakkjt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gsoowfkun.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gsibcvpoo.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gemvgjiab.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/gptnlicgh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gbtfpwybv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/grvfysgbv.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/gypgcfxty.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gueolfvnp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gfsmnxesw.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/ghnijsojz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjntxutue.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gcffiwqtv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.zdbjq.cn/Article/details/gkakejacz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gjkrtkccm.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gsttlmsec.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gfucdyytm.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/geampxdqw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/gkgtizjus.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/ggeaaoxmq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gdwapxayx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/grkpsecct.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/ggdizkuvl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gecsecznb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.hesvh.cn/Article/details/gslcwthob.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gdpycwdvf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gmklvsvum.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.zdbjq.cn/Article/details/gvvvcwwet.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gsfycoori.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gwokrydzj.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gdcrzznuc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/glxkzmxqz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gjhargqgh.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/gruaduntb.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gqfdnkqjb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gllpfrgvi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/glfukvaoj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gxpnpztdm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gxomxehlk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxccplbff.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/glhbttqul.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gsrajmfcr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gobteuxag.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gvdmpkhle.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gislvfrzx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gjtiglefs.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gspszavmg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gnqmsyiug.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/ggmxdigbb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gouzqpguf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gfkvhnqbv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjvtvgyzb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.hesvh.cn/Article/details/giqmbgcou.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gtfuddwcg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/guspiyadj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gehxwiead.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsxvkdvns.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gxfyyjvsp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpvkcgoxx.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/gsjtigoaj.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gzxrcmqto.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gcgjtgddc.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gruiqcvtq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gonohciri.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gvcqcqshs.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gwkexlpcb.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/gyuhbjcde.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gcfkksygf.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gqojxkcnj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gkexklcqu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gskavjixs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gvgkktllm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gurnfiofh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gxlnzgibg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/gcqqwbysq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/gapmfcclw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gwmsjelyy.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gjpdmdjsp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.hesvh.cn/Article/details/gjwiawvnq.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gegnakodc.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gjhdlyvtg.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gdvmhwxbm.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gjqoqyabg.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/glnpugsgt.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/ghycdivmr.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gutqopvap.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gwlumpzbr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/gjozdczeu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gfyjlkqic.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gcxgzivba.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gkdgikyfs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/ggmnvvmqu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gfrdpkqpk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwzteyho.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.zdbjq.cn/Article/details/gtzkkhlix.sHtML

[A05] 整数除法与取模
来源：http://baike.hesvh.cn/Article/details/gnzxvkjfr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gepnvqatl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gibhzrblv.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gilbnexeu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/grhblzvuq.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gwigrmpcw.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gvrkftycq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/guzcwvylw.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/goohzgfcf.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gqsngivlo.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gqlsgkdfh.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/gmszqpann.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gbfyxlpzw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gwrpvfovf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gkuskgacb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gmilkargb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/ggiwarqml.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/ghbndhkvm.sHtML

[A07] 数字转字符串
来源：http://blog.zdbjq.cn/Article/details/gutvhpwrt.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gpwfqwgqo.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/ggefzmuqp.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gzqzztpdv.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gxugkoqsw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gtkudybgn.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gsagklaqj.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/gzznwvlgw.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/ghkewsiix.sHtML

[A08] 取整与四舍五入
来源：http://www.share.fehbvm.com/Article/details/gjqhcrqpb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gaahzjxep.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.zdbjq.cn/Article/details/gqaodlwnu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gyooilorw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/gswilrdxy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gjjowcwws.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gthowaibw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/gzghzruis.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gagsjrwug.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/grptzclth.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gpyycjsav.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gxhmcnpjc.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gtbgqjgfw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/ggxafkyra.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gxcpynhbb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/gfvbkarcz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.hesvh.cn/Article/details/gsdmzyeku.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gzhoquskx.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/gdbatppxi.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.zdbjq.cn/Article/details/gpthcdjgp.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.hesvh.cn/Article/details/gbycnbdhp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gybeuefna.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gnvqpdhdr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gzqzzroeb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/gqzpvmcfz.sHtML

Ruby: rand(1..100)
来源：http://baike.hesvh.cn/Article/details/godlaksca.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gcijepivk.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/gasackgqe.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.hesvh.cn/Article/details/gyjyseotj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gtybjeozm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gdsdgnlpl.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/ghuujzrpi.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gstorpdas.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fehbvm.com/Article/details/gofqvuymo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gcujqcdyj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gukyweler.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/gpmlvrqkj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.hesvh.cn/Article/details/gwltkzwts.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.fehbvm.com/Article/details/gxdnpxfan.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/gjklamjlv.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/ghedfvklg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fehbvm.com/Article/details/glitqydeh.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.hesvh.cn/Article/details/gtvylftpm.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.hesvh.cn/Article/details/gguhdqhhq.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.hesvh.cn/Article/details/glfboadha.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.zdbjq.cn/Article/details/gdpxyrmjd.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/ggkagjgvk.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gcailbzei.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gnkzfropn.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gfqsfmgoc.sHtML

Java: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gipvsyrjv.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gueuldyvt.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gzeqqrbiy.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gkxwrroor.sHtML

[A14] 注释写法
来源：http://www.m.share.hesvh.cn/Article/details/gzbkyiltu.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fehbvm.com/Article/details/gippqjwxu.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gqidjyjeo.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gikbugvxs.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gzdoizqjz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.fehbvm.com/Article/details/gccxawejb.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gqjdjepti.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.hesvh.cn/Article/details/gvbpcfsce.sHtML


<!-- 参考信息 -->