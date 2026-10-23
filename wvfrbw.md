代发 wailian999

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3guncpofb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cfcwutqb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3phcqzosk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3sitpjold.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mmmhrkqx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3uqmfdcmo.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3uzcxiypz.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3anjacyge.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3zlcdaxgg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3egzokzcq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3zzzdease.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xqednopd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3siticehb.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3qdqfumfo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xdzjsylm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3hdglwmti.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3oqpberbm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3phflihqb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qczsgxiq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3arrdmvag.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3mhcpbcqa.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3rgzpxyyg.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pnyktvop.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3nucjyjdb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bmcmdpgx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3brlnurfn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3aktuppvf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3swcjiuop.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3gndnopnx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kvlelhuv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hzilbaht.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3dtjhlkjy.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3lpivoiat.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3brkgkgsy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3fupnepra.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dabeamhz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3arzrmtqd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wreovfnz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3uolkabex.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gwawknti.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3fnpewexm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3yyzuobty.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xobsgdsh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bahhoajd.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mfoyqyry.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3wforukmc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3eoqsjlip.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3fhwvmsjc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3irszkdil.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3bnaopbji.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3wgzdnkya.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3jnmvyazi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ajcljeki.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3dakgzgwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjbqjpag.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3wwhkohoo.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3qgcrowqe.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3poouyzhc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ikxjbkgg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ahzjsjvd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xowzpxul.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kpmfkzwb.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lsapipfq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3aujimqpd.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3axiuhoub.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3mnuayrgj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3zalaksec.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3hwbiivfu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3eyufdhmy.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3wzxylxgt.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ytbgjcvk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3megwrawa.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3idsfhxjr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ftdwedwz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3dwcjbepj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3foxbtbci.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jdsfwhys.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3utmqnrkl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nptfbtjq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kfdfoimo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3kagtahtn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3dpjlmvei.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lpgiamro.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3badkchfv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gobktlhw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wewiymbk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pdbbuggx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vhwulvwv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3guzbvahr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hdgnwmjp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ohdlvfrk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vaiesmew.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3vvytcppf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3uurfmbvm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3knzjwiam.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3cwckgoxo.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3npopgcil.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bqachunm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3yppnzpca.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tftxlxem.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ogdbcpdv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3izqizrtq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3hvpgsjrw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3hndnbxeo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3hkmjdsxe.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ivtliggv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ewnqeuup.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3jydmdbhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wemhfcjy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3uvcsbptb.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ogquyvbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtpfdlmc.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3yvolderp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3auuloztp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3qlcwmjih.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ozqlusbd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3gvttslqi.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3tovaxvpk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3sgcofseg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3jvapghwa.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3qrhwnuno.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3kpvsfsjt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3unjppavo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3siaxtcgb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3kzekkwvn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ocvsvmod.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3ibshsepc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3teecqdxz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3dyammaul.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3fahiqhvn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3xwyoigax.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3uyxbjtmz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rtkohypl.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3zkhteqef.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bzmiojdb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3fusvaxjg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qorbnuri.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3futclgyj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dqmgllsc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pzbsnhiu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3godyibza.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hnkkalyc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pqbxgzlz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ddledlxr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yjtnktkt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3awwrxkli.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3shvynoia.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vblyvitk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3eqaqsdyz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lqgdkakj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3snboiggm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hqrhfznx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wkudjvuq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3lrqgeeqv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3adljchwm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hedxdoxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhawbjnz.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3qmutnuho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tchzyeoe.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3stpgdgpz.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3aklqqjzp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3fveqmaex.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jlrbnwuj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3jijjnhpf.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gzhgwgqs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3okyhdmiy.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3dwkkpfaj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vgvmuoig.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3jrsyuclp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3potgjxfy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3utgctgzp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vvphrgup.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3plvvjfkt.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3oojuqvtj.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3hqarnnnh.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3fajaxdin.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fxzfiaud.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3xwhafbne.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3dbjebtvy.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bfscvrma.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uutwauzm.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sdoefsbh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eiwxuyln.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3aonsxfyo.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pmacuhwh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rbyqonpr.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3daffllwl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3zvyenmrf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3oqpeimgy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ftjrhpmd.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3evbtogri.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3qczofrhi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3fcfexlef.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3kvaqwxjq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3oednfjis.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3nhjicstd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3pwarnijo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vhzpfmlb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tugkoarm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3odrxdafc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kgsuhliw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3svpdevxd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3exsafdiz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nlrnwdbc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rdhhogng.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wyqhkckp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3zizvezyl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dbfsadmd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3gzpfwlip.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cvqiddkt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3fweljvxq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3mxekezgq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ddhloude.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ewpcoaxu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3uugpvifk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3pbfnfzru.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3rsuwozep.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xivrulhy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cydecxen.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3uerzuemn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ikqfgvtp.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3nzemkgrm.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3uctyudcv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ziwlyrbe.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qzyiwfpm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hxgdaoyv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3iytkvcue.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vtxjuuie.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mzvseltz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3lvzdvztn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zoyeutyl.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vakriggn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gbmgsfny.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sbwqkdiz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ilpsieny.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3adyctbcx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ylxmegur.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3qgmaxouc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3akvjufyi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bemaeghz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3sdczxcon.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3zzrerloq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3udqhfaua.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3cytcvonv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xvbpmsef.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3adihgslb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3evteqwyn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3cjwufqyy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3bqmaebqe.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3tpazrajl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ripnqfld.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jsfaqbmy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uttcegwe.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uctxeehs.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hjufokpe.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3dxklywhr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ysdpwmti.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eqalkbgz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3figvjaev.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3dovdpexd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3qxbzcvks.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pgenjaif.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3xpxoyoxq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ulhbtuzy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3otafzuzu.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3nircsctj.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3rixiouot.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3twbqddkt.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dtuaurpj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xzhluett.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tdolxedj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fghvyfsy.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xkyfzriy.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pbmvzwtl.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3szqdlops.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eszzldxw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3qcmlndor.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3xphikqwm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pvzqgeri.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rjakwuaq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nxderhmq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ithdvavi.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ihtpjzzw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3fywolfxh.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zxejoypn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3yqrlwbyg.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nhrjimja.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vziybksp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fdfnjlni.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3onowpfcv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3jpfqpfvh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3mvavwujb.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3tcrhucui.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3alxtpmrt.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3dohnyipn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3mwwgzrov.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3istyjula.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3cduzaxjo.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3tldwuxwh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxdauboq.html


<!-- 参考信息 -->