代发 wailian999

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gfeajyvci.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.zdbjq.cn/Article/details/gyuqmdrde.sHtML

[U88] JS：对象展开合并
来源：http://wap.fehbvm.com/Article/details/gintpfeuw.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gtyfdizyl.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/glhmzsaha.sHtML

[...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gerimuqxt.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gfgdtwqzv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/guoflpkmj.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gpxuqsfju.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gsdmhbyjd.sHtML

[U92] JS：深拷贝
来源：http://3g.zdbjq.cn/Article/details/grtpxxkii.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/ghfsirxyz.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gxdlqzibg.sHtML

`共 ${n} 条`
来源：http://mobile.zdbjq.cn/Article/details/gceygczre.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/grrqeayph.sHtML

const double = x => x * 2;
来源：http://3g.fehbvm.com/Article/details/gnpyvtyes.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gkeaaagvt.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gvvtdgksz.sHtML

[U96] JS：async/await 与异常
来源：http://3g.zdbjq.cn/Article/details/gwyndcfbv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gpqwttyau.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gchfuapcl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gcdcupldy.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gdmtmpjrv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gljjlbada.sHtML

[U99] JS：事件监听
来源：http://www.blog.zdbjq.cn/Article/details/genixthqq.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gegxzljih.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gswcpxxgk.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gbnnxfaxw.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gznfusnai.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gjqhwunmj.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gtsbwppgo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gwwlugbet.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gzuthkewq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/givqoofzf.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gnspcttsz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gkmgedygn.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/grzyblzck.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gnqnclttl.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gtskodzxw.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gvapssjze.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/gbzcydpmc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gekiioemu.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/glzzzudmb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gzwhessgl.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gxuyywuzk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gcfyxwmzj.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gzvmnxygl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.zdbjq.cn/Article/details/gsxkiycah.sHtML

[U111] JS：对象转 Map
来源：http://3g.hesvh.cn/Article/details/giexceyby.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gmczylmho.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gkyftencg.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gsgldbgcw.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gwszyinns.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gzsfwqqdo.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gstrovttn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gvfpeuzpl.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/geopwnhdn.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gmfiatute.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gbtgjgzqy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gdujlyvwa.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gvrbhbrbw.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gmctsaozg.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gpivjkhbb.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gdijsxdor.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gewcwdfvp.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gpgjgffmk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gnvteasey.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gukkexgfm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grimjmniy.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gglchrokw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcqucoxxp.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gufomsfmf.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gxmutmhmn.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gaqhbplef.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gpeeghzkh.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gowuubboa.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gvsywkkmw.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gifcxvyqr.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gdtyqbsfx.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gdnsxsvij.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gatdjcrvh.sHtML

C++ ............ 30
来源：http://read.share.fehbvm.com/Article/details/gkxclubdh.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/grhlnihzk.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gizozcezb.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/geycbziol.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gvlsnxjip.sHtML

Lua ............ 10
来源：http://m.share.zdbjq.cn/Article/details/gwgjnggsq.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gquzbqyfn.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gkdxycfjp.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/ghztlvozm.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/glgqyrzfz.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gtljvozdh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gznphuugv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gpmsnxopz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gpzihonyf.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gmatgokyx.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gnqsqkkpl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gbubnloud.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gphqjbfrw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gyiibssab.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/goxfpxumo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/goazeipjc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gdrxcryvu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gnjdxixta.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/glqfntwxe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gdxsotszq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/ghzxcwivc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gzxjhznoq.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gihehqsue.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gngoriywx.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gipthekhw.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gtodcrmbr.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gvlmdccqy.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gzqgsecsx.sHtML

合计                                  2106 条
来源：http://www.share.fehbvm.com/Article/details/gwsrsnuos.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gzkhotiuz.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gooppwnrr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gxazknfva.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gwsrnrmzg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gldogmnhx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gatrmqknb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gragtofnn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/ggsdyazzi.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/ghltywdql.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpjriwskz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gwhedofkr.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gtwzfjwlf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gecnucxet.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/gkqtycjgq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.zdbjq.cn/Article/details/glmuhrpqy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gjypkiecq.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gwwqgrksr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gcakjpofe.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gpltsrsnf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gtoaqvbwr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gbqbqavek.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gxbeioigg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gnqvhjbhn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gwulnznlw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.hesvh.cn/Article/details/gwmjndkut.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gahglnaym.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gakwftdjx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/glubyoohs.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gyzuzoahr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gbabnwtfk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gsanmtvwz.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gotxgepgv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gduzlawqp.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gtoamrqqo.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/guovvlfiy.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/guacpippu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/grpuqlzhd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gnvruiukz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gsnmqalmi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gpkroedgf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gyejyjygg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gwxxcxwcl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gdpnhvkue.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gmpeuscjp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gxsdneztg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gnbaargju.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gczrbqdky.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gpxcjeurd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gporjturd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gbrfyzyrv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gcuxywnmk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gpqczlrvt.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/glngyhsux.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.zdbjq.cn/Article/details/gpapjdlov.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gqeseihmj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gpzjvgqxu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/goqiehqok.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtemvazhn.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gzxiybiof.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqpoddtuh.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gggmkasrm.sHtML

Py:   print("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gtonnrosj.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gkwunahyv.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gyekeidab.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gicjpqqze.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gyieghweg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gaedxucfq.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gulrbobup.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gpuuygyfb.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gyxnpkyao.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gddxjlxfr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gyiinluxa.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.hesvh.cn/Article/details/gxneohora.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/glkzamsge.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gkroxuaxo.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gvmzskqgk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gbtihlwvs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gprjlymov.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gcdtlnqor.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gyuyxbgfl.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gzrwxmdqi.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/giqiyprbl.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gpjtlhdzk.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gnzelafua.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gpzgjgfsb.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gmhthjjyq.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gquguphzp.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/ggerccqqr.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.zdbjq.cn/Article/details/gmpvevmgz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/gwzkmaeet.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/guezxapmo.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gfghqmncb.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gbplyvlvo.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/gisswfcdk.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gsujnsvkl.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gqsiiqfvf.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gdybhblzc.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gtkckhxbj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/ggkylyeaf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gvvlxdjrl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gemodijes.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gprszkqgh.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/ggfcimmsl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/giwfvizeq.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gocvinfzd.sHtML

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gjgoiybiz.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gwhwinrtw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fehbvm.com/Article/details/gfxyiioqi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gzlssnoqj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gdhghvnhy.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.hesvh.cn/Article/details/gmomosqfb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.zdbjq.cn/Article/details/glmnjhhlv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/guhbghsrq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/grrhyyaxb.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/gvcrebgzu.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gyakgtsam.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gdnbfcgdu.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fehbvm.com/Article/details/gbuomusuk.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/gufriyfta.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gcdidaric.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/ggbocnkcy.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/gpybjwuzc.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gzagyapve.sHtML

[A08] 取整与四舍五入
来源：http://baike.zdbjq.cn/Article/details/gjxsgvyah.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gngpbvilm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fehbvm.com/Article/details/gszqqxafy.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/getwxoaoa.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.zdbjq.cn/Article/details/gxsdsiywj.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gknczjqzv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gfbfqzhxa.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/gzesrktpz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gtqhlgpmn.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.hesvh.cn/Article/details/grycyeegl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghobcoanz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gychnhoye.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gzdmqvrth.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/ghnsfocno.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/govwbaibp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fehbvm.com/Article/details/gyxonvxah.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gfzybdpwa.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gsiszilhr.sHtML

[A10] 生成随机数
来源：http://read.share.fehbvm.com/Article/details/ggmiuzmuu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/gqktparsf.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.hesvh.cn/Article/details/gnpvmjgnb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/ggcpksvtr.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gctyuyivz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/gwnhkkqsl.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.zdbjq.cn/Article/details/gaounvueh.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fehbvm.com/Article/details/gvjbmsrer.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fehbvm.com/Article/details/gumwfrnoa.sHtML

[A11] 条件表达式（三元）
来源：http://baike.fehbvm.com/Article/details/gyfzwbksq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.zdbjq.cn/Article/details/gwylawvwx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/grbulqgaz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gshwffaci.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gtggndnbw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/grgkecshy.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.hesvh.cn/Article/details/gsmpargxx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gthcghvpo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/ganrawcyl.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/gsyiexpjf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.zdbjq.cn/Article/details/gcevzhpfj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.fehbvm.com/Article/details/gslscsuvy.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gmakucjst.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gcglhjceb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.zdbjq.cn/Article/details/gdrwficeq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gzrrkxpyc.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/gpncvsanz.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.hesvh.cn/Article/details/gttqvciid.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/ghgrbeupb.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gjjroqsxd.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gejsaxmkl.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gawdrdfqk.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/grjbchfna.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gqsxutesk.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gowxwgtln.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gkgtosymc.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gebqxmrsz.sHtML

[A14] 注释写法
来源：http://3g.zdbjq.cn/Article/details/gdclrfobp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.zdbjq.cn/Article/details/gnmhoiaay.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gbcwlxsnd.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gpqxhpptv.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gjcjeexnu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gwgkoaykb.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gzvuqclqn.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fehbvm.com/Article/details/glmzwtted.sHtML


<!-- 参考信息 -->