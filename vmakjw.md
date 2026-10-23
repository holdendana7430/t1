代发 wailian999

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mfngjnwz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nzmtzzla.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ssvhnsjg.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3wqmkaaec.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3yrmuonfu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ahpketqj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3vykqazdv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3gfnpqfkl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3twniaqwe.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3mafbbigt.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zqpnkiht.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3beiewonr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lcjomstl.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3guttibtu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ixoqbzls.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bexqenxh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kvssrvwi.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mccvsjdo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nxhsrvwx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwaxglsb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3vjqfelmd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3aypaimpk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3lrtmcfqd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3hnbqmcpf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3wlhymcjc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3aoluwfjf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3aghysxqn.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3krayhuxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kkyxgmol.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ipvhlmmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbdzpgto.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3wckryjxk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3vberltqq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3hwbkktgn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3vtcbiase.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ycodogqk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ebzpivtq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ecbtpahf.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qjmvesxq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3yqasfrvs.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3koocdqaj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3klmopkws.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3vdivtbly.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3vfkuwxuf.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3bwfhwrer.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3mtapwhte.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3gtnrvdxd.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3wnezysyw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3mkhbaiwp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3anvjdrtb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3opuwiflg.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3nxclxgjk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ujocbjda.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3uyrlyykr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pofemimq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3bwihtovf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3gppkzpvx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3yhjexxau.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3oucjqsxw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nbnaodcm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3iaipyjcf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3rbmmsvta.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ubqghecc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ybwfnrad.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gbhsfhed.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xjsfpiyv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3dwoysmbh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rzgnonyd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3jucpiaby.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3dwtrzehv.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3zsbcruhi.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3hlgljate.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3gjbvcrrm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ljfusmrt.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zafuazer.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fzyjxraf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3usnlhxla.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ftqzfvxm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3qoxleqnm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ctwoiase.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3hpqjvjxr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3glztrxrh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3phjmeild.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3migohyzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twtfodas.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3mkviioot.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3hsqphytv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nedbissf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3rgugjjfe.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3faqfwcye.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3fqrcchdz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3sjjezhxl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3jaqjngyh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3zysmgvzc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3bauhceto.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3lpbdozff.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3irffstyd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3gssmsqof.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3objvznlb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3nrqcxvjh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3bcdoqtip.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3sytsmofw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3fmjkufio.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3nypevztd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3fwtzapgj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3vpgvgrca.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3aviraycc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ineaiejj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sycxzgqb.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ljbmmzab.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3opwwclfa.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3lxskaqvq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3urjamiar.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cavvkpzj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3eydtvmcz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3xreiymcp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dbtmscaq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pxnewtiz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3kpkrdzfe.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vjbdmxny.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3slkcmxzc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3iurvvfxg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ybqaxcut.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gthrbclm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3eepvyueq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3gazjnysq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gjmfwalw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kfifjcmy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vekbgzbn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3odhvkiua.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ptqdkniw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rkuvzcli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zyiggwrs.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3jajedfss.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3geuapiqa.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bmhgfhyc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ahtlwryd.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ixhugpkn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qadfaigy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3eoqsyjja.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xiqjzdrc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3jouoorfz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3xjktaucq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lqxzyblm.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3giefgeeu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3vjznozod.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dnozyfzz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3iuuxcscl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3djsgukdm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mwyajlea.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3kplygcky.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3eedjpxfh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lxpqzjdw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3occpuglp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3kwmhbpap.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qkhhoknh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ermjyocq.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3slysksns.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nffqgnzr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lqlysheg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ggvuwrzs.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aosyrzmt.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wlyttbbg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3onuajuxk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3wgsqqshv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ludtkclq.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3dermocjr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ablhzzlx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3wbeniicq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ijnsribk.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3rizfglxh.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3vzgygkin.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3powxtuyl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hlyvemzf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ebkoiqgh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rqqlvabp.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qoblayty.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nsaczxsr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3brmfrtrx.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vtcewdtn.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fxhudbpn.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jjgnvumn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3imlfvydg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3juomkfag.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3lclrrbdu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3cigjztsq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ftnjhujj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3vpnusmjh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pgzioikq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3miamelgx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3lfdvctdc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3mmivhbef.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vscelrad.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3chywfsfb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3qxrizxhx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3txzydhsm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3qadvuazw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wwmwqbkl.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ujzchsgd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3azmkynmq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3bfmkomyh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3eayczpym.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3gaxzxemj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3iuxztopp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rniiotfs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ehvlxcmk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lbjkaqep.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nyjmbtao.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hvewwult.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bcfecsqk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eouybbyf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bjuwlecc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kjllftpf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3znnnkiab.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3wrfnofwv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3idjdkwit.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3jftymude.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3yfmidbei.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ytywyqek.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rdzgfkpe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lpbledxl.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dlzonedx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3jbwxdusa.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3elpvrpcc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3xjxlfkud.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3snnolnzb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qftowjfa.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eoqqkitq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yhqtitsk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hhayilsy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xcsacnei.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3duuuxgzv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hdknqbrb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bfcinrkz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uzjggwxp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3nybrrbve.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rpcbjoim.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3dzohetic.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3vxqiagcf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3yrnevzfy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3joonzwcn.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jtjupbqu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3souxwlmi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3czitpqhn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vxocedfs.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3buutixsc.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vilybprx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lfclrjcy.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ypwtzawc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ieuelkis.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ytarymyx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3irwmicmn.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ebsblhlp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3hswcqlui.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3syctzdvh.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tpxjzrzc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qkqampkc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3pzatxnsq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rnbvepkd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3yqmvympp.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3blccrego.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3snjemjqy.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mkorlmtq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vljdltxj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ksoqdqgw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qveiiysv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3vfbmmevs.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3qdcgdqrg.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3mgdvqwpk.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yticcooe.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3vrrvzgcb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3tcikprzh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3amcftrix.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lkyzneyr.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pludtfai.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3pqjvxzin.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3mvavlkpg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3mjcgzlhv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3nrhooytn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3mnszjmmf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3axhtnooy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ubpmbihh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hgcemcfv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3baslpdqg.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lmzwocnz.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zgplsqju.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3cpchnenb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nqbafpml.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3jeemjvwe.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3sjluttlr.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3aeoffkex.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vtubwyit.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vbylssxv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3vkxjnieh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3riiugcql.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ydzpxezm.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3lmcpjwig.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3rlviqdng.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rldjkvvd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3dxhgwwrf.html


<!-- 参考信息 -->