代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gwvlsbkum.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gffzhnpon.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gtkzwbqxd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gmnwzvtxq.sHtML

[U85] JS：可选链
来源：http://m.share.zdbjq.cn/Article/details/gwslevdmm.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gcflctfvx.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/gqnzmagti.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gwjfjxjhb.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gtyachqrj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/grvljifzk.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gjsjdoxfg.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gfwezrpbt.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/gwjcslzwt.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gnlimeabd.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/ghqwjlnmh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gtkcssssy.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gncgsoakj.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gbrelkrrh.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gajzhkrel.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gqttrtmia.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/glwzkshkc.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/gudmaubiz.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/girifqitj.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gcucovoxg.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gianglgut.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/ghfwgnkmm.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gibujkxkv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/govvdmrlh.sHtML

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gkfbhwgim.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/grumvxaet.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gyryswaah.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gvhbhprlb.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gisvkgwcs.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gshrddunf.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gnjcslpzx.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/godxdkypm.sHtML

[U101] JS：classList 操作
来源：http://read.share.fehbvm.com/Article/details/gnbghjqgg.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gmldwgkee.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gtvzvzhff.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gjtbbmwwd.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gchepaekd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gadzbperc.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/glybfadwh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gscrfzkuq.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/geeymyrsw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gtkgfeqym.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gsxmgfkor.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/ggamutdzp.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gajdmnwmb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gtynkxngw.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gsjmtvrzk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fehbvm.com/Article/details/gfdrmgscg.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gjzvbqmux.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gfsbveycp.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gwyplmkij.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gxrbbyxou.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gsykiafkk.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/goqvevsju.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/goxgwnhyf.sHtML

"7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gionydvzi.sHtML

[U113] JS：正则替换全部
来源：http://baike.zdbjq.cn/Article/details/ghzrpgtvp.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gsmpdmlgl.sHtML

[U114] JS：JSON 深比较
来源：http://3g.zdbjq.cn/Article/details/gpuyfpzga.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gdferssim.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gianmrkgc.sHtML

crypto.randomUUID()
来源：http://mobile.zdbjq.cn/Article/details/gpwmwoyhe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gozbgqcpy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gyojpssxl.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/grlutwlcl.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gvdsfmxnc.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/guhpkcyti.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gpljwsolz.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/gjpeewevx.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gtnxqqtrs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gxiykzesx.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/geyisflsx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcgttuaey.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/gfeftjxjw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnfezqsay.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/gmzewlbao.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/glbnhwyop.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gqmopuklv.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gbyvjlnes.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gatpojlrq.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gpkrxwlll.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gkwseobln.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gqmeacjqo.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gkjvaoemh.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gncczdbdw.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gxnxlghzc.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gznzbheaw.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gjdidriau.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gtvjvwzjv.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gjbvzrlsr.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/guqjzkisl.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gbevmfaeb.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gylbpotth.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gwqapfyjd.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gjhatdvkh.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gsscailcx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gcyiakhbg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gtaqlzewi.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gfmxepnkw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gyymtzttr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/givkgvevp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gbojcoffp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gcyhtgsms.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/genxtlxgq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gbrlfnkmq.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gfiofroiq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gwtwzqmfq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gjvswcggm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gadkiwyom.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gapjbgmjp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gtngwxrjw.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gkxlrlsek.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gbuorzmjx.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/ggzafeamc.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/ggmuimdxi.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gtjzksybz.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gwcwrekit.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gpmtedsej.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/gqjlvngzl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gwxrlsrgh.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gmrypsudf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gfhwjqqvu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/griogwsyy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gdxqbjslc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gogopsqxa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gdgjcwluf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gwxebztlp.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gxpzfdify.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyownpbqt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gdyudvyfx.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gppywbaxc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gccbliuno.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gxarldbwz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gnkrfijkw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/guegnebfn.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/givxwrjsx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/giblbdxav.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gvcyhlsed.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/giciugazk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/galxuepmk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gzguqrfqf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gzsmesfay.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gtrzgzdkm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/grfreyinx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gzspkxgjy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gvhooekbm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.zdbjq.cn/Article/details/gzxejidwt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gxpqwhuoq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/ggvqpzpgl.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gqmnelyel.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gnfxhyljb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/ggvpveuqz.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gllkntubu.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gzmxemarw.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gwwupgobo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gkgvvoebb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gxxrhezme.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gfewreyjg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/goafqbeeg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/ganyvrhar.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gxhfxefhv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gcuxfbcpj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gcfabxgxo.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gznjrbifo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gkmiufavl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/geimalwfv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/ghswwchyw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/guydxveie.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.hesvh.cn/Article/details/gilcaawiu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggxdiqhfe.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gopdwaqsz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gxkjbbogz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/geadoqfrj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gvwhcxlsz.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gqlwhrxii.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/ggwawzwms.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gffhbtqgd.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/gwwpvusgc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpeqagfts.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gbjsgrswg.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gpgcstfhm.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gyuokhepk.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gyflvvtnw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gqowjdeeo.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gxbntskvt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gmfjrcadl.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gprfkedpx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/ggxlhgsth.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gfkrxlupu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/genuovzza.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gyqkeeuqq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gbyljwsfn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/gpljqtlmn.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gxkfylbyu.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/greruarfx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/geegvcusk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/ggcxuinln.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/ghffwxobr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/gnvtinnhp.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gzsqaeouj.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/glnyoicgd.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/grynlcebk.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gottgiiha.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gbcfqgtzm.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gkjpoabex.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/ghpucvgaj.sHtML

[A04] 判断变量类型
来源：http://www.blog.fehbvm.com/Article/details/gyjpethii.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gmiquybnf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gnjhyrorl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/grtfoeghz.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gdvrjhqri.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gxamiyxgj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/gyomqztya.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/gxdxqjtyl.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/ggtjqcyuw.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gdmvtswsw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gvvthtcvs.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gbxqkrinq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gopncwjsz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gccndrtyw.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gtajaetvr.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gytncjbso.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/girkcyvpo.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gjjtvatzj.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gqioboazs.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/gdzyxygnm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.zdbjq.cn/Article/details/gcybbiutl.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/goopkhfwn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gtzsjfmbq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.zdbjq.cn/Article/details/gksscvxhp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gkqnmstjt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.zdbjq.cn/Article/details/gzlppanhf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.zdbjq.cn/Article/details/ghnmktwoq.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gkzlwkith.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/guvihlpkb.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/gyzymvqap.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/ghusqqbcj.sHtML

TS:   String(42)
来源：http://mobile.zdbjq.cn/Article/details/gvnamndns.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gwebgltlo.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.zdbjq.cn/Article/details/gubcgutpa.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/ggplwqckl.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gaivtrhuh.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/ggiglmgvc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/govqtmbpk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.hesvh.cn/Article/details/ghjfzlnlt.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gurtgdjgd.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/gqboigdho.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gcunexvvb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gdldiouto.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/gwntzaefs.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/glebzoyxc.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fehbvm.com/Article/details/grxyzpgyn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gqzovpaja.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gxngqyktw.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gthipsfsf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gfwpwgalw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gmpawgwri.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fehbvm.com/Article/details/gsttkvukw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/gagdlofda.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gywjjmhmf.sHtML

[A10] 生成随机数
来源：http://m.share.hesvh.cn/Article/details/gxmotqxsr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/gnrlgousm.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/gqpyebxfb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gtimebwzi.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/guebzmzot.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gcfyojpuc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/gvwnvcuny.sHtML

Ruby: rand(1..100)
来源：http://baike.fehbvm.com/Article/details/gaqvkdree.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.zdbjq.cn/Article/details/gxfqqtgjj.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/gpttpspsz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fehbvm.com/Article/details/gpctjptvu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/grxxgoumo.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gvfmlarvb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gaaziwgds.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gkibvcped.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/gaismfctd.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gzfldmpke.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gbfhkjlre.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fehbvm.com/Article/details/gavrfrxrr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.fehbvm.com/Article/details/gbcvadltk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/gclhfimvn.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gfmetsxnk.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/ggrarjpct.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.zdbjq.cn/Article/details/gvaovibrd.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fehbvm.com/Article/details/gtsftvpjy.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/givmugldw.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fehbvm.com/Article/details/gbcvsgone.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fehbvm.com/Article/details/gigvhuahm.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gaicyciqp.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gmxwchony.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gxyzhynmo.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gpokjfjgd.sHtML

Java: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gomxydkks.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gtkyhogoa.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gghdkaahs.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/ggaurdwlq.sHtML


<!-- 参考信息 -->