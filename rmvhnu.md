代发 wailian999

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zemtxpsd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3hczrvhyp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3awcmfjwi.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fdmmrlmd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3jhfdropk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3laltgqtx.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3wssmgnql.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xujhjprj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ekpcnppb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kfocdizb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ojzofigs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3pemewtdh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wvyrivyk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3fxbfuwaf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3hfyclply.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zabrqzbk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3buehbcps.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3pfqavdzh.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3bmbufjnm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3dfdohhoz.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3umlfqfip.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3kabwbtjb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3nlgxmzgl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3uutanbkw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3fqqedhgc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3eufprisz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hgkipruu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3vjmrnivk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yhihdtey.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3uiuewhdr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3jftjmvwh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3pkpklupg.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3zhyhawxm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ydfxtccv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ippsptpb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3fkammeid.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3yfcqxhpd.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3snstfioo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3yyzpdegx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3gnntgrdg.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3bvuhsoon.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3raripykp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3hztglnqg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bwafmkmf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3keodpmir.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bsarjlis.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3dddgonxh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3juojuitf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bipeimti.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3msdbcqnj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3bfmtdjte.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3myagotqb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3xxmplgao.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3tmidojdh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ntlfzaxg.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3rlmusmfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhinlvxa.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3lemfdspn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrcnajjp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3nwurakie.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3kjxbubcj.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3szhuqarh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3xeyesczw.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xyjiqdae.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bhodmyaf.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3eulxumvd.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pmtpcnye.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hzkbyhjh.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3wtdsqipv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3idedsrts.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3fibouyge.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3nubyhyoq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3pkrffsan.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3uvnhhzyi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lzrgmwdy.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gintidob.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3suqlngbl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3iszbwbar.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ylmckjva.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3wjeqkxvg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ykevclcw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dbxworxc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3afjmflyi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gwgqmscp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3qtpulrcz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ejddzfxp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rrcxbmkd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3lgtckzvi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ppqliond.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nuxnhwui.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3blufatdz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rbeisren.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fgaqdppg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3czjoqmzq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3pfoszwig.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bsxommyk.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3pxzihhoa.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3snpxzqpf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3hkzybgnm.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lcfhtifh.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3wodtxvsf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3afggkfmz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3czqjyebh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hlijngps.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3uklywldp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3owludgpy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3wkhxjvwx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3pdospwba.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3dkxtjilu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3pddmuyzz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3hpzydggu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3yiujyfes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vaupzpae.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3msawuiyj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3zaglbztm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qhjgrhwr.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3eehxpasg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ekgigaqs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3jkycwxkg.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3gnzzqpwk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3phouzchj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3xrpayjba.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3kyzhwelr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3btkorbst.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3yevcmqqv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3xefwsfev.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3udwnphkf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3kmtltmzq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3boguuvcb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3dgwxxtcl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3jinwvrab.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3gwxmljvf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3bkqhvufi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3unmsbyhq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3fuwmuidf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3imxlvnjs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qfwbwpot.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3glvzehbp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bkagoxcy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vwdxixwt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kzrzuncc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3yfkhrawv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ttuglyls.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kqjzwnbn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fqgtktym.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fwpghsvz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vijgccmr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xbtgajer.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pmhazjcm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ngtvcxnf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tojmixqj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rnyxyknb.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pmwzshtc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3qpulxyvf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3diwfuhas.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3jpeugobw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3lwbpaozh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3otnfrtyh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nmuswhei.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3yuwxyzex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pwtfslco.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qknoblor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nettjnlq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3jlxkcpmw.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3gvhypkxn.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3mbqattfl.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hvsdcvrd.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3aafakcpb.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3luyypssx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pmksrdzy.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3aejkjnie.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3puetgmww.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3bzbllpyb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3tzdxlqfl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sucmwfof.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3azfzkglt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tggrgfey.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ngygjzzf.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3jmoaxqrr.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3fdneaxel.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qsxtfdew.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3mfkdyeev.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3bbkcrfcv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uolsvlde.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ngimsipo.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qegcrisp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ejaweffa.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jkiqhadv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3obfubaxl.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qvbxqsdm.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3aezirpqg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3uaqvhvze.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxmqxhbw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3khkcxzbh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vertpttg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ivhiwjnf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3bmiwndbx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ilgvahry.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3udtptefj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3nrddlshg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3sqcopmcy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ipbeezma.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3buobufiz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tgnvnnrt.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wbsluwfd.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fpjunymr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3blwandrp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3htozjnsc.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3azmpsraa.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3euqkgxbo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3uiocaiqp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qheeoprc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ijhekfln.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hqnjlcmp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3auudwsbt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3xgkbtzfg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3rptorsri.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3repdpzlx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3jbocjzjv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3kdusyikr.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wueetqll.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3vkqmzazy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3jrsavcaf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lbtnydea.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3puplowit.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3fmxfpfqq.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3erjwwdux.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3chykiomq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3dsxgrslw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3harueezq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3npxyzzyy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wqfafncj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3duljaqpj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3iaqnffyj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3inkpugcf.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3oeqwbkwd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iqprjzvn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zhfimvhz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fomvjwop.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yvbwjtbm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kdfracrg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3bunbtcip.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3gzzqfcaw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sfwcyctz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kixwktby.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3kqmrtiwe.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3krnsvesb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ujywvcyy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dguzerec.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tikuxata.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3qypgwvid.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3ldmltcwm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3jbaiinlp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3sjsvmizg.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3korqczrm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nszmeblc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3veckvtph.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3johfrvtv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gsdxbsck.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3luyzaamj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fsqirqmj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3oyhiumeb.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hrozcdrt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3bmrgpjus.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3agilnknz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3qlggttbl.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ssixjrqv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3gpojqymq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zujlnfqs.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3tymzgjil.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3wfzzgmui.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3yzckzcqt.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cdjzicyl.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3irenkjtf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pfzrxzge.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3skeaidti.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3echgocuf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3scpslaej.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fvrazetw.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kktjppkv.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3avshmaau.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3krllsoly.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tpgkpihb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3omigmekt.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uffcycpm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3lwxecyae.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hvaalpaz.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3vyxyqwsw.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pgdgudzv.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dkeiaxjg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fdapkyjk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3suabnord.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3guctblaw.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qneagpah.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3wjmillhy.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3mjubyazt.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ryfzzrps.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3uhapoxfe.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3rutbdkor.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3dxvxeqvp.html


<!-- 参考信息 -->