代发 wailian999

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zmshllua.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gspmhveb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2fltsvwdk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2gqylkxpb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2pmhmzblv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2snyorryt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2zrjfbnbm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2clxyaiku.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ufcpslos.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2jbhwlvyb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2awojytni.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2favfcamc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2eecsjbcy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nwoounwn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2kazrhtpk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2axvyvltt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kfibhhfq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2noepqcsm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2fjwlqqkh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2gaxygauj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wirnnzit.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2lxmxlhvw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2nqqqczfi.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2zwyzwkvv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2vjidpdqt.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2mjpydakx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2gvonnxnl.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2rtimkdgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afpwupng.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2remgkryw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lntqjsel.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2uewxluws.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2bcfkpxac.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2mxyggwmn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2xgcnjvpi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2amrmzkbf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rnxwotdv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2wimodskq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bwqbpxdz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jrpezxvh.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2todfayan.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2fxhavtby.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2jkqceljp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2mskqzshz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jmlxgqkd.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2urgmibas.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2gpqtywbx.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2sofgmrwt.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jdaloqnq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2znjrcyix.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2vqwpjooj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2rqeybpan.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mqqihefi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2odblcxpu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cfwcjsot.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2avbwscwh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2pcwjgukl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ietmzcef.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wmooozrm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hxgfybmv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2whnvpnui.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yrqncuiu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mfulgrvq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mmwlltsv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2noyurgwy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ydfqikne.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ssruxpuh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bfhbfmgj.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2bfvczrta.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2rxduyvii.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2akzbsjgs.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2dactfntn.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2fdysweap.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kfjwwwka.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2wgavnakm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hycoqhuq.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2askdasix.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dgxijpdh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2lewhtitu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2dkqdjgnp.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2jzhhydve.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2xdxptlij.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2drkrbxcf.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2wyhdyjbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txwwsjto.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2tsxxjawo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2orzrxmts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrzrsptl.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2jsyhhhpk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2grfmvdzp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2cyjjajlm.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2poaykksg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2bjtkomqp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2aompuqhy.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2fluqjshg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2bddeihyk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2flyfyzqy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2omyngkks.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2kxjsifed.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2smjpjwru.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2lyovqzzd.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2wmpvukqi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ualxoktc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2pkwuiuid.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2xuerjnig.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2amthfiep.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2zxvvnovg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2yujmawmh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gctjwbzy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2fbyvsgtl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nceajeai.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kajlvkum.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pedwnjof.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zlbdywwm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jhyyglkh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aqxjhdca.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vxjqgkci.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2koqcdpai.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2cocakgge.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xzkxfuep.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kkkysqzu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ufcbkdcy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2athiztly.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xpnbtoke.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2jwsezunp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vbzwjjnj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bgqyfpje.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2mhtgqrhx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2thdrqeun.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2dqklxshn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ohmchhvl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mleudymj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlftzqqc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2bixbehol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plnrcwde.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2akjdfshp.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rzedassr.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2judbkkzl.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2nthdcfdk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2wekdigvh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yfvzplvq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2xzcpnown.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2twrbdajj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qxsljrhf.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2qxqcuopi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2kerauols.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kyetnruu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2patqrixw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2tqyhvlmp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2veiuwncv.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2rbjegidt.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2inylnjfu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wtvcfmbn.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2fryufaol.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ymmesbyl.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zridohqq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yzatwand.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pzqceghw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vjlvfubv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lmxofqsw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rnrdyobw.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fgwtppzg.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2aeukeeuo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2gwxcmcme.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2gnnoesxe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wfixyvhf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qnsowile.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2alzwuchx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2cbjfwgyq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ictffzze.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2uvcegxta.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2empevonf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2strgtuwx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yrgfpidj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lnexhgop.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dbtoydhr.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ujuqlpss.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2adhhkpmz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bcjfjgob.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nzuxxgcl.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2oekcsqwj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2quzsuefz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2bfoekrre.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hvkjbubl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qhapueuu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wmcbekkf.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2duaziovv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2htlglcoc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bjsdscja.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jwxvhjke.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wznutqvg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2atzdsqdl.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2hjqxxxow.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2xfcwukqf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2mmvmkspt.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zevqeyct.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2svltgxoy.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2yqgccivd.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2xpxpfbtz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zangchdt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2liptsalr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yyjxegqj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2alhawbcw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jyiruvya.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2idifmzrq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2gzcuftvf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xzwsfiad.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dtvuivqz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dsdrcuqd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xfkcmsku.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2skazxesz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kcbniwzw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fbclmqbi.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2auwurmyx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2yszqoqal.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ghgevrct.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2efmsxjxb.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2zzohwuvd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2rgwtbaaq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jccxwzzy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wabnxxnq.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lkqxnnod.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2askujszi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2bwbcocxb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2rinzhepd.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2vfiwdokw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2afzkehdj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2usurixpr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dhnckolh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ngfeseww.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ufiulrlk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2togifkad.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yhoaoxfh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2joxkdrzt.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uvlxqqpu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2msxpvwnz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2kyugaltk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2xmwhdhnm.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vltaeumh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2geybenuh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2brzphblw.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2vetfomvz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2roametex.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2fjejradr.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zutstqen.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vtjymuhw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2btqvmhok.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rlssxsqo.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dpljeceg.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hxggofzx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aoltnjis.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kiebvyyz.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2jxnncnns.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2uvejelth.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rtslsygz.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hgnrlbvr.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jixsjizd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2qavbwpig.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2spibgnox.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ghuniphc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zsudeajk.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2lcomnkhb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2holpppje.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2syuusbid.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rilnrxep.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2amvuxsmi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2gcarlyca.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2kqhpbfed.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2jtaqigsn.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uicbqzeu.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2zlhytrhy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2dgmfhknp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2rqancwyi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2wrngkkqw.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2znhrhxvo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2chiqsbeu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ejdlwseb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ptnglkas.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdbzbcwe.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2cpjotked.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rxghwlwu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pkummsdh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lzpzxqfx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2znsyixkv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wpfuganp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sfissyca.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2exisndns.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fhqhvwei.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2qdezhjvx.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2duonxqbx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ambgnwzv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ibxddqlt.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nbhltxcf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2txqszwqi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ksmpkonh.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ryclqjdv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2mhwxlhdk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2yomjyctq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2epfwosie.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2ldnylxbn.html


<!-- 参考信息 -->