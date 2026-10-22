代发 wailian999

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2akrctbuk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2etuexpom.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2jivhgazw.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2oldylmid.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2tzwaxuyi.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zfdwkxol.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2xxbfdocj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jprqwzcn.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2fajzyqah.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2idhegqgh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kfzvyjpx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vpsnqgmo.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xvnnaxqp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2tttyvhfy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2gwmldomv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2sonkughv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2wnggztjo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xmjghkeb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2fqfxkdrm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mdcoooqr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2krwwjfpe.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rjzyguny.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2zspwucwh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2yrkgosof.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2mehrhzyc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2hbcrzuvn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2dgytdllz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ppnthwjc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2xktvwixm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2vonykdjj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2cngcqgpy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ghruqich.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2hrkbxfqq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wwishonv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2jvylkpgh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uotwjicq.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2wezbktjt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fpaxxlwq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jfpeeqvm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2mpfgaugl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mzibvpvm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2okpibjyi.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ntbnnkrl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2qpravsru.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2chetqpyr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ivakxvla.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xktupbhp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2pijxhpup.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2wyyyxwej.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2nqllikcz.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2hwrlsjss.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iqxnwdog.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2bfnrinhr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tscvjzma.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2dtyebdbp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ggdqdhhm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lziukwtg.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bxbmyqta.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2sbiqtdux.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzqpzths.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ykmxfyer.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2dwetnsxd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2qllcthux.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ejkidvvi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hcemkxbj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vhzhllgw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ddiuxvjb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2mnujukmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dspmcqyl.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ivukofos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2azanqlxr.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2dwnujxqc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2gweqeabx.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2qeuuuffo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vprtrxcu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2qhtxnwnk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2htwdsgvw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dyeffvcn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tltqfprn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2atvjbqzi.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2vibxrhvd.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rrjstohg.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ziqimxkn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2hwpjfdzj.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2owntutrf.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2veskoadh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2xukuubaq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2fmkgqxjz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jbnpjvjj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ygfoocjs.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2sycjquwh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2caoqvehf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2krpglzbi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2udemnqkn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2opdkdwnb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dozisatv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2fkeosptv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2pfsobhaw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kmeqsxlw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xfuzobfi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2usdanylg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hytyvkvs.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nloquapc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mctpukgc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2evwwmmnx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2dbgxcuvt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2foipsrpe.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cysendpz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2iadtfytn.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2flxdjgtv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2tkyjoumy.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2rpkhhpzh.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ntljkree.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ilnjbfuo.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2sonaxuih.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2amhmstex.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2bzkjtgoe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gafuoaev.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2wlonqiau.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ismvgeeu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2jkkbixbk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2hdmkfzme.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2trrmlzje.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2wypoinnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqfxothj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2krgpipxk.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2quihnbkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgrqylzg.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2scgozyhy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2aerzweww.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ddaycewi.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2qnkvpgpd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2jrxlcvka.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2kdrdmrjt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ctayfsnt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2bhxcechb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2jbznwegd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2sqhtybnc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2erlmmyhu.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2gxenjyxh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2nhgehvbn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2pkuorxuy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2xkwxichc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2mbwpxpdq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2hidwsmvi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2stcuugcd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2epkjqchh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2kvgnfkkt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2snlbdysz.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2xnsdwvws.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iocqonns.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cgumtwmj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hexmqpup.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yyumzkal.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2scwmkeaj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2imtdtgxl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ndgtkscq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ejcmolec.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jxkxjqmz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xqnhgknv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nmypnpip.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xkvrjplc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cqieuyuo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fvvtdlet.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2idnqqgeb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bohkgxky.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2plrmgnxh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hsftbomo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2sqqqxbqn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2pikepmdf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2loyodhzk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aepxmbrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrkjgxmq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2fhqgkonf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qldlabjw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2jhdiabsc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xwdxaizt.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2zjolyizz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2txdzlthz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2mlcgfxta.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ywdkmrmi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xquwdfuf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2stqobdot.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kfpxuunx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2swhiikbk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2okizunum.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rwiwxonw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lxhdvabz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2potztrtb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zphyxmtv.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2pudsetsx.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2movoqcke.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2usdgbfuk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2keyiikwd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ezydxjrd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kxxksxbl.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aplecrra.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ierbrtci.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2izoggmgk.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2pmcbjiwf.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ywlwjxda.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2toechjvp.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2maiktekq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2thktpllc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wjfworxi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2lefmcfwx.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2wahkhktf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2mrydgods.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2nmflxvop.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2slwivpss.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2lqdxuaab.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ehthakab.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2wclexybs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nihpszdq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nxdenuyx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dtzqdcmi.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2uyoloouj.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2juxvcwqg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xozurhdi.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2emwqoawd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2lymbtbei.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hjxjtukt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dkugoblz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nnyixzxl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zjxpyuhr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2twyyimod.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2usbznrvu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2dwserwad.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kiglfmfa.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2sewzwfwg.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2obahnbzu.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2fgvdphza.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iqtcnwmw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rbcqysrh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2giqtuuwy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2bbhjpwnp.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2aeljhzgc.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2nbpisoyn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2vakxyalz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rdlgypef.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2bkgylhes.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lybhfzqn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2hqenxivd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2esiwtnrr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kiyvafge.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2fpoxyarl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bgwynknu.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2trujnmel.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2virlfsdh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oaubtxqa.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lbkxnpwz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lwsmqhda.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nuofmqxh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2nsxdwxsq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2kdksfxzn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ddqtkdcz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tqrjqztv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2qgcmrbix.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2mnuwcijj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2irycpmrc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2shhoddls.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vuhhdeop.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2ecyqwqbg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2buvuahkq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2epwkgxbk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2haoctcvs.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2nbupxidn.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hqglgryv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vllukzpn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lqpscrhd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bwovhbdv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2qgjozulh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pthwtpfx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ymxpntvn.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mqhvksdv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2ptbrrkju.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2tbfnrpbx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2evaocyea.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rqaoptnc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2cwopfrpv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rqydiafh.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2vpxokiit.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dvuobouy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2icgeoddq.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cnthvkiq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cupgtolg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wvqtphms.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rejifubv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hmvkjnpp.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qiwjnmwa.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ppdtvmaw.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xzujhyhi.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2namasvyg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2zfzxxsqj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zlirjtpv.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qunwjwff.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2owcrtnjl.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2fmynjqxr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zlnqamth.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2lxntoymc.html


<!-- 参考信息 -->