代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vximstcb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3zdjhongq.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3vncpkmxg.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3avupcxhc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3upxyzlek.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3teeiqnig.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hquhjlrv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3hljcrupq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3jpymkbmt.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3emkpozxj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3glzhlqtp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vgeiwvlg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3aqhlbmxp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rgvqolbe.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kdvlaoav.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wjhrksak.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3thsoxjdm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3wswfqoeg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3vedndihy.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3xvaerifv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3koszlkvc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3aoirybhn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3aropuxne.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3yfzpluyb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3brycwthw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3xehqcwgn.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ipaarabz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jifvxdgl.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mnmcvftu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vwrvzgts.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qhbnijoi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3hfwvchfe.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hjpyzgmt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3azbyadpz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3jtvmlrut.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3lvzstoxy.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3gjqrkbfa.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kkskbkcw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gnkusxft.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3cxhyjmpo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3twoprmsq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3lmjhrpsx.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3nayopwjx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yyieweni.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3gzvzwzxz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yztzjjyv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3vuvvjjne.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3grsoyaxy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3piaweqvr.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3objrvvxr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3afrjwcbm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fjxrzise.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xrdtokuo.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3iuvdqpep.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3oktcpiyh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3mosawnvn.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3zegazpyc.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3krpmtvpr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3purpxbif.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3yyoaqank.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znbnqpwb.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3qxtnyiaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipjvlqut.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3smossfgk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3msyjriwz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3pgkajpbf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3saukwncb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3yhuzslha.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3smxkzsze.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3sdajyzkc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uobkejue.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xuxbbcid.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3tepewffz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3kepcgjpb.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3skzjbngp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3yhmicjse.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3wxwveeyw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zkmzthvb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3gjfdnidf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jrdykbid.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ruxytick.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mlqonlua.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3oavoibzt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3veufbrrc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qxvrzruj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zeldmufp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3efnunulg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ljtmztqv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3hvogsaho.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zaxooxwh.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cniurobr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3jzllhnwe.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qygoqmgg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pdciranh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mkujbtcs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3iacesuet.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ayiifiuw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3yqmaifts.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3bxxlwadb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mlyzutsi.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3euqgywit.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3vphzuadq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3azfbfepa.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3mthvrmgq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3sgfjkpjz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3blzlatau.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3tghatvzg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dnfsjqcx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3jpzpnxmh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pdrijbqg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3yvhzkarg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3rlkbonqf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3zusfbuea.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3vqsqsval.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3wvqwaeug.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3jexcumsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upcqdvyc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3orwwxvmu.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3gtgkvydl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cchuxjwg.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3dpuzvwav.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3nzbbhihx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3wdpzsdyq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3ycocnzvk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3uveywnke.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3aupnxulo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3incgbnlz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3wjcfwjtn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3tqjxrlha.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ydlduoec.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3mpevslwo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3fpropmqv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3wecdwwil.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3neungsaf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3sxeaihng.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3fhokcdjr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3fquspnuz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3dhjyhdwb.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3uosgpkwr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3iqsdafvj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kpktazbq.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3sfdmflfx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sbgwqyem.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tpdubvew.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3abrvwpxk.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sdgvjjur.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3pkbrombr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3whfglhfm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pxtnyman.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3vvruovza.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qprryfgg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vrzertzr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qitaeqcl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ylzviuld.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vutypgai.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ebqyzmve.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3quxodukq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3npjmguye.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ybribaeb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3fiiksttx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bkfhfteh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3wljlirve.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3hwsawwwl.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3scbmivum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skbxtyva.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3yhkfdmfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxomxlwz.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3bwcmsvjj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3gjbrnosk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3pfqimugl.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jrwccmsz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3htlogrou.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3sandmdfx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pmxexawe.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3kegabtkl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dxyaaqfn.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ogfsmksq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3tbiqzfhr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xgfllmtk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mqcbbyqq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ybtqczzz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zmwlhxvt.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3xuxeiqgn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3lunyiccr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ftzuuliw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3fqukzepf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ubuwdcdm.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cvlgcrfl.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eqhpprzo.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3djgjjepx.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3viesrmko.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xmdaazii.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3qwzzgrdo.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aptjcpru.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3uktnnfex.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ibuzpgdm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbtxgyef.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hczpmtbu.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3haqqhlvf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ralxygut.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ilpzerbl.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3etmfgdrw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3sbwfdhhm.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3krxbgswm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3rmxupxel.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mmlsqmxq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3twrgqlkx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3thtipbgo.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lrqinrog.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3swfdyfxz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lmhszovf.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kqgubdpy.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hyyrboat.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3plujjing.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hgebvlrw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vcuugtwq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zfyeglyi.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qcjqnmsq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kbivtgea.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ccuwfqzu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fdluyfkr.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wseqpobm.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bxwrfvox.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3gmeeqmwp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3orjhgmov.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3kdwxdcbf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3xwkmtsdq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3fhbyyfcb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3opqzflys.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3meuxjktc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3sffnodod.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qxfltnzz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3aqvadgsd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ncutxzum.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ijlfyinb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cnjvezry.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tsmumvgh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3dlvhzwtg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uhyodaaz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mpqywnqt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qmpitlxb.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xbufnafe.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wsjdosvn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fyibpeye.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qhyjugtn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3yzisresq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3yuvyzmqf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewneuquu.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3wwtmppql.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3cgpinzfd.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3cfijqwjo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tgzwtyrn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3typivijs.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3soreayot.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3hxbnmwyb.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3hxekhoaf.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3cudpjmws.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3rdgjpacq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3wgzvuxgq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dnclzmax.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iksdpnkr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3evkwtojp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wetvednc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3vudfltha.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3oddzuyhy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gztzbeex.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mmhzhhhm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3eeiabwsa.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3tlnrumhb.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ikuwollw.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rvzkekcw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3jbukunpg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3phebkokq.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3gcfjsais.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3uuakrmjb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3vdxhrnhd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iysrhcpd.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iyizjjpy.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nxcpeyzm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ufymawoe.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cvnfxlhp.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oxzupwgf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mrohzsrx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qoqtkjae.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3nzflfhpr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3pnktcwgo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cpddoupe.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gwwsxtkf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3pegyjkxd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3jdbqqfsu.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jxlhcxau.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3yvuxvrgj.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3atbtmnzo.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3sycsxqvb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3pgmxwbid.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3unokfjdg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dgivtlai.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3wjhkadra.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ljlelqki.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3offflgqh.html


<!-- 参考信息 -->