代发 wailian999

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2yeqntoqd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cakllxaz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hsvyyvkm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ffbbfjxg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ntbxkrzu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2mbqpmkrt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2gaverhbs.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2mxdxojbe.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2djiqcycd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2uzrjyzpt.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2uaevkdsr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2zmkynwhm.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2rheaibyd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2xurqxjit.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2cjktcvql.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xwoymkmu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2eejigjmp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mtsvnycn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mqofkzmd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2hwsshepc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fhqkwlwm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2eiwsvpis.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jiesevqn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vprtxmco.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jshcklnk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2avimnxul.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2latsthfo.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2xdsjksbf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2tuiuzize.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rqiwfkbm.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2dbwjdqqp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sxpxrqdw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2srolgoqd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2goktufnu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2twizjbru.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rqpronyk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vvyxoggd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vphsmeve.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ipxupect.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2tbwjywkz.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ffihguzv.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2qdsqtjys.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2otrzerfd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2fawkenwh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2qouavkyg.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2glggrdde.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2qnlgasxc.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2uiqinvgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2olthmnpz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2odlnjoac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnjckvbz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2psdoydlf.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2flafktrx.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2bkskrqdd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2tnnrjodn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hfdqzorc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2isvsheib.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xxwxvsrs.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pfvpjzyb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hlbsjuik.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2pdqqgmrj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2wjttunfn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2pqtegivz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2okcxbzsz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2uwvqkujz.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ghivouvv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2jmaunwsr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2tipdkjcu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2gerzeyma.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fyzewmly.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ezpxltca.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2fzrluwez.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mbgrajcr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kkfvvkrk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ataxkujw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tsvgrxhz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ubgowrru.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2dylifxpi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wdqoknax.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2giomfwlb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rizmuhrs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ksoksgqi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2abrtjusj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vwxscvoj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jvgzokwf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2joiwyjbg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2orpnjtkz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2khcmhlbr.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2qopqdgcs.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2aelakheu.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2orznkgon.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ajwfnzjj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ahshckcs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eyonpaca.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dhbuxaks.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fqkrxovl.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2utyoljuw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ipbjckyw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ldxhgfzb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2enlhjtkd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2qgkajbht.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2efgimnby.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2jrqacsbk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2orszdgka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nliaewsj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2kuitokht.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ybopfmhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oaqgoltq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2xjkfzphz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2lzyhgmsg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2zencereb.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2xqkbdfej.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2eoqpjgna.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2mucnrizi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2yebtrput.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2dhaeubko.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2jlwfhkmm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2occigufp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2qceszlhf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2minrzviu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2nqhumlbx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2vfvjiybg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2zqqikstk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2nkwgzuyi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2xvpuhacy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2khmpxcbd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2fkaxingq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2pcbleomu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vcjoxrhc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2aoycddhw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iwbhtpfj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cedzsdbt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2bfgbhwel.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pleniomk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pspxixzs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2cbxopvts.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2qqdeijkr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gdrcopim.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iubjdwtn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nhyxasho.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hjabaqji.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fhyzrsxn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ryzkviav.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gqqvauad.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wdlhawrg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2surkaxod.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gnjvygvz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pwtzsdmc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qagupcfw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xsksewue.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2etinjmex.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dkmzpnql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbzrxxlm.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ncwqoqha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2joxmgyde.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xqybgqtf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2fiktumaz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2xzamtmwr.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zmqzlyun.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2icenvivu.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2dmlszydd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2fyoqmtnz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2cwijdpqh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zadonwxp.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2cfaaptjb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2kvdxbtch.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yclthrwz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ctdbkmuk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2jhxmvpzh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yhrkbwbq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2abaxxrhz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2valtwwwq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yyrzdsjr.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2kptkmczf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2gaidovla.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qlvaribd.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mkgulqtt.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lmsnbokp.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gxdnmwpr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kmaiuasi.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vwjxekjq.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zotnvetw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2stbxeoqq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2viwqwjnh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2fcstlccy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2tdqjfmje.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qgcbcixa.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2cwralxwg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2wjrtgsfe.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ryhrdops.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2tiqqzuyq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2kpmwnfuy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2qachiqed.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tpfjmqlp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ziebgpbz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tkzctqmc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xhiiilpy.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gehwchqc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yykdgdmv.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2agntqsva.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zermlcaw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bajcuafq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2vkjmtydo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ybiexdbk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cqdrntsk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2roompssd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2zpevfuyb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2guhtaaid.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nsbwernv.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2mtoeeveo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nmghuwqt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2udubtcxk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2sektzwzz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2vgwaahid.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2oafqxowq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2umkskhmd.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2alidacps.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2pmdkzxbr.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2kuvtadps.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2grpteplo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2tanrhuij.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nekrkoiu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2zvutnlhb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ewcgohmy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vhzayedz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2btpiaewx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ofovgbmc.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2suzlnfmb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bwkdrtgf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yshezjvy.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2isyxeobv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aisxssyf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cubinpqg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ufzykwdo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2zeqieebv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xmgkzcrv.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mqokbeqc.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2tdywtjzs.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2iiipbfjn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kxssstaq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2iprbylxw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dvajlduq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2scthntrl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ebieqpvw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2azoumzxv.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2xsjkvjhw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2lyzrxgtr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zuzhnlsk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ipmqrdxu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gbahpchl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ilkgnomi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2gxeqdzpl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rkdvxxqw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ivlczjxv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2kxookuef.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2xbwuqpuy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2vjftmmie.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vcdsdxxz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ozydarzb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vcwptpyt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lbrubdar.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hwezvxsw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2odgdkaar.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2fnjwlzth.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hvagrgol.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2peychref.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mqhkmklu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ohexowkq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oodhthqo.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2setawhtm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vbgcwzdw.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2telefqxi.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2hbwyhoii.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2lulxbixo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bdolwdjw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vdzhiowh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rmvhxzym.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2rfdsjbgg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hwvcuyml.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2iukjgxpq.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2heqscmyn.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rqugkpxs.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lfxreiki.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2boldxfbv.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2enidugvy.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2elfdehkd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2sosislgm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2faceusiq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2hoqkhfnm.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2enuyemeu.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ipgaqtvm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2knmfczow.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2ialhkylc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ghdrryhc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2obgjwrcy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcohztpb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2rcvcllbj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2qaebejci.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zairiccn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2qumtqygr.html


<!-- 参考信息 -->