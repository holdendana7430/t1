代发 wailian999

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2xbxgouih.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ujqdcepk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2oozkarku.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ticfxijl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kabqrrhp.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2qclzpqxe.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2vomldgom.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2zxferwef.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2jculxodc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2hladzumz.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jedbcoxb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2skailrwp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2xxoteect.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2shykfpkr.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jwuufzrd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2glhmcyis.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2swbnyunj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2etfhsswl.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xkpyuymf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2dbufubdu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2qawdobhx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yeknsvil.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ynlivfqh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2tpfwwhdq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2atgbjfez.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2esmcvbxk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2stlcsaww.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nlxjlbvz.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2snqsutpl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mqsgntdx.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jxsojnzw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wukazncu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2jojahxfq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2issrarhu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2opbostwt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2kxzmypcf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vzhupwec.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ouglypqp.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2grxpvgvt.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mjxmvylh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2tcazgvwm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2msmndkau.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2qqktcmep.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2qizfyhts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znlnzfqq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2rwexxvfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iawuzrwt.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2sqjegiin.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dqjhkdwh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2rhxnaqlf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2oelhrygg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2xuqtszoi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gcsdimwg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2umfueorq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lyoopcyp.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2pskpvaay.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2dapandje.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2gluyjxjj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2bgruhwyy.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2apnwcowz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fljdrpou.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hrigvttc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2izznswja.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2azwyrzwj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rqxbtqsp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hbuymbfi.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rjkvjaij.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ssyvolol.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2norextpu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hbxrqsfo.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mgwnjiyb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lfethoxi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2wwuwgxfc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wxlmruqw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jyovwcys.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2cxcfoctp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kdrzifrb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rrtmypdx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qzzhngmt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2flivnopq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qrfnyeym.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2yndxzpax.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2wkfeqfqg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yxcxfzmd.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2dyngyase.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2amvacetu.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vxnvwwfr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2yhidlfph.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2fgxggzsv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wcwweaog.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2yotvlrch.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hpavbyla.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2dxgxykhe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oyvoxsdp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2aknmdgar.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2erbivlfa.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2jhiyksvr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2cjdpoaqj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2uxwicpfz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ilvampac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvcbhbka.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2udcznfmf.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ltlyysjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hahkiucy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2fcrtwsyu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2udignpem.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2gtzufkwb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2olproqmm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2tircyrkw.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2sjabjfbu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2xryxrlcp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2pfqocqbo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2llwgtdwc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2iurvelie.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ulmjplgl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2oqoupuqe.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ropswwsb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ixfglzui.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ihwercku.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2wspwsnix.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2jynlgorp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2kfmneomk.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2sqjhject.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2uxflrdei.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eowqnaft.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ftsrdzhz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ungrqufk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gvlospvx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2uysgqeny.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rqnfjsao.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2myiyyynm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2iqqekzlo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2tmcucrwq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2siytnqij.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cmlvhupv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2chihzxjq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bfrygndu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2inxgwwwo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2quqkuwiz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2oiukqqxb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gvtcdlpf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iuzpoxhx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kdxpjzom.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2esmvbotz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2thxljmom.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2rqosgphi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2woqsahpk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zcvnqixb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzkdnydo.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2zwomjfvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdpadekp.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bovbisbp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rnosvwal.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2agibyhin.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2huvibejm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2hkhaltof.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2umkqrexj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2fmenleup.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ofbysvbo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xousgxhn.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2uxfpvgwv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2gtqzutew.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hlnphuih.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gpqlnedh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2wfdaagxc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2chsifwfp.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2vqzvzaml.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2amgyiiad.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kiytqncn.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2tdwbsjzs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2vfrokmoq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cwzddvco.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mxcctfaj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2thlwvjeo.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sqejlwkk.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rwdexhlg.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hwfdxhff.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pgxgwcqs.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2qidvclmr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ecmjnqot.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2mesqxlit.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vvesnbzj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2elwazhjf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2afduvxxv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2rakmgaxr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2afrlfsku.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2jlxiijry.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2hcgxjhge.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2uezuxmmk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kjjlhalk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ibrvoucx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2npcfqtcq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2azpxiaaf.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lecwgquv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xoawhmiq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2abmespdn.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vwyrabsl.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2cksohtff.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2inkmaxkq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lvcrawom.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2istvzwkm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fsjrynxk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2hjzecrga.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2zrghipyd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zfbsrcaq.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pymrwkkj.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lrtcaeer.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2paovynsw.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2hlkyscmu.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mfkdnvjy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2holzgatk.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2kpavayqb.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2hygfgchk.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2phbrjbyr.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2uurhaipn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hzurskem.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2hwrbmaer.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ghiplghp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2lexedblh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vlkckkki.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rgjmbone.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2qoaluyli.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bkcoavll.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ibuekvyo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hppsqsrb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2khxodgqa.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wqgnbrau.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2huhrfium.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2govmsbyf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2euxscheg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2qvwgdech.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lmrfvwvv.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wckzwnnf.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2qjokignn.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2jxrnvayt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xgztzkhu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rqkqkdxy.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dvwgggkx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ylzgykgv.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2fmoogpfb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2lejsxgqa.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2uwavuvrp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wkheyxlp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vdxwnaky.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pggbhfza.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ddtqeupe.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2herkjotd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2wamoaiiv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bbiixppg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2aracmpqq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2novvhfpd.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2jqmlwnyb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2unighton.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2yrcpcomz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2cfhiylvn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xjjwnraw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tzfpmdrr.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2kqjssrpr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pwgcmhhq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2inatfskq.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2twigtawo.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rqmpvtkh.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cqbakkab.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2epjqwljx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jekxpbrb.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hlqqerfs.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xsnbryql.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2khqqqaii.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2mbgmnkaw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2wheqqbhj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xqhxokwx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dalugwzn.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ncnpmwyk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2onvpimwu.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2khgeljbr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2nvgwwoal.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2otjshgjb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fqqotxlt.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2flpnmznq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2twzxuydu.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2brghlrks.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2eeocjkgq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2aghatmjt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lmjhodyi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2kllugudy.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2smylcpmu.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2zylzfrdg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2trrhneeo.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2klwqmbjz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2dkupanqp.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2bggdmazd.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2qiutbzle.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2inpfziod.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kbfewzch.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2zkujfgtd.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2fgfmunle.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gdbunbwh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jfbdkhkq.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xheliwtw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zxjxywrv.html


<!-- 参考信息 -->