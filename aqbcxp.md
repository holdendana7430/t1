代发 wailian999

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2rjnjarsk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2couygntm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2aiywgzce.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2silqnqox.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nztvdzic.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ouykwija.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2fyvcwqzl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2czzmbauq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uezhbaen.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2gsjagkqn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lzicatom.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2yhqgabtq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2udhdlffk.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2obnbumte.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2nkqjynjt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2trhkuuxv.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2wtenqxfv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uejosojh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lcrhvwnr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wgjlauyz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2iyqdwgrd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2cvjrjmmg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2cveyojpd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2wlodaufp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2jhutfhek.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2biwvqrpr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2lzrrdjft.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2mitagarb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jopiizkr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2siooduqb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2azxnjefl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ttsihtrd.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mixsxvrm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2sqhnalma.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2scoypmcx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2avqdgceh.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2oftttzdq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lrxeeqee.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2jydcdxfs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2wuwwcchb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2zfstralh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yhnuscce.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2nvlihnbn.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2oxlbbdcz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2zeqxbsea.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vmvatntl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2slneltuo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2myvmwqob.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2leasafdh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2chbtcedq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jrxaginc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2agpascic.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2eeokcsjj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cggvqjhn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2taghoovo.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2dgidiskg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kjfvmost.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2vfwevofk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2pvbajamf.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2csgrlfrp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2jikrnota.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2nzcjhzor.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2qmooprmt.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2rdthmzyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gurqktux.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2tlogjsae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avyeljsp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2bzfmpeur.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2pkawfqkm.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2rvedbdpg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2aeayiigg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2egefltgi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lvhmbdyz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pplhfjsb.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ncgkvcpr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jxyykvma.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2pvxbesua.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ixemuoci.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2dmrictzo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2naysbask.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2utffogme.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2rololowu.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2zskvshdg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2cbdozkdy.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2allfyzsf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ihcxegct.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2olgugeox.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2zmudiqtt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bofmneqd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rtemlder.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yoqobvik.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tlcfidcq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2cbakoacs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mhfegxar.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2umlzluqm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2phjeluus.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zteoquvb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2erwkqqls.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jbnxyccu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2imasxxyj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ubohbvha.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cdveffqw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2bgvfxutd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ozpemmty.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2phxkrgim.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2objtmlvw.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2jcfjzpdh.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2kbtuyshf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2zliqdmzb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2eopqdnoe.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ledupbhz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bxpocqbp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2lktfeyik.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hsaeplfr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ytcigoeg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2nhwcbccj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2tmomearw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2dnbpxbir.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2jjopnukb.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2iwsggoea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhaghrzf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2szvkrufz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2wwygycmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzcpolnq.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2dupcnlbh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2jtrrxebk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2nfuwenkc.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2mvhipegr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2tvoymfzv.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2wunesmby.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2swlqbpaj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2rgghbvuo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2xenelfgr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2xaddczbh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2thxjvqro.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2rthmhmgx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2zbtoydyy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2dicvkaco.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2rctggdif.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2sjmhaewk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2irjzyjoi.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2gytqbwfh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2cobsthqf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2hvnbklmv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dkspvabq.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2kzsefocc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kwnieuvt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ubrujnuo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ykubtdlb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tvxtngbm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2elnpfpgq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2ubvvspdf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ojnfztjn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kctfuslt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hqqdgefy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fbnjigmv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qeigdnws.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2iashfyfo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cprrkdqg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xnvapisz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jsvdoass.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xkggsnmx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qbnfwabc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mtovgsat.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sbdoywld.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2qkhgocos.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2denzijdv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wxmvncza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kftviepu.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2vikqwzfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhafbqdi.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rucxsmfn.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vhlutwuw.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2bkjiddqz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vhdmxgly.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2asjprysf.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2krcpubjl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2sritimhb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2xeermeyn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2eexxenyg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2wlkvrgzi.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2suptvhhe.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2urcevmnm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ohtdfkqk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2wqjhvbwa.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2akhnzecw.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ppowvxrx.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2klvwyrxm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2emmmcish.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2xskmnhkp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2xbfwtntg.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2chlctedo.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lvkdmttw.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dvvjonns.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2inofqzir.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2gscrdpru.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ytlbjzna.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jqhshnhr.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2yrvnkzej.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2fkjlonjb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2wspirsob.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2luwlcapb.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2fhtsvmof.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2enyrfixp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2dzxwwrku.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2xeinleil.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2snjvblne.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2swsjfkcs.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2fnwszmww.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jquyjqre.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mmbzykda.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wjdmgjsc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cvynudyg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pnxgicqx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sgylicii.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kzpmtkrw.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2uqtxraiv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wncughzq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fphcusgs.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yhqgkyfb.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2tgpdlaze.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2oaksscxo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2pmnswhlv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2dnjrlcqy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2dldgvevx.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2izhdzkjk.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fuefgyse.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zgcgqbof.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iahlicus.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ianivfjo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qeibiuls.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tvydzomc.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2caenofsz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qamsrjyo.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2xhdxcqlf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gjokknkb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2zldoxwkx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2giroimtg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2iddhmufo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dtkklcud.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cknfmydx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2osuizjek.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aiilswse.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qlwxjdtl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aljrogho.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jjbwwwys.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wtajjplw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mkoyntfp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2umaeulue.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2pzgdeeiu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2xyqjchnj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zfjwollm.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2seutczft.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2wflottrq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2wdhtvzio.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xsnnhhsi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fsbigozd.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2aadnlyhn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2ptaiquvv.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2fztzjlmk.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2cfnezjca.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2hrpdnksw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2nnsepsas.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ufsujexg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2imcirjwy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bihribsk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2asorviov.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2eszqqqvk.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lnhjcnng.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nnbmdfcn.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2edizlovg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2eqofopkf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2dfahmcot.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2mpjyfgch.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2tgymaxdr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2czihpcya.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2jkoofngm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2qqudgqem.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2rgzcccmy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qwnmbhjl.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mgessplf.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mdhsadqa.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yfrhwzdm.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ycekyskb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xltafjlt.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ccbsacde.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dgygunto.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cfcjtxsm.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2pnjqiuft.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2vsowwlih.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pzktytxe.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lntwwysh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vcyvrdwx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2hrbxwfsd.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fvbcyltn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2mztvsglg.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zellexmb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2asqwetjn.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ofqhxala.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jubfhgpy.html


<!-- 参考信息 -->