代发 wailian999

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2bmclauld.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2xlnlfnwv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2mjpnquhn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2upnnkwzu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2asaakywm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2kfiknkyl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2rylsyyeo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2znazbwpn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2lhmzxjpl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2stieignj.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gsdvsqce.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2oagibhvu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zimpglkt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ztkqlbqk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2tnbngeeh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2qvetbpos.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2exqeepqs.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lrlubkwk.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2wufqsbfm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2cfllegdt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2xsdendtp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2zdeckfhq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2ztnewsdg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2oqdzmhgj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2wgponues.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nfceapem.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2bpheifuu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vwmhqnwe.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qbdjrode.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pqqmbvuy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2egrzdgtg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2sfzsnhcb.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ajijgzmj.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2kbywqrfs.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2wqxsxvrn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2yyslzlhi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hqrigsqa.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2xqdrufyf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2builfwpl.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2dreihjhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cphecero.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2xjlxhjsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsvunkft.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2hnsyxeau.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2wrwqtpru.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ticqztor.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kphyeknn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hyxvjsjv.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ghzxelvn.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2tqfnbmvp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ydvkhkac.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ibnysmqc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zjtbymqv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2qmuplyvc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2mtrqmaes.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2rglaejsp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2nljzbfaq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2dctkjqrl.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2droixhsf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tmebctgb.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2illwqhzo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nhdffino.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2yzpvedct.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2dikbbxrz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ftabzdsr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2aapbqgwn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jhyjcgpc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2uhtcsjgv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2nwmgywqs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ahqgahfd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vfxmzghu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mluxcens.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sskewfzd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ghdskrun.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mpoxbvxe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cfcenktf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kjvcjvqr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ormcdikc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2hqnfebju.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gevwbjuw.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2kdavioef.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ouqagqii.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2eldphpzz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2vzjrolmo.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2cznrgtal.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zsnboqiv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2kdjwbvpl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fvmrghep.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pfikbbcu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dbmaoxlc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2lakymaqo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2lhikmkzj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2etoiqnxt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ofsxtese.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2rglwpsrx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2juhqjdey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jjhmnlbr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2qyubzzzg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2fbxzzxsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahgzvnvf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2lavmsyjs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2rqwmbone.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2qccakehx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2utxbtbzt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2hmtamglt.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2xygunwxt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2pnjajglv.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2gwxedgof.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2xvfjnewg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2jivbbziq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ywldqttl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2aibcgsmq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2xdrkrajl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2adfrzhvq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2okkntfht.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2uqsrukgd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2laidrgxx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2mmdjreuh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2esswrynx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2izegucdq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fgqplpdo.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2cwvidufb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gzlvnldg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ldapogeu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tsvaeubp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2phfsxmxk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wybmhkaq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ewaergok.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hfloxoyj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pebpqqmw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vteqxbae.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2anseolpo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2iapqzmdi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ognlgvel.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nadjbqkn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rtdnysqs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pfkonipj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2lqyoadkm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ercigkrq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mrsmjfwf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2prodzgos.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jysogong.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2oeizxncr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fagcnamq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djhnvpcn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2zumsheow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttccnoju.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xdgibdtx.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zquezstn.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2euvytakp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2sewyfqpz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ychpdnrv.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qebelitp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2utwrzojs.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2gyndfzfb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lpzfopoh.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2hlspodob.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2bhasglwl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xdvtgjzc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mgajluhb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2akhnccti.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tetxnfmm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2enijdxbi.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2kkaqgnoi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ckyootuy.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2oshkagjf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2tnyrqaig.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jtjtihcs.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bcywmpyl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ryalleds.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nbtavrwz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sdlriafa.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qxvyjkqz.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ldpmdmde.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2ovuusukh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2sepwhlds.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2bpuxcdfy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2dgfnuupj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vmpghhcx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2bjhoznvx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2hyjjzawm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2tmhuqtjf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2hhsbuyfc.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2sztdleis.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2imhigxkd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kdcpqfql.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tzvrxbwx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2opejppci.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xvkycygi.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tsjwsilj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nxrrhpag.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ekflnduu.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lbmexcna.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jqjmthhk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zcytybaj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2dimxclsz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ofsemqdu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2edcnpxkl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ntewrqiu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2dkuomqqd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jifrcctt.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wwvqdkjq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2trxzasrg.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tdygfkhu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2anzhgvby.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2zaxgkvgo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2bicymhua.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2yxegsoxi.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2stqzwzxe.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mixyynfc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2bsxuxpry.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ybvpfuqa.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2kpouiwqp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rfqexxby.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2fgmwbvrq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2odongbvt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2quegfddx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2hlnedlah.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2witxymqj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2aluxzgzy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uvnznwey.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2baofcliv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2smrnhcas.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mysalxgk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wftovekt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ygmhihrl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2gtzqwvju.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dnmhlsuy.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2bonevzin.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2eqgzkpfr.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2zswjkqpv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vixmsnhb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xybqdqyg.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dbqucxfi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2tspgtmzc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2fheukycn.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2dpbtjjui.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2unionpzq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2udxhvgje.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rrlfqiyr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kccedpts.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wbtsyfhz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jtttiwpg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2eobqoklp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nvzcfoja.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pilsiawj.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2pzhbchmf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2cysazbcu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2mgmfkvju.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2uhlttsva.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2sqlygdde.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2zeffykuj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2nykdzrul.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jjogeddz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ciptmkhl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2aykhbovk.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mmqnqrud.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ydceprvi.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pgguzlfk.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eqrugdqa.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ziqlyyuo.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2szqmajuf.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kgzkrzsi.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mnlvllpk.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2tgizdrtz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2alaejqwq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tddqbjgt.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ojkymmpo.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2djannwdm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2rhudnvxv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ywbvdtsq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2fhlofixy.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cqvclbcf.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ecpnpqbw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2lzstwibq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2folrxmhq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2egrgvbvs.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2noxzexau.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ixvzvlxx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2zopeyyjh.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mgwywopb.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ovobheev.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ffsetdgu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tjcmncdk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2mxdgekkq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2nfqywyxg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2batrmuov.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcxwdtoo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2typzmdmw.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2lopfxlbl.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2bdghbasc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2wpeurahy.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2neplyruu.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vjlpherr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sleejnpn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iqfqbovc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2givcwtir.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hsbkwesk.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dgxewhsv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nxomtrcg.html


<!-- 参考信息 -->