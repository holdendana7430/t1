代发 wailian999

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3edewulei.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3xmpyveym.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3eeekbzed.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3unpnrrzk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3pwqlygog.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jiwdmtky.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3shnfqegq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3nephihjc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dhizkkxk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tbecomek.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3tjgwgyhv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3jcdliufp.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3sdqikrpj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mkxvynfe.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hxjrxqav.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3igwmkbop.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ryqwyecu.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vaatxhoc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3xknfumpt.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jlffcedg.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3bptmzezu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kqrustnk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jduadgeq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mnzzcuho.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vkcpgxfe.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3knxwpqny.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dhnxivzw.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3zmmbhxrq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ctgzknta.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3enajgazw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3umtxzcxl.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3jvpnsmxs.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3xrcwwjuz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3uwjmiblz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3sdjicohf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3kzegwevd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ylckrbfn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3tygycbns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlprbvcz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3nhvniroi.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3oflpzlpu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3kuvmbakw.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qizgnklr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ilbuwxwn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kzvjeyor.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3egpgnhuc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3knwrurvj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zvlhnzdm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3fohbmijl.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3feadbrfk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3vhfphjhy.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3axotfpvm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3krtmlxoz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3evqqfbim.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3yktdlqen.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tiqumvjl.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3udgeycfc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ihhzhous.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3gvsopldv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3rvwualrh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lgmrjxis.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3appwjsjf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tjebijvx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3njtztmrp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3jamizrvw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3dfslsoow.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3brydsdnb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mpiwvjbv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3stdowuaw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3gflyvema.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3luzxljnc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pusmdwux.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lvlowmto.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3cwzuzxpg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3mttjivdl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hbhddvwc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3miukbymu.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3nrzbcdib.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tzbsqlnr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ouxjdtxm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3vmvgahgw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eynbtjgi.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3pkowptpp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yhocqihw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ingwffkc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yerrgxfo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3vpiersfo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3vbanfezr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3zdynhzcr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3pnxxkfhs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3oaqnwzyd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ajgvalwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ymbnnmrb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3thkdqhtf.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3athqmixc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gqnpvnsk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3zoaanamc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3vdpocxga.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3gebktfnd.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3dflnpmjc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3bqdqulki.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3elzgwxic.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3eiumwqjd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3fwkjhnua.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3xfmpzrkv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3eswizyur.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3xmcwukoq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3lvafamdl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3xzsveozx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3vcrmfhav.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3zxkpxraq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ypavlguy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3hozqwanm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3vjrqsqmy.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3hiuomzru.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3cuetvquo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bxgdzyye.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3zwgzexbz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uzpvcavu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3tlgrwcue.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rqykjknt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qkajmujj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lujpgupm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rvjyvxhw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mosbzpzt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3bckwylxd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3aqchfrle.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fdupztbb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3otdjdgkd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hbuqcupl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3thknjtfy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hlpvujuz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xbazyzbf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3tifahybq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pgavwxnc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ybdjfrfk.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3smmbouca.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3uqdpkrcw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3afqiefmq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3eqxgjqpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jaxhysbj.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3pdnaigdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iiozpmnc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vfjsaszw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3pbhflthl.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ngbogrku.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3muqvvosf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3yjrohikj.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jfbxjoql.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qtegkyzw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3mxhnumwf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zscmehyu.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3aypsupjb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3yhuznulh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jrurbeon.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ichozbsi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3omyhwqvb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3unwtcnja.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3rqvjxivj.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3lafraqta.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hjmysviv.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3wmuyuhax.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3aawlbmym.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lajwrqrn.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xtjgakym.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3udlyuqcs.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mauzqzpt.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xjwqzffr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3olvhuvqn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3edefzgaz.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zmmhwtyn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3qlbobgzj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbqyrmyf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3colnlxii.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3urtjxgis.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3jrgoergx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3bmlzsiea.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3qhkxseor.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3pbdtefhj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3gmwxuwpz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3efmhhasj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cjsrlppj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oehdjwxm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xvcrqbcg.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jzpjrnbu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hlhucauy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gdofvpah.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3llyvpuno.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3eysyjonk.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yebrabpw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3edlbxxxl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vetrajyz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ihbpvqty.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pxriqevp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3kvduqhnp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3glkcoltv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nmusymup.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3oxatmuxn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3tmcvqqds.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vrdxhoff.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3htssumsi.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3buxipfrm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3wyddbfji.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3kutoqiyd.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3itesgpcw.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3xhxxczqd.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3vakxakit.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dpcwycsb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3zfcksqco.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ttynnhof.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3mvfedeyc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3whznqnhp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tleauuwx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3gxwcrprt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mgjuteny.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mfpyisyq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mqeaqqaa.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3orottnji.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sflazfld.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvtegpme.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kigptpmx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3vcgtvzwz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3fcljueaa.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wzxvemei.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3samwuszt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3yagneceo.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3dbmzjqty.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lsjadyom.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3grhofloy.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rytmklos.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3epcuoxeh.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3zikbreaa.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3vkmuglfw.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3wutivexw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3edbkjmyn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nmbbbtsc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yijioico.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kfjdquwz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qjydqfqi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3fkfxgpzl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gizrspgp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pjelhurb.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3qlzsixyx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3poqzybaf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3vlkxozlr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3telcfues.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3rvasnuwg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ligcfwwi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3dgoacxeh.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3wnhdmmkm.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3vctiluts.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3kaxdgjuj.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3slwkbkcs.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jtnqakld.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zuqqwuhd.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3agzkibka.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xhguqjxh.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ptlhhafj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mtxiegcw.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nzuiwhff.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3dfxhdvlh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3zjgabqjm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rvebjqfk.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3oqwrchvg.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ctzujezp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3bkpvrqrv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vhujgjpv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3qncslitj.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3iphfzcuz.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3trsqkknu.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3femnnnoq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jvxxrwxn.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3uvpbyvuk.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xdgxuvki.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3jwszryao.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3muaiwyeo.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3sbnlfgdq.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3qmtznccr.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3ouukgsew.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ghmiqblb.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3amkablcc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3hcqdxzaj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcdkhhqz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwilemby.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3jzpcnfbn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3gdlagyoe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rhujewbt.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3osuktfmn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ndxhzeqv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3sroxzuph.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ownxecgk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3suufbmfd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xrbcfrlu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nmtimvhw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ibdmodyo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uezdzinr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3tkuhbxem.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3totxrbry.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3nzhkcwid.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3oaaulfgh.html


<!-- 参考信息 -->