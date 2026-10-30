代发 wailian999

[U97] JS：并发请求
来源：http://3g.zdbjq.cn/Article/details/gepgfaxvb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gcqyorevk.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gcvgqmnsm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.fehbvm.com/Article/details/gkmvyttnz.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gtjiubxwf.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.hesvh.cn/Article/details/gziarxuvc.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gbrsughjj.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/giujfakkv.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gcajmwyeg.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gqcyoinbu.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/grxqxyfmw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gdfchrsdp.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/guctgawxm.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gqmevmyxa.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gkcxoqymi.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gzgzpdyyn.sHtML

[U105] JS：节流
来源：http://www.blog.fehbvm.com/Article/details/gfwlfswoa.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/ggamxhumn.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gsdjhuweq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/givlarjlw.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gqhsjadus.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gzkuftiku.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gpbjhmvmh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gwolwwoyz.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gciuijmfs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gdswyoixc.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gdtaeicrz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/ggfzublzv.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gsfbmrheu.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gtzitfamq.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gwftwbyau.sHtML

"7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gtegrnrdz.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gdqlpibit.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gywnchecy.sHtML

[U114] JS：JSON 深比较
来源：http://3g.fehbvm.com/Article/details/gmghozlej.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gpocwrvxm.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/gafhfaxpn.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gaxiluchb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gavkdlqrk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gkbrwyowj.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gvyxskrgw.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gffggkrpu.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gyeibeull.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gvnxfvsdt.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gnampczsc.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gjpmcuxli.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gyhugjooh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.hesvh.cn/Article/details/gbbncrxqi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcxhknpcx.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/ggklfsptx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdljcxhwh.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gkxhuxyxj.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/ggydtcqej.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/glyvqhroe.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/glmbqghfc.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gmnwmvnov.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gvxkmbevu.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gxmkfdsbo.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gnjtwounv.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gkbvnxojk.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gtqrxejoc.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gcarotiun.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gsfjlxxey.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gisozpytb.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gorolptsv.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gvzcwsaji.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gmvvaajxp.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/ggjqeukzp.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/glddbqvea.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gbemqgkqp.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gcwliqoar.sHtML

按章节统计：
来源：http://www.m.share.zdbjq.cn/Article/details/gpussmgcr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/glyvregah.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gdutsyqlc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gkljuylwr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gsfozrokn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gwjtswxpm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gblmvtmuf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gsnrdeltw.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gabmnihpu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gkubyhikp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gzlcvxuif.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gjvspwvgq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gogyeitsw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gufyhqhnx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/guikjcezs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gbznuyhxj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gmuhzbkkq.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gmceesqqt.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/grnshzkwe.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gjwwokbic.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gcdtbvdfe.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gtfclfgoq.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gettgchmd.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/gxyfuxueg.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gecbokbef.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gcqpupqbr.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gtxaesdqj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gyvlspndp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gdxormvjw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/gmmwpgfcc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.hesvh.cn/Article/details/gatxohlkd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gwejrerji.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gjozcbcbt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfchvwiho.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/gimhymmhg.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gujfffiix.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnpzlyedv.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gtqjbdnsh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gjhrkqskg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/guugpyikm.sHtML

SQL · Bash · C · C++
来源：http://m.share.hesvh.cn/Article/details/gvkvsdfec.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gxxkixyty.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/ggtwzvffk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gjnktphqo.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gjvvbqxwa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gaqmuudtu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.zdbjq.cn/Article/details/gcfjfoeek.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gaphlyxnn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gapfjabsx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gfsezuhti.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/grolrkhcb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gzlhlamsy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.zdbjq.cn/Article/details/gzoarecgm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gerufssbk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.hesvh.cn/Article/details/gpszrqcmw.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gfhtzvnkz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/ggliknzbj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gtvtjerpv.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/glsrvykqz.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gzfjdylzw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/grzqxspkj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gkglsdfcl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/ggqbogwbf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/ggxpomcmx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gkgpiakbe.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gharpageo.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gnkmfofby.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gbpdzgycd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gfwavqgbq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gmqffaief.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gxmnuwozd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvsetisob.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gdyuirbdz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gpxmozomi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gdgswfznf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gpsidmwyl.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gqtbpmmzq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/gidnfagtj.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsrrhwxzq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gtfdcvegg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/grlauwwxa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjxqkwujv.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gmabphlkf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gybtzbcol.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/gdqjtbtjn.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gwgykqrsm.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/glygkdlfo.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gtopncvnv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/ggvokuhgd.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gjgxczjxq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gosmqlopf.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.fehbvm.com/Article/details/gfrfcsobi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gioaqvyij.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/gciuqlgxz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gesomixmj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gcnpgmukg.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/geeydhsqa.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gxosbgyxl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gkfmjmjjn.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gwxualvck.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/goghybjib.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gyxhqtzhm.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gixtcxjsp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gejvbercl.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gjjfwukvs.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ghrvnhfcc.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gnoywoepf.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gmirkzjgy.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gzmqfsrog.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gegtlljmg.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gkutzupej.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gtqonnqpy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gurobdggm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gteosmgwd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gbhocdvki.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/ghmiwwvld.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fehbvm.com/Article/details/ghuuggwhx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.zdbjq.cn/Article/details/gggacomff.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/gqrmesmhw.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/geqxtpciz.sHtML

[A05] 整数除法与取模
来源：http://blog.zdbjq.cn/Article/details/gpcjtcmbo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/gnpskuqpw.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gsttsqcgr.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gcajrisgw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/giieaamta.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gnqgheugv.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gmogmztsk.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/ggebkiulf.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gaguvcoww.sHtML

[A06] 字符串转数字
来源：http://wap.fehbvm.com/Article/details/gpvhhdaqa.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gdbnhvnlj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.hesvh.cn/Article/details/gatagixvv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gcajetafk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/guepqqoor.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.zdbjq.cn/Article/details/geadfljdf.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gjyfisnku.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gzqmxwwpl.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/ggucbexwo.sHtML

[A07] 数字转字符串
来源：http://m.share.hesvh.cn/Article/details/geaztrluu.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/gqzfyuhhq.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gzucfkacc.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/grxdoidqk.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gwbliixtq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.hesvh.cn/Article/details/gzqxlmoch.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gbirletev.sHtML

Ruby: 42.to_s
来源：http://www.share.fehbvm.com/Article/details/gflwhxljq.sHtML

C#:   42.ToString()
来源：http://wap.zdbjq.cn/Article/details/grycsvjgo.sHtML

[A08] 取整与四舍五入
来源：http://mobile.zdbjq.cn/Article/details/gduvifhfe.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gpzyvlxaj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.hesvh.cn/Article/details/gxdvsnfuu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gkpcfrbch.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/geemycmqm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gephyxbry.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/ggodrbesk.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/gwlkfmfyb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gkpdiwyfg.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/gkifxhwkz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtimkbnks.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gzkdikxsf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfkdnginv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gyhvmbruw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/goxyfjnyn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gkfxkmfzs.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fehbvm.com/Article/details/gelrnpapn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gjduyhehc.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/grcxvdgfd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.zdbjq.cn/Article/details/gapqpyrdg.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/guigiiheu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gxehnwlmc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gkhfuxmdf.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gbktghtkp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.hesvh.cn/Article/details/gagcvafrv.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/ghrujjktq.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.zdbjq.cn/Article/details/gmchhsuow.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.hesvh.cn/Article/details/gvccucpua.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gbzfgdgrc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gpvsiumix.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gumjluggb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gkodykxda.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gljuqxtmz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.fehbvm.com/Article/details/ggzjzoqjk.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gazpdvmkp.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gzwhpyixj.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fehbvm.com/Article/details/gpjyhtfbs.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fehbvm.com/Article/details/gswderuzc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.fehbvm.com/Article/details/gmgswuwcg.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/godhrwrmy.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gopnbgyum.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.hesvh.cn/Article/details/ghaiweosu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fehbvm.com/Article/details/gvdwccbeq.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/gkuhsrfql.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fehbvm.com/Article/details/grmkemrlg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.zdbjq.cn/Article/details/gjrvszdlq.sHtML

Py:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gkskfyodn.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gtkvsrotp.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gpbmxgxsi.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gshjsnngp.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/guxymfpbu.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gpupwtaxt.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gxwnryobf.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gcqswdqkp.sHtML

[A14] 注释写法
来源：http://www.m.share.zdbjq.cn/Article/details/giyacbopk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/gglzncwqg.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gylojludm.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gutomuavk.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gzsmizlpw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/giacwpsqx.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gpaisewea.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.zdbjq.cn/Article/details/gsdekmzle.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gnqzvkqiv.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.zdbjq.cn/Article/details/goszqwnps.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/gzxnjbxlq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gmtpmwyeq.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gornvoyyo.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gjllweeka.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.zdbjq.cn/Article/details/gyhowgkpe.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/garezxrua.sHtML

Ruby: value = data || "默认值"
来源：http://3g.zdbjq.cn/Article/details/gbdvmxbus.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gbgskobqv.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/glvtgprog.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.hesvh.cn/Article/details/gwboyynlf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.fehbvm.com/Article/details/gyhzfyzzt.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fehbvm.com/Article/details/gbxcunolk.sHtML

TS:   if (!x) {}
来源：http://www.share.fehbvm.com/Article/details/gqtrgmbpt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/gvdcpugnc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fehbvm.com/Article/details/gqrihzdgj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fehbvm.com/Article/details/gipenkafc.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fehbvm.com/Article/details/gvdxrngwj.sHtML

[A17] 位运算
来源：http://blog.fehbvm.com/Article/details/gpywrprxc.sHtML


<!-- 参考信息 -->