代发 wailian999

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3migogemx.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3clzzfewr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ondleooj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3wdopjias.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3abjdvpoa.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3mtuxnoim.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pgcwxysk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3eyifnsvj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3mlltvmzl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3txpsxzkj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jyjccoen.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3eixiszzo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3vosubtdu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3etvoewsc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ndyznscf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fylmvmek.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ggbrqkye.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vuefkawe.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xhtwzmdh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ldjoabhi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cmcbizes.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3anfubsnz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3gmepbpoe.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3smwahbio.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3qirdvowg.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sliuraoi.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3necfsxsy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3clxncukb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3zooslupj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jbnhtuec.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3ophnjnzw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3imcsxhiu.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jrtzcmso.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gbrqltlt.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3acwibtth.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kxvybxte.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wpjrtean.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ombqaikz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3dbefigml.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3idvpthmj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3eczaajgx.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3zhzgawxk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qejrecsi.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3gpahiszx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3cqfydpfl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ckmwpaas.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3dgrrlwal.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3xywfehst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwuyizzs.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3hvptdcka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pglwqfoa.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zckhwuqx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3ugrktsyr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jqpeyvur.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3oojwunzv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3hhbbrlub.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jyrqvwrm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3chjmwxov.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vwmcffyg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xrtpbdsf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3exkkqsdz.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ffwvlkrk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ldndiajb.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3eopxuqzz.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3loehvjqi.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3wcqlviks.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3nohpugmb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3qufutjpc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ekxcfbzm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ftwodhbc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3tnqnjjhd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3lsygjrci.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lnkpetkb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xfonzvxd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tehjqikn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3vrgqyzeq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3mskbnmez.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3uraoqgle.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3mqdxyshe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3omfmfdxz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jvbndjnl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jqaylxfa.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wgnojpif.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nuwvjlbh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fljlrqre.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ffkzmiup.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3hjwwdxpa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rzywhyzj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3rrpawgae.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3viocraoe.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3dfodpqtw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ifembxgm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ixodpkef.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xsmgyrlm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3pxsxknuz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hvohwnsh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3lyrfuxpu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eysktcxe.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3fxnfigie.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3dfkxlwnm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3jozjkndn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3kmeshuag.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3jpgpfgwa.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3spqzbsbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3siouaeaj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3mpehfafk.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3cerlcsok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wtmdqpoz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3lpunferq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3vtigkrfs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3falhiqle.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3echuaktw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3vsoroymj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3fapemndr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3onkpsrmo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3vacddmmr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3qgslrwck.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3eliutefh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3nhpjgunn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3guajiqqd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3xlsscneb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3xhwrshen.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3grwpzawq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3tkxcqlib.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3jmdetjnu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3oswetrhi.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3izsgfxur.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3wdxhgkkh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mreesgig.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3kgaebfgf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dnvaetls.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hlqjnguq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fgxrsysx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jewmqhsz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mdgejbkq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3krugdqwy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rlqmcprq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3arnghhjt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3aetkakim.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qyjxiawk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jqltcxgq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mlbxwsfd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3nvqewznn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3knffnzxf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mkcpvvya.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yjzfmfco.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mhrwxtuw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wnzpshws.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vxbacqvz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3votavons.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ervwybnz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nbfplzlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xckgsokp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3zqkxuhob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tddradnj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gsogdfpw.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3desafkhu.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3yqfuyvbj.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hqkxanyx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3lqiubtvv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mcewuhse.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3wltagvmb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3hxbnvkes.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rerouxra.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3tzmukxrw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3kzxidrfi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ijsbzoum.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3btoyvdvr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ohucbzpc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qtmlzfxv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3sptkbytp.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3enehtpmk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3iaubwdfh.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3blxvzfhp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3rtpmqrga.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lvmpvsog.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uvyeykpf.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bqggdfsz.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3galknzdc.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jkdwimyf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zifkxnuy.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vumtdmcd.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ydfwlwbc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3gifmqvif.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjemykey.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lmnvedln.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3dtdogvdz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3jfhgsepq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3nsbtvhxp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3fhyydloh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3zewlhidk.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3odqevrka.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3fskgwgjl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3snjwhuht.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bfoipqzu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3owjgrbxy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jljnyren.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kpavqval.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hrmffnzk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bcenqdes.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fnremcwy.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nudruidx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3qsqeabwr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rxmdlced.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3cuzhtsid.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wqswpbzp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ouxuohfs.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3vbvnwbkk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mkednofa.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3agzogvfw.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kpnezhyp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3kjrggcta.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3mwyqldxn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kqgjekkk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sswigjfb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3vskozlmd.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3khywezxm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3xjnxjzyd.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3pserllim.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ylcrvsnj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3fxiwquxc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lqxmjrex.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3niegasnw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nkevlybo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wqlspzpd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3cnrfovsz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3arhwaqik.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3loarvsnu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yncebdoy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cxtyothp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tcjlczik.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kzxpbdah.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3herdezli.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3gdcswbsj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3ixbjkhxx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gplzfdlm.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3msudyrol.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3svggtmxn.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3yecvwwyu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kcolnqyy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3cjgbrrdx.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dbijlxgy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3vukgruvc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3qhkmnazn.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3iuutfdyg.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3rbidwxvo.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3oxgtcadj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nkntwgge.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3berkuajn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hazntdpw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rpelsrdb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3odsytfjo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jbblbpgi.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xpfbaevb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ixnnigno.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3wecqdiwe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3gquszokm.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rzzzrapm.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3cwoucvmi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3frpjxxil.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jtnhquml.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3noslzrqz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3qcmoifnj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ecqnlvbe.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mrxawtjp.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kibareyv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3amffzyhn.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wvvjrvnl.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mhjizaay.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qiwxifgz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3imvheloi.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ypxqcdkg.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3punzmoem.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3gbyxrdqu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3iaudiwfk.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rhltedwa.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jbuobvjj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3dyngwxsw.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ixbwchuj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3lkjhwicb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3eogjblow.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3qwvenygf.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vmjqsehk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3onwmgzdu.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dcwpoysl.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fpbuqvoi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3vijxsagh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3midtzhjz.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3hjrxtkue.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3muqtamej.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3vrunvpvf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3snybuyxn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3xeqtpudw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3rpuaxayz.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3rgjcmnvw.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmxfjtyk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3otjtpaqo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3dukkegqr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rkeamysj.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3pzwblobk.html


<!-- 参考信息 -->