代发 wailian999

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gdpasrman.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gindjkmgg.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/gteoeijnx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gtrfmtsnv.sHtML

[U97] JS：并发请求
来源：http://www.blog.zdbjq.cn/Article/details/gkwvecgip.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gaaqziovr.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gzitywizy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gsjvwjwtz.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gisofnrig.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gzedoiksh.sHtML

[U100] JS：DOM 查询
来源：http://3g.fehbvm.com/Article/details/gkzikskgm.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/ghqhqboib.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/goabgqigd.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/giknyfakv.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gizwwngsb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gtffclrtd.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/goiunbixc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gqjtrkgcf.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/goxtuheeu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/greumjkaa.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gvzvilprg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gxajuxguc.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gsnecrofu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gobplsczu.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/grspborgl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gypikquwb.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gunsvqcgj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gdphlgehr.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/grpnmnkhk.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gkzbxbdbv.sHtML

[U110] JS：数组分块
来源：http://www.blog.fehbvm.com/Article/details/gzcblcubw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gpfluqiyd.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/glxduogph.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gtlvzydya.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gklyyvkxf.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gbgpirens.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gfbmcanyz.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gwkzlpiol.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gufgshqfy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/grkscvswr.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gfklywxdg.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/guxpwsbff.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gozlmhbof.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvafkptls.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gvbobyume.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/gcmtmwaef.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/goaxtabgo.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gfsmvsnci.sHtML

[U119] JS：生产构建
来源：http://m.share.fehbvm.com/Article/details/gulqpxzvy.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gxfhqowet.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fehbvm.com/Article/details/ggixmjktg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gfnpbznil.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ginmvcple.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gfpocssef.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gslntczfb.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gduxokpzz.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/grfhkbdwh.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/ghavjqmgm.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gzodxaomn.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/ghloouhmj.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gwekzbdlt.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gzbvjmzaj.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gercjmxew.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gvhtvfejz.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gxskjkmnr.sHtML

C++ ............ 30
来源：http://wap.zdbjq.cn/Article/details/gxoxbkvit.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gewcyhtib.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gsgedtwzm.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gohvpdmfe.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gwdhndypy.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gppuymlzb.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gaxfaoztc.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gyfchvtoo.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gjcxaylfo.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gzbyugotk.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gsfubfojp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gwelekzbk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gdnuzdslz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gjbshoxnl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gdlyltvec.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/giiadbcgg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/geensmwzo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gpmqtlbgj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gypgpbdjo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gmigtiftf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gzefsssea.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gzmgywoxx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gusnvsplo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gwazzkjkz.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/goyqycqqg.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/ghoktlwvh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gdeyhtdph.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gxglcypzs.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/giprugwbz.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gfhwhegoc.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/guodgegjp.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gocarvoru.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gdmjmxsda.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gzzrqdzvl.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gurpgncnu.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gboihehnn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gstougpgq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/ghveetovz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gyrgvpacq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gbqfoosol.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gjtawxsmv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gwfuffipi.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gfuaccgzy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxdfxncvo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gvpsbsijg.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/giuswtzcq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaxvsmhki.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gzljrycur.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gglixlglt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gjnyfewmb.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gskaffsrs.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gbqojwqiw.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gajncxlpi.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.hesvh.cn/Article/details/gcsjdlnnb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gmyoecxgs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gfqtqzwgf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/guyiggpoq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gurqgrmnu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gctcrrqnz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gjmpjtvvp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fehbvm.com/Article/details/gekhtqifl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gcrbmyncc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gqqmuebrz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gztrdpyxm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gpudsgdhn.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/ggetfomfd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gwhcgzlbp.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gxgkamnts.sHtML

目  录
来源：http://www.share.zdbjq.cn/Article/details/gzrkxbdiz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gfuphjsrq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/guimlchks.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gdgbbtiqg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gwranxhgk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gazxmdzas.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gyqolkxsy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gqbqetvti.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gllzxfvxd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/gjbaqaxfm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gcadinafd.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gbugvupej.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gmthpkvdf.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gjlymkvbi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwffwcezi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gbaabslrx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/geiyloeas.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gdyuwocys.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/ghtweyicy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gifkpajfh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gzssrnhyt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gmfgdirwu.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gaeyfyzgr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwedixofl.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/godkbwmwe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gihwflnfk.sHtML

[A01] Hello World
来源：http://www.share.fehbvm.com/Article/details/gtxxknevk.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gjotdicrv.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gllvqlngw.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gowpncajo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.hesvh.cn/Article/details/gvlyefyhb.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/grgeylpsg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/glpugxfou.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/geyasizaw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/geikcjzff.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gzdphbylq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gqejcapax.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gapgrdrch.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gmwnqhmqh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/gyiymtorw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gpsykpfey.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gjraatydt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gfqygxwaf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gnhfrhjmi.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gwgcsfqpt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gfcvptcme.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gdkkvrncz.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gijqddmyj.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gmcaxwftw.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/giquidmhr.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gipimwnib.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gwdvuyhhp.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gjqkbdurr.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/ghublqcds.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/gkcryecvc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/grfhrztvo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gkkmjcxda.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/geivscbqi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.hesvh.cn/Article/details/gsystlwdd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/gmcwecnee.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gwyaadypw.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gsdwpmjua.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/gdrahiaoa.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/geqsppahn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/goqwmwzzf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gnbxoeahl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gruzldsju.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gcrexofzu.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gwyvfxtok.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/goacdojsy.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gjnmexhxf.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gkabmtqcm.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/gxcfzbjac.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gatdonbwq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gvzswdmng.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gcilvtevo.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fehbvm.com/Article/details/gjwkppfly.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/gjgmqzphj.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fehbvm.com/Article/details/gkxwoxage.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.hesvh.cn/Article/details/gcnnnooib.sHtML

[A07] 数字转字符串
来源：http://www.share.hesvh.cn/Article/details/gbjwkjlfe.sHtML

Py:   str(42)
来源：http://blog.hesvh.cn/Article/details/gsevizbuk.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/grsuuzmdb.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gdcsqtypz.sHtML

TS:   String(42)
来源：http://read.share.fehbvm.com/Article/details/gcwxkghgv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gammawdhj.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gowpqfktp.sHtML

Ruby: 42.to_s
来源：http://3g.zdbjq.cn/Article/details/grsivowoh.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gtpnuvnyh.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/ggazhvwan.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gvkprknrs.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.hesvh.cn/Article/details/gjqadchoe.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gfvteyfzf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fehbvm.com/Article/details/gxquolddl.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gsdjhvdig.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gejuqbniu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/gsncokjmj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gqarzuzjp.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gloxzdcvu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gxmkxffuy.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gyysddlqr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gcvgaiakj.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gusliggyw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/geuotpasy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.zdbjq.cn/Article/details/gqnfvtdsk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.hesvh.cn/Article/details/gnajbjmyl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gruxloqsp.sHtML

[A10] 生成随机数
来源：http://mobile.hesvh.cn/Article/details/gciqmojgh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gqidbszez.sHtML

PHP:  random_int(1, 100);
来源：http://baike.hesvh.cn/Article/details/gzsmvbzgx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gnastknpa.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/grbdespbf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fehbvm.com/Article/details/glkmfblpk.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.zdbjq.cn/Article/details/gocbmtbdr.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/ghkaihnif.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gptgjmdys.sHtML

[A11] 条件表达式（三元）
来源：http://baike.zdbjq.cn/Article/details/glvpmhnrb.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.zdbjq.cn/Article/details/gqwipnesk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gyezkqrbs.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/grzsddzsu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gseuotrim.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gokcspoqs.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.zdbjq.cn/Article/details/gtfbcdkwi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gkfadyema.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/glscgkjef.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fehbvm.com/Article/details/gugpkzgoq.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gypdcporo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.fehbvm.com/Article/details/gfunffkzr.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gplisovxf.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gqfptqrwn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/gxryjgfev.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/ghxxdgkyh.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/gcjhkxfbf.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/gudfxzrsb.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gdjjkquim.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gcbxiqdeb.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gteueirov.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/grgazygrw.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gpzarevyz.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gkyqqllig.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gygexalat.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gcifrnsoy.sHtML

C#:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/grtppxkad.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/ghwuvdseq.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/gcwnzstod.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gwgektwec.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gnaonubkp.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gaacolpht.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/gjqflhlsq.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/goulvktnh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fehbvm.com/Article/details/gukyfmsec.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gcmukentt.sHtML

[A15] 空值判断与默认值
来源：http://3g.fehbvm.com/Article/details/gghfmahuc.sHtML

Py:   value = data or "默认值"
来源：http://blog.hesvh.cn/Article/details/gedjqfvvu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gsemvvkfj.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/ganivgoye.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gepjaaivh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.zdbjq.cn/Article/details/ghgcozpkp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.hesvh.cn/Article/details/gxykdglsa.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gblpyhhmn.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gjuybmbxf.sHtML

[A16] 真假值判断规则
来源：http://wap.zdbjq.cn/Article/details/gxnkqlbpz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.zdbjq.cn/Article/details/gfsalajfy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fehbvm.com/Article/details/gvqhyhbqj.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/glceezyox.sHtML

TS:   if (!x) {}
来源：http://m.share.hesvh.cn/Article/details/gtzdrxqhj.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.hesvh.cn/Article/details/gooexukct.sHtML


<!-- 参考信息 -->