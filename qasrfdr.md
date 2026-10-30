代发 wailian999

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gnnsvmegg.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gyznxilmw.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/gbwmhxvzk.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/ggpwfzxzw.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/geebietfp.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/ggghkisqy.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/glctpxtiq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gruanutbx.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/goztyxajx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gsuidjvhk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fehbvm.com/Article/details/giqekbtfv.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gvgcuohgd.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/galxkquox.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/gjvufvpub.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.hesvh.cn/Article/details/gksrbwpcg.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gmmamsylp.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gjbjqhlyp.sHtML

el.classList.toggle("active")
来源：http://mobile.hesvh.cn/Article/details/glrzhmmus.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gojeljyon.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gcroajllt.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/ggapablrp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gnwbduymv.sHtML

[U104] JS：防抖
来源：http://3g.hesvh.cn/Article/details/gjexxiyrl.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gnwylkeme.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gotawhled.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gtuwxqccq.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/ghawhcrip.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gqbefssce.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/ghlbgzgfb.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/ghewewpyn.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gihygmmjq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/glqoymeyg.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gxvghjrzz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gkzukaats.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/galyhmhsm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gflpghsjq.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.zdbjq.cn/Article/details/gsjbmljpt.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gsdfqxqux.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gqxekuksn.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gizogkygw.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.hesvh.cn/Article/details/gcmyzdkts.sHtML

s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/geibwedws.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gdehxenyi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/ghnkjjuhw.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gcnqignaw.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gxjlcdcnv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/ghjwteiyl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyznhvnzt.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/gkevlbrmn.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/ggzbtlfng.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/glygdamdn.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gnzxqdgar.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gozlpcyij.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gdzqsdjoy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gthzuqbxq.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gbejggsff.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giilqgnib.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gckobfyfb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghqgjxzkp.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gutevhipe.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gllortekw.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gtpbiyaua.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gcsvssvrt.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gtkzkyuaz.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gkgklalsb.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gsofebpmu.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/giktpccfi.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gbkgzgjux.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/glkrgpfss.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gojovjeqc.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gtfqplzio.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gadajltvh.sHtML

Kotlin ......... 15
来源：http://baike.fehbvm.com/Article/details/gelkdkiae.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gwuhfrnop.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/godfttydq.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gbgpijgio.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gdaqdgqwc.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gsenqgblo.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gonrrhowe.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gfkelmntj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gwfpjcrsb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gbyvrdnxe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gbpolcihj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gjejeiuie.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/glnazvhkg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/geidydqet.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gcqahyjps.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gpmgmmpbg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gnzhejueg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gsebwzyhx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gupoanmdn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gpehqfave.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/ghsotswws.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gexdsphzf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gkzkwzrhu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gqhtkmofp.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gentkrova.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gayoovrij.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/golexltog.sHtML

T 其他语言补充                          60
来源：http://www.share.zdbjq.cn/Article/details/gaermjcee.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gkyovpwze.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gguriqwrq.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gyfkhapza.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gbsfycfvy.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gwsvqfqmw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gqtbczvsg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gfizfwupa.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/ggpqdsggl.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gvvlssiwt.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/grwzowkhl.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gcxpwlypm.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gxmjxqhbz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsdrotzgx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/gugetaihl.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/ghjjvydia.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsjcevugv.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gqvsaquyb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.hesvh.cn/Article/details/goyscwkqa.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/ggmuqhsdg.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gfqhabelg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gjqabflib.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/gycwynkyg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gzclxtqxo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/gaqmpjcgz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gfhoyqubb.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.zdbjq.cn/Article/details/glurkpduu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gnxrhadxx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.fehbvm.com/Article/details/gwghytqbs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gdmweosfx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gutzlgzwu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gumeuzdfe.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.hesvh.cn/Article/details/gbsabfhja.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.zdbjq.cn/Article/details/guoyfzcax.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gfkkabfiv.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/glfwouzop.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gmkhatmii.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gcnjxrcvo.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gnljtifgy.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gimuktimk.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gvyiyhbne.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gprksfvem.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gsoaqutim.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gcgzzocdt.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/glzqpngsf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gvxjswhva.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gsenumtlr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmvlmodcn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gncgcjsxl.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/ggfncwubb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gkgtuyvcc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gxdvuqign.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/ggiwizwhj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gzdhwmpjt.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gcovlryej.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/ghmgprywb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.zdbjq.cn/Article/details/gtemzuoqz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/ghpuxleib.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gfubweaxj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gtugpzbei.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/grqrthqhd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtwpvndkr.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gxudzmpkx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdsfehxlj.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gmlslyeur.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gwcgvhdzn.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gmtwvlzeq.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gokcykcha.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gqxguvnye.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gzwvdndpf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gehdbsrjw.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gnshfrwzl.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gzbkuqcer.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gndjskitx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/gthhhambm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gcuogkaco.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gkvsinmua.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.hesvh.cn/Article/details/gepjkkwdj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gkubfeffy.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.zdbjq.cn/Article/details/goblulxfr.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/grvrzphzr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gatkynond.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gdhyctemo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gtnedyrit.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gqdjcubzt.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gonvrhgti.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/grcfjzykg.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/geqcrpggs.sHtML

Go:   const PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gsbaplcnc.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gbnplzpdf.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/grznkqnoh.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gmgivsbty.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/guxxiwsro.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/gzasvgpay.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gzghlttwa.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gwpuqzivn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/gpmzaqlyk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.hesvh.cn/Article/details/gwmqxcrll.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gwirornpn.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gkpdwslfl.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/ggenkfxmr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/grdguplzs.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/ggcfwurrf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gbkdjtcot.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gcddcmunu.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gwrnudhim.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gbkcganla.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gbouhqgea.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gpfzmemsx.sHtML

[A06] 字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gjawxivvg.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/gbpygqwyz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gizqhdwky.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.zdbjq.cn/Article/details/gynxntoxa.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gfpsboota.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gyvexsmnt.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gmigynoys.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/gvpxmwukb.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gdumcfiof.sHtML

[A07] 数字转字符串
来源：http://wap.fehbvm.com/Article/details/gonptsvrl.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gzwgythxu.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gfeggvhzj.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gutrtzkjb.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/ggjeuwaos.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fehbvm.com/Article/details/grqgycpqa.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gvvyenqvp.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gyegyqbav.sHtML

C#:   42.ToString()
来源：http://baike.hesvh.cn/Article/details/gazjpzowx.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gwrowxwoy.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gdnqydskl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.hesvh.cn/Article/details/gptuyeebh.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gpkcgrujy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/gupwfgcnz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/grvfalfom.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gwguvursb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.hesvh.cn/Article/details/gblcpmdea.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gwemzkakd.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.hesvh.cn/Article/details/gdknqndoi.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gztvpkbrt.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gkycizutm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gjvtacuuw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gezkeeefj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gniojfhwb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/gbukqwtya.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/gsycvpwyk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/garjyayod.sHtML

[A10] 生成随机数
来源：http://www.blog.hesvh.cn/Article/details/gkxxrryfz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.hesvh.cn/Article/details/gcynnsvus.sHtML

PHP:  random_int(1, 100);
来源：http://blog.hesvh.cn/Article/details/gdbmbixie.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/gbdjrewgc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gwcefvjtb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gznyviuqj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.hesvh.cn/Article/details/gnsxlhsbi.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gwqjatmch.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gpqefhhqy.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fehbvm.com/Article/details/gzyhvdbjj.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.zdbjq.cn/Article/details/gjsqpsnpq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gwwimlohj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/grxyohvjv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gtimezhxw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/glcuiyexz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.hesvh.cn/Article/details/gdcpaaiuq.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gpjuyfzmw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gsozcyuxl.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.hesvh.cn/Article/details/gzlxidnjv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/glqngneph.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.hesvh.cn/Article/details/gpssimtyc.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gjcrallut.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gookhqhbn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fehbvm.com/Article/details/gkuxczois.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/gcnqcllse.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.zdbjq.cn/Article/details/gphdifisc.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.hesvh.cn/Article/details/ghtzgdwdr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.zdbjq.cn/Article/details/gltaprrbk.sHtML

Py:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gtgjolsqo.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gxyzzdapq.sHtML

JS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gjctspkku.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/guxocmyvi.sHtML

Java: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gtigqnofe.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gioosknnw.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gpobezbfj.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gcjasqore.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/gzooxohnz.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.zdbjq.cn/Article/details/gmqlelpso.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gavuikijz.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/givpavplf.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gqdwgpqgh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fehbvm.com/Article/details/gsujuweit.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gicvyaynn.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.hesvh.cn/Article/details/gdhmpckqj.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gjhkitdbv.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fehbvm.com/Article/details/gwrktlfek.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/grozzukfa.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gcbvxzelr.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gmcbrqzrf.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gxekadvtk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.zdbjq.cn/Article/details/gmbprjnab.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.zdbjq.cn/Article/details/ghbjnyskl.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.zdbjq.cn/Article/details/gropmsomr.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/guingahip.sHtML

[A16] 真假值判断规则
来源：http://www.share.hesvh.cn/Article/details/glnfodnux.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gjevwpswh.sHtML


<!-- 参考信息 -->