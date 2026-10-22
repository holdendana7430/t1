代发 wailian999

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ewfjvooe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sgiupnzl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vkruuden.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2wvyrtjuy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cpcgxdku.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2twdbnrlo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2uorjjjzj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2qmroeakv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2pijwrikd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ltkewvdm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2feomlrtl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2wyplydpv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2ahqgftgs.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vtefztfd.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2zrfeewsg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vhznkjhw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2wxselxsi.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wnjqeral.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2eagiqdfi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jpioerbo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2relxaosn.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2csnoiavc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2dwwixlfk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2dlojsgbl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ekeghabu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ntvovilg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2xqnixhmk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vniaqluj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ldgdquid.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2nixkxlpj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zrpovwyl.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ihwhnkum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyemdaqa.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2lixapesa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfelbjop.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2vhkaenua.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2legebkzx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ekduokqc.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2pzmfssrp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fdxlsvvf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dicqzzwj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2lpcxjufg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gjwpkdtz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2azwxtoqm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2pnfcrcmr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ydzgvihi.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2byvsdmrt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2awwwhkxc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2nyeccgxi.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2tjtwzfth.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2knunvfri.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fqjoazvm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2oqwfahvf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jmwpqmiw.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2qleahwcu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2yvhbizbv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2uyqdpbra.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gvzlvlyq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qyqlycdx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wmeqiheh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2jgfdorbm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2czyrvlxb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gdqfrrra.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xbxihqls.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2asirkzai.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2gubkdsou.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qcmnsqxd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ikwqovdz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2koytzsoq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ymvcswsp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2jwnkowla.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xxmxeojf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2fyxloemr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bqnwpqpn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2fqqxxutq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ouqouctj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2lgddfvul.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vzqtjznp.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2iyvghcpv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2znzbtvhp.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2lyaimbgr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tarxrcba.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2bqcnkbly.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ksuzwawe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ppyfjrjq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2dmtyypmn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2dsejyzii.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ussyabjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akdmutwk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2nfvvdzmd.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ycuofkcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qwieemnr.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2pmhfvqkw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2krjxjjnx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2hghulpii.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ytjizspc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2yttvlvvl.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2himpkbul.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2bhbtcfmd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2kcsouwuc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2dxlivfhp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2hkrplfsi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2fdgnhoft.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ghqeofqy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2cpfzlhxq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2jpyqfngh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2koaxkaid.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2xjhjymnm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2pdfuwimm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2qvbmbkcy.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2vpadocno.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2kjduxlyr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gfsrhiby.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2eqnkiyhl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pirjonpb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hmernvgq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cqlttvio.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gkxuwzbt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uxpvoiwv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2zsahkkpv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bqtmjmly.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uxwnyqll.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dfmibefi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hnofsuiv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2igyhqixh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vstdyjwl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hhsfugza.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tavylihv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2twpjhpvn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2goynhpqg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ffvyfxdb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2qxbvohzw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lzeamzwk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yhrykfwj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qznuugxi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rzofvphh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqojvega.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2wzuuggsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jozcdjnj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2emjjfzyz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ieuyqcun.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2arbngysh.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cyxwbaqo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2kspxhmhr.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xvpgwtqj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2duycusoa.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2fnqbclnc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2epeogkyi.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2jvqxlrpf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2frxqwnlm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jedtpoqm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uucvwpqe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tvgcwljp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2raatbtwr.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2vcjxmmby.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2cjanrgiv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2flwetmer.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2cktvkriw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2nawlsznx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dqfobqan.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zkssgstn.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jynqimey.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hpwyrnyn.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ugbwzuwp.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2mthwoxvu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2extpauns.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2llyarjkr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2kfuxvyxg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2kzhisrex.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2zqyrxapd.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2cbfiuggb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2tkptwjnl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2mgdcvoac.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2zzqqwxxf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2oachsxqv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2subdrzgv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2mqtpjwmz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zmqwrbov.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dazurino.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ocdnazni.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2citsibfl.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2didsiflq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ffxjsnze.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bukmjhpi.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vikykyte.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2eplhjeqq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2npqjsinx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2osbjdkfg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rfzvvswf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tvjhvlbw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zrsynnxy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2blnhpocs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2duysdauh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kqjceqxi.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2sjvekfyo.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tyryuldf.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kpwpxfwn.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uzqzbesn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2husjcbed.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ugzugcmu.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2nbyemfkm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2gpmatmvu.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2brigbftr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ievzmcgw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2qpbhdqmm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jnijnuwi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2twqdpnte.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kdkutkoy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qvcvtoow.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2mzozskps.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vvfiibfb.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2otoilnuh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2drxgofyj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dzthahkp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bvisdgne.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cibfkfqz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wvfqpwzw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2wtlkrszi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2lpgcqzlx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cotheivh.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xrysgxph.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2wezblhvw.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2uhjdckog.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hhzpgszt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2znzohugq.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wozyfkkn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2fwohnkqu.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2llxyqcai.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2tbcxiryx.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2pefqxytb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ctguqtvj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ebmhqgma.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kweaskvj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mpbnkoqk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pwdnnyzb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ahkbywsn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mlpayvfo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rzlijvse.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2miobpjpo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2xevswqfk.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2vhkzblgb.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2siuddvvt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wlbuhkfk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2tyvpabui.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2yaedgcnp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2wdcyojts.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2oysmysgh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2qggbuyip.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qyqsqklf.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zkynvcdz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cwvaypsr.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2touqpqsh.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pmfxstie.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zxkddpzp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wgafykvw.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wbpnibvl.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2wsjahwus.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2uribddou.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2aifpawqw.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gqtabqtq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wqjzxmhd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2mybefueo.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qgxerjcx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2mcnmialx.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fokzkvis.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2lejxtrqq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zoxvzgir.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wfdhtwlg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vhtzfjcu.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qoctregr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2olivrhdm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2qeqfhzbi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2bkiblasa.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ziedbxci.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2sndebvfk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2lrhsgbma.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2dzssknsu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2nswrncoo.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2clkspzen.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzocqqzd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2prjdozwh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2zgzelqzr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2beevufie.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2gnxflnwe.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ixworjjb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gyrsemhr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bkpjxqtc.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2upzbwfph.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2epiojoux.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2zuvdipsk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mlikswyw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2opflpslk.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2pzxwgtdu.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tekzkoiu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nbqrjlzy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kmmjqvtv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zpjrsiib.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2zddhedeq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2bkdhlzkx.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2dfrojxup.html


<!-- 参考信息 -->