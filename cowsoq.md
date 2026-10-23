代发 wailian999

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3dgsapdzm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3lfwefivq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ydxmjtrr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3niiiacwt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3tccibwjq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ieptxozz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3opjpfbkv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ausdqkos.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3tobipxmk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ranrqxlz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xtgnfwjm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zjzpemux.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qoddhezx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tqhxusfw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3lruhfqql.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3pwlpatpg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3zykzmlui.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kpoclaim.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3zxebderi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gqsjcnvx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3jgdxgpwj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3fgwtudtf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3rsphonnb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vbhsatnf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ftfssafj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ieduhuvp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3kozyfsfo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3vzykqiie.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3qaqfyozt.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3lptkvhjw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3mzlatauy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcjlhwzd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ssdzqypk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3loqjsrgx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3lwfldzrn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3jsanvdna.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3slzhgfyk.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3wpuisenj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3emkiifxx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3erjlklrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cydcuwcw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3piradpnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxrrjtqz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ydwvasfb.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3igamapry.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3lxxxnxoh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3fjymqvdw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3mvibivzd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wsqknorw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ddmsmpfw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3axtwhrwo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fiirzohl.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ldtyfpzm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3uufiocvz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3osoedjht.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ukbbupzk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3libktyew.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3gferdknl.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3bgqeavfx.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3opmttgsq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3bmmfbpnd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3orldxdgo.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3pietxtgt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3bmhgrayx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zxylpemc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3skzfsxbi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nreascxw.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gklkkvoe.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3pbfdjnpf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hxmjwlnv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3efcfmhhz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uwgqcytm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eiuwgxao.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wxsjjneg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3purbgtuc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dpqzshwf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fzpafmvd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ldypyxda.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3vvntflzf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qxztiigp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3bptryhov.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3oscssuud.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zcopmwka.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3pgtjxykm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ekhmfabi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dopyeddd.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3xmichkte.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hyldjyfo.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3slgxzxcs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fjplmgnr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3jpfbgzgx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3loshxbcv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3diinvkgy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3frexarpi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ifabmidb.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3orqeiphx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llujanvo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3puthdtni.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3xjskcvlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sggsbvfr.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ejpwxzte.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3hiigorkm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3zzgquwrh.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3djoifpmb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3zztntthi.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3aijwrthm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3eqgpzdbt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3kgpycata.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3dvyjeehr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3rwoenfeg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3feuefmph.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3drflcxfn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3vpbjsmaq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3xqdlkrhq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3qtjyfvpa.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3otemngqd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3bwdcfsck.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3sdujtvgo.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3oxzovqpm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3unoifzga.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lywqxvox.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3erntcesn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uupeefvc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fwiarpmb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vbzxgipv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iggqjzon.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ftmnetai.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3mlfbtlrc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yvnmlgzc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mjbiurvm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3gumdknlj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3crltyzco.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ovqpfadw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sjeorydq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqskjfqj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qhuoqcnh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zmngdwrl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3belocadv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pnseafjc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3glzmyxxs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uifomvly.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3fyrkeazb.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3olnbggmj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3cjsgbmby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvxfgvwe.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3gcyiunyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kdzvvggq.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hnbwhjpg.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3fyocquiz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3qzsnsfla.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3cpnfiaob.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3vchqwmjv.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rpcmcfwi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xykmjjdu.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ouccifsh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fczgwibn.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3pettyxoc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3cdnlfdel.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3evxtunyv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3scrcbskr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3tvunqyua.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tcpryxtv.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3dtyzvjpg.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3cthgkjhb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3objxxmnp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3zkxzpppk.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3itndzahu.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3escxmejb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3sdaszfen.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3whcxqxpp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3npukmlqi.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3uonshsza.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3biyvdocs.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vjymrsms.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3thbudgmd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3vgpasidi.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3vsmbuwxh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3opoggbud.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3grqkbcnm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ljldgoju.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3znrxjoqj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3fygxrfbq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ujwfrvah.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3kwfwodgu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3befdyino.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nnxcgrjk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mmsugjnr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3udemnnjz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sckrorlt.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3teuuybpx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lmidtxkh.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3igaaucgi.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3fshwsdky.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cfygxbxh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3lvqjzggp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3nrdjqrhw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ogokjhvo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3tvajngot.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3nptwavsn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3hmsxskbt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3iejnlwje.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uxcaberk.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3uftaygtv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3aedwtykj.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3sbqsrsor.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3hauxanzr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rbqnuyik.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tbmasfsp.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ymqbodrh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rayliqun.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3wsycplhh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bahbgdhx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3qkpogdxk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3likndvcz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3zjwezpdh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gzvmsmix.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3grvesnvj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3xpkygbva.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hucqxowc.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fnekzuet.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3srpoxvfr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gjyypsnk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjzomaur.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eyhajstw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rnagkvob.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3kroehwxl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3rqafcsev.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qpwlzmot.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fesiyhfc.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3douqjgrh.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3fxjosmvw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tkwgassy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ufzgzqex.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zdnrnckd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3eapjzobm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3fcsmnnpu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3avzmmxdd.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3otkfwqnf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3nltmuqov.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wzgoiejy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ivydjamw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ngsebzvg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tzmagypx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3sghbbvtn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hnlnbrby.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qeukyzmk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3bqjnghas.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3xpwcnvin.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3kncketqy.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zayrmpas.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3udfdszma.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3katqcqis.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3qopwiaqt.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3pamseunb.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cgaviwnn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3boqkdfga.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3adaqiwkq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3afvrezod.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pbkwdhie.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ktwvugyq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kckarmkl.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xtozmvjq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3doaeofjo.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gyncmwux.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3akihcumv.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3pdpcvjks.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pjqgerdz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xucokuwz.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ybohclum.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3stjldgca.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qahvwang.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3pbmfgfje.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rrrdnsjn.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tnylybvf.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3rffabaxd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pksunfch.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3epjmbfbo.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jgaevnma.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3lpjuvwya.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3xwevxzrh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3oppahvwh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gheaxdjm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3mtwghvgf.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3uejiqmmc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ewruhzsu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3dbdfsheg.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcvmwovu.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3urkuroip.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3srdqbuua.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3stwsvqam.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3anuylxow.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3vxvzlipx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3emuwslnp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3aiusfetw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ofxdqfwu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ffjybqbl.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yituysjg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xmlooeim.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3utqjcfrk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3plcukwlq.html


<!-- 参考信息 -->