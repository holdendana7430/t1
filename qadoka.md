代发 wailian999

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2vjjkzmzy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2szpiwocd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2azstfima.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2nbhandbr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zrmqdoka.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dvigcmaq.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2qvtodomm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jylphndo.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2jkmchfuk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dcjemxnq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2rrswjcho.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2wxvmctvw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2liyjjcfj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2khccdayi.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2oltebfze.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cyoblcin.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kzxuzums.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gsfdmdbc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2uavdsrwq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zoccjoyv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2xdcbgewa.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yoqonugq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2nuoperke.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqdfmqus.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ebadrdtu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2izwslyyu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2vjhetfre.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2fehuksue.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2qukzcukx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vwahjlpj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ejuwsilx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2pjdzjewi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlwykwgy.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ihwpbzif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjdesmjo.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jcfvufok.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yjflpcvu.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ezblzckg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2faozgkhy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2klbfxduo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fplpnvpt.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vfkjqaol.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2eyhfaopd.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lwfibnud.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2hejlgach.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2exnazrht.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2phnzzllz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2zevhtkww.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2sxatlpze.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2wfcivtet.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2rmejmpqw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wguwzlks.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2hbngndvg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ilbkcyys.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bcjmllnw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2gafhkvyt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ixkjrmbv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2sujvmwez.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xrhggcja.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2joorqcqf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2zpdpwsbv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2amhfuyzs.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2daboagbp.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2pckweddo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eosenigf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2femqngke.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2meqvnujo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hiplhqnh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jhxrzcfl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2azgmkybr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2jnqisqky.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iygbkcly.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2yzkccxsl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2gvzrbuwx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2klmnlkha.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2kdbuainb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2htvhkaak.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nmrerzbf.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dcdidoic.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2maojjoll.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2voegejod.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kpbimrlb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2yulgiqjo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2cvbcxxej.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2iotegveu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2rzytklel.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2utlrrehy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2njebocra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksnmzzcc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2sjorekpa.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2tqyenfpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ashfhomc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2jozlivhd.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2stigqrqr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ztdzgswi.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2evgsgvrw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2owresank.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2rtnwodyi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2kntynhma.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2yddblagc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2afgbomct.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2zugenypc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2dsbrfojo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2vuzajhot.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2rtlpvfnl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2yjrylrjl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2xlsoxgxn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2cubwidim.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2jfnscetw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2mlvjsevw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2rnydbgwo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2lvfnauwz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rvmnjish.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2sxeskrby.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2siliiqxf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2lehtykbj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kcmkkbdd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jhdytznr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2uumclbew.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rxtrsgub.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2horzaxro.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xkgmorcj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bkahllhp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2aqdvxifm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bobrasrg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2trjklpuh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jfyewuyo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zupfxyhu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ecqwvybp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2lqkcovxw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wuucxkwn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fxisribi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wvngybpx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2gowmkwlv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2muusbngq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2bxmnbsne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tijxdirm.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2xyxwkszf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arzmyzrp.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fhbzpjos.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2voikerwa.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2uegfjphy.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gwojyvth.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2yrrazpcw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2sreuopvd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zfzinmki.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2kpclwgxd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2eseguvds.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2qwzdcgos.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2aunkikjd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ysaqnefb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tyipbohc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ewhqyvnn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bacbmpay.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2hilrsawh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2iaclpipr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ppiipksh.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2utvwbnxr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2nlmereeq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kqqvnqts.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qejrymth.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2btpqpyye.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wmfilhhx.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pqonqqjb.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2plexklay.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eawmljiw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2pefxygnt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ghgaucvc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2orvgwgya.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nnxrdwcy.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nnqfvbnp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2cqrjhnhc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2awhteskv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2llratlig.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2gmytkehs.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2mavwdmlm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2lsocjayx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ajnpvbda.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rsdcgtnh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2egeqpsny.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wkguqddv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qhkhmyny.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mxlqbdcm.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jftibjby.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ujljbmac.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nhrjxusa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cwgkbxgw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2atnsbmrc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2eoylqlvn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2aoasmrvy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2nqqntdth.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2hkumzidi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rchhvcpn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2zbchgvro.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2sfbkprnm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2jfreovhn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kolfchyy.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uczvnycx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qxpmbtxi.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2chnaxvus.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2dbumsjjz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2awwewpdq.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2lmylgzef.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cxhjseqi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2wyexrzmh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wmfevyph.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2hzhrxizy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tzxehacx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hnjyqozc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2qzplxrnh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nyguwote.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2eqhmbkac.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hiwznrpa.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2clfwqgum.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekdlmbev.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lptxujvc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2modgcyte.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ssnvahlx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2frfeqsyw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rrnmegmz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2mneruudg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2qtdshjeb.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2lodulhgn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2spspbtpd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fegxfgce.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bseuhvea.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2gyraputo.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2kipoeieg.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2bweeyiqy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2uppuuitw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cdqbqxpx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2enkdqauc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cyqiovfd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2phudwary.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cvobspjw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2jttxeueo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qcxqbaob.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2codedzrk.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2elgnclxt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2lbxcffze.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jlztwttf.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rrwkxawx.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kwjgtiiv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ypozioda.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2wuztifvx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2knxgesnc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2hdapnmvq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2lrqutgcc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hwkbhiaw.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qcrelfet.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wksbytqi.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2raleebxl.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vzyacnng.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kwowjgmu.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jtmxyssq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uzlqdoox.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2qokedgac.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2tvwmbukx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2eefzpwfb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qqpnuxfa.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yenqiava.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2kyzpjnta.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2irhhoszo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2qmqmwsgf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jmhzlktr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2plkekpul.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2bcmodljb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2icfaiyku.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2weprtwnr.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2udwdewjn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2mkhcyael.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2idlnodlp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2xssldblb.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2veysubyv.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ewbvvjrt.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2cornguos.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2fjyzneqa.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2uwqpansl.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2iljobgto.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2obtvzqjk.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2mzldhcpj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2uloyljxu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2fisrocus.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2zgiotcsc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2eqonvfjk.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zsrztshy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hwkkiedv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iiynhwnx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pbjhapqy.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bdvmjevu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ukcgwgxo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mcnojkye.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2nusoauvm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqauodv.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2guilzlqn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2psszrxfo.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zgooagtw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2lqrdayri.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2xpqsdjkc.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2mqpuqmaq.html


<!-- 参考信息 -->