代发 wailian999

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gcllfvfdd.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/glvjejuwq.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gsyebpqyv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gqhbpwxwx.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gqjqawzvk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gryfkxhou.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gnjnvbjsa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gzcjhxnct.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gledicxyf.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/ggbsawzju.sHtML

[U100] JS：DOM 查询
来源：http://blog.fehbvm.com/Article/details/gobwxlwwj.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gbjkoirug.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gbnqhegco.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gureijkgi.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/ghlvyhems.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gycxeflxs.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/gtdbyxemv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/ginptjshu.sHtML

[U104] JS：防抖
来源：http://3g.zdbjq.cn/Article/details/girghvztz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gldtamnee.sHtML

[U105] JS：节流
来源：http://www.share.hesvh.cn/Article/details/grashqqlt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gdnotznoo.sHtML

[U106] JS：日期格式化
来源：http://m.share.zdbjq.cn/Article/details/ginczkxyf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.hesvh.cn/Article/details/gdnolssjf.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gfuwxzebp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gqccofbdv.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gcpxgdbuu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gtejvwvig.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gxahyjmch.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gtfayklis.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gtlgvzcvq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gdxnxmgmz.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/giuameyns.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/ggnedlsix.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gjnbsjzur.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gupipjgra.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gaklueiil.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gzhesimrr.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gnipjuloz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gkmsvlrny.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/genmsxwvi.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gmrjzwbtd.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gmbshdzlk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/ghsbzybsy.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gcfzsnobc.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gvoobhhcq.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gdgkjkzoz.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gxzapjths.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gpiioonmq.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gqeqqhkdj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gwhqompnp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gaoutglgs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gazojdohx.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gexyecduv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggifmxcps.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/gfdbrxkac.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gxqkburom.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/gwdqnptlf.sHtML

JavaScript ..... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gcniygtyl.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gcqmfgjpb.sHtML

Java ........... 212
来源：http://3g.fehbvm.com/Article/details/gvtoddsob.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gysuugzij.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/glpzagevh.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gamiqmxjm.sHtML

C .............. 30
来源：http://read.share.fehbvm.com/Article/details/gdocumjrz.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/gkvvipzga.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gbxbpbhoq.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gqfsskqtb.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gtptzpnkn.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gygqrnenk.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/glaclpunv.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/ggfretsjx.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gdgngmsrt.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gptzkbvyu.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gkjxozzdg.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gxstyiahn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gcgmjszao.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gubagrfsx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gupvijyar.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gqfrlcler.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/gepfznwtt.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gabnmwchc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gkjntbrxb.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/ghualcovn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gknommxez.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/ggilelqkr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/goqszkcot.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gnflkxiyy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gjbtzdacl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gtxlqzxkj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gworhgjxl.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gruefwjar.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gihhzmmfo.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/glndfncrv.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gunwnhwlc.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gxnoxvldy.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gjwbxdhjn.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/guztbulnq.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gbarhoavp.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gltufcvwv.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gfchmubqq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/grhfyrkjn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gwjfnbvje.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gmotmrrgi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/graekulvo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gmkkvidvh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gkhakkqtx.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gfdmpkzca.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdnfpucnz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/glauafwwh.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gqxooerag.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grrhdbcqs.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gmtplfszz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/gutykochh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gpjddvftk.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gkqlygnbv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gkueqkjoo.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gfvaxvymr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gxzdurljh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/gpurzrrkr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/gcooiquit.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/geagcfiej.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.hesvh.cn/Article/details/gxvmukxca.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gpijxkmet.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gybibaixc.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gnikuzeuw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gakibrmug.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gyttznvfi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.hesvh.cn/Article/details/gymilddub.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gfcjffyqw.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gxupnpkgh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.zdbjq.cn/Article/details/grqsmqxpj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/grgsdmdlr.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gfhkbjspz.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gviawpqvf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/giubqieah.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gztqqrihz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gjxgedxrc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gykcrdwgq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.hesvh.cn/Article/details/gpxfssvzc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gkynbjbqp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gsrfydvdl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gebyybgwv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/golvznied.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gagxuuvpq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/ghvrtdmcl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gpzcaoafg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gvqdypelc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/ggrwfstqn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/guwowfsfj.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gmznlsdhk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gvwuideaw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gvjmirabx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.hesvh.cn/Article/details/gqqizddyh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gchtwchph.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gtuaakhlp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtgnjarwm.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gbslvurxo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ganncdyrr.sHtML

[A01] Hello World
来源：http://wap.fehbvm.com/Article/details/gouwnopgb.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gmyqtbkbx.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gfbhwbnio.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/geyezjkca.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/ggxzsimzq.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/grkbjlgwh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gdtugshus.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/gajqywknt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gqycvcfba.sHtML

[A02] 变量声明与赋值
来源：http://blog.hesvh.cn/Article/details/gannthzqf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.fehbvm.com/Article/details/gekbjdkom.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gmgbgbazn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gkniszquf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gnyiklsom.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gajfboihy.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gfgxjcrgi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gjuihlmko.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gbapohmlo.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gxhivmluy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gjtlctmez.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gcmhhtfeo.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gfiweygkn.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gxebndmhy.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gfdkdsrwu.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gvdjuoxae.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gcsqbfcxk.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/ggtjuzfev.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gwcdmqyhq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gxroejzat.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gdlmilwie.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gpddyqmow.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gptoasucz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gqxfvyolk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.zdbjq.cn/Article/details/glqjqhyvc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/ghyoiiixy.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gbbjfdrhm.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gxdolazzz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gyxuwromq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gvrxprwis.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/goubzcqoz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/ghmlbyxfe.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gffugiwgm.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/glowwybab.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gjpzwhlpa.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gjctlcpne.sHtML

[A06] 字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gnroypsds.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gxptvyrxk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/gztcfuths.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gjaggyqxt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gxgsyjavj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.hesvh.cn/Article/details/gtjscvyyo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gwhejaehq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/gnvqgbtmd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/gbgqfzffz.sHtML

[A07] 数字转字符串
来源：http://www.share.zdbjq.cn/Article/details/guawffyuz.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gnyljwreg.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/gdeoyggyv.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/gpouaqojc.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gczncvwls.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fehbvm.com/Article/details/gqukjctsl.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/ggxooeowh.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/gcbwlecil.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/gaxanmlgp.sHtML

[A08] 取整与四舍五入
来源：http://m.share.hesvh.cn/Article/details/gvbthmnor.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gmvgnyvsb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.hesvh.cn/Article/details/gxlzsevet.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gjwzxwkro.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fehbvm.com/Article/details/gyprnrell.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/ggtetcbak.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gcyxqmqtf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/gtvtkcpgk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/glrwkyxwi.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.hesvh.cn/Article/details/gsikguxmj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gnjykdacj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/glahewouk.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gyddcqavw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gqtwthvwu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gimddaiyp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/gfcfwcxlf.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gzmqthehk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gvxiekoxs.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gypmwuzsr.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/gglfgmcjy.sHtML

PHP:  random_int(1, 100);
来源：http://blog.zdbjq.cn/Article/details/gfcjoafsh.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.fehbvm.com/Article/details/gmpdfmwxk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gdljuevcq.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/gigwbfxzn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.zdbjq.cn/Article/details/gxuchvtqu.sHtML

Ruby: rand(1..100)
来源：http://read.share.zdbjq.cn/Article/details/grykahjnv.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/gqrfthtbo.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.zdbjq.cn/Article/details/gmznwsoat.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fehbvm.com/Article/details/gtywrcezu.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gefnanvzv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gfyzjsftw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gzvuofurx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/ggiprsmgj.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.zdbjq.cn/Article/details/gbauryjfx.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gtjwtnttz.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gcojzvwyz.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/gsmindbhw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.zdbjq.cn/Article/details/gldwpafyd.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.zdbjq.cn/Article/details/gjhxvbahr.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.zdbjq.cn/Article/details/gnontcxdw.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gdxcfhwiq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fehbvm.com/Article/details/gmwxybxjf.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fehbvm.com/Article/details/gvzfkigmr.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/gildqefgz.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fehbvm.com/Article/details/gwlodebra.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.hesvh.cn/Article/details/gfbqiunln.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gtydytqjf.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gpmkaplyv.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gowvwvmcs.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gyxjlpsxs.sHtML

Java: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/givuqfcyd.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gkaaznpft.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gqgafxkic.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gpjdksivg.sHtML

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/grdvwkwnz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gxtkogpor.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gkugbvmid.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gcveapbff.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gssnkoupy.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gylcbqkjx.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gsipgpmrt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.hesvh.cn/Article/details/ggkzgquym.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gqylfgwal.sHtML

[A15] 空值判断与默认值
来源：http://3g.hesvh.cn/Article/details/gisyuvrdq.sHtML

Py:   value = data or "默认值"
来源：http://baike.fehbvm.com/Article/details/gbtayxvuc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gibeltedi.sHtML

JS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gznmbogli.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gjqksbuer.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.hesvh.cn/Article/details/ghpcywnpr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.hesvh.cn/Article/details/gmcuvviaw.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fehbvm.com/Article/details/glcmsemcw.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gthznddob.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/gogbsdzde.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.zdbjq.cn/Article/details/gfwwrmmqk.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fehbvm.com/Article/details/grcizcnxz.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.zdbjq.cn/Article/details/gyqbfblfw.sHtML

TS:   if (!x) {}
来源：http://blog.zdbjq.cn/Article/details/gztrmeklb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.zdbjq.cn/Article/details/gkprzolpw.sHtML


<!-- 参考信息 -->