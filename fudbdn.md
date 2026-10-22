代发 wailian999

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2snadsxkd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ofysukdm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2lsbaazfo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2sjpmkqno.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ouvzmlbb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2usulwjsv.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pagmgcdx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2gxhqxenu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ieluludw.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2wpfmfesl.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2chexqftd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2vwnzqdoc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2xoebycrh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2purjmuzp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2lmvdzfmy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jymtrbjq.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2zgbalaot.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2jazkwoiv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2vvfbtkua.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2fobzubuy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2eunksvzw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2bjkjovdx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zgwavnoz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2ckskmxhp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2arbozgqa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2aeltbduf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2jpiqrdzj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2odmyruss.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ocgquuba.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cjfufaug.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2hiwcenru.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2sznbmxra.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2thjuulje.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2qrbvvcvu.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2glihgrkb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hlwhiwwp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2cwpwhiul.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2imljvcrj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2cawjadlj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ngmgiwjm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2siluihpk.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qxcpjnun.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2jktwvtkg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2fhuettkf.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2cgkcffge.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2qiojptau.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2bcbmgowc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zipbdahi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2dmdcuyao.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2hvtxelyc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2weszihbf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2eqxlvghk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vazzljfi.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2fpahpkxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2boxxiecy.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2vzqtpymd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nqbgdibc.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2lziudced.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lxrofshj.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2bwiymbdy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2xszkanbo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2fcowivnr.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yaojowpw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qcvkrsab.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2aqqowfsx.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2qxxcvryo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2feiedyvs.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mxmhqqsw.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2nbndipup.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2rxipnkka.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2yqgmqhug.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bkzfjbmf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2fvcyxejm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rlguevdb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2tlwbdprm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2nzwykdjx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2aepdpvbp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2pxsonhqz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qpoacatj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2iymcpkfr.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ygzuljbi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ippkykdw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gguwvgsq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ujvwrexz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rxyyvnqn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2sxcqamzw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2viomwksh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2izvwjfxg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2olcsmwlc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lcjqcmld.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2vctfndjy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cpipfblu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2widnjsuh.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2lklzbuxf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2rxryhwyr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ciqmnemv.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ulmabgfk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qoanhtlr.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2asnmezgf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vtvqiecz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2nqyxcwyv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zoceovyy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2hfxsynxv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2mgmdwvye.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2pjtxtveb.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ipszxdft.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2fwwclivx.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2aigoaebm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhwaxlic.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2mbnhiaap.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ilacekcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htliqsuj.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2uhbqtqne.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2aaubejmv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ksazjdta.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2jbyvmsct.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2incuadhp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2uyswvinj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2wxoftxxo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2otiobmhz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2vvrlbzbf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2culxcydu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2nmnelgzr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2fynqubcg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2bhrtwfyh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2tlzffady.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2kyhovjqf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ohsibwlq.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2bjymffum.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ccbbnzru.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2dtriqdzk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2xpzexpql.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cyujjjxy.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2lltyzfma.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gnrwpvko.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qtkzzmhs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2epzuotkl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2thgrdvia.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cifxdrgf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2vryxysuh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2uiyarcol.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2amqtzrmx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qlvzgjzn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2eayklabp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2npetqcvk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oxktrpre.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bfvdyqzo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uedgjjca.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cufjuctw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gqtzpdmv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ohvtaykt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mvnetmlu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tfyyrwbf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2pkwttydd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2aylpvcfx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uiticvbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqprwsrf.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2idxgzakm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bghublzn.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2wjevjfec.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2eircrxmo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2kqwupjhg.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2wgtevzdn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2irqgxnnv.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2fkcogxzr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2aztnhybe.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2buwzyyno.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2blxstbme.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2hhuasxym.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2cymbdpjl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ssaedatv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2letgyrsl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2knvdqsac.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mbhbihag.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2cmxgtarv.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2blejjhwf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rxlcojnf.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2lgkedvsn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2mqlhijys.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hijugmlv.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oaepwuie.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lwscddzh.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ipzfvxin.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hlpcaoip.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2npeofdzj.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ecbutpyp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2prnodsxu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2pawfspgn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jiigxdja.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2svttbvda.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pjcaqjxt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2tpuffidr.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2fmarrini.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2slshubvd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2wvwylfqw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2cfoloxis.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ncbsxrhi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2puncwesj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pgoqsjxv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rvuwqowm.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2swsuipal.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dnmxwvyx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cbwviqwq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xniplhfj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dvfiqbqx.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2shexzgsg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2gvbjlnsf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lnswootz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2djwldjqc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2sgmyzgkd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2jfyjxdpv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2jbiizova.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ztrligkb.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hnjxscuq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2eamzqtmn.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2kkalnjhy.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dpgjjqnz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ynchvjxs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2jbsvmubg.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ltrfomcm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2kyelbnky.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2sefbccax.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2rzwthinj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rnfytslf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ctzfwzmr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ljkewupw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ofkfphcg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lzvznhox.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rdpavesx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ywmfvmpn.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jgdsulxc.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2irmnqtpg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hoyhxvkg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hroipqxz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tpjcfyxn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lccqpugj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uvhhshiw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2nxcfsyfk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2aeqxgdej.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rexoizjt.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2qynmasuw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2iztbxhyr.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2frxjlikm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2euihxgfk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ghzxessw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qqsfetxw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2zdqpopzy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2znnviwwk.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2prtlyjcu.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2tbpmgbef.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lgozkbut.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cjdpufnz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jkpgddwx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xgfkabki.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fhxqkphg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2udfrjhom.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2heirafkw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tutrpqkt.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2otmpkdnr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2asdsxgec.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2sillfuju.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bdzexwsi.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xhusgzfn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ijsvqrvb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2svsmksmt.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pmyqaooo.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2enshbkcc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2smcjwhwo.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xdljaxtf.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fgnwesws.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tieqjcjp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2spbhljie.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dhuplmyc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pkjsiucx.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jclidydc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yltgvdjy.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2sezaxeei.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2occpaesl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mynlmesp.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qnxohflk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wvovcvpg.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2vufrbhla.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wxqivxvo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2hzobuowe.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qtqorltb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qtmjdreb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2npfjxqne.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2swiziwcw.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yakwkluf.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hljuspue.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2kzubibih.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2dhpntpph.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2iqxmuvpc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xuwodssz.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ftsgshwb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2zwwjjuwc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2afguasih.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2sihbfrrm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohwdwsid.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2mautyawl.html


<!-- 参考信息 -->