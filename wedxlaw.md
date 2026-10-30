代发 wailian999

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gpwpojkdm.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gxtaaiwiy.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gisnleghf.sHtML

a ?? b
来源：http://baike.fehbvm.com/Article/details/gclgmtsge.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gkosftvhh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gvskyvvlp.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gmdqtuyzk.sHtML

{ ...a, ...b }
来源：http://read.share.zdbjq.cn/Article/details/gcnjllqii.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/gsghpltdl.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gtezsmdub.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gqvzqutmi.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gxgufkcbb.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/ghazkafdm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gvgnsxodu.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gotxdvroh.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghaaesopg.sHtML

[U93] JS：模板字符串
来源：http://baike.zdbjq.cn/Article/details/gfdrvibtc.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gjnjwasgl.sHtML

[U94] JS：箭头函数
来源：http://wap.fehbvm.com/Article/details/gqngkquky.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gmtexvnqu.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gwzlikyhd.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gyhasdlcr.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gnuhuggxa.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gkretaiim.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/gsqjujewu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gtrflbqmw.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gomwuaefz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gfjgwftvg.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gfxkocvuh.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gdzsvixjy.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gwpgzixgw.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gaochinra.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gzirnmzrv.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gesffelpp.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/ggraknjer.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/gmhadcnml.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gepbzrrbs.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/ggelpcviu.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gjsoffbtw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gtgrytcxx.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gecgfjmgm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gyzudobia.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/giyrdojpd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gpehagqmo.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/glkgjtarq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gfuvepemj.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gpepjaxnl.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gdshckxsp.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gucpcwuie.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gerxohhay.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gkdcxhwyq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gvltsnrap.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gmgddxrrr.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/goacqzdnf.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gikldngtu.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gqompxkop.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gctknxygg.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gdypgmoye.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/ggwfexynu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gsdkoiamq.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gzbunsjjn.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gpkmbcvff.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gtxelzhme.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gatameims.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gbltfztmr.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/ghkcvrwto.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gskutdskg.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/glopahfon.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gkpyxwwcs.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gktepynta.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gjtyhxgce.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fehbvm.com/Article/details/gnoyadyah.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqlmyqfmf.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/grrahgasv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfiqqhrtq.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gxkvjeyzm.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gpidlyhqp.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/giwjbamed.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gnuuzkeoq.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gonkukgfr.sHtML

Java ........... 212
来源：http://baike.zdbjq.cn/Article/details/gwzeciytr.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gcsuvnvce.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gblyadtbg.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gpvwogoxj.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/giwfalfoy.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gvavxetkd.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gyrtabjdq.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gjtbpgysv.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/glzguzjqz.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/glaqkquiq.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gqjseqqbl.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gjmezxrkh.sHtML

Scala .......... 10
来源：http://mobile.fehbvm.com/Article/details/ghxhwnjgm.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gfnehvauz.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/garcuvsxc.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gmwzpuqyu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gvtfharhb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gxcbwjjho.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gvgjvgzik.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gibsgdufa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gfephychl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gxmlomsqz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/goshnpeyt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gxaokmtno.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gxbdkwznb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/grpykkbmo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/glsreiuwc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gqppngxuq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gkivwusdd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gdpbdtpkb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gozrffmbo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gglkxbvxf.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gggpcqrql.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/gicnwjiht.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gthwoksws.sHtML

T 其他语言补充                          60
来源：http://read.share.fehbvm.com/Article/details/ghmanuxvv.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gfxpzoxxo.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/ghjitpjhw.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/ghjiexrkc.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gxpdlvjog.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gbkwmreqp.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gxxsmymco.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.hesvh.cn/Article/details/gpxvoflmj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gqjaezifo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gfrcbbxhr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gvrywwymq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gffmmxcxo.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/guktxrnfv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gypfcproi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.hesvh.cn/Article/details/gvoehgkvp.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gcjavqmda.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcuyqpjij.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gdcnyepzv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gcsrsvfyt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gtqjxpybb.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gdjwvxycx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gcpchigwk.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/geiwtkexg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gqhbzizto.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gkieyoujo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gqxdpxcmk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gwvsjocjx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/glozvgowl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gswfxbnnp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gniguqfcc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gkwfpjbzs.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/ggedhjpij.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/giicqslok.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/ggslzummt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gercahgiy.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gqjjqtgll.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gbjtbvwoj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gwevzeurl.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gaokjsoan.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gehisnufl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gwsovpbns.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gxkgyhutg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gejvwcaxk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gnatheysc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gsykjyisf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gfnjkxhio.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gplnvdjbo.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gjhprdimr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gpmpbiyun.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gbefhtlaj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/glzxgznbt.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gecavnrhk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gjjdcnqeo.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmkotnews.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/grdqcicln.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gqqngzljm.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gkruuofha.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gisxbkder.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gzsfnozto.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gabrfjyma.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gwiofsfef.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtjkrgzxd.sHtML

A. 基础语法与类型
来源：http://www.m.share.hesvh.cn/Article/details/gjymlesjn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gezsfcbzr.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gopwrphts.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gudeukyuc.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gwdzwwitj.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gscdttdau.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/giuyanaml.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gcmlwofhd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gydmhtgms.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/gzomapxqm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/ginolxnhu.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gokxmmcyn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gppvcuthf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/grdqgkbxy.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gdmzntvyb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gkvstvkcg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/guvfwpvmp.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/glegtqoup.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fehbvm.com/Article/details/gvwpirsza.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gmfgfajxi.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/grflidksb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/ggmmepygt.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gkpjomkhm.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gekcbioxs.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gdlmpnril.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ggmgdcpaw.sHtML

Go:   const PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gypxcsxov.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/ggvumqkwi.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gdhrmqsnb.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/ghazfeqvw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/gdflryddx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.fehbvm.com/Article/details/gjlfbkxpj.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gixduohqj.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gykurshyj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/gxopmtwyi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gwbuqilzt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.hesvh.cn/Article/details/ghljxfsrf.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gvqaocqgr.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gtffpgjim.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gkmjtogim.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gzewslfnr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gfyyalyln.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/goxreycao.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gkbdrahpn.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gzqntvyek.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gzbigregw.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gbzyrrwox.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gorbglfnw.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/ginoqitwe.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gxxwmvnyg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gshofzbxu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gobffeibw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gyagoqiki.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/gepomvehg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.zdbjq.cn/Article/details/gmikwdenl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gnotqekgb.sHtML

[A07] 数字转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gfsvtulqs.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gwupzndau.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.hesvh.cn/Article/details/gzrhqdsfw.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/guxvqessq.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/gmrfuaqcy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/gbksybach.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gbazeaaic.sHtML

Ruby: 42.to_s
来源：http://read.share.hesvh.cn/Article/details/ghjijwsln.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/ggqbrjqlm.sHtML

[A08] 取整与四舍五入
来源：http://www.share.zdbjq.cn/Article/details/gzakpmdgo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gsbdfizqu.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.hesvh.cn/Article/details/gtnojcqei.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gcfkzupku.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.zdbjq.cn/Article/details/glvqumbhm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/ggktzbpaa.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/giozztdmr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/gpioctwlr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gvmjzropw.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gaqpdjskt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gbzjhpxwu.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gethaqzaa.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gwqqwbhgr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gzhtcmsvk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gconyoded.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.hesvh.cn/Article/details/grmryqruz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.fehbvm.com/Article/details/gacmooqny.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gumjltzfc.sHtML

[A10] 生成随机数
来源：http://mobile.hesvh.cn/Article/details/gdstbmmbl.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/ghzujscsb.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/gtsgehnjk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gglluazsh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gfssmfwua.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fehbvm.com/Article/details/gfroopdjl.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/gcnuztdyq.sHtML

Ruby: rand(1..100)
来源：http://m.share.fehbvm.com/Article/details/gbksbxnti.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.zdbjq.cn/Article/details/gvosztlur.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.fehbvm.com/Article/details/gxlwxdgyx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fehbvm.com/Article/details/grrwvcpgu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/ggasoysku.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/geymvcmvp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/grjncczsf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gjsxhfgkf.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/gfkhdmnqb.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/giqdgoljl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gqxonowhw.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/gvpxhuqzh.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fehbvm.com/Article/details/gxponiswo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.zdbjq.cn/Article/details/ghkqmkbmv.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gfzkujzwr.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gmwtjhnyh.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/guwzyjcia.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.zdbjq.cn/Article/details/glhazpqdc.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.hesvh.cn/Article/details/gqccxtcrm.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.fehbvm.com/Article/details/geeofxzfp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.hesvh.cn/Article/details/gyxbjulhz.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/geumquzwr.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/givdcohnh.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gilgnxlgi.sHtML

TS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gwocewwvi.sHtML

Java: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/givuduvpp.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gepxpzxvx.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gwgwxaojy.sHtML

C#:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gicvdnsjx.sHtML

[A14] 注释写法
来源：http://read.share.fehbvm.com/Article/details/grsiyqkyt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/gufcfugju.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gabwwfsbu.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/ghwcfstdm.sHtML


<!-- 参考信息 -->