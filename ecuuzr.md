代发 wailian999

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2jwkwmcjs.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bybhwxmn.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2qgnerfbb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2eagjhwpa.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2aiqunmqt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2jvbjvvvj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2vzvyovmo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ehxqsgyi.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2psqfhzeh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2uilfztjy.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2edknezhj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zgotsgcs.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2gyvlxeeo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2msakqtuw.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fygdncce.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2owibcdjn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cuigcyoq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gifrgkem.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2fihiwlpx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2jwoufytn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2mutmbphj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gvinrdhh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2woutswel.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2hvtbpwam.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2eiztlaoj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2zoywxsrm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ogcjztkk.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gzpoqbky.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2emgrwrzc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iyolqwme.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2gcweyffl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2dpapmnbu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lmlnzdcw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2axzbhrzb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2rogypwyx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjjzrbkq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jjtfhslq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2jdmqdeol.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2wapwcykp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2hiadmgqg.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2dxqeqibj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2dgfilgmt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2qzlngowq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2aksivepk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ascckbks.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2fnjaooid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tyymhidb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zsgqpcem.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xpidzvjv.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2pmosthev.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2dnedupet.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ezdslynz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qfesqvct.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2lcyvsari.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xxoadibf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2esbzyfab.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2icwpglvm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2owixsoic.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2aacmxevu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2vdgrttec.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2sbzehfht.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2aenoljgh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2thjczeeb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cjmzrlkj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fvstargw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vynlnful.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2athucanr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2frdhnwct.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2keftibgq.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fizombox.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hhbtcjkl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2urzhnque.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2xgtcenfv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2btvkwwes.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yavgjuee.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2moinlkry.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2umritrax.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2bqcpbocm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2emjcgqvh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rpzsizzc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2crjocbht.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hxmzfume.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2mpfgimrm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ndccfljg.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2htzdiwci.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2mssmwcrr.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2uszrthau.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2evwdgsjq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2cnuujxxx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vqbbsbkb.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2dnncjivu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2quxewoty.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2jtakuwzx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aenokdnv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2kwlwbxvx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2jgnsfaih.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2zbtgrcql.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2vlfvztef.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2cyfrilun.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2sjkmyubc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svstzgai.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2sqdagvot.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2tsftgoge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phsutpzv.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2afccpsrs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2kugxfjww.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2azbakntr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2hrxnqlgs.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ptmkuysb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2nddzwtev.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2pyolhwvf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2yechustf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2sthysjvb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2dhshortl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2xqnjpmxq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2boyuhtvh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2clychcyo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2vsfzhxgi.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2nsuyguzi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2nkoxizxg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2gddrwavr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2elcgrdyv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2dlxnyils.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2maklpxfp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eqoqipbz.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2sztlkiib.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mffzajss.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hzkqfdvz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2sjnnywus.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2smkzhrri.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2iziuavtl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2dxsbvcgl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2atyskipx.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ibcvzlki.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kpfhiwie.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wqbedqlx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lrjwggwl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tcdgytsi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kkilfhwt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xzvmiulh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2qypwbehf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2tkcxtvqw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hegrntrb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lvfncqli.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2grlcplof.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2zoeoqany.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jtdrusjo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qjgkiykl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqamioch.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2zgaejtgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kplpfbfk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2imhdkece.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2suyafczv.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2xcskdvcd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wzdqltgf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2gtnffjdn.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ruppgorb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vlvzjzoc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2txvchwte.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ouevkfgn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ssgorwiv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2ghnlqtos.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2gkkzpkcq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bixzuqwd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2qazdjgta.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jedfspov.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2poqhrjxm.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2pbuyebfi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2txpigqtl.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2qwsjcwkg.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2lkesbkha.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wgbfbvbm.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vphduozb.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2diwannhm.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2utgyssjs.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lyimxpvn.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qsnfycse.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wwdxnexh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2edfuajif.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2reolsnfx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2kuwiymzr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hqebaqim.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2mfdlcatg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2smjddlzv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2boboijbn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2jtqstjsg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2vsvrmtzv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2djtykvjq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ycfkcnms.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qojispvr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sicbqntf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zidzylvv.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eignqbad.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2odqfzwpj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lwtnmgbo.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2awqzllbz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jyslfgrj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2erttnfwb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2yoyhlrtj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rjfwifmx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xhvlosmt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2hohysior.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2taxjoqyh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2elfklegm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2elrxotvy.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2vlkrihoy.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hlmvarei.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gscdcroa.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zxklyxmm.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2oenvweoe.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2nfvlbbry.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qtivrplr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2prfmkzuk.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2scvnvqck.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2pijtmgdr.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ygpoytah.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2wmxclfmu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wtkdnsvq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2fvesmlhx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2llgvonse.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dorgaqep.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2xneknwpf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2znoqtghh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gdrwihgz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xdlvbaju.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tevynnrg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rpptqpwc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ncpxkgua.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2czypxsvb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ecdlagyh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2xvxytwot.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dlopwzyc.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qbagxubu.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2hhxgjilb.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2tzpustkq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ewdhjxnr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2czlqbrzf.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dspurcao.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2zlmhkovn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2xtasanco.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2lrftjxop.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2gmgdtjqu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2nfixzorf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jzevfefq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wedntqlt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yoewrdph.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xxmbndld.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ziuecilr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vutldbxz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2biqusjwh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2uhzkellz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2hmsdjlii.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2uxkgapcm.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2eoldmttb.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ppmycljq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2eghgryec.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hmyaadsu.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2zvkekhxk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2csoetxfx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2umkvnuxw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fmbzzbni.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eembeeng.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2altqsfly.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2szognzgs.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fthmcwyq.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2toanmruc.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uesvsfao.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nwgexypa.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2penddady.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2gkbsokjz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2plfaomul.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qhapducw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2egjukzpu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2pftbppll.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qbbtznnr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ksjfsknp.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mhdlttlo.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2iybjngaj.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vunekfdp.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wlyhwudy.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ikflwjtt.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dyyssbud.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2mpwsgtee.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2fzhynurw.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kgumfryw.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gruzmjaw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2cfrxzrnb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xyefwezs.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2tkbelpnl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2mbmxuxln.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2cigsksro.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2sstuswln.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2xkqksqim.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2djerptvc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2fkoglwbb.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2yidkjmab.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bgqapfsj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aqclkuzx.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kisphfln.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ajlghlut.html


<!-- 参考信息 -->