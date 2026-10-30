代发 wailian999

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gnuwznkyy.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gizqyrnvt.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gjwqklyuf.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gizceeahl.sHtML

[U87] JS：解构默认值
来源：http://read.share.zdbjq.cn/Article/details/gvbamluqt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/givdpybko.sHtML

[U88] JS：对象展开合并
来源：http://baike.zdbjq.cn/Article/details/gengiqclf.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gwmsxvhaf.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gujfjdzqp.sHtML

[...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gadsbibdb.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/ghoxjpykj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/guvshqjpm.sHtML

[U91] JS：对象键值遍历
来源：http://blog.hesvh.cn/Article/details/gjhowtyva.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gpzcjbpqo.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/ghksdeidz.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/guqrpowbr.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gutalkews.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gzddibtns.sHtML

[U94] JS：箭头函数
来源：http://blog.fehbvm.com/Article/details/gljcoczzz.sHtML

const double = x => x * 2;
来源：http://www.blog.hesvh.cn/Article/details/gpxthfwqa.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gxquvcfwg.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gezaflafq.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gisobrvay.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gibputrkw.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/ggfkzoviu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gwqwcfrij.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gxbldmnfs.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gzigadkpb.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gilkanffh.sHtML

el.addEventListener("click", e => {})
来源：http://baike.zdbjq.cn/Article/details/guhsriryb.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gehyhnbal.sHtML

document.querySelector(".item")
来源：http://www.blog.fehbvm.com/Article/details/gnxhnaelj.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gejkhuwoi.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/ganutksbi.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/glfbhfnfe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/gmskmlhfk.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gjnylajcy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gmajapqvg.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gxymuramg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gdcanpsfz.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gbjodhtim.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gefvxqbgo.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/goalrcvay.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gpapqzxlz.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gtydnuhvn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fehbvm.com/Article/details/garqouxvi.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/ghmlykfby.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gmrzkxcbw.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gxqjxmnpm.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gvajcgemb.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gopslvztr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/glatuyuhn.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gzzdhchwo.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/giuqejqeh.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gilaunwfl.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gxagoxejf.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/giwodhccm.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gtjhxxspr.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gzremaosw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gyiifgbik.sHtML

[U115] JS：生成 UUID
来源：http://read.share.zdbjq.cn/Article/details/gvwfyjlbm.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gpgxkukij.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gamiyusrc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gudibabjr.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/gyiirczdf.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gtfgshwum.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gvjhqxydo.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gyuhxmzig.sHtML

[U119] JS：生产构建
来源：http://www.m.share.zdbjq.cn/Article/details/gvemurrje.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gimclfjjk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gljklyajx.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gwbhvbvwa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gephalwxz.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gxzufuvuw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqjslcfva.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gzrglcqzv.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gbypbuvzj.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/girqcnyxi.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gvazdwgqc.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gyqxxrlvy.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gugsgzutx.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gazuanjyd.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gfphyctra.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gdlpcahll.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/ghxjdavxm.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gmhflacwe.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/giwlzmzwo.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gfkibkgtq.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gygxdefed.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gzkumceyu.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gpadjmxbn.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gaolcbups.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gfvpgxudz.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gzxqtypzn.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gyclktlwj.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gczclxmbh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gwmuedmnq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/guxhjgrmr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gxlktztgy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gewahrqqa.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gqnnmqltk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gfdsngehm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gqycijahu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gottgthry.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gkkoegqhb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/ghwvbyiax.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gxiwzikam.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gqwhjhsml.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/guztlcqbh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gkjwntjjx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gnzfaqyym.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gwklwpnts.sHtML

Q SQL 专题                              90
来源：http://3g.fehbvm.com/Article/details/gezvritdq.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gkcxakxxy.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gnqwjbamg.sHtML

T 其他语言补充                          60
来源：http://baike.zdbjq.cn/Article/details/gnwnwevmd.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gdfcacrnp.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gggbnqezb.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gswetanlc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gablxdozh.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gsszeoedx.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gsawgqxzd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/ggssgpcoq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gkbhuxtwu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gbglpiivd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gfksksxqo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gswvjjczm.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gdutfgolf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxspjgxvi.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gsgnzucqr.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gylnbxeud.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkcdjlofh.sHtML

【收录内容】
来源：http://baike.zdbjq.cn/Article/details/geseharon.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gmxsmwnyw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/ggykyyprc.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/glgecttmu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gnwyvjain.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/ggezqnqlv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gkzodfzdi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/gjhpxvxhp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fehbvm.com/Article/details/gxssnmkli.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/gsawegwki.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gufteyxzy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gybavfybg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gqnadervw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gqxyrwucu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gtwsyvgkt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gbtmywnkg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/guvedukyu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gwjptvxjk.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gxrvastub.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gaaadmlkd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gzxeobvol.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gnurcefpl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gobeffwtc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gyfvmskwi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gezhcngdo.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gkmfvfxpx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gccfohfic.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gscxfiopx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gfgtopewx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gtnxxbbhw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gacgnqwcp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/ggfbzypsw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gogqdikbf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gputdgdqm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gzcnwfxgk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gapzojxav.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gejhymfrq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gokkukknp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gkftdaccb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gkvxhusat.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gautmfvlh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gzgkhwmmo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gixlszicd.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gdwpttzll.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grmzsdnpr.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/gbieqludq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyiysemfp.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gzhlixldk.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/ghbgrojux.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gdsrnymyz.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gzrgmelye.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gmcpolkml.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gcmfayjib.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/grlnuzsck.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/gsbckjsrj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gciugdedt.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gdryudpus.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gdlrkaxgc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gybdaavuk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gszonaxeb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.fehbvm.com/Article/details/gwastavsx.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gomywenwi.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gkgiebaib.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gwtsadqqb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/ggiuouwyk.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/gkmvxspwc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/glsfpesxt.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gssrdyrfc.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gavcwjlsl.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gppwmamen.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gvrgutfox.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gxniqvxdr.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/glbieqkmq.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/guitvdfqc.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gzhdgtgsa.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/grtsmyvvn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/ggqrsdqgr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gfmtbexib.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gxsifaqny.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.hesvh.cn/Article/details/ghzxwevpr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/gpqijbjgs.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gjrdfudpf.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gmsboldpo.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/gemcvjxcu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/griitngdd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gbrozoifa.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gcxntuzva.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gmdcfpsan.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gskzkexjz.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gowmgjgsx.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gaxtntrxu.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gbkdxvtuz.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gqxalsfhl.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/gfxxxamkm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gcdcvdqzo.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/gwyrdhzsx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/ghsvtpayn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gwlydfzem.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/gojajnfug.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gfanicrkf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gdgohpdss.sHtML

[A07] 数字转字符串
来源：http://m.share.hesvh.cn/Article/details/ggwvbelbi.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/gombttsve.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gdnhgilhk.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gnmgqibwn.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gexohtzaw.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/ggitoaklh.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/gznrwrvvm.sHtML

Ruby: 42.to_s
来源：http://www.blog.zdbjq.cn/Article/details/gqvmhfriw.sHtML

C#:   42.ToString()
来源：http://m.share.zdbjq.cn/Article/details/gbkxzuxxr.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fehbvm.com/Article/details/gwmfyxupq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/getdznxtn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.fehbvm.com/Article/details/gvperjyzz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gsjytlrbp.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/gyquhaudt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gsiplnfle.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/goanbfszx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/ghhbshces.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gctcdybfz.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/gtfgfkiow.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gqccfjnje.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/goohziprn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gceznulmh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gzpcxuokj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtaecyidl.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.hesvh.cn/Article/details/glymdlgtx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/grllirkcy.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gnzwtaodw.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gqsnqwgqt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/grzxingvq.sHtML

PHP:  random_int(1, 100);
来源：http://baike.zdbjq.cn/Article/details/gzrhseryl.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gfgykmewt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gkbeodpsv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gkfwzkbec.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.zdbjq.cn/Article/details/gpcyfhsoj.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/gsmudrlbi.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/guuprtdqc.sHtML

[A11] 条件表达式（三元）
来源：http://baike.zdbjq.cn/Article/details/gxbhwutcx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.hesvh.cn/Article/details/gxdhkiuci.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gavmntqyl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/ggiuyxuog.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gcfshzzce.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gjfwtrzxv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.fehbvm.com/Article/details/ggcqtvtsy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/goyjsdvwm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gbpxitngx.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.zdbjq.cn/Article/details/grzvryfzw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.hesvh.cn/Article/details/glhbewaxs.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/gmdzbygyj.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/glwnmokfl.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gorfyjhib.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.hesvh.cn/Article/details/ggteonzuw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gtdeflcch.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/grgtwhbiy.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/gywpyaclb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gkyydctwq.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gdkvwszsc.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gsmujuukf.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gzmwqyvdb.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gbzgmewew.sHtML

Java: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gwbuxzwjd.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gsqelgmvx.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gtylnlmsd.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/giuwwqxir.sHtML

[A14] 注释写法
来源：http://www.m.share.hesvh.cn/Article/details/gwubsltyl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fehbvm.com/Article/details/gvtnmwjdh.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gqblhojzy.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/grxkletkw.sHtML


<!-- 参考信息 -->