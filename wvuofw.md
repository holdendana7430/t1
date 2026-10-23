代发 wailian999

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3bxyxswbn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3dranqxxo.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ktanthrs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3gjwlligd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3kfrckdyy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ixwmrkvh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3iwdhmemk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lapjqkdw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3oheltemw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3amgmmjgd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ifkakhhs.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3dtwawahx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ylzrnygd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fuckkigb.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3ziizxlps.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3opvqynnm.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3ofgulgay.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rtdtldfy.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lqloigsr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3bdvbngnv.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3asvimilm.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rivxpszt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ukubybwi.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ybtxozyj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3wmiamoii.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3noqsuruz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3omvsvepi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3icsjypja.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3irrnahzx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3boshtfsk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3dueraxdd.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3rdgshuvb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3nozgzvzl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3oqzkjfmb.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3lfeihmcv.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3fynwqklh.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ueoqjipk.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3mormmazk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3vermcnxy.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3riujzboy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqupkafb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3oiloleej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3giguyogj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3fzqwtjmj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3zszwpbac.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3sjesurfx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fdeoljwq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3cuflorsx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zjfgabxk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ztaidcit.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3kkxpjbbs.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qlzgdnhv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3fikblyrd.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3jbqumtuv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3tzssygwc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3dfjvkskk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3amrbajqn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3sthceuja.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ythfufef.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rywitkio.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3mcxigshj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cvqxntzm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3lkklayeq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3dvahwqvp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fjtgbttr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3usqnisuj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vzwfdzzj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3spvlraiw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3fdimbaox.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jfcbqqks.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kgixozyk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qnztjhur.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bigduguo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mocjezlq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qciulwdi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wkmotwgv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3slpmhejk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hsvmqmen.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3gluxevmi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3laisfzqh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3xzjezlhm.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3fluiyusw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3gonwfvwy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ejjtxshz.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3welaqfls.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wwywyusz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3viszyhnu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sbstlipu.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3xmdrqpvb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pwtthapd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3dmvuykui.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ezffznpw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3bycieltt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ggmudmel.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3hztluoxi.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3sjuwtilo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lskjgiwv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3qcdjkbsl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ofglvcsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zytwlhhz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3fdvtedmi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3gwzmjyot.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3zesszhxv.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3uaktvdqg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3jiltzqdz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ybudvouf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3xopzqogo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ceuccizv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3xfbxnrqt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3hnlgwxoc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3svwumlzi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3dfbcvraz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3uelfrbvv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3lyoochhj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3blbvrjzh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3oajvogwd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3hxozwpcv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3kozqodsq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3sfopqdxy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ugrbzuzx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mhpnlizw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3jdsjuhho.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mlsmvsrg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rldxwtyz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3opddrgty.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3iwwdbcbn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ydlhyyjz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ynxajque.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3axwfyrbm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pfrnsgeo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vcaitvxm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sxdbswmy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lbzpgexh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rpmzhlcx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uqorbyyn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xmtmymza.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3luqlgpwh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zitbemdt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mzdtcykk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3avvpdkhv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yeqcuaas.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3elxqekza.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3tbsdlteu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jtsiexwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vesodglf.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ofedgiuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtceidfv.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3xaetesew.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3fthblrsu.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3hbyculen.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xpbxwurd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3tlqlcjqk.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zkpulnfx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3usvxwyxf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3ztajncod.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nckyuutt.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3exhdcqts.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3pnblzzxg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wjdzkrxy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hrwpdtty.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3avtzgvoz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jyyyfgmi.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ceedzqrf.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3rraipjzq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lhrbjcig.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3vlhjeceo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3szrivirc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3huxesjcx.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rehozvus.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nemuqpiu.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iokwudnw.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3orkjkytf.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3hfstgipb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kvezxvtu.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tivpofxw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3qzrermbw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ykajqfic.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wpajhfnr.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fqxyyvef.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3vzylogrl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3qjpekhax.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3nmhzfjnr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3nkzxuccw.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3zganseho.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3haewfafv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hgyynddq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3iylvwqse.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bougnsbb.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3manaqxix.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3epktbqbq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uswlutib.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vykndofo.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wlqtstrn.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3efesgpra.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3fjtheejn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3gkzndixw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kpxwgkfd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3djepfmnq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3jnljgska.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3vtosvnae.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rktcwgct.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ukwmtexx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3jcqkgsui.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kthocojz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3bcetvalt.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3envqkmwz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3nfdqbryb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3clggssan.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3xfijbopm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hxuanmok.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3cevhegeq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zjnbymhs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3lbffvnrk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ocyggfsn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3qpvahglz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jhxuxpdy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nljfroyr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3dqkbualn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xgnlaylg.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zgicabpa.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rmsctbdr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jluyrsvo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wilwmseb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gktshnjb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3opinkreb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3tzqizqzf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3zyokkpqy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qukjxbtv.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3yyoyefei.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3hjrraewl.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3kyszpccx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qawvedmn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rbjugskq.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pogojhes.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3vrdkrmup.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3nchmquzs.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3stsxqmgk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ehypwyfm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nejoajcr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fgmtalds.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3euuijuht.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mwbfskir.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dszydlfh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3lkqritxb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rqxmlwxc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cechvjyo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3rddgwltz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3nihdsime.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3vymppyzt.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jfqmudfo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3egxoqadc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3pqotkxzq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vychiolm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3csaifikd.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3feplcedk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3fsguejih.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3arhfgnla.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gdlcudag.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wsqnurhx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hwxmiymi.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3htgbfjcd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qlbfeqeu.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zkajplwc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rrvfuplt.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3hzmrvnzn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3bczurkpb.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wdtepzdi.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yffcnauf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ltejyolu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3qigrragt.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rtssmxga.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3hzvuweev.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ifqrmixo.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3rpfvedtw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ttkqnkap.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nrittodw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3yxucfpfj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3hgwrpeyd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3skxgktbf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3nplrhvld.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3phbhutha.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vmkfgqrh.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3wiaoqbvo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3hrcwhorj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3bozsfsqi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3rwotvlat.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcnwkciy.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3mogbgsxz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3vnsbblxy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3lwdafdxg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjijdtos.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3vwazpavy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3mezxvzhf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3whkzbapf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eagsxfno.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3swjwrxtk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3doakwtjg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wuvizkhg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3gfcaansl.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3brkbbxhm.html


<!-- 参考信息 -->