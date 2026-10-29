代发 wailian999

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gtbviovlj.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gxbksuutm.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gzmppcvic.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gzdzgvgil.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/glmmjekxt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gzcwdhvvc.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/goyzdphga.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gazcdmwaj.sHtML

[U89] JS：数组去重
来源：http://wap.zdbjq.cn/Article/details/gbpukmkur.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gipvkckon.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gcyepyyda.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gsmexecqi.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gwqmzrjfn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gjxdngadc.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gomkgnqxa.sHtML

structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gckydboyl.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/godymckul.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gddjxlfub.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/guydbdvfs.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gzakfgboi.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gscaybnam.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gjviuvqsf.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/ghuwowxyk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gbynwiovw.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gwbthvzdg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gizjklxif.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.zdbjq.cn/Article/details/gefllrgyv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gtpewotmx.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/gsmzoqayx.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gkjzuycsf.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gddltiybm.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gpoeyxqrx.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/ggfibukzp.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gncmdpwcu.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gqbnklnvp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gbksinros.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gwtnbnahi.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.zdbjq.cn/Article/details/gnrcscawd.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gyvmwyjbv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.hesvh.cn/Article/details/gqjzdcqxk.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gfyywkvpu.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/ghfpkmuee.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gijsvjrqi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gadzzkndy.sHtML

[U107] JS：数字千分位
来源：http://baike.fehbvm.com/Article/details/gfodydtlt.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gcpkmtbjc.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gcverceeh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/glcgrdzff.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gjmxvryov.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/glqivwcel.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/gawtiafaj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gybzzxdfv.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/gwjawygop.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gqkshrplz.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gxytxswab.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gxjevoubt.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gbfraubcn.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gzurzxexb.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gcvllnccr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gbjnybfjn.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gvtongoqh.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gvijzpsax.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/guvpwybff.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gghjnxsog.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gfqntqmsp.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.zdbjq.cn/Article/details/geoheqfgv.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/ggshrjtms.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gsnsssedb.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gcuxplzxm.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gtlwrpnyy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gyvafnsja.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gkxrkqqnn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbasrrvxt.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/guvvytswh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpxtyhmia.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/giekkdqvn.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gmwzqklwg.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gbdcyxduq.sHtML

JavaScript ..... 252
来源：http://wap.zdbjq.cn/Article/details/gpalwyqum.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gnwelikef.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gvdembldq.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gimjluzuf.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gslekgxhg.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/ggjzxjqov.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gzifxpcem.sHtML

C++ ............ 30
来源：http://www.blog.zdbjq.cn/Article/details/gnfnwublp.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/goquxdglo.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/gwjzinged.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/ggmowuvtr.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gtaratpdf.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/glaqhhkji.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gnspsvcmn.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/gbjpfiakj.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gkxooyqps.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gxwutkhnf.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gtbxioquz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gagzbeilj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gaubrgdri.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gqjftkxem.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/guuuzxzih.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gvvuhraaq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gmuaqxhos.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gjkqxgqfw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fehbvm.com/Article/details/gixihzmnv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gfcvlkqks.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gvogomhji.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gaakpxcbe.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gpbjgorut.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/ghrbzvrnt.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gdmctruwg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gdomxdrwh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/grpiyxxfy.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/govkzrchx.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/grmxqided.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gnbtoybcl.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gdpndrdsn.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gwsygckrk.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gjksmnbgy.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gcedmnjpo.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gybzwonaw.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/gkyzynchb.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/geytspxvm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gjapnnhtj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gpspbnigp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.zdbjq.cn/Article/details/gytzqxjlt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gmflfhlxx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/ggbsybedo.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/glxpgoopw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnhhhkmse.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gbtcrzsra.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gcgobbzvt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfskgpuyu.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/geaafexco.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gqowubmbi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/glbctchwm.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/giekgjasx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gihlckgzz.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/ghgpdksmo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gavntcagw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/goauhlmpi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.fehbvm.com/Article/details/gzxeoqnck.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gxrcmbdni.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.zdbjq.cn/Article/details/gyizeqdnw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/goolzgwca.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/gqwtraqzl.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gkzqmtdtd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gtblrmzaa.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gihtutlxv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gmvhpqeyt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.zdbjq.cn/Article/details/glvgnhkyd.sHtML

【文件统计】
来源：http://www.m.share.hesvh.cn/Article/details/gthjrgnfr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/giucdtjok.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gjbcaddfl.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gclxnthdz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gxnjsnlnm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gdmhivymb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gpisgqwuw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/ghgtllecj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gpzddgpsu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gidmoxudm.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gyvuaarkj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gyjiivcut.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gqxuahjqq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gbxzemjtx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gjvqhxsod.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/goqopxbed.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gktftclju.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gjcbsqewd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gnuwhhcck.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gvgnawcuz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/govlzciza.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gsufaxkit.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gwdughroi.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnpqcbgqg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/goalsftio.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gzmbmzgyt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glgifmxid.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gzcqjkosa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gacmvwnnb.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/gspmarlhe.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gberzkrol.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gttzluxje.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/ggamatflf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/gfxpnupjm.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gyabdcmfc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/giycvtlag.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/ggjphawkr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gqstxwodz.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gqrhtxdbp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/gvcwapmat.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gptkehoom.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gvekmkkko.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/gzhwsdhzo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gestulvyb.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/gvxvgasgo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.zdbjq.cn/Article/details/gkpjmuccs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gzthuwcev.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/gsljvsrfb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gmvkhgszh.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gbtiorgnp.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gkgevqjmt.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gulkyzbar.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gdljfnwwy.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/grpihugno.sHtML

Ruby: PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gqrcsptgk.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gjlbekbla.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gwqkeeeii.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/govtkehea.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gunaabfdp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/giirnufvu.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gtmezvfjh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gwviqqkxr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/gvyilgiav.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.fehbvm.com/Article/details/gkwqhshvu.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/gzlvsnxcc.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gbvlzbwil.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/gilgopxhq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gqswsvgev.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gkxhfnapo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/ghjvfwzuq.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gvgdmfnro.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gbfrththk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gpirjugow.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/ghtgubine.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/glbwtydmv.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/grfcxlpwn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gixhluxrn.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gvcgastuy.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gtmkcbezj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/glnxlbegf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/goajireya.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.hesvh.cn/Article/details/gulufstxc.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fehbvm.com/Article/details/gygvuuyal.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gbluvdrvr.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gjllvlmqo.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/ghkbpumdx.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gbgpwnxtm.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/gbnnvammv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.hesvh.cn/Article/details/ggkonuqef.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gyzxsttqr.sHtML

Ruby: 42.to_s
来源：http://read.share.hesvh.cn/Article/details/gcqkrfyfg.sHtML

C#:   42.ToString()
来源：http://m.share.fehbvm.com/Article/details/gulayfarb.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/ghdqsifhw.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gmaqndxpl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/gqbgzqnqx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/ghqfwsuvq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.hesvh.cn/Article/details/gnxuhgwlw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gvzazlwzs.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gcyvxyysc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/gzfzkakgk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gxpzzvqgj.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.hesvh.cn/Article/details/gdhauuyxw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gynwjlrol.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/ggchcduav.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/ghsksekwx.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghnnzsysj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gixiaeoau.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/gdywbqlku.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fehbvm.com/Article/details/guthlojgi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gknlhlebx.sHtML

[A10] 生成随机数
来源：http://mobile.zdbjq.cn/Article/details/gbdkipunh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/gnmwwnjeq.sHtML

PHP:  random_int(1, 100);
来源：http://wap.hesvh.cn/Article/details/gujwnaits.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gujyulivu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gjxsgjhgi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gahevkoeh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.zdbjq.cn/Article/details/ghzdmgftt.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gpqsggghd.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/gfebwptqu.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/gmijnutvk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gtmkhdrof.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gyymkdvch.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gqojporzl.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gzngiwssg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/ganuotcfa.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fehbvm.com/Article/details/gflygovxi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gtkmljdpn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gccqhtjbp.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/gkusevuka.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/gzbbdonxw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.zdbjq.cn/Article/details/glpdbyhrz.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gztefuabz.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/grsmlzzkc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.hesvh.cn/Article/details/gnojuztln.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.hesvh.cn/Article/details/gcmouqbtp.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gmepudgsf.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/gprvnauho.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fehbvm.com/Article/details/gfzibezeo.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gtmnsrhjg.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gftworhmr.sHtML

JS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gzjuawgog.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gccaerizj.sHtML

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gndmdrijq.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gydpzzwgk.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gcrlydxjb.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gxkcwcaiq.sHtML

[A14] 注释写法
来源：http://wap.hesvh.cn/Article/details/gnejgnrun.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/geufupsdm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gaolanvkl.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gdqcojlrm.sHtML


<!-- 参考信息 -->