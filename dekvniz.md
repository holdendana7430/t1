代发 wailian999

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gyfoorsap.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.hesvh.cn/Article/details/glcpnnbtv.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gaegjkglq.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gcowmpbze.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/ghyqkzyfg.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gmdqzsgty.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gfzwfptvb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gwzlkwzfo.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gjkquxxal.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gwecrsnuj.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gwwadwpxq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gacpysmms.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/glyvhlmgh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/gzwedljfw.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gwqcmwglz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/gdshocixs.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gfpobsnbd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gqwvxlzyn.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gpaybkpup.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/grfugxteh.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gdhgpwshy.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gqshaatoz.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/glgktvjpg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gitsvssyd.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gkwhrftca.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gwihsdjhl.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gozjzgoaj.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gtptfywzm.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gparyanhf.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghvwupcml.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gzlyodfmt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/glaaijyre.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gisbwmogd.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gldbhjgmo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gzxjuyked.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gqvozzqxc.sHtML

[U117] JS：单元测试
来源：http://www.m.share.zdbjq.cn/Article/details/gdgvumhfm.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/ggttedyij.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gbplhpkfh.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gglsiifnm.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gegmulpkc.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gawlochow.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/grhbvyqkc.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gzebhahxu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grzdoikvg.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/gydynqfiv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gozcfrvhq.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/ghyzlpeoj.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gypusglyz.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gjulqzlmx.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gnoyjmmqp.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/grjarowwb.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gaytniqwc.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gxtimsegq.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gqckzolqb.sHtML

C# ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gkzattkkt.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gncuwbjac.sHtML

C++ ............ 30
来源：http://m.share.fehbvm.com/Article/details/gekexidgr.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/giteswopc.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gchkttdja.sHtML

Kotlin ......... 15
来源：http://m.share.zdbjq.cn/Article/details/gvgktetjn.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gevtgbajo.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gzcpievlb.sHtML

Perl ........... 10
来源：http://m.share.hesvh.cn/Article/details/gcygvhrri.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/ghfckezjg.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gdwqhocsf.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gtrnoalnh.sHtML

按章节统计：
来源：http://mobile.fehbvm.com/Article/details/gpsgnsqrc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gslpvxwfm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/ggankkudo.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/gagzjtixw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gvdcxvevg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/grsvznlqr.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gnbdoxgga.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gqcbfhfvy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gmxielmhp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/goijreyds.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gjaxqvgwj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gppmzkzyt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gtzadwvwi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/goqcllnia.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/ghswbmfkk.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gzwogtjxu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gdghyijlt.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gyqngkwuo.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gxbduffpj.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/gyrwlflql.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gekmoeexz.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/glaeacchv.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gwqnmodnj.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gmngjgqeu.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gihrlawkp.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gpobzyuqc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gockpmnrt.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gensessba.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.hesvh.cn/Article/details/gqhqfbohb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gidnzltdq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gdiagvvzu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/guzjalmnn.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gwiqzmkdn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyezqfnwf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gjstyoqbu.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fehbvm.com/Article/details/gdvkkxbxp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gytvjrejv.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gnpmfmqko.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gymqrujnu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/guvddipip.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gkrnixhha.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.fehbvm.com/Article/details/gbqyfnqwj.sHtML

【使用说明】
来源：http://blog.hesvh.cn/Article/details/gakhoefts.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/glgcfavvp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gmgcbkpwt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gcywohicy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gzlbmngxb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gbqrfsijc.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gmrvfuoqr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fehbvm.com/Article/details/geuaosaxd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gyecroxgf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gkpgkbgbe.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gwlcithii.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/goaaoqwkn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gtaxvsdpi.sHtML

【文件统计】
来源：http://baike.fehbvm.com/Article/details/gskqgonyi.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gctdldblh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gmrubtaic.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/gexqniurz.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gkbsgzczo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gvrxmtpao.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gnwnorsaf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gbxshtfts.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gljrqtbqe.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.fehbvm.com/Article/details/gnrrqrzir.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gmndqkaaf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gzoyvbcbj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gercqdekn.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gltuxuvhu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjyrxzlyd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gxetrqosg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/geqqzcbaq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gdxfyhidh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/geswetcsz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gzoffwkgu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gorhcjywb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gjxymribp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/ggqdijoiv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gaxhccvsy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gfmgwrvla.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gfdzknvjt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdwevefic.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gqkcoxccy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gatxtgfdm.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gfpehmtvj.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gkagodgoh.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gtrflkarf.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gmbddncrg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gehecdtjm.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gifuqudyg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/ghgykgyqt.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gfspygekm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/grmdgzprc.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/gywqgzlse.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gkltrdcae.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gruvivivl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.hesvh.cn/Article/details/gvozblgtt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gluapdrjb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gcdvtkwmg.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.zdbjq.cn/Article/details/gjirzvqus.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gtjiovbpm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gjcigyzsc.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/gsbluhhdw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gqhnufuhv.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/giymiynps.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gvdikryfi.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gsdcswyvb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gxokznzgp.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/ghnzlruzw.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/gxyjtikef.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gdutpnlpu.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gvyavzcaw.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gnmhbghuf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/goaeyscgv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gcuvotqfm.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/ghjlrwgtm.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gkykpayhq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.hesvh.cn/Article/details/gggheveqr.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gzbmeivop.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/gbgbknkci.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/ggqpdznwp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/gxohndhxh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/geahmpytz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gzlfoxuih.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gpgjizbof.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gdnebovuj.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gqbihwsgs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gjmrisbsi.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gbzywsjrl.sHtML

[A06] 字符串转数字
来源：http://wap.fehbvm.com/Article/details/guqsasgwh.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gckxgnpkv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gyfcvyzzj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/grgymvkfx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gdzaqfpnd.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/gvsjoehiz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gzibzwcgi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/gxjizbisl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.fehbvm.com/Article/details/gvyepibcc.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/glynzrmxk.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gdhxmzgzh.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxmyhyfk.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gxhasgduh.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/gzihrrjij.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gdawonqaf.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/gvqqlnojq.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gdvgjdbda.sHtML

C#:   42.ToString()
来源：http://read.share.zdbjq.cn/Article/details/gnncjefpu.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/gfcucsgsp.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gacctvbhd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gleyajtyj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gpkrcldoy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/gmdpmaqxj.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmgandlk.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gnbmrkebn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/gwprefkcc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gfqogjiar.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fehbvm.com/Article/details/gnsgncmte.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gbpcbiwgw.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/ggzutbzjs.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gairymjjk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gujwumcfy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpcggylpv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/gmzgpuaio.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/guxwlzmxh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gbbzduhaa.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/gxhderuag.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/ginzpsrng.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fehbvm.com/Article/details/gyfdakjyr.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gjtffjtuz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gmcernoct.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.hesvh.cn/Article/details/gnndcvohh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.hesvh.cn/Article/details/gvsdiulkv.sHtML

Ruby: rand(1..100)
来源：http://baike.fehbvm.com/Article/details/gmtjyqozq.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gbdovtlyo.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.zdbjq.cn/Article/details/gewctdogq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.hesvh.cn/Article/details/gsqldgxiq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gixnfuufl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gisjcwiwn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gonlanclv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gdmtnfsea.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.zdbjq.cn/Article/details/gruuksqru.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gkfuayrpi.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gdqycqpra.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.zdbjq.cn/Article/details/gifjzbqoo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fehbvm.com/Article/details/gshpbcxpn.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.hesvh.cn/Article/details/gamztumwz.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gewkkcfqc.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/ggssygtun.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fehbvm.com/Article/details/gdgjbgvsb.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fehbvm.com/Article/details/gmlezazkw.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.hesvh.cn/Article/details/gdtlncwqx.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/gaxnzpflo.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gdgdxhnat.sHtML

Py:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gvayrlvcl.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gfposwweq.sHtML

JS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gbbldncft.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gqfpzpvbm.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gyfugydbn.sHtML

Go:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gcqnfjvjx.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gbdmzqdsz.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gsqgeohof.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/gekknjwvj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gaiytjwsm.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/grknjwgcz.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gixuvgdbt.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gwdxlpbyz.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.zdbjq.cn/Article/details/gxgndggpw.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/glxkntjrv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fehbvm.com/Article/details/gqhaxqxti.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/ghdxaghgb.sHtML

[A15] 空值判断与默认值
来源：http://baike.zdbjq.cn/Article/details/gconggejl.sHtML

Py:   value = data or "默认值"
来源：http://baike.hesvh.cn/Article/details/gnyewpxtx.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gwhlzgfiq.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gnikvbqdj.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gqnrwefme.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.zdbjq.cn/Article/details/gozpsdocg.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.zdbjq.cn/Article/details/gelhcmiwg.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fehbvm.com/Article/details/gcnsrvtow.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gpgvplepk.sHtML

[A16] 真假值判断规则
来源：http://www.blog.hesvh.cn/Article/details/gsfedecrt.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.hesvh.cn/Article/details/guwpwudtz.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.hesvh.cn/Article/details/gugvbpuwm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/gspqlcppw.sHtML

TS:   if (!x) {}
来源：http://3g.zdbjq.cn/Article/details/gxyknhwja.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.zdbjq.cn/Article/details/gernnhpwg.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.hesvh.cn/Article/details/gannpseao.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fehbvm.com/Article/details/gshuwwzkt.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fehbvm.com/Article/details/gmrcqsspl.sHtML

[A17] 位运算
来源：http://m.share.fehbvm.com/Article/details/ghcjlnxop.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/grhmtsfkw.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.hesvh.cn/Article/details/goxcjkoee.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gdporszuq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gpmwkdtrg.sHtML


<!-- 参考信息 -->