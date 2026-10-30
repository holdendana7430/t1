代发 wailian999

[U105] JS：节流
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuojdrzl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/grecmeuyn.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gawsxbzhz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fanxiaobao.xyz/Article/details/gpaemvobm.sHtML

[U107] JS：数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnnwurvk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqqetlfp.sHtML

[U108] JS：随机整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gesnoiajr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gpkhvaowk.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiidkmuh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gchocsbck.sHtML

[U110] JS：数组分块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvmszhkw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gdirdqkno.sHtML

[U111] JS：对象转 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gzkgmmvrl.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnmwnpyb.sHtML

[U112] JS：字符串补位
来源：http://mobile.fanxiaobao.xyz/Article/details/gmktwbgwr.sHtML

"7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gccjcnrti.sHtML

[U113] JS：正则替换全部
来源：http://www.share.fanxiaobao.xyz/Article/details/goitoqyjt.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/ggfkojqrj.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezmqjgvh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnpegffd.sHtML

[U115] JS：生成 UUID
来源：http://baike.fanxiaobao.xyz/Article/details/gxgkawimc.sHtML

crypto.randomUUID()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthwnpioi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvffzxinh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gpzaxzvlk.sHtML

[U117] JS：单元测试
来源：http://www.share.fanxiaobao.xyz/Article/details/gymqgbelr.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/gowvwzxec.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/gxshkcpbf.sHtML

npm i -D vite;  npx vite
来源：http://baike.fanxiaobao.xyz/Article/details/ghgejqcez.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gnfpophey.sHtML

npx vite build
来源：http://baike.fanxiaobao.xyz/Article/details/gclzcqqqr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubaoukwi.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkmkwnrw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbsiggmd.sHtML

统计汇总
来源：http://baike.fanxiaobao.xyz/Article/details/gecuysyov.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gimtvqwur.sHtML

按语言统计（条）：
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwqsgqxj.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gkncrjkij.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvdshluu.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/giwbrfzjt.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmuapdti.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gmjdizwxo.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/geweafhzw.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gywsukmmt.sHtML

C# ............. 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdwhnsen.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/gzcbvnnbt.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gawchfkiu.sHtML

SQL ............ 90
来源：http://m.share.fanxiaobao.xyz/Article/details/glrisyuoy.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorkvwlyz.sHtML

Kotlin ......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjawxaba.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgzqflnh.sHtML

Lua ............ 10
来源：http://blog.fanxiaobao.xyz/Article/details/gwdovkvfi.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gevkqkidz.sHtML

Scala .......... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/goaokvqtx.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gdisuvscw.sHtML

合计 ........... 2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gzyfhqabq.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/gkryosvrb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcupalvd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gskkcrbke.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnfwgkoy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fanxiaobao.xyz/Article/details/gldmcpwae.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fanxiaobao.xyz/Article/details/gamwvqqvh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gfojqbnvv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fanxiaobao.xyz/Article/details/ggszmgsur.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gxapacnoi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gsrgrnhpg.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkiwdkii.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvlmnzdz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtknkgsvj.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqutyjsb.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gnavmmkvd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/gcrcrpozv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gqgpuehhd.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/gjufllqkx.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/guyqhnoqw.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/gqzhvwcpk.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnaxxskh.sHtML

U 高频实用片段                         120
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaptyypn.sHtML

------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/ggebqhymd.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxounkjl.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gxudekwwk.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gjescuyuh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gqepyaxaq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/glivbnrqq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fanxiaobao.xyz/Article/details/gykwhouiu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fanxiaobao.xyz/Article/details/ghjbhosxw.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fanxiaobao.xyz/Article/details/gkavtmsqy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fanxiaobao.xyz/Article/details/gokamnmag.sHtML

—— 文件结束 ——
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqbqnxvt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gapzdpmjs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fanxiaobao.xyz/Article/details/gigcodena.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/geslvclst.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gszjfpmwj.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtalqbhet.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fanxiaobao.xyz/Article/details/gpcyouncf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdpkosshy.sHtML

SQL · Bash · C · C++
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyqxxqfa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gpufbbjcb.sHtML

【使用说明】
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuzkicly.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gxlgrntcq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfiumnls.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.fanxiaobao.xyz/Article/details/gttfrkrzz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/gbyxesfee.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fanxiaobao.xyz/Article/details/gyahhrhnm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeouzxew.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/glrnlvcsd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwmykoae.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fanxiaobao.xyz/Article/details/gtqojznjt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiatdgep.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fanxiaobao.xyz/Article/details/guufsbzhd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/gqgwwyitm.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gtnsnzpkh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/grtgijlxo.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyhnhjji.sHtML

目  录
来源：http://blog.fanxiaobao.xyz/Article/details/giovnyuuu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqziwvat.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqjmazvo.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeqxzscs.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhwzxsgg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gxkskacqd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbjptffc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/garkcfiel.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmccelewq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeiesjya.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbxptsko.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggknsfjeo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmibgxifl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrxrqlpf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/ghebtxnyi.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbqxhizy.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gwdnpdmvf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganhzndao.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gegxzcfbq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gjocjsnvw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrzdqgkf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghluxlkam.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gauyjnwht.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvalehgy.sHtML

A. 基础语法与类型
来源：http://wap.fanxiaobao.xyz/Article/details/gvwetqbjj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzntsput.sHtML

[A01] Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnmonley.sHtML

Py:   print("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/gqhmqrkwo.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkinyujd.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzjwzoeo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmltsedua.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gygoehzpj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fanxiaobao.xyz/Article/details/gemxdtpue.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fanxiaobao.xyz/Article/details/gxgbooyau.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksxiwyck.sHtML

[A02] 变量声明与赋值
来源：http://blog.fanxiaobao.xyz/Article/details/guonelvba.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtunnzlgk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gfnilxxck.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/ghokjybme.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqyayjom.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gutmzbefc.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gjshqwkgh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.fanxiaobao.xyz/Article/details/ganudljbv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqhsnasb.sHtML

[A03] 常量定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gflrohspu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fanxiaobao.xyz/Article/details/gfrswbhvj.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfljmbnf.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcfqizdn.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqpnsddz.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gwedwvpds.sHtML

Go:   const PI = 3.14159
来源：http://wap.fanxiaobao.xyz/Article/details/gtaytouff.sHtML

Ruby: PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/gziwgzzko.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gslanhvlf.sHtML

[A04] 判断变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrswphhh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fanxiaobao.xyz/Article/details/gjzhieqyx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fanxiaobao.xyz/Article/details/giarhnukb.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gcotehxmu.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzziwpnjo.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfnzkbkr.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.fanxiaobao.xyz/Article/details/gwgkcrhit.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkvbkrby.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fanxiaobao.xyz/Article/details/gatvghtcv.sHtML

[A05] 整数除法与取模
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnacjpri.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fanxiaobao.xyz/Article/details/gnrmdispt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gtpmilvjc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwzrgdntf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrsjoffd.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxnemgqaz.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gnrdklqit.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/glhunnfbs.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/glejhjlnm.sHtML

[A06] 字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdxnyjfk.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghfjkqrz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/galykdsfb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/grfutfunp.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gicsowezm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkxgnkir.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbbsjbqz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.fanxiaobao.xyz/Article/details/gtbydvjmz.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gntztoyvr.sHtML

[A07] 数字转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwllqonvk.sHtML

Py:   str(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjckcfgus.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gbzkcxkpf.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gxjsrblne.sHtML

TS:   String(42)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqaptyoq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fanxiaobao.xyz/Article/details/glxrvacix.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fanxiaobao.xyz/Article/details/gyycjxjbo.sHtML

Ruby: 42.to_s
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyaeuisx.sHtML

C#:   42.ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/giittnani.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fanxiaobao.xyz/Article/details/gefnvggbn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkntfykmo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gessqjqyj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gtwkdhhfc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fanxiaobao.xyz/Article/details/gnyezbqga.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/guntrfwtq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/ggkdztfwe.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbudxtdq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyikqjxp.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjhgdmgh.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpydizlb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/glkkcefnr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqlriqoa.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gjrjlaulh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gctnuuyfe.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrdkolgr.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.fanxiaobao.xyz/Article/details/gnitgjsgr.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdszkgapi.sHtML

[A10] 生成随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gxtlbhdrp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaajsbvx.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcfdnffy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghclgnzpw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/gunebwbxi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhhbvvus.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmntglcfz.sHtML

Ruby: rand(1..100)
来源：http://baike.fanxiaobao.xyz/Article/details/glahtdcuz.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcniyapr.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fanxiaobao.xyz/Article/details/golphyisl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gbhgfoode.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/glbslifsn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gerbefdhx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gyfxifkji.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavojuyjo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkiubwekl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goftsytxl.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfuxzzca.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmtwkrni.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjwkhivie.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwtmmryp.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fanxiaobao.xyz/Article/details/gbkarjusf.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fanxiaobao.xyz/Article/details/gekcouqgz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.fanxiaobao.xyz/Article/details/gdylyinqa.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqprbfck.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/geamhbteu.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxketjpgc.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpjhtnmt.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gsezkajty.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gnvxufobq.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqztyghgt.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gygpzdwes.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gakhsmxgi.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbfvjjzy.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/gavvsenbx.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbiabujua.sHtML

[A14] 注释写法
来源：http://www.share.fanxiaobao.xyz/Article/details/gspheylvg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkcswnbv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gavjwvwju.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gnvkapxgb.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gnypxftfr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmicuifws.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjnsrvhk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfvxnecr.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fanxiaobao.xyz/Article/details/gcllsqoar.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrgixjoo.sHtML

Py:   value = data or "默认值"
来源：http://3g.fanxiaobao.xyz/Article/details/gigrttaib.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/guepsxdul.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtipkskz.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/giowknxhm.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.fanxiaobao.xyz/Article/details/glgvopvor.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fanxiaobao.xyz/Article/details/grdvewaea.sHtML

Ruby: value = data || "默认值"
来源：http://3g.fanxiaobao.xyz/Article/details/gjqfbelkx.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fanxiaobao.xyz/Article/details/gdlefftiy.sHtML

[A16] 真假值判断规则
来源：http://blog.fanxiaobao.xyz/Article/details/gbohokalh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.fanxiaobao.xyz/Article/details/gxicjtocw.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fanxiaobao.xyz/Article/details/ginwspyoe.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fanxiaobao.xyz/Article/details/gmektiogp.sHtML

TS:   if (!x) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvvbltkw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmgqltkm.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fanxiaobao.xyz/Article/details/gplcrhkld.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuawrnbw.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gztppqhgz.sHtML

[A17] 位运算
来源：http://blog.fanxiaobao.xyz/Article/details/ghvncfbca.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghinatgvn.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbaohocq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gncuhpvzz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gnoznpijo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/giicezsyd.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gepopsbcb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfejseqdd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giicnyvpk.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fanxiaobao.xyz/Article/details/grehvrwpv.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiberxzo.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.fanxiaobao.xyz/Article/details/glpbfeial.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlchhtni.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://baike.fanxiaobao.xyz/Article/details/gwrcpeatp.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvedpjet.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://3g.fanxiaobao.xyz/Article/details/gcrxsvcab.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fanxiaobao.xyz/Article/details/gkucqgnng.sHtML


<!-- 参考信息 -->