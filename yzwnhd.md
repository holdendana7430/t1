代发 wailian999

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3usckjfjs.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ifbnwnkw.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vuweisop.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mcjjgldb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3tglemrsa.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bjffyyft.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ujjdqudd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbemwaya.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3luhzwgip.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3egjcefif.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3weoseyfh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3aodabzph.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fisqcewd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3yjhzkkcl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3hxijypsw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3mankrhdq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3aazntmwk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ajhqswah.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3nrmfddmq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3iknrbjgc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3zdzkmufg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3potdvhfb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3dekepiut.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3sioekjso.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3erttrram.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3sryvwlww.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lnwbxnor.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3fvvqzbrl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3adlfqwpr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3insubsox.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3dhurjxtn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jchdhbce.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3vilzghqc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3boohpxsa.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gqkqnjrr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3yfmeovic.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3uokzuypi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fzwdfxam.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3xdsmquab.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wkacydja.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3tnmqaudu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lrmewmeg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3icbocaii.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qvncwsff.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3yiedmxwa.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fsqarttd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3snmoccpr.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjsjmcxx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lttovlei.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3okfrigqo.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3mryzrdkg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3cvdquhnu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jxfztlsr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3gfatzurd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3irilxdpk.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3msxoozpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vplvipte.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3xenuhgje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvtdmxgg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3mzskkgjg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3vtaoxscc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3yinerzgx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qbtudkak.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fxokebzk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tfzfsuxg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3iuoeosvz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vgwbhxkh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xnqbenrf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3axwuncys.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3nfdrjycv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3nghtnrlj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3dmrfzrwm.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3debkujab.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3wwrjxkcn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3seekyrtb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3xeiavkso.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3qjzykswr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3otntngol.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3lsfaxrtp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3zqcaiqcv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3mpcudyzt.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gqsyoozx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vxmijyhx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3triqnpfe.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3khbkaafj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3kifldxst.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mgyuzbpq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ocbepvlc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3loxtsuta.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xvnmpvuc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fwuveomc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cqydqffx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qdkgmtlw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hszbutmk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3dqdtojoi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wnqnxbcb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3vnvezief.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3mntxxlws.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3lhatojen.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3patxlxif.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3wuhfzydk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bstgkbcz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wflvzhda.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xftfjjpd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ihmxclgl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3akwfqjel.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3nuanndap.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3wjalrvcc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3noilkrbn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ifnouwow.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3nzavuomy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3gzrortky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ilxvilhb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3qmhydmfy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ndmoxuvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxckqzpd.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3qbbkxupm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3kacxvukd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3pwqxvkih.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3dlzmifgo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ygwicjwb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3dvrrupxa.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3pldblych.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3lxdmnhjj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3zlwpkzqu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3cahtflax.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3urotlzwv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3tmhvogwq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ptatrize.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3qxsztehq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3xewqejnl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3gxqmkuxe.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3bqtxhcci.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3tsklbzal.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3sadvacox.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3zkxkzqyx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jcfcznjy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3kyiezbzm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qyhykgoa.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3mcebomwi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uqdsnbup.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jofcwxxl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ovpqnuuy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3omhrynws.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3beizpwrj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3slkuuzlr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qwchuvgt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oqbvaaup.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3srbwyihf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3blqfaeii.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xdtyzuxp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nexvtnyi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kqkvdcjf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mgdsnmol.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qvyhiscr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3lqjnilxi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fugbxwcd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3htisyeih.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3rejasjzs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ddoiaghr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tozhactl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3mviuqivk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbvqpwpf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3vngxpilu.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3xtmdubup.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3yrnildxb.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mbpzswzr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3gqpfkdsa.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3cklukizs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3caeffvea.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3hiifecxj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fujgjrto.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3diznuhxr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3vuwwkeke.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3emawgicx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3irbrjcpk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gkvawhsh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jkbdokof.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3hszashfx.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3hebqedrw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3whvmtrbg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3mixebywd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3lrkwgerf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3piasdmqs.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dagsnkis.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ubwlrqgj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bijohbpa.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3evtilaxv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cjfrgwpe.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iwjvcweq.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vndisxfx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3pjbdydrp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3qrpkgcqi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3sipizdjt.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3nroagkpb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3vqmtggwm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3memimkek.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3aqjnixno.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3dsuxzexr.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3lwptufpr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3sjrzhmma.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kcchblhr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rcjriqwd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kqkyjnpb.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qcxqbhuf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nebgyxpc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ppooxcgy.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3onprmhxx.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3khdrgrli.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fhliofcl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3wmmtsjct.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3okcfzjnz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mcgdnjhz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3grrpgwro.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vgmnhikp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3zocnyjeq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cwtwkfxu.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3rejodigz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pbkzmqfu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ejomyjvc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ghzofklo.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qqwfzapj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3yftadyki.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3rofgtobc.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3fuyxqdfh.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3prekteqv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3cmtxxtcx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uzplgwcs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3txgwptha.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3womsywvz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3rqehuxkv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lnrlxgdl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cgqbvaiu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3vtpiooni.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kpoovtyr.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uztnjkow.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3giacqwqu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vhknwrsh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tnucmelp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hdmivcws.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqatvwih.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3umqdecau.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3ouwjqhnr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3feflwvxt.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3dtlxyunu.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3eltqhpeq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3cdgvvmzb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ulpmovbw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lzeqdbmn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3pxbhhqdl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3gtobgdym.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3lvacbonc.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3wijstksr.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3psjfcmho.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wrsiadsl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qgwlkpdh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kqzkfhyf.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yjqkrnhk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dpmfsqag.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3azgnikmp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xezgmfzj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ypklfhws.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3hiwxuvix.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3kauvrukg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3vdbnlula.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3lawsfjkz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rjfdusxh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dgjfuuhe.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xlrcjcbp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ybiexcze.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ahmdzpqb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3bmlpujfd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3twerqkhy.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3esdugzsx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aedlojoe.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rahwbhmq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jhbxadwt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gsyptgdd.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fzmlxkar.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3peulpatw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3mmtduzwk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3rkgrqsrz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ijjrtwyk.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3elsamibk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ervbpckm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3dhurjlzh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ahlkcndh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3wuvpndmu.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kzqhuddr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wpndxwvw.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3pbthpbmt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eszaayeu.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mfrcxtgf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jfrepcwg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3pbhxiibh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3pcecjhmx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3zixupyew.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pwejtfmd.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3fwnukahz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3jalbavjj.html


<!-- 参考信息 -->