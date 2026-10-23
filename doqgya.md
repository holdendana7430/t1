代发 wailian999

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3juphilfw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3seqvthrm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jjolvfvf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3iqqpyxaj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qjhvuduh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3xhswhabd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3rubxqmco.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3yhhenhur.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3tcxefpcl.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3lscapfdo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3cpksbqje.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3roztxlrx.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3xlzdpckj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3coozmaia.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3kmimpezd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3siqbipuv.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3oyroxyfn.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hgbhlati.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qrmhgkap.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3mkoojpui.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wdqiotji.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qsvnujcc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3eyvrkjwm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3uzswgdwm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3rbuzifji.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ihhykpht.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3henwqjdg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3eplvrkeh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3txlajvch.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3odkbhvmm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3dmbfwrar.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3addqqoey.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3slbksjia.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gcmqxigy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3klrmlkkb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3meqnkzut.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3enqnrhgd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cpddjwwf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3joivqivd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3npbxgevj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3vmxljsih.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3icazplst.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3gpffyflb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3ozlyymeh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ogfxyorq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3yksawlfn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3wilvcgcu.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3dfhagrix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzzovdaz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3qyusfzoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bcernpae.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3grjmixvt.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ccjlcnqy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3twgxspgy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hjdeizrb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3bdjnurte.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ysfyznll.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3mgjejoab.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3fvfcljxo.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zfhibynl.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3oxlwmclo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ydevkdoz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3hxrflmqb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3tshblkuj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3lhkphkvq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3kmnsmycg.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3zgfzepoj.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3cwvbkqaw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wowjfvka.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pxddduqh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3orljtokl.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ctrrfamb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3crzvwslm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3oylfljvl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3updleuke.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3eqrstpyw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3xikamkge.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kdmjgtai.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cvoxkhlt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qklscchp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ywnriruw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xtzyvjls.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tfedxkfq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pwfnerok.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hxgldvvg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3trtnkmgk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3mhgyhybl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uncggjid.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ynbmowat.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3snbtsmml.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3vosghmsg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lloocshs.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3lebahnvh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xtjhujks.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3yofsnvru.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3urwzrfzw.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3cwxjsuja.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3npyikosn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3emupboes.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3hpmdxfog.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3zdmriean.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3uslnmxnw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3uuoazbmz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3igmixdpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssnkzsep.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3pncwqewm.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3cvyolnam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ippqxpsm.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ifxvuvcz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3yqknvsug.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3uykasnde.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3fdklwrow.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3bsvzgzyd.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ovkgscsj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3qvmboanc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3hygwjviy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3awclvset.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3wopcevwt.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3znarevyp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3tsaglzaa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3mdidswdw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3xhnwwziz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3oixrdgwl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3owwrbzhq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3rrlenglc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3opkismaw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3wecxfvps.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3hzlnlwnu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3innrlcrj.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3joqjrmqk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jhthwmkz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gdpmoxoy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hbsoauqa.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3beyzcirr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3oinfyvrx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3ghqocgyw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3slnrydbh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3krjfhfvu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wlzmetks.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ugpyzecx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3kaogcojj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lzoihton.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ouyppkod.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ojvmduey.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3nurvohjf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3savnbzhp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gmjigrgg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tausidid.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rmchasss.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3bsmvcorw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3inihboip.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3djhmbeeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gghjelir.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3naydqhth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swezwvsu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3whrticib.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3cdowsdub.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3pxyaeydy.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3kqaprjzh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ilknkjyl.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hggircaz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3licyhtau.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3nlhzphku.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fnavjpgt.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ztdsflzz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3efofaudz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gyctbfla.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3choeupcm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ijijrksw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xejuqizu.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ggylgbrp.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3zfqivadw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dpspqqkg.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3huiaepai.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3znabhfmx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yuovaamw.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zrqpofee.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mbdmpbgk.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hfuowvuy.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3bukhtzkm.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mtbgyuvr.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mnctctui.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3aansmpdj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3vbqlyvly.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3xiydomsb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wibmdxyx.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fxmbqgmc.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3xpayyhds.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3wkrtarqn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3zpaywbmg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3mvynlwzt.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xwmahiyx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3iuqooqlb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wcizwzuh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gtlvnubr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tvcctrzz.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ffjguspy.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jqhkymgj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aptiplxo.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rvfimsti.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hgamozvj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fuslrzwu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3drdeumrt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hjqitndr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kqaczija.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tavxrtpd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3oggwrrab.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ipgfhnst.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fvvxtcee.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3gjdcywix.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rneisegi.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3phrufhfl.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tzvcoqhe.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3pahzdtof.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3avraourb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3tpnzquae.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ogdfzchn.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3utvmwpyf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3xucfbbfs.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nmgdywzn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3izeduqub.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mceiwgbg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3igjqtyyw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zzemomdk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3opzvxbwu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3zjmmadjr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hazodiql.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qvjhqpeb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3baiaugck.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ptmwjjzc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eirzarvy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3htodriuq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gkfuxmdp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3bjarzudz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3tkkntxgt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pypocppy.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ukfcoetz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3qtxkgxzq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3uvrdaqfj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qwqjzadt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ohyxihyv.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dywixoll.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ycdutyym.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3daxuquvl.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3wknkfedr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3gtfvrglz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3awxuvkbr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3chcypuio.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3imhzdybq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bxnvixko.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ojlsqitl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3xnjrflun.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xpkpwcya.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qiqdftqz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kaohctod.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3pyjthuad.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3dcgbglwt.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3alhrbbvm.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mteccmro.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3mjvmckei.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3fzycezue.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3edqezwcs.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ubflzdrv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3fuhgezek.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vettkpvr.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qkrvfxrn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3abgwfxan.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3djdijeeg.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dpdfvmjd.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yxxltihv.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3direrqoe.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3toicbrkt.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ickqexgw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3gxfpgvmo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mpfneixe.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3izioxtnz.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wtpcsnxq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3ubwvvhla.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ygoofffp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3oubcjmkd.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wbhslnnf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3iermrbqq.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3kfmiuakm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zmhiesxi.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qthovnvc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3avbrrpju.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3gtfomuze.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3twhgwmmc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3gjyfsqko.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rnylnqkl.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3facgizhw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3zukiebqi.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3vqbfofkl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ygcfosxp.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbivalhp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfefyttv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3nvejkyro.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jabdidjt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3wzoqdhbu.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3surdypoj.html


<!-- 参考信息 -->