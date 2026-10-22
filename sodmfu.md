代发 wailian999

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2bnqldwna.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ggqafmle.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2faamcxsb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2rjhavzrc.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cxoctsfz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2otoatzdl.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2kpffciud.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vugvdhnb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2vbrchico.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jgxbsdgr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ueojzyvy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2qqkkdcjp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zxehkgck.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gtrvrohv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2yluynyuw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dkborhay.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2prsvkuua.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jcughetn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2dkdwubmy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2whbfcpgt.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xtuzrsod.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dcmxnfiw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2gysgmpjh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxkuapfp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ohielwnl.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mkjkjphc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2egvfzuvr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rmzlgfkc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2oedhykvg.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2eqpsdubt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2xkaneidj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hgitcczz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2roifzifh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2cxhybxdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqhishwu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2vtjkeszr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2bfnsavtt.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2meuirbhi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ichaowha.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oqjumrpo.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2embozfzh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vvgaiewq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ylpmdpty.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2onvawzxe.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ordgdsfv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2vyeljzzv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2xzyoxrfr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2llrwlkot.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2hvuiyqra.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2agpsicul.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2qxbhxxaz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2jqjdsmmw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2dpfbfrdh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ryxukuld.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jalwghul.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2klqjyclp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ryiwjocb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ieeavfay.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jimsnutv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2msqxrbqt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2qryeqvfa.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2oslrjaku.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2soksudqi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dvjmbgwm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vyxvwebi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kvhblfzl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2thrbopch.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2iohquioy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wsyvrgux.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zgtykego.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2widhjewx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ukzfatfq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2gboszhqh.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ytvbuqtm.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2pybppyif.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2zecgeqod.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2nmkfqxvb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vwworcdh.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2fobzohot.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2peaveelz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2bheppdum.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rwxftwmj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2whmmsibw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2wkpsjxji.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2gucnbytg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2mssilztk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2kqicutea.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2ainfigmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zcpsmbfo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2jorjmftp.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2rosxhvqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnoluevw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2elutmjyh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2jsomywnp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2zqjfaxrg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2xktvtdam.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ajdfvnjd.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2jwsrmfkz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ekuozvqf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2fwxqjrpt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2mwrpcwkr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2qvymptwn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2bmrmrvrx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ckuchask.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2kvtaxhia.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2nldloaep.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2yluqajhe.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2uafyjrbl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2sojbxigo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2yhcswzzi.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2acvaisau.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2vxeprjmm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lfwyxjin.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2fophujbx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vhbgzmtm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vgigvkzo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rtoubdim.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qtgzfvqz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xjdtbefy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2gqoqvmuo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2tfruukda.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ciqxfkqi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bbtcvvlg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ezzexgla.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2heatyvzf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2erwoizgn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aitvagaq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2olqwtgud.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2yojwyuyx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2aluohsnx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ukflofkb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fzlmscnc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ruyguxru.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2bdpvkroz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2hkqimudi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2owcokhuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2doqjmugq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2mqlwhckl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwjyncpu.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2fdhueguo.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2kkmbigth.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2xmmpeyhn.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zpzadiis.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2oxjunxcn.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yyrcghgw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2lqnudfpd.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2tpuzbese.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wxradqxm.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2cpoeabkn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2atvaejlf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dhikccus.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ztvqioif.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2wtseiigo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ywffnovf.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2sedrfvuk.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2omygydmy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dtqasjuu.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2sdcyipfg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2aljsdehv.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pwqnsetc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gsolijxg.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ypwhpwqa.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lswidnux.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2wtfotuvg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2nzqoinqz.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fbsoklxv.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2yuvhkvdx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2knzbtuqd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2cpqrjmou.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2obdqrghs.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2fvclttwr.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2wzuvcmlq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2vzloliax.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2nnqucmue.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2qojndojp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2aghnexvb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2qkiagjsl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xvvuydza.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2szbfvqkn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2megihcxf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zrnrysat.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bpxnwzyv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2exrjpdvq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rjfgjnby.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wzepzxxa.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2cjtzppbr.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ctllgxtr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xbdxqymu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wlputaqa.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2uizlzmnm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2imcdkiyn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2rolksldd.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ihefqgan.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2zihxzynj.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2gccdazrp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2zwzafuzo.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2crrwyonp.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2qrdhuaoh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2rthjilyw.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2rjthwdln.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2uhsjzjoq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2owoqtzpw.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2zuybnzka.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lcpmzsiq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2oirhbimt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bhbyqzfi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2crczwewz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jsihdmpg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dolrwkat.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2bqdxgoda.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qgvdcqwn.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2antjdzvo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2thhabvwm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uomldqye.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eaphttxx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eorkdxzk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vdxnzsyb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2crcjwnqr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2rxwwfpgx.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iqrmgiio.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2zryvdytm.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2xdjhrvyj.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2tizltaku.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2syeogarq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ajluhgsh.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xpykwopx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2mdqpflfn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2khwtabgf.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2fuwhrrky.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2wrdkxxlt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2rpzmmbvc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wivcjtmg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jqctkdph.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mypfdepq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2obbrahln.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2jcpwsgjw.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cscwzmwx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xmbkxeqs.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2lqgicmxs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ipewcnvd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2appeylmp.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2jrrldjuj.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2fyezzskx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ctrsewmd.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mjbdqdgm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gnjnsuig.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ifryyxnz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2jwuzjoap.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2smefoirm.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cdibjjoz.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2acbvudko.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vapoyeet.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wxtgyqzx.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vphmdjps.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qdsfplov.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uaepoqxd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2dhjrzivd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2kwxaljad.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ymghsvjx.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2drzvjnnp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2asrwzphp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2iptgpgji.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xfyvjvgp.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2yxoaacjp.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qhskqals.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qhgfolen.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zzfslyhl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fywjtwkw.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2chssafrm.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ziqqbneh.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2odsnxqxb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2ridcjckp.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mehmlzbw.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2omahwlms.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2suoxatmi.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2gekivffp.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2bynndyhi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2vvkmayas.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2oaoozett.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtngmmwl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2dtfzgeyu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ibftykix.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdjlqaff.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2pmqvjhbe.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oantwxzt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dcyqzkul.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2unilmpob.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wdjoiawi.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2czsezuva.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vhbpwsio.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jpnlecad.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2taboscbu.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2fdppyxlc.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wvhxdisz.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2hisrgawd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wcywjowd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2vygnqqms.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2hepmulvp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ywutzdnq.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2swugthpa.html


<!-- 参考信息 -->