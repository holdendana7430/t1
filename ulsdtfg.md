代发 wailian999

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/guglgplon.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gpivykyli.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gchumodzu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gyupkpvby.sHtML

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/ginsiddei.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gjyygcpio.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gtosdmwtc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.zdbjq.cn/Article/details/gjesyrbbq.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gmsnxnnbm.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gtgynvayq.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/gzvggrgct.sHtML

document.querySelector(".item")
来源：http://mobile.fehbvm.com/Article/details/gxwjafrxg.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.hesvh.cn/Article/details/gnpvtpaqf.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gszmfivfv.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gjlbhdzjl.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gvtkzmyoa.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gpwrhlgvk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gnrttckkm.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/ggbkfeaaq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/giwrzpbky.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gfqmnwbrt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gwyxzxkum.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gzbjvkikp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.fehbvm.com/Article/details/gyzlsnaon.sHtML

[U107] JS：数字千分位
来源：http://baike.zdbjq.cn/Article/details/gskozpiag.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gmbsxnwwx.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gvfppfarg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gmfskdzvd.sHtML

[U109] JS：数组分组
来源：http://wap.hesvh.cn/Article/details/gntuuqlml.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gnqizhymx.sHtML

[U110] JS：数组分块
来源：http://mobile.zdbjq.cn/Article/details/gdzhjdolk.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gddjeckbe.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gwrackbyq.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/glwbalaxn.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/gfvwmcxtm.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gwzlkbqmb.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gzyxeners.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/greakoyif.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gcfyuvseu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/ggqacfkqs.sHtML

[U115] JS：生成 UUID
来源：http://baike.fehbvm.com/Article/details/gszzcuwkf.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gblpoeunz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gefjnklyl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gsbeigomc.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gznwdapqc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gnternuty.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gtskesoao.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gueegxdxs.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gsytaqtgk.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/ggqcdacte.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gkqkcfmmy.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.hesvh.cn/Article/details/gjuyflepu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjbygsors.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gqiiifpas.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcgxdfsxl.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/geztlpgfn.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gybxomtio.sHtML

PHP ............ 252
来源：http://mobile.fehbvm.com/Article/details/ggzllfluw.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/givkugrtp.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gpezopzio.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gkcahgvjz.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/ghhcprlvc.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gdykvovki.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/govhvkgkd.sHtML

C .............. 30
来源：http://baike.zdbjq.cn/Article/details/gsvvhmqsy.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gjpftzkuv.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gapuyenvr.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/geisdcruz.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gcbgensbr.sHtML

Swift .......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gfrgqfzpv.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gkefjucuc.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gwniwonne.sHtML

Scala .......... 10
来源：http://blog.hesvh.cn/Article/details/gvsaddghs.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gijiaanxp.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gswqrjxri.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gsmlpxuvm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gfcnzpbxq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gctzoqcnx.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gogllmxwq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gkppzhguc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/gobvjooop.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gyzqwgrzx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gtmtbfwkz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fehbvm.com/Article/details/gnkuwqfvk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gsgrsdypr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gnnncqymh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gcezzhyvk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gcmfcrsud.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/genvnsczp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/ggprcvlsb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gjdsxyaua.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gnstfebxp.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gxbzmdhhf.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gojhfujic.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gepdvtdwx.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gvjdbrfuz.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gvjrdwvgx.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gtkvrfrzs.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gclhppojb.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gtmunnuqy.sHtML

使用提醒
来源：http://www.m.share.fehbvm.com/Article/details/gghivhbvg.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gqtdkhubn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gwmbvaczq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gferkcbzz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gyqiyczsb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.fehbvm.com/Article/details/giosgjxdn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gthtyjsnc.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gruchkeku.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giqobdshj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/gcdgfcyod.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gzxuvdkyb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvecjoefw.sHtML

【收录内容】
来源：http://3g.hesvh.cn/Article/details/gjjnfgtqz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/glosveisl.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gfpuferwn.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gnzlpypot.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gllcyqahz.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gkbzivwpo.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/gvfgrewdb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gsdqhxffi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gtosyxdpj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gnlzktqdd.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gsvavttgv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gvgroknfg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gqrlirltk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gifbaphjm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gqzqvdpgc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gizqtwpvc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/ggonjorbw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gtcfqyyft.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gxwanntle.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gjpkwcwac.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/golscdkes.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gumtiymbn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/ggclvecqk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gslgqxohb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/grlzaqlft.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gciefmrde.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/glwkbhwea.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gmryxbipx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/galwovalp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghrklvtpb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/ggzhknlfw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/ghobqnuia.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gqerbcdjt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/geqrncdge.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gsoiffjyn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/grxhbsgzv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gsdonyukn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/gfjxiuhky.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjviksvft.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/gcxlttxaj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gmlvbzjjt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/ggcgaqlwr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gckeuvslv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gvmolbajk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmzrvdqvk.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gadbcnwrt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gshkoogdb.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/gzvluhkrc.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/gqhiaamzg.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/grqsagucs.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gojzpyqhw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/gncgnwneo.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/glpnknolp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gkpzthhaf.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/guzboisfj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gaileiwon.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gukiujcly.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gsyqfbret.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/giunuivvd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gytiofahm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.hesvh.cn/Article/details/ggafwlbqc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gnqnplblg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/gdinzjxgp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gpgavhusm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/guyiiahlv.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gwbnjvwxe.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gmhbiewxf.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gxlzmfjqq.sHtML

JS:   const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gbkkanlsk.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gkdfstfda.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gtsgcnrdh.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gnvbuqnji.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gmezlbfyt.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gelhgvgmm.sHtML

[A04] 判断变量类型
来源：http://www.blog.hesvh.cn/Article/details/gkgbbgxqx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/ggkdsnpcw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gmvzjmrzg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/ggrkmxbpa.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gqzajssyo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gchfeoxil.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gsrkfpxbi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gxpriqpiw.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.hesvh.cn/Article/details/graerbpkc.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/glrvdnhzh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.zdbjq.cn/Article/details/gdbzizjjo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gohamsvax.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gryqzaqov.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gkcfbsqml.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gvtlbsycr.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gdzidqyne.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gcgrfxdyk.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gftvmznnm.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gxswarlpq.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/gsafpiwpq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gkiodlpcb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/gnkcgmpeq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gnymytrtv.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.hesvh.cn/Article/details/gasfhfmfi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gcowdsmzg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.zdbjq.cn/Article/details/gznfnszsg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gicywoqjx.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/guppkaefa.sHtML

Py:   str(42)
来源：http://3g.zdbjq.cn/Article/details/gzepieuwg.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fehbvm.com/Article/details/gysuxhzdq.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gznnosplt.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gbdcwtgth.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.fehbvm.com/Article/details/goiekuwrx.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gzltoopju.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/ggkfhvkgq.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gfjjggxlp.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fehbvm.com/Article/details/gmhaovrwj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gdeqkakqe.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/gdlrirpfw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gonmvpegs.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/gtzttwjyj.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gykjmqykx.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gxsyobofh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.zdbjq.cn/Article/details/gjdoshcxf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gtnscmknq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gkjdxyzgj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/ghllntuqn.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/guovwzlub.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkcyzcvhi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gyssdgung.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/ggrvlxuyx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/gavfdoycz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gaxiqswqr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/glfqcsdvr.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/gwilomtnb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fehbvm.com/Article/details/gpeoxrgwl.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/ghldkacue.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gkuearucj.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/gmmnvkrpa.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.fehbvm.com/Article/details/grbuntvpp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.fehbvm.com/Article/details/gyineibsj.sHtML

Ruby: rand(1..100)
来源：http://m.share.hesvh.cn/Article/details/gjwmrsakg.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fehbvm.com/Article/details/gkamhbvkl.sHtML

[A11] 条件表达式（三元）
来源：http://3g.zdbjq.cn/Article/details/gmytujjsu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.hesvh.cn/Article/details/gbduusbyw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gujluvdai.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gcuopnkiq.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gedsuviec.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gtwtmfmea.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.zdbjq.cn/Article/details/gzwcgwrxq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gdszixvqa.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gzjwzhmcc.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.fehbvm.com/Article/details/gssnlsypn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.fehbvm.com/Article/details/gmflvcdpj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/gdaapcaxi.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/ggzhlmiqe.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gxzewzvgw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/gsnemztec.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fehbvm.com/Article/details/gnwwjrxpx.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gimoqalvo.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.zdbjq.cn/Article/details/gdraktzca.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.hesvh.cn/Article/details/gpfnfdnvq.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gauztqdwp.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gberbkcmh.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gadumavsc.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/ggnkwmbml.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gnqdaeine.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gzzeroidj.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gifkrdowo.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gnizitspc.sHtML

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/gnqhcyvth.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gumwreiaa.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gtbixqshv.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/giobuklck.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gcswoivru.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fehbvm.com/Article/details/gkybvtgna.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gtbaskngv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.hesvh.cn/Article/details/gjbcrkhta.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/ghhhiqvyn.sHtML

[A15] 空值判断与默认值
来源：http://blog.hesvh.cn/Article/details/gqeuyeqig.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fehbvm.com/Article/details/ggkirkien.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gyslmatda.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gzhvisvqu.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gqqqfrhyh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.hesvh.cn/Article/details/gkjbjzxma.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.zdbjq.cn/Article/details/gsjtohsaq.sHtML

Ruby: value = data || "默认值"
来源：http://baike.hesvh.cn/Article/details/gbcuzjiwl.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gjeuxctah.sHtML

[A16] 真假值判断规则
来源：http://mobile.fehbvm.com/Article/details/glgpldtvz.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.zdbjq.cn/Article/details/gsmumrbha.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.hesvh.cn/Article/details/granwlmvx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.hesvh.cn/Article/details/grauboues.sHtML

TS:   if (!x) {}
来源：http://3g.hesvh.cn/Article/details/gbcazdmgp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/gjvbacbmh.sHtML


<!-- 参考信息 -->