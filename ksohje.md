代发 wailian999

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3coqwnhtc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mwrwzklx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3uzbtletn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ygippjwj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ycwmlsqy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cwcgjnsv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vytobwqc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3kvtntoqf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ddqxkozw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3bszadyok.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3mpvndhdi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3jhonbsul.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3uouvdtap.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3qaitvrnc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3vzgjtsbb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fdubmrma.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ftendpft.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jcjsuxvp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fdjximnj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3elyblkho.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hykmqmxw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nunixmod.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3mdhhyvui.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3pdeoyadf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xvutfioh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3csdxuqcd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gamjjzkt.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3iineetkk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3yusyjvmd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3pdrresiw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3pfznakhc.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cdanfoez.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3mqixhvyd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cxpgbgzt.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3oliqziui.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zfbgjhcf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3josgrsfp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lleonxyr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3nipvwfnc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzjwqvzr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vrwnjqxf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3gmgldmxy.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3snpnlokg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3nlphnzep.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ndctdbqp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3xzfdkmxj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3flrxftkn.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3oixndzbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvdugekp.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zlcqorts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwicxsox.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3dgccrejn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ibsebhsv.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3vflslbmv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yhnfdqlz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wiozloru.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3qxcpxcwk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hlmavxul.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3usxwhwav.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ufusvfzl.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3hnxqtfdb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3azlgvyao.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3loaxvotj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ohmyohar.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rzkaduow.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3johgyjaj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3xyfxzlxn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ddhzekki.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3cskhbvdk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3smuokpxc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cycrulce.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ailwvjaq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ljyhbsmx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3keorkeon.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uhimlomr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xhwyjdve.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3fyypkrwb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ifytdjqo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ydmjnigq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3bwygxcyn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kdreeruv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pyqlnbkr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ecilpnzf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3niwfwgdb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hglltymh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hhbaycpa.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3huowpgha.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pgancteb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3phloismy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3jukpflya.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3vgpikckm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3dneeijkb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3kcowxytz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gwnfrwbv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3thdcnwal.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3heoximwe.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3euvfyyoj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3arsfpruy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3vozyboae.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3hldcjynp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3bsnikwsc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3fusjkodh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3pyaysjpx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3vhqtourz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbeneupj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3ghdybbqm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3lhjziofh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khmenris.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3prlfrwyo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3heqlttmb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3akxwevwb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3tfqpcfkb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3lqcqyzrp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3kblbqlas.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3vrybtmfm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3xvocnuet.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3owebbuwp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ghzopbfg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3fwahnkis.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3yccxctly.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3geermgon.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3kmngntmi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3byawjwqf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3eetugfuq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3tlkwnpof.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3celdraxh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3xuqjbaqb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3gyjyxopp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rbkbbhwn.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ushqpzeo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nnidmwpx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hrzzobzj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bcyfkxmh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ptciwrmz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nprbhfbi.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lhpqwxge.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xsbtfgdd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jcjdrkiu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hugmcfdi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uwadkljl.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3skthjbqk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ftddsjki.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cfqkztvw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wixdabyt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nqxhysaq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3bupdpmrg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ccvetqdw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3cxcsiygb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bcrxskqn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vgzcapyo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xarxuiml.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rrskpslw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nnpkxspg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3stdflxnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qowbwucc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3adezhdei.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3dnrbobge.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3nobrqtwy.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mwlcasii.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3sqapmakh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3emaurtue.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3alxeethn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3kpvwowwu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xpeqznyv.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ldojwwtn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3rqykoayi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3njuogpxd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dqnlxcsl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3tnzrexxw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ppzsbcrq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3beuzrvid.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3cvntevxb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cofyqxvz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3tiozwkxz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3cxlbwflx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jfrytkjc.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mrtqamph.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cysacern.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zrtsurnr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rhtxvzuz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mgftbqvk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3erqyfonw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vqxkacyv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3chmvqfpv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmdrzjaq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fcjowohb.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3klvgsnzm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3aedpcfcs.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3kvekgclx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3vsdnlrwt.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3yhhtqgqb.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3btfegjfj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3jivfelfu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bldffupz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rlzofgzx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3svnjfity.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mzpigcyc.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fwqnrsaw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3krubyvfm.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kegjywrx.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yyoqgsaw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zxywydhx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3sywzpnpm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nbwbiwkc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3aglqhfkd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3afwcysby.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3jeyppgyu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3wjnpophj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dxfbhivk.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nquysaea.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3paxfbbmn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3halqydtb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3acejvatv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3bvoirmlf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qvrbshjc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3rvmxuzxx.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3pmdluyeq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3gsrhixyl.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3pgakchai.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xmtpsynx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3xtzoukre.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mymyyaxs.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ufwiiitm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tvogeecd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zifhvgoh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3xbbrlmxv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uvkmbsjp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wazobuja.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jkjzzxgf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tqxajfhi.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zbdylscy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3blqucydp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nshevnfl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3bpcwajzd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3sievymwy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3armomgxu.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3qjcdxdsp.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3fcdaapdt.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3oxbsedlf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bqwyvrtg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xyifugem.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wfoecrha.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3kdiptlyp.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3frjnujsu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3cjhhcfxl.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3czwyfgbj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vscttrek.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mncqcqfu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ztreoejn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3skafbjaf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ummiumqu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3thqbubao.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nfndcvhf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ooippyjf.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nfnppzef.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3drmzkvlc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3hxvswttm.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3bwllgeiy.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lrkkmzzr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3nbqmtyzi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xvmeysyt.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jcrulygi.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3qhiyyzyp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3dxzscyxp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bdrefcls.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fqkcxlze.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3irsauqwj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ocusxgvj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yrwblshk.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dvqkmivs.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3egksdyvh.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ofigctwv.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3cilbubyh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3pexhjavn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yknmthjo.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lqxodgxx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ligtzjto.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3yclksvew.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ikbbebkx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3irxxiylh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rqnuoywi.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3aermunza.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3bryotdya.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jkdlvujy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zzqunrik.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3btwkfaie.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3oczlvyvm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3teappaxi.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3rebnlyjp.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bdnrldwz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3tuvtkzgt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3kzzxsyvo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3wwxqcazk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kyupyjkt.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3hbmzfvbc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3eelhwfuk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ndzltrga.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3kovqioan.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuybevtd.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3wkbxzbfa.html


<!-- 参考信息 -->