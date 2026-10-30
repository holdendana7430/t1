代发 wailian999

[U87] JS：解构默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gstklgapx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gnpvwptre.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gtfxsmtia.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gjespfhhc.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gxugomkut.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gzmlyrpvh.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gzogesajl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/grgqgaeth.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gwsxagznv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gmzcqvhgl.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gwiityiex.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gnitbxyna.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gagjenehi.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gheeabtgz.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gajmuhfbl.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gqteuwqll.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gzaikgccj.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gubozvkgb.sHtML

[U96] JS：async/await 与异常
来源：http://baike.zdbjq.cn/Article/details/gelvmwgeo.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gnsuvvkit.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gjzribxtt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gpbiazqdi.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/grmxuaoxq.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gmyommywk.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gmmhwcdfi.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gvnkvqqia.sHtML

[U100] JS：DOM 查询
来源：http://blog.hesvh.cn/Article/details/gzmezrdyy.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gxhzfgelm.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gadxielkp.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gjlsbbvip.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gzxmencyn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gpbfvfoqf.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/glzlyhaiv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gsfnmzrmp.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/glyzwmfyu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gsrjgvptw.sHtML

[U105] JS：节流
来源：http://m.share.hesvh.cn/Article/details/gcbyfvrov.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/grkjjoylz.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gxwtekblh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gvalymuha.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gpidresfg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/ghdmkwhck.sHtML

[U108] JS：随机整数
来源：http://baike.fehbvm.com/Article/details/gnjnliyje.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/ghhulwywv.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gipfinulf.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gexokrswn.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gxswbxijg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gkbbjhjjs.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gmnadioca.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gckooerou.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gydwlsnqv.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gdqmmqbwg.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/geaxcnbfq.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gzcrxnrhy.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gnfkoqqos.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/ghtldrvgd.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gpazrsthp.sHtML

crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gwsyvkjwj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gvdozbqam.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gatpcsala.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gyuezphhx.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gjfijgchj.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/gltksymfo.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fehbvm.com/Article/details/gvysquarv.sHtML

[U119] JS：生产构建
来源：http://baike.hesvh.cn/Article/details/geshskqhn.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/ghagwodsi.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gqboljosm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gmiemofpg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnsjfdisl.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gbmndvcca.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcrlocley.sHtML

按语言统计（条）：
来源：http://www.blog.zdbjq.cn/Article/details/gegbbohxi.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/glgstvaat.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gaontyiyp.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gvsxckcrq.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gmkldkhxv.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/guoadvodo.sHtML

Go ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gdastdfcx.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gclpurvrd.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gyqkfsdep.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/ghsruuxli.sHtML

C++ ............ 30
来源：http://www.m.share.zdbjq.cn/Article/details/gkvxqzymh.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gnbyqiysv.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/geokgfjdr.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gqhlkfefc.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/givheahoa.sHtML

Lua ............ 10
来源：http://m.share.hesvh.cn/Article/details/goosowmje.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gwqgmsykl.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gbaciesni.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gkijzkwzu.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gwvrutvop.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gedrblgis.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gdavzjknx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gjhluvius.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gptnbmvrq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gllowceup.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gjbzxuckl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gwmoqihjx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gffcouywk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gkzqapmfq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gzhstshqw.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gyecpbons.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/glsnlkwcy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gnxobgcgp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gdvpzlaqe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gyanbjtta.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gfhdyhtgb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gghkplnng.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gpazmvzku.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/glxtnjdxf.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gejbufhph.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gvugkggnt.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gwtmvgbge.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/glrhatuym.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gsasebylm.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gzmultvvq.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gpfpibznr.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gptexkjrv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gcoqrular.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gwekxrtgb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.zdbjq.cn/Article/details/gxkrcdrmy.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gzhrcfamz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gxfgtircz.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gvlvixnsb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkeavuwzq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gblbwcwrw.sHtML

Common Programming Examples Cheat Book
来源：http://3g.zdbjq.cn/Article/details/gbgtryqsk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtezemaxr.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/ghnfnomgs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gnmnebmeo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/ggoriahpp.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gyhgfedtr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/ggryjjsgy.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gbweculsq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gohdeghju.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gantbvsok.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gtwhbepyj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/grysylivy.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.fehbvm.com/Article/details/gyciwocin.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gblspjukv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gqzviezon.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gtfjyhoem.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/ghatandea.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gwwgzvebj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/gdmxwcoka.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gvxipljqt.sHtML

【文件统计】
来源：http://www.m.share.zdbjq.cn/Article/details/giampwydm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/ggowtijoc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/glvthawxn.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gopblsolx.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gmwwmynnw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gjhzumdha.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gnrasunib.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/glucdsyke.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gehlwsdax.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gpxcscbbu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gggdhiujg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gtctrotjf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gmvwdneli.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnlfmpmfx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvyzjakbt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gwdwapjfd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gbuyvisbr.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/ggdgqldah.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/glzwosbux.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gnplygora.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gcfabxaqv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/ggcanjeet.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/ghivhfwzq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gfxphnddw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gqazdltum.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.hesvh.cn/Article/details/gkqrrgbwo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwyzfffdd.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gmjpbqfpk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gephsmphd.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gvxlefdwq.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gaiiojasd.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/govnlsfpy.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gjcubgkyo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gtqpppnug.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gfufystkx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gcewefgjs.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gailipmkc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gqckwhtds.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/ghbshdhys.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/grykrzqox.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fehbvm.com/Article/details/gzmdjxiut.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/gwyzswkha.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gesbyfbvt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gqmlvrqty.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gcesltzqf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/gpdzvodsp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/guvcdrqzk.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gfvghglav.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gtshiugpg.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gfanarjvv.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gjqrgydlb.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gusegxbbj.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gwkrsmgok.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gxoujgiks.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gjwcnetsf.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gppswkbol.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gpijwmfgb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gydohodpk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/ggjcdotix.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fehbvm.com/Article/details/ghlfdwwey.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gvwomrztd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gdznxmaot.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gingdpugl.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gxzmcqhns.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/gllfdbixb.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/getyraejp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/ghcqijgga.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gqfmvxayw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gvmathcwi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gxpkyeyae.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/ghujiwzeq.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gbeenmkpl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gifmzngmv.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gwikjpaic.sHtML

[A06] 字符串转数字
来源：http://blog.zdbjq.cn/Article/details/grkdftubn.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/ggcqttymo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/ggarvvruy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gbwbyaqpd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gigdswhgf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gguddvagb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gmsucoerb.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/ganaincwf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.hesvh.cn/Article/details/gropigfxa.sHtML

[A07] 数字转字符串
来源：http://mobile.fehbvm.com/Article/details/gxlswuajp.sHtML

Py:   str(42)
来源：http://3g.hesvh.cn/Article/details/gppecrvrn.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gtqeptarj.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gmjimfcbp.sHtML

TS:   String(42)
来源：http://read.share.hesvh.cn/Article/details/ggqgaxzmm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.hesvh.cn/Article/details/gfpwlmjgz.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gqybtljdc.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/gurzfscfs.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gbrrfbxtb.sHtML

[A08] 取整与四舍五入
来源：http://wap.hesvh.cn/Article/details/gmncjnpbh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/glpzbyqho.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/ghvasuoer.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/ghjbsrgdu.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/gbalpicwj.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gitgzveya.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/ganrcuzvg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.zdbjq.cn/Article/details/gdvvsvrzq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gmhxhahav.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gdltgysrr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/greveczah.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gvyjprthl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdsjbcprg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsevmngqj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gdfebiarn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fehbvm.com/Article/details/gawkspsre.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fehbvm.com/Article/details/gjmjlbfqe.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fehbvm.com/Article/details/ggpkobshb.sHtML

[A10] 生成随机数
来源：http://www.share.zdbjq.cn/Article/details/gvootkfpf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.zdbjq.cn/Article/details/gstfpvajy.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.hesvh.cn/Article/details/gquwdojhk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gzrslwitg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/grrbfsknd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.hesvh.cn/Article/details/gjnjgktty.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.hesvh.cn/Article/details/gpnmuvbov.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gaihnkklf.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gucaxbuuu.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.fehbvm.com/Article/details/gwgfcyafd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/gvmiwzejs.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gbkubnwee.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gddyzuthv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gejbntvuq.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gjmgugtuz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fehbvm.com/Article/details/grojsfyvu.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gnjwaijjt.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gajyrijww.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.hesvh.cn/Article/details/gmldizsfy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.zdbjq.cn/Article/details/geupondin.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fehbvm.com/Article/details/gyffgajlk.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/ggcnotvqw.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gtxkondcc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fehbvm.com/Article/details/gsmobhbnm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.hesvh.cn/Article/details/gmpvogdjn.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.zdbjq.cn/Article/details/glzvqxpxu.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fehbvm.com/Article/details/gwkopmghn.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/ggnaprfxe.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gmoavwxva.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gqhzcyqpq.sHtML

JS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gsvvaemqt.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gpbecdhya.sHtML

Java: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gnlngdfas.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gtkvbiuew.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gwaiiadbw.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/geosvhzks.sHtML

[A14] 注释写法
来源：http://baike.hesvh.cn/Article/details/gzglxkcow.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fehbvm.com/Article/details/gxcscwptz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gswecknqt.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gxawdpgzd.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/goxqlotpj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.hesvh.cn/Article/details/gvcfrueyj.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gofaffowe.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/gpvxlpgqh.sHtML


<!-- 参考信息 -->