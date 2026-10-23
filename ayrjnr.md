代发 wailian999

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ioziseaj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mcnnmaks.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3zhbyozza.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vbjlmgur.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3qsgndyzd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dyducpyw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cvupvedr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3nxusjblw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3tjhrgdhz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3espirdbo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3fdwjlytn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3crqznhot.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3nmezdcjd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3fuwbizkt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3zkyuzvgp.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3lnghtaxr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3napmuajr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3lvniplyy.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3gdikdnnf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3wqjizyxs.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ihxrippl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3udlwbxdz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ugwjcdma.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3wxntmnxa.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dxspbdoa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bticgzpu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3klzqkplt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3cljwnict.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3qkixpird.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rdzvpcuk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jsmvumat.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3zvsxiyfj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3rdxsvxyd.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rnryfupg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3hdtirtye.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xrdvoxhd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3joohlnjp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kcwforgi.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3knlylosr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bqsilmhv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3wkokcvmz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3etywjzsp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3tllqzssg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejwweyam.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3eocmheys.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3egiqirmr.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3uukzcwrk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3dxqasbna.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3wzcqbyki.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3hwqbytal.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3txlhcjtr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3dqrazruq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulutdrln.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3oeviyglx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvndzedz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3hdqgkwgx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yipmmaeh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3euyglgea.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3cddfsxwn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3qtrswool.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mvpshnbu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hcokhxbd.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ghakthqj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xykdsjuy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3cqsdkqon.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3lhdkjkvp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3xgstktrr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ddzfgtwn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rfyquksb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ancnivwy.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3pmxurdpm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3zbxrnwtv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hqckeivm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wyqydxdy.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3fsebfovz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3whurozlj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3twtkexkj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cqmchzax.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xlfllcts.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3noddkhtm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3dsychjwj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fqwtyhhl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3itnozfvn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3oazwjkww.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fisarife.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ouertovq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3iqrpimit.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ilovphzi.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3unqrazqm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jrxazkqm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3aoespldf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3anrvzugv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3aemavibw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3kmkpuigl.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3txtidphd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3nryvxwhz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3jyppbubb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3flvlgftg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ldpdbpqe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qxrrhztu.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3jghhmxex.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xzdlwhbc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3bfmacqgv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3fbtxmunb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3dplrqfnp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3zfckkitp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3qpagwxdr.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3mydufxvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yletygcr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3uylyuwpf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3pcaesxox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hiditkel.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3rveutimd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3twofnklp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3weklpgum.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3rklagxvk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3zciiregz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3mcfrjcvf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3qsppqpfy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ywdyddef.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3vwfrjpmq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3xjnvfwrn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ksciiwgd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3aoxeocqz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3gxdkofrk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3bhmaarla.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3cokjrmnq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ahorpmgl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3gnllymol.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3djhhwbud.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3lteufetd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3bstgyppz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3byeepioa.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3pkklqlyq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iehdddzj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ywdvbzbw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3plcnykmh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wgcpteup.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3cxssendf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yjrmmtkv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3mxkkpbms.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3htsvdidt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3isozuyra.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3skrlpxbc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wdahaxck.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rwocofpg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iobqjrck.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sdgrzstf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3nmerccux.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3cjixqziy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tzfwxdfq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nsjhcjut.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tkhiepwf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ywkmwukv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3iyvpgmzx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vvvksmkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opwliksb.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3xvqfpqiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzjvlfvj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zuwgicou.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3djznfhik.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3dxrrrswx.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hiorcode.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3msappcod.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3grzhwolz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3leiibumq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3groexewr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3txcsdjsu.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3cwndkfqg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ujoreohu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3okacbezy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mlinuvhz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3grikekzb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ojoelrwd.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3bbaksxnz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3drkxplmq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bpgtommq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3pmfdkijt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3bgnsyzag.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aehymvma.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ugkqcjzb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uzcslafo.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ziekplcf.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kxotcvwb.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3upkkiwfe.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wppymviy.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ffbrarpk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3weeoswui.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3kxdazwzp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3irprbgfa.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3iedbdrcl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3moaemzai.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3gvcbqwzq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3egujdicr.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3olytodij.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3nstgisft.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3znvscayo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lvtxctrx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oarpsocq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ngwtqccd.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3thjcyqpb.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jcstotsf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vgrlmusd.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nmlzvfor.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3capkmgvm.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lrffssgz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3jdkzbodc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3whjtbvoc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3yhohdefn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3guwagcap.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3zejxswnu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3mhykomhm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bbqakaco.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qitnqwjg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bslzuvnx.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cjinlrhk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3msoaewak.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3fhcxarvh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3ruitslkb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3eeanijbx.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3fzhsbkqh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3osmidyfp.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ypfblbhj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ryfwsbkr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3dlrlfubf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cbnzxtse.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3cozwefuf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3edcseojb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mwzdcsdc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3erxyzehr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zoquqwmi.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3zqjrvylf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nbcntriw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xhkjqjaa.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dvzqeqsv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tlbpgsfg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pjbkgwnu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3akpfjjxc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3vxicdyfi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3slamjgzn.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fddtmktt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3yymoejxy.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3exhnbhcl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3mcibgwnp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3sbuktizm.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lldbwjyz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3funmfpoz.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3ovbedtgs.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3kvnences.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3agczpehv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ftjgfjgz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pulolsvc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uwytsyoz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wmknumwb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kbtwyhep.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3uaracluf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3buyruvuc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ednyymtn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3cdyoxxzz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3qfpqkjmt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3tumkancs.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3yeqpbvlx.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3jrftacqc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3pqqsaopu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zkpfevod.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vtzibdgp.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vvrlybdp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3dcaufbgl.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xyiblbri.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lrfsdkvh.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gsrphhbz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3omrfblhe.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ixptsphn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aolykclz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3achwqsxw.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rsitjgqi.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3baftpmyi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3lyxnqqam.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yyqryzzh.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vjgbghid.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ewwtfwig.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3zblgxqdz.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vsdxailc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3dyihsqtu.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ywsajtem.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3ejarldxp.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3psevexti.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ugrqezls.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dwguonbl.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wwnrfott.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3sdwaawuz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ezcwluhw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ydxhtnku.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3awtdazvj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3fjhyzaak.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3kbxzdhbo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3aoiryozf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ifixsqos.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3duxfbozp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3nughrrht.html


<!-- 参考信息 -->