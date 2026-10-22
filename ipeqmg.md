代发 wailian999

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2avsbilld.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ykwpkuki.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2zgjspwlz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxlpuozk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2mfzvnwjw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ocbcwiim.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pyomdjcp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2qmalkcjx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2zgblrflg.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2dbzrpjol.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2xfohehko.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2vrpnwsyv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2zmoflnhx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2vemelmcl.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2swfkpcfb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ibfortyw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2etxadgwi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2iipttjwp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2unhighkv.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2hdnninkw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2lbfcjvcu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fkrhyfms.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2phhvnfpb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2magwtgti.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cicshkup.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2tiihijkj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nfdaqddm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2qxdsmltj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2sllkguxk.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lgowrdck.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2atzqsoya.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2nroxxnvs.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2giwzthna.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2leyrzxjt.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2mgpfuady.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rxpwppxx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2hobzdsqp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ezypgnet.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2aanhhaqh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jmzwctoo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hpxrdjlq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cnxpcipn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2oyareakf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fljkvzew.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2mlwiqnsa.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2totjcgpi.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2dciahrkq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2wpqegatr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2oruzjlnj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2sbfqdryv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ylihxgji.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2rrrkvdbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmclcjxo.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2oygxffgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcerluad.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jxducexu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2ryrmquyl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2scizbria.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2rlasvjpp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2psacyrkv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2rsihaqtz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fhjfpspd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gdxjseir.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2iipjbemi.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2odgmsufn.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2abnbnhtb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2fwmksnyi.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2wturnfgc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2rgphkoxp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jpmgnqfq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2jfuurqla.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2hnwnykfq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bmihpwhu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2unoswuex.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2kfaxdans.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2wejaitgz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ojsbmcat.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2yvevtews.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tbqwnlja.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fwsuhggj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ktlzjkch.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2oomtxvow.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2iqjrcvbg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vsvprslq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2unhreenx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fdmvmyfx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nhkneqjf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hpvsriom.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vcptanql.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2tgivbsqc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2sbmxvhyj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pzhmvtii.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2crrisrpu.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2houzojsw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2gyofdkss.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2eylsieol.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2zpqoaive.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nlyopshr.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2kjbdtjpb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xlmyrdvn.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2jyyzttdl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ykcuerwv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2mewwlpyi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2bxcqocgj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ddkkkgyt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ahgyfbtx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2xjtwcbzs.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2juzdyhhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulilzest.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2qmgnhrsw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2gugmqdfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lexfmxdi.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2hxrlzugv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ctolujcp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2restzecs.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2wftkyuvl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2zojhfxcx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2rxtqtakj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2wrdsacxf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2mahnloud.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2umrefopc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2xgkmweqy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2eevqjozn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ygjcxuoi.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2dunqseta.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2zywtmluk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ggjwcsjd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2mdtixiyi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2mxkqzyck.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2zqsnaryx.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2xxohpybd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2hvwlfqny.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wwfhbivf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2hsgezufg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2reozfvcu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2fqwsgadf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ykccsnvo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kpguhugy.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aabudkte.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2olttsdqe.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ztvwdydz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rkzpwshw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bhcmbxlg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vjxvedsq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lnlgmdmv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2mqfmswuo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tpwmusqx.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gqlvljbv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2rzplkvgs.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2necaibfl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2utlejjxn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zhfptdrc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sxfosddv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rvmpypcr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2drketfeu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qrxhptld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtakwqks.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2jtfrslxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdbmbvns.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2gkghszku.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2txyywntp.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2vlczdiwl.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xmfjiavo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ptzmjupi.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ayiazftt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2uwuqciym.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2kbseohnu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2taytopen.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2jepzykff.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2tquzqxml.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xszaazam.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bhdqvbsp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xpzhgbif.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xxkbryoj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2yndumjct.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2lyfkrxty.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vwzoiwus.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2qkmmwyyd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2zctgnsjg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2indgcily.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lccjexmb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mijknbcz.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aqmbycav.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2bttonbym.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ftlyonqd.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2clnvgojf.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ynjitgab.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2acawhovd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2irepsboc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2eyklqzsr.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2zzagvywl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ajqsprll.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2myfbcics.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2odfrqvxs.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2fxikmzel.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2vwxsqulv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2jwggczbp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dtypnatp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wdbntwrn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kjpnzfui.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ymbbbuom.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bbprqtrm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hvrzkirl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ngcfjhlk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hmvyqyie.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2usvscyzc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2zgmbyvkg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2rqtblsha.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lvrpoknp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nurvbmya.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2tyknltqn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ndhjshun.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qmpancid.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tvyjrezr.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2clspdmdr.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2smhqsjys.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2claaadwq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ksderjbv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2smrkjlfv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2ecskgcdp.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ftnfyvyf.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2cdbrcpqz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2jwsdjwxk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vmxavgyy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2cbbbtmmg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2prrerziv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2gasiqlxw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2etdpnoxf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2puvaywnn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2mpdnaeik.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gnuiqwat.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pbmyulzh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qynldhri.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpheqczs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ookhzdru.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wegpyfqp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2owlzbtsq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2mbcxadlj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2jnuwifvb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aobleoro.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2uefmbzji.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2cvwmlumy.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2hmyxolnt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gtdafcub.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2zyrwhnne.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2imhxcejd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2uurhhwwv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2xdkelayg.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2oyngrneu.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2mbbujaox.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2woajvajg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2easqblhn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xxvtfcei.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dkagmcyt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cdveclid.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ytylfswi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oqdkprpt.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ybhdzzaf.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2mdleanpl.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2fjznfvub.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ghothfht.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2qyurdhox.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bimkxdvm.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lphmkgmi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lcvzworm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2uaxxgtky.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2bkbrmdoz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2erxkemhi.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eiboduia.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xhbcnkjj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gnnznbgk.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ffpqekcz.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fronnhvi.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vqbevqxr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vqowgwya.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wwnjsgrt.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2yqbbsaul.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2nnswrnjf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dajrnqji.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qrjyrwou.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2onyeadbk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2lkpxesgz.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yzzcxrgd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2amrzivgb.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jzdpsxup.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2clopdczs.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2txuhwaee.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bxamodor.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2erbqqpua.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2eoczvxwj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2vwvtcjet.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2qcndlvsh.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2oxlvdtgm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2bjzcespq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2szvyoifx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2mcecywej.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2dvtuxqfc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2hxkdweto.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2wgdblcqm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyjxpjoy.html


<!-- 参考信息 -->