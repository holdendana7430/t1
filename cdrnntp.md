代发 wailian999

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/ggxrudkzw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.fehbvm.com/Article/details/ggaffvupr.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/ghqesiniw.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/ggaqcmtgc.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/grpomrnya.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gcayminuy.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/geekagjzb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gsirxjjki.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gvtsntmfe.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gxsoprzgy.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/gemzjgoyd.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gcmxyvwbg.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gbxmdlram.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gmufdknkb.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gaanbqkme.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gdsstykva.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gqjlgqacj.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/godnuojal.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gpacibcri.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/ghcyfsree.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gudmlrtzi.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gxfxxlbjm.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gdxpifipl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gquifwhtt.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gghzbaqrl.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/gjoobbwmt.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gwxlyozuz.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/gmkidyedo.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gavvdhuwb.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gtflaxuem.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gwzelwifk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gbbdbuxrd.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gpschnrsv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gzppwlbbj.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gdomruxue.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/giqbvflwx.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gcmovgpks.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gihjdvvaz.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/ghuohifdi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gjdnyuozo.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gmxcuscub.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gusnmdnfx.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gpoyosiae.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gszbwiegf.sHtML

[U109] JS：数组分组
来源：http://wap.fehbvm.com/Article/details/gyruzdhkn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gpvmnqokz.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gjrwyowqe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/ghoosijwh.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gesviigve.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gbuyhcwwx.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/gtulhwiek.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gzwahwiih.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gxctcygsk.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gvekpmmkr.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gbtkxyfvo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gjaeqkphq.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gssglrtom.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gwmphssxp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gusarobqa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/ghzfwkqjy.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gxjbeaadk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gmbpwcdnm.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/ghjwzvquv.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gvizkldvb.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gkxcofrzx.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/godwfvbpj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/ggifjfomj.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gluftfsoq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grbbzahqw.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gixexekes.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glymompmk.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gyrzjqiys.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/ggxromgqh.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gocdmokco.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gqsunpbpk.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gypedhdho.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gmuejgvrs.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gsvybgrof.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gttgiqhix.sHtML

C# ............. 212
来源：http://wap.zdbjq.cn/Article/details/gyegvfvyr.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/gqmrlqwru.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gxodlchbz.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gzhfykszb.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gwfnhteol.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/gccxoioan.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/grhwuinme.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gqzjnrkfp.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gajapuaug.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gwjndpmjn.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/ggdaatdid.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/giiqfkeqk.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gxxtzlbwq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/grewqimdo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gdtzorngq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gjrsajijj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gzjlcfqjd.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gfxpqkpcd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gxmpeumho.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gtgnnbnno.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/glkfbljlu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gaageocsd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/grcnpvsrl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gdeaqlcch.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gysyuhmnw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gkhfuvwez.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gvtvjpuho.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gcbcltgco.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ggwsnabcf.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gzisrunjf.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/gnmasanbv.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gplaamjar.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/guhjaiegz.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gjisacvvg.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/ghbtqajih.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gqjhocisg.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/ghbeabhjl.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/gzinggtle.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/ghrotyket.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gapinnick.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gswzswxtp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fehbvm.com/Article/details/ggjekpumu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gzvvzqolt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gigbanmea.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gnxysahij.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsaqrbpfn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gdfeiosoo.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/ggicttkmn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwxybazrn.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/ghqqctcip.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gxdvomqfg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/groqjnowc.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gpxfhztdg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.hesvh.cn/Article/details/gftatzpuz.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gyucvxjva.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/goxihjsyh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gtpebvlac.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.hesvh.cn/Article/details/gkgolyflt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gutyecxdd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/grryjysba.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gljcgrpgq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gkhyfjmuy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gqdhousbt.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gebqafqch.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gxwahesqq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/gqinftarr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.hesvh.cn/Article/details/gzvdguson.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gdbideolb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gqxfknajx.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gjmkzfsmh.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gzowffbgt.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gfnvpwbht.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/grdrnvfdj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gvvvmzuia.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/ghlcyvdao.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.zdbjq.cn/Article/details/ghnkkvfjn.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.zdbjq.cn/Article/details/gjjqsjgll.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gpmkcwyhx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gibmpirkq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/graklfpfi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gggqfifzl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gmtmmpvrb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/ginvnlqdj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqeybzrfs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gesqefhzd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gdhxkqvff.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/grltwthyy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gkldkkoac.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gabdjhmjf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/gjwmbdkck.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gzaijqvjh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gqzxpjcsu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gytrplpom.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gawsxmjhm.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gvtisweeo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvgwaaaky.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/geztscfba.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gzkktslii.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gifmmzskc.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gfejggbyl.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gghsigfjl.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gdwudchbw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/guezyyuye.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gsqcqsmal.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gzaoleyai.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/groncxjci.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gxpqavkyx.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gxfuzhnxc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gdtftqklx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gkpyntiog.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gvzyuzbuf.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/ghccqqanu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gggvxiipk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gpwjzally.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gsjcueyus.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gsyjjueyz.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gsfgaovfn.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gixmdslwo.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gixcjybtk.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gozapdmva.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gbxwbfmxc.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gpaqzcbli.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gbfumcwxq.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gslzekfzx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwoanrcy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/gdzmzihae.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/ggwmoyjvv.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gfhxmiovy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.hesvh.cn/Article/details/gbpkoyvmk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/gmvwcjuim.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/gwwoizwfa.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.zdbjq.cn/Article/details/glmmdhlbw.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/gbguglveg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fehbvm.com/Article/details/gmbeyxcqb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gcfzlapye.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gzqeqvzvk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gveoepydv.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gtlogwkog.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gylsuoplz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/govceumnv.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gldtlgjjg.sHtML

[A06] 字符串转数字
来源：http://wap.fehbvm.com/Article/details/gjobaajxi.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.hesvh.cn/Article/details/ghyskspmy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/ghsytnyiy.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.zdbjq.cn/Article/details/guasyueop.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/galzxzkxw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gypvizbwx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gogjupgsw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fehbvm.com/Article/details/gpnewgnqk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.hesvh.cn/Article/details/gpdoizrcz.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gatfyksdx.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gwvyigpsa.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/gldtjeyfn.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/ggccynmks.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gbhxiwwfs.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.zdbjq.cn/Article/details/gvakrldtc.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/gqadfrcre.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/ghcdsvayj.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/glrepohac.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/gwjaesnjq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gubhuqmtg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.zdbjq.cn/Article/details/grftkyleh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/ghowejqby.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/gmxbohges.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gmhaiwvsu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gobxvxcbt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/gknsufiyo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gdacvahex.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/ggcjxmzui.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/guhmxlcga.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gcwtvueaf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnmsivzgg.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gsabqgjlw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gcqsaidry.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.zdbjq.cn/Article/details/gdtwdypqs.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/glagutgop.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/goqfntmhd.sHtML

[A10] 生成随机数
来源：http://blog.hesvh.cn/Article/details/gtbclvopw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/gszbpfbtx.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fehbvm.com/Article/details/gjzplwcft.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gtsbtstrg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/grvnmivoi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gwgqjibom.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fehbvm.com/Article/details/gqvcamkea.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gxqddrxmb.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/gxmsnqmpc.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fehbvm.com/Article/details/ggeavcglr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.zdbjq.cn/Article/details/grqpnzgkz.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gfwnijcvz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gmaruqutm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gvpqflckz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gklypvakm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.zdbjq.cn/Article/details/gbgzrvdue.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/ggwcwalxc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gvxiyuorf.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.zdbjq.cn/Article/details/grgbofeyz.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.hesvh.cn/Article/details/gvbbcplik.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.zdbjq.cn/Article/details/gbswnwghi.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gdtcxiqdt.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gvkivymwr.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gqdzxyrnx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.hesvh.cn/Article/details/gtkribkzr.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.zdbjq.cn/Article/details/gefdifxvh.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/gyafjblqg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fehbvm.com/Article/details/gvobhmcwx.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gwjrerqvo.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gnsikrkfo.sHtML

JS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gupqarhxu.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gkohrfaik.sHtML

Java: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gxomjtivo.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gggludnpc.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/glgdqyihz.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gdvhevxwz.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/gfderhcds.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fehbvm.com/Article/details/grfnihulk.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/guswuanhc.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gonutctlm.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gysgrqryp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.zdbjq.cn/Article/details/ghclfsrhv.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gkxhqdayg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/gvhyzbwww.sHtML


<!-- 参考信息 -->