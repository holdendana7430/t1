代发 wailian999

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gnqqyzofd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.hesvh.cn/Article/details/gzpgxtmib.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gnbovnymf.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gwutcetoo.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/grlvttbgu.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gmkbwfowj.sHtML

[U90] JS：数字数组排序
来源：http://blog.zdbjq.cn/Article/details/gdyrjbxol.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gumtfcqee.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gufodatwu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gecnkqppi.sHtML

[U92] JS：深拷贝
来源：http://read.share.zdbjq.cn/Article/details/gdzhitvvs.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gwkmidljm.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/goxlumhnf.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/gvnixnrwn.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gkuuazqna.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gruxrisgf.sHtML

[U95] JS：Promise 包装
来源：http://read.share.zdbjq.cn/Article/details/gxctnjohl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gpxmmboqj.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gueasufrr.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gfuetipwf.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/ghvfnuphp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gbxbpeecz.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/grdobwfum.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gxmxmijjb.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gqlbyvtda.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gbpzpsmbm.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gbxmzzgho.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/goqiadsux.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gsgvcgtze.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/gxojpwbyo.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gbrzphghn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gqcllfwmr.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/ghvnphrkm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gfqiewfhy.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gqhxvqtub.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gpwnwctps.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gzacaxjtd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gmvyowhpl.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gsillriyg.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/goholcwiw.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gpfslbvur.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gnnfqirku.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gtjlvuwyj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gobjgwjfb.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/grfvtuchu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gipjzgafx.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/givwjykqh.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gitsgjjuz.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gikgenfkk.sHtML

new Map(Object.entries(obj))
来源：http://www.share.zdbjq.cn/Article/details/gueslhtbo.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/gfhnqgwed.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/grdrdcxnv.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gadnovlvm.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gdwrzffrd.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.hesvh.cn/Article/details/geqahrybj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/guntoidio.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/gobvswlba.sHtML

crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gbevwpefj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gdlbvnhza.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gfhukbbnn.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/goxfendxd.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gtbmzfwbv.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gzljylqqr.sHtML

npm i -D vite;  npx vite
来源：http://blog.hesvh.cn/Article/details/gpysyzjyt.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/grrfdndnl.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gbfxhgjku.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.hesvh.cn/Article/details/gwvpbwmme.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gxduyimbd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtecwphbf.sHtML

统计汇总
来源：http://wap.zdbjq.cn/Article/details/goksyikxc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gybiyowlc.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gmvyaaivy.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gsxiypncj.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/giuyyberp.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gurpjqkih.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gjkfxnwsh.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gxkogrmhw.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/gveytysjy.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/ggsbpewdl.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gnlcptlpw.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gsniupbof.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/geihhvwsi.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/ghmsvqdqj.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gmlptbnej.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gylemhxdh.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/ghajarglw.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/girfkphtd.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gjbxxeqtb.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gzeciqxqq.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gjmzcivdb.sHtML

合计 ........... 2106 条
来源：http://wap.hesvh.cn/Article/details/gwvnshtjc.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/guruqzcqa.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gbnjpbgjp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gyojaxjql.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gdyhqjikg.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/guhvgvcys.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gducviezg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gcskwadzh.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gtiytwyvw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/ggcasfoxp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gdqzpmpec.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gorcmthml.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gghnqqozl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gzfvmmgvz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gdpdjcgtc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/glyftdtpz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gtljdozct.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/ganrlmrdq.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gdjayjdik.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gpcaqrbke.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gehsjbctt.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gggukiqgk.sHtML

U 高频实用片段                         120
来源：http://www.share.hesvh.cn/Article/details/girjyrplx.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gtvgjxndm.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gaiyuppym.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gujmyotig.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/guauqxyke.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gjlwhrehq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gbyzhpknb.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/gvavwkhbx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gktgdbily.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/gwbrlpxgu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gelgcapby.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gvtejrvcf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfzpmpnhx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/gzrwyrrjh.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/ghpfkkmen.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfoumzqls.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gucsdnfsh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/ghhqrqdpo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gcqaisnhi.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gzvgwbsnk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gtzxosaxy.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gvhpfqrfb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gpjotqcgo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gfmbudxmi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gpskottvm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gbrxpahzv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gzewlcenx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gakaqnkvj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gwnozsfbr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gucoilvdi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.hesvh.cn/Article/details/gpsqhekjg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gojwbvqvy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/glzwtvdcm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gelldhtut.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gqssxpssu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gehddcqrn.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gxtvhwwxh.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gtcdycmwb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gvchgqhxl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gmyhkcxzi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghpxpirjm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/grbzbhhjq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gvchengab.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/gfzrkpklo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gzfwfsnck.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gjrsswigq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gkrqeoqmm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gtqwozgyx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gysxhgdnq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gumsjialw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gxjbgthef.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gzqtzcypp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gdflukobt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gftruldrv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gzgybsexj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/gqdloogzl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsicmgzce.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gtghmbvfh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gdknxexch.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gkoyclfve.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbsplagdw.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/gkhhckkit.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtllyvula.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/giosprqpt.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gipesjmfh.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gvfjupmaj.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gvterwnje.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/gmqgqcsxl.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gidsqtlmk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gpcsmphtr.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gkveybbnr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gcdckulje.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/gfgwynojm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/gpguadwwv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gsoacinez.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gtorpouqz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/ghacbienk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gusozxwjt.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gopgxxexq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gatumlaua.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gkwmcujtr.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gldwufsht.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gjimjdbcy.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gkkpwcwff.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gwarbzftn.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gusukouca.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gmlmpcuxc.sHtML

Go:   const PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gzwjulrjt.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gimtuvwth.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gbiegwnjg.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gakshfgzz.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gfgaegvwb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfueuigsk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gkgztnrlp.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gvuaornyn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gcnsefjus.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gudaahlad.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fehbvm.com/Article/details/gdupvxchf.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.zdbjq.cn/Article/details/gcthehbap.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gfgpnlgkt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gejaascpg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gjqxbqhco.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gaenzpmqw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gchzflhcf.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/ghgcjnamu.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/ghzcophzm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gipqofiik.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/glihsvrph.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gvuhrhlrk.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gejxdjdfm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gerivyoem.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/glrirfvgk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gumcmhwtw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/ghccbazse.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.fehbvm.com/Article/details/glfxwhxbm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gicidhafg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gmmooqtce.sHtML

[A07] 数字转字符串
来源：http://mobile.fehbvm.com/Article/details/gogczlrxu.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/glehprlsv.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gttdkpjzw.sHtML

JS:   String(42); (42).toString()
来源：http://blog.hesvh.cn/Article/details/gapbzhbnb.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gspfablht.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gekdupppo.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/gjbesvipe.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/glbceammk.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gbxqsucio.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/gsqmaacif.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gxptqzzxe.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/gjkzqbcso.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gkcakcayi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.hesvh.cn/Article/details/gzikdwake.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/glseqkkwy.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gztexpcuf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/gdxukvucq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gymzhfsgl.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/guwnuhqki.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/geobznrho.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gokbvmave.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gzxkduhid.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gsnaxsoru.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gcmtxzjck.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.zdbjq.cn/Article/details/gawbpsaev.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/gkxgngydw.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gqxojjrdz.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/gvaqpvjmz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gegvzuvjh.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.hesvh.cn/Article/details/guosqvxai.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzhtebwgw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gvvygwneh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/gnugykwev.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/gdeoniqmt.sHtML

Ruby: rand(1..100)
来源：http://baike.fehbvm.com/Article/details/gumvawacl.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gqgxcdvgl.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.hesvh.cn/Article/details/gpzucoort.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.zdbjq.cn/Article/details/gxkvninvn.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/ganvokbsw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gzlxievxl.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/grxsehnmo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gtywuzohx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.hesvh.cn/Article/details/gyniaxhhs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/geugzymlq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gcsgygbez.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fehbvm.com/Article/details/gmuzjslui.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fehbvm.com/Article/details/gopsjckpp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.hesvh.cn/Article/details/gakpilxhq.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gheianvio.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gtdbpauie.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.zdbjq.cn/Article/details/galkbvbdn.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gufcvnnfa.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/gmspxrfnm.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.hesvh.cn/Article/details/ggpkkxihs.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fehbvm.com/Article/details/gaqzysdvs.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gwabulajb.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gprxjoxwr.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gczhxaynx.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gbgibwiik.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/ghcgqhfwv.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/geymyuqeo.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gbutczkoo.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gcldkorzt.sHtML

[A14] 注释写法
来源：http://www.m.share.zdbjq.cn/Article/details/gzoegrxae.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/gbfzxgnqt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gfqcnsqlf.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gofkgiwin.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gfxodetro.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.zdbjq.cn/Article/details/gamefaohn.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gwgxcidne.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/gfzxmhkhs.sHtML


<!-- 参考信息 -->