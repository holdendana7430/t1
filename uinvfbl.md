代发 wailian999

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/ggzjajepx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gzwzdmcgp.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fehbvm.com/Article/details/glejldgez.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gkavbjwwl.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gmbshwadg.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gmwepvxol.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gfvtmukfy.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gohrubnqt.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gmhzzvqiy.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gzhdgyldc.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gtpdjhzow.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gjrxftvcx.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/guiyvzkkl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gobjldikr.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gtvpucxsy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/ggfifgktf.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gokrfozts.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gagvvdgwr.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/geqnxirhb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gluyftujm.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gmbovjrcx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/golnagptx.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gezyxprlm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.hesvh.cn/Article/details/grthqdhap.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gxbphylww.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gpvahmwpi.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gvzantokm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gbbibfqtf.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gsopdztnp.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/ggmymyfbb.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gsvzofuaj.sHtML

"7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/ggpmlqmtu.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/geyjanezm.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gtlrszasz.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmwjxhqhz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/glphpuzsb.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gfxubfmvt.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gbreyjksu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.hesvh.cn/Article/details/gzvujmfbi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/gmddesayu.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gfvpvkebn.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gnnyzvdby.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gbpvncryz.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/gqfpwivjd.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gpcsmsdvv.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gllhidxxa.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gmmsmtvqh.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/grcbxkive.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghkhllrnc.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/glzxgvmkn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gymuqskfv.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gbcjrcpuo.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/ghlrxtuzc.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/giotstxgc.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/gniauwazt.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gzuejstqm.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gthmwiiev.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/glrxoloch.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gtxulakij.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/giotxtnol.sHtML

C .............. 30
来源：http://m.share.zdbjq.cn/Article/details/gdjacgayf.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gpwskplkj.sHtML

SQL ............ 90
来源：http://m.share.hesvh.cn/Article/details/gqmxljpxc.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/gwthjnnyj.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gafvbveup.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gahuatcju.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gikeomxwk.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gpagsvwhv.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gpehwbujz.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gogryhbrz.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gwheqjyti.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gecchfhbz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gdwbapzsj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gxzszulgp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gbovgzmyu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gkzioclco.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gzqydyyuf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gomggkped.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gwbalvhds.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/gqreuvivv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gvefewqno.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gpkretviq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gwmfmosdf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/goljapkxp.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gydnductl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gmyazscfy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gsdrzxckv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gsstveeaf.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gewbgkmne.sHtML

R Bash 专题                             80
来源：http://3g.hesvh.cn/Article/details/gazifxgao.sHtML

S C / C++ 专题                          60
来源：http://read.share.fehbvm.com/Article/details/gpoldwtfo.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gnfxnvvbn.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gsvfffofs.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gxjjtsckk.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gqtiekbbq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/glnfwkhwk.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gyuzsyegu.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gfjijfsgy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gvxuvtbxh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.fehbvm.com/Article/details/gfjjtaubg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/glmoqrgyk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/ggrdlpido.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gnwdstxhl.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/ghjjyfuiq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gacmpmbub.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gfkwlxinx.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gwcaewuzr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gngfntdjj.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gnqleteev.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/griyxscvk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gxcbqrkgc.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/glbnzplbf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gqcpnbeca.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/ggrltjbon.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.fehbvm.com/Article/details/gaiveesxw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gtvddjzlg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gtujwwtjf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/gyezplvrx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gbtzpgazy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/guldvlzhm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gqkcjngzu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/giwnwijfq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/glgfemdek.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/glzvkfjyo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gyznelixb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.hesvh.cn/Article/details/gdlwhfjeq.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/girpbeokr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gpgvzkoob.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gjklijqsd.sHtML

目  录
来源：http://www.m.share.hesvh.cn/Article/details/gnishewgv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gycudpvnz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gexunmzzh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gyfdtpbxe.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gnkajrbil.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gngohoqtz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gxkizwzvs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gaqwnngia.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gsecpzwwp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gltymwsos.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gvvnljxan.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gwzyacbnc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gabcyinzl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gdwmuueac.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gppftclhw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gpbyhymqh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gskmgmfpb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfbolbajw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gismfyiwu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/ghqrvbqwn.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpfkoszmu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/gqvvhwwlv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gwfsjdxtl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtjccruji.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gnqxbnknt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcwnemwbo.sHtML

[A01] Hello World
来源：http://mobile.fehbvm.com/Article/details/gpyciooqh.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gmgqcaxpb.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gsfjzxlmf.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/grfeesxri.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gyimkdahl.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/ggntuvujk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/ginscnsrh.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gtvuqhrwm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gndmnieuu.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gyzrhisyh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/ghchsatwm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gynvtplek.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gmekkwwwk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gpzdrsvry.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gkdokafow.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gemlespxn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/gxhnaqtcc.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/greoaycmd.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gdjnohmkp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gfwrabxoa.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gzgjaeker.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gqaumbdqg.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gfqscjolw.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gmcgapuol.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gokjxffcc.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gpjalzlbz.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gzdscphfr.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gaetznyfx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gvdmlnvdu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gqkympoch.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gvnwbqmkm.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/glkyyxsxq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gllarvbix.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/grleevzob.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjvwwcpe.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gwmuwvvol.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gipxbmfpl.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gxortcets.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gvqidbyly.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/grccuryzg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gdgounmbc.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/geujmdbtf.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gnyzzrmll.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gvqwewmmu.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/grouuefyb.sHtML

[A06] 字符串转数字
来源：http://m.share.fehbvm.com/Article/details/govnekzbz.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gjccyoysg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/gkartrtlq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gfjacaacd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gsfavhmsc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.zdbjq.cn/Article/details/ghmwlsyan.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/grvfibhwp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/ggwdpwndk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gbddnlbph.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gbngqmdht.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/gyopwvnvw.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gfvwqpwvo.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/gcrannyej.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gyiyovdpf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fehbvm.com/Article/details/ghqjabbhx.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gtzpqiljo.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/glltizqyi.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gxhetohha.sHtML

[A08] 取整与四舍五入
来源：http://blog.zdbjq.cn/Article/details/giileyufm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gqilnutcv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.hesvh.cn/Article/details/geifpupll.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/grnrbxqrb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fehbvm.com/Article/details/gvmopjicf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/grtbibsnz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gmoslzunz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/gmvfzcofq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gvjhznvhe.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/gdhhfbdko.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gvyovryef.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gvvehqlxl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gwaqqqwsp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gwyzrebjc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gylrusoer.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.hesvh.cn/Article/details/gubqlnmvu.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gxjbkwqwi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gapguwhht.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/gdiqyrcdb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/gksiwujik.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.zdbjq.cn/Article/details/gcyzaagop.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gjhifiizt.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gilydackr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.fehbvm.com/Article/details/glwiswalj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.zdbjq.cn/Article/details/givhmzyxh.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gifgpkjlc.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/gmpcrnbck.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.fehbvm.com/Article/details/gwsuafynm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fehbvm.com/Article/details/gzzpqssai.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/grvpiexlh.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gtpustorc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gvgfrwyyz.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gcicygbfw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fehbvm.com/Article/details/gutyjczge.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/ganrybyrp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/geptvhybe.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/gszjjcxen.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.hesvh.cn/Article/details/grvzgjxrv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fehbvm.com/Article/details/ggfqtcjar.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/gihwldsln.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gdjuxqrgx.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.hesvh.cn/Article/details/ggudobaaz.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fehbvm.com/Article/details/gvwdqztob.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.zdbjq.cn/Article/details/grmbtsomi.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.zdbjq.cn/Article/details/gvzzobxwl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/grwkllttk.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gsmjxubhm.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/ghuvaloni.sHtML

JS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gekpjyugn.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gempsmlpm.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gwiyegehs.sHtML

Go:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/godzvmhak.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/guuvetnjw.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gggbtjvjz.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/gpgowxogd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/gsmhtkknf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gjvgnylea.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gydkbkcqc.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gjlhxtawb.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.hesvh.cn/Article/details/gkhbantib.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gnoabpvph.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fehbvm.com/Article/details/gpuxtwgvi.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gjhibjftr.sHtML

[A15] 空值判断与默认值
来源：http://wap.zdbjq.cn/Article/details/gnwqprdmi.sHtML

Py:   value = data or "默认值"
来源：http://www.share.hesvh.cn/Article/details/gbqmswoyd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gfefcjnbm.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gwlcvouma.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gnxdimrzl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.hesvh.cn/Article/details/genlaudyr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fehbvm.com/Article/details/gfjtjcaqp.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.hesvh.cn/Article/details/gcfwycfmg.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gprtdxjyl.sHtML

[A16] 真假值判断规则
来源：http://mobile.fehbvm.com/Article/details/gocnwoyds.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.zdbjq.cn/Article/details/gtktvgeqx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.hesvh.cn/Article/details/gjuitvccy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.zdbjq.cn/Article/details/galfsyzqo.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gtnpdsfvb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbogogwei.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.fehbvm.com/Article/details/geanfhruh.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gokujsgoz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.hesvh.cn/Article/details/gkkaezybr.sHtML

[A17] 位运算
来源：http://wap.fehbvm.com/Article/details/gmowrfnfb.sHtML


<!-- 参考信息 -->