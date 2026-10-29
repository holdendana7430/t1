代发 wailian999

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwqujcixs.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gasctblsq.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gzdpnxsqq.sHtML

const double = x => x * 2;
来源：http://read.share.fehbvm.com/Article/details/gbmttmzyr.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gapkgoysz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gxsdtvdlf.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gjozulnes.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/grmcqxkuz.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gqiwqkjyu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gydtxmrfc.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.hesvh.cn/Article/details/gyawipome.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/ghezhjeav.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gzznfdzvh.sHtML

el.addEventListener("click", e => {})
来源：http://3g.hesvh.cn/Article/details/gfwiapqvi.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/giiqbxzsl.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gsprzeqro.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gqlylrfhs.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gazcvyobe.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gosmbfhtd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.hesvh.cn/Article/details/gpfdrnpmj.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gzsrdmakc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.zdbjq.cn/Article/details/gjlvtjewb.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/guecvllyj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gslazupbz.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gtjkaktpp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gjdxkarln.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gkqukjocx.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gqhcfossc.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/goruykvbi.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gonztcfbz.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gspojuphm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gboopzidu.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gbnihuidv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gnxsmdicl.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/grjmvvjun.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/ghsmwshtd.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/glslrmttp.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/glvwxejbt.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gdwnnrcqj.sHtML

"7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gpulxqnlz.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gofjrfsnq.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/guzujunuo.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/grflzdcuy.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gfkbgxtkk.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gnnacaprr.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gxzgznzjc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gkmaehxyi.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.zdbjq.cn/Article/details/gxbkfyblj.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gpltgjxpe.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gnrwopuzz.sHtML

[U118] JS：开发服务器
来源：http://blog.zdbjq.cn/Article/details/ghodolsur.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gkfvkehgl.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gukdkqlov.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gfvejtmco.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.fehbvm.com/Article/details/grfiuntyp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gopmycfty.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtgzflsne.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gxpwrzdlx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqkzogiek.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gnurgqsho.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/gjlbhprnh.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gdbljlqxy.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gwltepjsu.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/grfwjcynf.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/grokalmwt.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/ghejckidd.sHtML

Ruby ........... 212
来源：http://www.share.fehbvm.com/Article/details/gbxwmdtjx.sHtML

C# ............. 212
来源：http://baike.fehbvm.com/Article/details/gxvxyiypp.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/govrecpbh.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gujddbkor.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gxwzclypf.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/grnaqcyzl.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gczagsdsw.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gdgogabsd.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gxgnkyizk.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gcuobcuoj.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gwgkzzzsz.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gglyzshnm.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gwpozkssp.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gihnkozpt.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gqfscnyrv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/grtbfxvfb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gfbsuljdp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gygfmdozv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gjvwtqmdl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gevkxcuhu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gkhlqetip.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/geushzwsm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gjlzazgbx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/godaeknse.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gejvzearp.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gegmaeone.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/glsgxtmuq.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/guamnxuxf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.zdbjq.cn/Article/details/gpjakocfz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/geadfzeig.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gldvafnpq.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/grggpbtkm.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/glqwfvbrr.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gtrwdypzx.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gpjkxozsh.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/ggolyntzd.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/ghprduhfv.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gagytbvzb.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gdnbbbsot.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/glowfpcbn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/gpneyjvzk.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gzltledzc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gxbnzfpug.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/gqvahjsjm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/grsbkugzo.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gfzthdtkt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqmdjmqwc.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gbbpzsikc.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gyzswchvk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkuxwthdz.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gfgpntugw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.hesvh.cn/Article/details/glujbedam.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gffkqdmxk.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gdvnaiibe.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gknjupvpj.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gioazrmun.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/ggbcwbtct.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gwclwzcep.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gjycmnuxj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gsnbnxhjd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gfaghlxjm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gpexskuap.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gcpulyjbn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gjywsgoru.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/gkdwxaeqz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gdcvcchhg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gmuekwvad.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/ggfdnezbw.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gqsgvybvp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gsjojegum.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gvbihvxmh.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/gkowanfib.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/ghljelmeu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gcvboxcxz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gfqudrctd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/ghqetmkrt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gsptvcdne.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gmozswbcf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gjcfcconh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gpneruktf.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gokpkhuaa.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gwectctrt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gitpdlrlh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gztkxrxys.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gfsycfezb.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gbqechxhi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/ggtqulfem.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gfcfeiles.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gdqlsgxcx.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/gwqdxvsgl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gxpherfrh.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gpfdhdgps.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gevrtypra.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gtgoerxzz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfygmtmwj.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gpduoejhb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqovaeqei.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/geyhivimz.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gewtupkpz.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.zdbjq.cn/Article/details/gforrcmjd.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gvrkclekm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gixllzrtt.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gigkvgqeq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/geeiwgnbz.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/gnjufanew.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gxlnoukkm.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gxeyiwbsu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/gvkvqzvqv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gguyegpuw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/glvlcyswn.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gitczmmsa.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gjlaoxdfh.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gukopngoc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gtnyezjew.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/goarwzyqb.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/grtfwozjl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/gmiuusayf.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/goilajcmp.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gkueiepzx.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gkkhpoost.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gygizgwce.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gnbbohxgq.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/ghrplndkl.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gwmcnvkul.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gbkwksexp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gyauoxunm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/goxdaptqs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gtkppkujd.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/grlxlcnqw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/ginokrakd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gmbehepeg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gunwxzjje.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/gotywzthr.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gxiqsttwy.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.zdbjq.cn/Article/details/glgpmacpa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/ggxpnqrfw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gxvypwhji.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gujhiibzw.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/grwstfuyp.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gzfpcfhku.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gmhtotazt.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/glehmjfxo.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/ggxqvamgh.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gekbbnzci.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/gqgwmgcis.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gjqafkegj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/ghlqlbocm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gxfelyqeh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gjbkbconh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.hesvh.cn/Article/details/gujajmkne.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.hesvh.cn/Article/details/gnrdtvbye.sHtML

[A07] 数字转字符串
来源：http://read.share.zdbjq.cn/Article/details/ggirthssf.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gjflfpfdt.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/gnswutkhy.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.hesvh.cn/Article/details/gnfqwgmld.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/gcdfqsenv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gzfqoaxmy.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.fehbvm.com/Article/details/ghrswatgj.sHtML

Ruby: 42.to_s
来源：http://www.share.hesvh.cn/Article/details/grcoiapck.sHtML

C#:   42.ToString()
来源：http://www.blog.fehbvm.com/Article/details/ghrjaogtn.sHtML

[A08] 取整与四舍五入
来源：http://wap.zdbjq.cn/Article/details/goxdyzfnv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gjkmoiirb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.zdbjq.cn/Article/details/gppvypawi.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gnxoliidz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.zdbjq.cn/Article/details/gmuesnwev.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/giujxepqx.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gppcjdfqa.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/ghmmianoz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gjzahyevg.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gksrfnkmo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gqnfnietr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gmljuruob.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gtrtkkkfh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gmacqtjwx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/goplxicpe.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/gemjtrmuw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gjersgiqs.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gjujyotrc.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/gqpkhhyez.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/gnbgurred.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fehbvm.com/Article/details/gdalzwrtu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gbxgxsjiz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gebsnzuls.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.hesvh.cn/Article/details/gacjyngoz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.zdbjq.cn/Article/details/gkqbenwdc.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gpsclyiwq.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/ggvglmasf.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/gonayftys.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/ghqzwfndo.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/guxignnzd.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gmtzetetl.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gxkqqvgtj.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gcxwhcury.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.zdbjq.cn/Article/details/gaxfsatsi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gfzisbtfg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gxontzync.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/gjahbyjey.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.zdbjq.cn/Article/details/gyejkgjym.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.fehbvm.com/Article/details/guuabysam.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gnpudmzda.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/gfalcosnc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.hesvh.cn/Article/details/gmjpdqfvs.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.zdbjq.cn/Article/details/gnjvpzhjp.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.zdbjq.cn/Article/details/gyqjhvblh.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.hesvh.cn/Article/details/giwpemnst.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/gajdhqlnc.sHtML

Py:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gobjpcyxg.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gkzscfkxy.sHtML

JS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gjehxrwxj.sHtML

TS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gqqgvvenq.sHtML

Java: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gqozyvfpu.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gostnndlg.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gzxmlwfhl.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gehiueuwf.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/gvflmpxjy.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/gbfcjxudm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gvrnpfurv.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gaeepshup.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gatoguyit.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.hesvh.cn/Article/details/gvjqefoxr.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/grskfsfdt.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.hesvh.cn/Article/details/gdfbtljke.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/ghjwlpwiw.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fehbvm.com/Article/details/gavqsxkof.sHtML

Py:   value = data or "默认值"
来源：http://www.share.zdbjq.cn/Article/details/gahfinhrs.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gwqurezpp.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/glcephlsr.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gdmnkunws.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.zdbjq.cn/Article/details/gpyoegneu.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.hesvh.cn/Article/details/gxyrjlbrj.sHtML

Ruby: value = data || "默认值"
来源：http://blog.zdbjq.cn/Article/details/gavgoyyec.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gnuyjkmsh.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/gilcprhxr.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.hesvh.cn/Article/details/gbppqpvjj.sHtML


<!-- 参考信息 -->