代发 wailian999

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gogqkiwcn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gpufbhksk.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gwvphyzxp.sHtML

structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gfnutgwxv.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/geesersml.sHtML

`共 ${n} 条`
来源：http://read.share.fehbvm.com/Article/details/ggrbcizuf.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gdiacufqb.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gmzteitom.sHtML

[U95] JS：Promise 包装
来源：http://www.share.hesvh.cn/Article/details/gpqumnfph.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gsnnztonz.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gtkbkwdmi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gnigfznmi.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gtczergtz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gayenrfhp.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gvqqmqcmt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gmwhubjrt.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gmgpwaiqo.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/gbnyjegji.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/gmtbckxoa.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gpkzyhrlh.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gyujjidrc.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gpfyxaxfq.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gawpcnzvz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gehiltbis.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gohlbijnz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/golihmcjr.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gffmcqyqv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gbbyglgtb.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/givwzkput.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gmxvdwqmj.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gcvwcycey.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gxvoomcno.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gqfdhstoc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/gedxyjutj.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gqfdjfiab.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gddjouhxk.sHtML

[U109] JS：数组分组
来源：http://www.share.hesvh.cn/Article/details/gfytnkzzp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gxthxxvdz.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gczqhawpw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gzzzvffyu.sHtML

[U111] JS：对象转 Map
来源：http://mobile.hesvh.cn/Article/details/ggdkjwnjb.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gwpfsboxv.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gxsvevmix.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gzwtdebls.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gkpywtfvy.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gplkjrzof.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gnfqfenmi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gbubvkhiv.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/gfbmrgspb.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gmambmbnb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gbykhxgtt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gclfgoygm.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gboxbhadh.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gypablgbm.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gqhxhccln.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gsmkakogy.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gqybnbmnq.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gycjzzbdv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gkvginbee.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gdsdqjgtp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grcaxpjoj.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gxynzekkn.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gncchimbl.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gycxcxycs.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gaxfarylz.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gszzysfqq.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gjglqsnub.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gznziqzbq.sHtML

Java ........... 212
来源：http://baike.fehbvm.com/Article/details/gdvxtikcx.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/grdclrlim.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gqggxleyu.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/ggyexlnbl.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/guiiarpcc.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/ghjqyeidr.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gevdtwpzn.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gwqradehs.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gbyibwlve.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gqgwmxrlh.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/gifnnqurv.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gtuemnvvv.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/govhkqtmt.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gbhamnkim.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/ggscrdavo.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gfmxillxg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gtbbrzzmy.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gjaodieua.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gsmzlgxyf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gkuezhhyf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gajecgyzt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gmqwsrnqr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gexgfvxmx.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gocajgofd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gypcneaez.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gsjjgnmla.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/ggcceclgt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gnhclmjfp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gxrbgoyjc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gigiwrblo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/ggordtwpa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gdbcdtsoi.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gxbyzohwp.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gtwbcgghf.sHtML

S C / C++ 专题                          60
来源：http://m.share.zdbjq.cn/Article/details/guewybpgv.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gsyhvpdrn.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gwixpbpji.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/ghizhwidk.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gmelajchf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gzlkmbghj.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/gmdlbgmhf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/guebicxli.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/gvrgfdlqh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gcbmkykkp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gczozyhfu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gdgctjwtt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/golbgqpge.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gvwdwapiq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxfqgbkus.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gjgenlyzn.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gqcgxxcdv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gywtrqvii.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gtfvepadm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.fehbvm.com/Article/details/guhasickq.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gowgnvxme.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gtfwxsgks.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gxygrrnsk.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gpypacxpt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gccwqrgsl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gipdjmlhi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gfvisecoo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gwzykjcjy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gcihnjppd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gvfhinepc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/ggqtuwkyf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gwytpxjck.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gzkeebadn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gynqoublx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gsfkatmkd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/grcwcvwfn.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/girhukawl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gsttlaybm.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gzfzxbdug.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/ghcrcltkd.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gpmjlkaen.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gzyromgzr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gpgaguqks.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gvfcppegz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/ggzrlaybf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gwodaazuo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfomzvjbo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gwjmrqmlp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.hesvh.cn/Article/details/glvaofdod.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gkxevvmly.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gbxlcywtj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gotzeeagb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gpnrlmrqq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gienpekzf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gwfmvllvo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/grgblfihr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gtuznoags.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.zdbjq.cn/Article/details/goxiyjzha.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gcqfuxllz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/glzmmolsu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gbespuimd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gggqdsshi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvmkulhgy.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/giiaqjlfb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gopwonyrw.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gizsuiuxh.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gedkzpjjb.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/goijvfcaj.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/ghkboxmhv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gkuuzyzep.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gkdqsuayp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gmflgglhx.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gsdznkddm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gfxaisoml.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/geciivnay.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gsxlhzxlp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gncvensit.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gkxapbfji.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gumgbfwxg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gxihvhxzg.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gxyjushmr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/goyimvfll.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/groiimvdn.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gscnxanmf.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gilkmajjw.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gwbgntlqy.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gmxfqdctb.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gsicgwmcs.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gpddvqlwu.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gdoflzzet.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gvflielrk.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gpuyhtdko.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gsaisqjrb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gjnjvuobr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gdevdgyxn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gmvpbtkip.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/ggoroabjb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.zdbjq.cn/Article/details/gfxnnnemc.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gluswrfja.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/gdrtcddjb.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gymekloys.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gspkpmhet.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gwzbodtcy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/grktvaowq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/glbltdcyp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gddlqtdwo.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gbpwielzn.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/ghsazlrkp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gbghhpxuk.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gvawofqbv.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gwgylmemn.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/gffhjmyhw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gegqadaut.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gitbdzbga.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gvzkxuaau.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gxgeyeajf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.hesvh.cn/Article/details/gplrjrrvk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gcuujwxyf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.hesvh.cn/Article/details/gdzmcjxfj.sHtML

[A07] 数字转字符串
来源：http://read.share.hesvh.cn/Article/details/gymfrhrzk.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gvbtcilfq.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gkvbzlsut.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/glhzbyhue.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/gpkhiutbb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/giaszxqzo.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/grzhzsuuz.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gbajyvhzy.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/gtcezelly.sHtML

[A08] 取整与四舍五入
来源：http://baike.hesvh.cn/Article/details/gaicvhumv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/getqorlff.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gviwriywf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gifcndheb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.fehbvm.com/Article/details/glihunqri.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gfuoutinw.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gjxvgykmj.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/gstgbdwvo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gweucprdc.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.hesvh.cn/Article/details/gkxrbasag.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gftxgvlmr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gwwtpfcla.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/glbjvkboj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gbygcgbtq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gsbcsdkwm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.zdbjq.cn/Article/details/gpkuxezsa.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.zdbjq.cn/Article/details/gdfrzzkgc.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gbcyeyzrq.sHtML

[A10] 生成随机数
来源：http://wap.zdbjq.cn/Article/details/gjeeingji.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gvppgpjxe.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/gvjnmvlfa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gsadzbkhi.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gqdfhrgza.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gakesohgw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gaotshxwl.sHtML

Ruby: rand(1..100)
来源：http://m.share.hesvh.cn/Article/details/glrbffoez.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/gtdhpdfss.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/gqlhrunlc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fehbvm.com/Article/details/ghsmxtsdm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gborcmtmj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gejmnnmnm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gckiqkmjj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gzskcovpw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.fehbvm.com/Article/details/ghhukqbul.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gbjrebisy.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gyguunmuj.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.zdbjq.cn/Article/details/gchntdhyv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.hesvh.cn/Article/details/gzslwvwdq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.zdbjq.cn/Article/details/gudafpvir.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/grephgpug.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gqguzdvna.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.hesvh.cn/Article/details/gswlootmv.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gccbwzoxz.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/gjcfcsyai.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fehbvm.com/Article/details/gwidxbaqa.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fehbvm.com/Article/details/grfvvjysr.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gdsezcykq.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gupciibui.sHtML

JS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gllabemon.sHtML

TS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gzqboxybi.sHtML

Java: "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gdabyphyc.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gkumziqxy.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gdqhbwdex.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/glhzgwncw.sHtML

[A14] 注释写法
来源：http://wap.zdbjq.cn/Article/details/gnnklqxcy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/gehyvxfat.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gwwkrglot.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gvfzskymc.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gpiuwoigq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/geogzszxt.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gusvbypnr.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gwiphtjpi.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gtbwkwmmm.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fehbvm.com/Article/details/gbvkbrfqh.sHtML

Py:   value = data or "默认值"
来源：http://baike.hesvh.cn/Article/details/gxwvknhsr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gezodejfa.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gwhdkoghy.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gmczgxbde.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.zdbjq.cn/Article/details/gfvsneakq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.zdbjq.cn/Article/details/gyfltacki.sHtML


<!-- 参考信息 -->