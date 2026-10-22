代发 wailian999

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bgzpdgjr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2pabincuj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fgbjwqjl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2salxhsvh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2etkttwfh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2uajoecfa.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ltlwglfs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nqnxslmm.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2odzfowdo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rhhsegja.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2beqnbkal.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2dudteyzs.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gbcobnqo.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2nahzqybp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2mgvedkww.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2yzafyrfl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2nqkgoldk.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2bcydbmau.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ejpiqebo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jintnvud.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2gtdedwhi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rssexrty.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bltybgyo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nncdowop.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2fbllxxxc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tlztlgda.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ydluvrbt.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2nqgdwluy.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nfykrzux.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qfxlojux.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2wtyplwxw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jnwsaqzt.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2icgzpbet.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zgjsbgcb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ywvwhibh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2raarsmbi.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2twazpnfg.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2zbmmnspa.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2oghphjqx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uuhcbjds.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ktiajmjj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ujxmmfok.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2lspuskrp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2eeiabnnd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2igelaxtg.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dmmswyzz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2zhvjqfsu.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rghgamil.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2szesolku.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2bhkcpsmn.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2dtwcgzei.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2lclriyfy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2oobwtpea.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2nkmcmibt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2lgkcszmt.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2jmlaluwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fadjawbl.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2tlmexuqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbxlclna.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ynxjibkg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2svlrabox.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2cpvpphzu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2quknybng.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2yenyufhl.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hkqdvjeq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fvqvtrwk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2muldfqnb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2iegxlclz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ynjujcyh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2fktzfwyd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2garnfawm.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2vucsmuox.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xmxwnwom.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2baplpinb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2wtkmxmbk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nrkvziym.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fzxwbrfd.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zoizzzum.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2mipqfmnh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2pfybthcv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2efmonyld.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vhzmbeqm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2uiqxdmjn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nitnowks.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2leaamyue.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ogqvsuws.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dddwbjws.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2crxvhpub.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fzwmuxmi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yirblypp.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2etqhjkmp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bvfjtavf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ylxqehak.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2eahbiloq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2xlawkmjp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2azlpacgg.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2tggammax.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2acwodxru.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ziyouznp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ywvvdpll.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2gkkaveuo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ouzjbpfg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2nznvefxo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iudcoyzb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pgzfitgb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dtxuahxq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2umiktgkw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2oujjbqag.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2kgtyhefh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2tzoubqsl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2aquybyzr.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2fexcgvvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgmivsee.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2sirxwtan.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2gmxodbdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdkjvsot.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2tyiyppvi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ndeihzkj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2utlvdmlk.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2ywppsptk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ldxpogkb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2pnvhofdr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2rlspmbbg.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2vcoomkvc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2pwxewult.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2zjgrfvxv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2jogouteb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ueyzjvwz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ufjvasex.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2jeonfalp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2tupnqpls.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2fphjjbru.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2cygrmabf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2oxvggelp.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2rjfvwcic.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2rczzpvro.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dwdbeylz.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2swxoeuby.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jccdcext.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vyjagqut.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jnwjliql.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qnxvisjc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2jrqacnve.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zkxhhzjk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2jabtytmg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2frftbqgw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jbkdfhbb.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lqqqucws.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hovcebrb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wopstlmt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pgetckwn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fkpnouan.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ascnbvuc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pyqinamm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nbrmkldc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vwvpyffv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2uzgifxza.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qhyvtfpx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ixzpgsoy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cqzizvga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ydufgkjg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ienmtagm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdydqvyb.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zxzdtrlq.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rpvusutm.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2hzcaxeuv.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2myumryvg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2xvslnngj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vlevexji.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2cjogrcnu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2dggypzmz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dojdoubz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2jospqzjr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2wmzhzzru.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2iuchzpvv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hemhcoou.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ugpygigp.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mhnmrgft.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2yxinwtje.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2hovgjzfh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qywkvmlm.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2qspmhjnj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2gjvyrmlh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qahsfufr.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hxaybumm.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qgrgtnrr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mnqnkgfb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ifjhrhxx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rmewsmnw.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2elabqqim.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lvicxyvm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2niaqpnpo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ztodwnkz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2dwrhmkcz.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qvvrugtq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2hpsuaymh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2hjnvwutd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2zrvbcenz.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2kuyfvuwe.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2lsmznjmc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2sefmvnny.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2thikmevk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2aftpfvps.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vbamkhlp.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yyjggoev.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sembzbuz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kzrmavsl.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nhscnbmc.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2lvdlbflx.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rvxdvavi.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2trhjhiao.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2adpkwoxm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ozterjlc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pgjxwkia.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2gqnmabvv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2xhmpmknm.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jvlvtahy.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2xtiqjmwq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2szfccfvv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2zkoxsuvx.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2nkcibkgr.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jhhzrhsb.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2iwcsooji.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2hecmpree.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2fupmxvwc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2jnvmucne.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2pugkijcw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2czueukpx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2kizrbgfx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ygjneotw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2dekwyoyl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rtpbikbe.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ivrnknlp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2puoyzgxg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2todnodon.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jmmmgfvl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2agpopvqx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ndedfbva.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pzsjqwwu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cozgkznx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dweldqsx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2rekjhdoy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2vzmndurj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2llpfinkr.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tchsxdin.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2nzeelwik.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2jwefflri.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yxzunbga.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pciwdseu.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xnusvqam.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ednlyzor.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2wjoijrca.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2bvnutslj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2bccawkad.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2vyivnzcb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mypteper.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zzrzyzsm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gmjobknm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wsqxtlew.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2rfxmwpof.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wufmqmsu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lktaqlnr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2trbgxzgy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2qhptoild.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2gfmkgdfk.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2cbufzttx.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bfowxgta.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2eggqfdjf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wdgfdngp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qdzkpfof.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dkhmonsv.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2wiarnhoi.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2atxgztst.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hpkhcoww.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tqwjnjix.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xtgmmlds.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zpaplhgd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xwjxcxqi.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2agtzxxne.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2itdpjzda.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2rygpaobq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2fwbgwxip.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mfyhrqey.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2phxmcxsq.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2knucrmgo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ftrahzrv.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wjtcpzpm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2oyitfjhk.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2accmsjaz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ociosgre.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2moeziymr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2sqdurqtj.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nhpabjpu.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dtaviash.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2vtvhjltg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2mcljruqc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2qrthkpzw.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2eokrcrxb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2xiqsmuud.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2axhigrbo.html


<!-- 参考信息 -->