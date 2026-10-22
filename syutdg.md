代发 wailian999

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2sxfomtep.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2qssfuvnr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2jzxasbyj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ymqmnwhz.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2woqzixer.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2hzvotozi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hatdstnr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2solblxly.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2voqtjcjq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tbpzsxjn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2bljtslic.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2sovrumim.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2wqvonhly.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dmsgkxtn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ychshyfi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xzscljgq.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2igpbqrma.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2poavksol.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2uqnboekq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kffryzbe.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2hhikgtyi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vaitakii.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ngjlscgb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2quwmbmii.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2lgitgooh.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lqkhjazs.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2anblkegl.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2xlnyqzxt.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2haoiqllh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2gftdrbbf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2iwqcgosi.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vrgfnnsr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2tmffstud.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2izlyjyxa.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2mxuqfnxo.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2dyjjeiuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rghiuumb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2fdkkpatb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kghddchq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2psdmxeon.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2uihimhey.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2hobamhto.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hqkuerpy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rrtbujga.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kvldhrxv.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ueqnghpg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ldwfobwo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2eaocqfiy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2wnifuegi.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2mptzeapo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2mlntarap.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2bsxstycp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qfgkhiqp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qjduhgjk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2onwynybk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2orwkzzuq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xobtvoxn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tehuuufb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2lequiajk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2nyxeyabt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qchfvlns.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cynbakky.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2necbujdp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kakrnxki.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2upcwxhwz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wieieeaw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jjmzwpmc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jqvczlnb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ofbftzwh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nkixwhah.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dsqyyhtk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2soucffrm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2afalnycz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2hknstbjk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ggjzyify.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dumapmhj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2cmiolblk.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2jukaahke.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2fhapleyx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hubfzyxx.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2socwfcit.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kudaaeer.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2xqezxszy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2umvjhotb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2fcmmawod.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2neyyjpdi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2kkwtamza.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2xbdrorlf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2tkaryaum.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2augwpqrj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2xittzoik.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2rmxczslq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvwfrfgf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2eyaonoiy.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2nhpvcsko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djwhzqti.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2rpwqiclv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2inautcue.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2irwwhqqv.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ydafpbab.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ahnbbtjb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2mifciqsi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2xmbxxuzg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2hxhnoaty.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ozdvcudi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ijdxsjsj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2cjlrjkri.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2dudhpdhb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2kxvvxiuj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2tfwyiapn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2qrcswpwp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2oftecagw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2qwvxrxsi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2hutqouij.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2fkknmaaz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2bczqbqin.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cuaapgvl.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2mfesuhjh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fmosnazt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nbymgmtb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2giiepelo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2fqsxrqjs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iaevegdg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2zcvunvwu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bmdlojup.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wymumifz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qplidmvc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zfpolymr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nqmpuwwn.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qtcoojuc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mstyzemw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2voxebihe.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mbtfyokg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sugqljgz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ortibpjh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2rlmvorpt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ggmvuwcx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2zswcywuz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ksztfijc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mmofyasx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tskvxtqb.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2tbshonjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lkzvvnvc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nulvzfwh.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2fpnxzhdd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2kjzzrnyo.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jliexcac.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2dozqjfxw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lpmwxiak.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2eryzsasy.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2phvlbyxm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2iygqrjvh.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2bxhccsjs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2fykfzlqh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qegfahtu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qzemmplc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2durcasqj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ygocriim.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2qrtcrydq.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2krmjzlhw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cbvznctc.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2jdcgsbhz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2zbpmtvhf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zqzaalzj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2anbnsaim.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tjnsfhch.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yzghfyko.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zivwvynk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2avyilpoj.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2glboiiln.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2egikrsiu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2camwptvc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xzzpdmsz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2albikprv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2byjglxio.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2bdeyqqcv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2llfnfett.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2nfxoyuud.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2nokkxbtd.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2gmfmlzfk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2yiblolib.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pdphctae.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wwcrbire.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fizuirth.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jwhwpkjz.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hmryuotx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2aogtexmz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2arrphqme.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2duaodgyn.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rquyqnhz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2banxeerx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dsweorxj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hmvsfppv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2fwscengo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2mhtziwlu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2cxkwsnkx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bximwhkq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2poumkzyw.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2tptebxlg.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kjvbqzph.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2dktegjmy.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xznldmtr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2znrjjqet.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2klmhkqyv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2baezhwhl.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ybtmzenn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2krvdyydr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gswxbokn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2btpdvckv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bpeakztz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2aftmdsoi.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vbpaatdv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yshjdzno.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2jozfzinl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gydbudqo.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yzuqdkhe.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2htzuopup.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2explpozi.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qywpiovp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2grywbpis.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2druzltzz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2vkvtmjct.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2kpxbrahb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zwuyjsve.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pmhajwwl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2hilhoiep.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2qkxqfuxr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2bqjpnctr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qxwfiprv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tahbbgth.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2okoxpobg.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ilcbadmz.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2uucsxvyc.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2fhqaxguz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hbzqicbn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wiypzmpz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ieztbdaj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nqdkpigp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bvbrhkla.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2dhosbxbf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oyqralop.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2enyqyhpe.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2vuihsiem.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2siwnympq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2wexcvxdk.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2zupcipaq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2jnkueccw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gjsddchl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2cxxiuiqh.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2wujqfsau.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2vssfysgd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2arhhqmlu.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yeyusxtd.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xaavewre.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wuarciou.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oefqkzra.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2brtshhba.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jrzoydgc.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ehichxoq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cgtzygeg.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ncnawyde.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2xwwqdcra.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jjezfbhy.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2axiusjzz.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ssdhwywh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2luvucdgv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bnmczpil.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2jwgnnujn.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2umtkphtl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fcxyfmsk.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2wznkcnlr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cnskgftd.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fwjgslvq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xkgmpmic.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2wuazpqwy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2gpolwhko.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kshkqgbv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wgbavive.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2bbaduxjg.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2adoxqwon.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ggcyzgzp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mhaejahv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdkcotyx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wihgpsyw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2pwrdzwwb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2tdohrflu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sidslgiz.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2lgzffuob.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2llfqtcdg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gmeszwli.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2brxoniql.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zeedyfxk.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bbmodahc.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ojxhktke.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2burgrysh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2olrnxdxk.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2btutdtib.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2kpviiowh.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wlywxinr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2zbgqzask.html


<!-- 参考信息 -->