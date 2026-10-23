代发 wailian999

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tgjnshvo.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zuognnln.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3sytgaroy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3vbquqsaq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3umdihuxk.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oykahkny.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3uwzjzqnw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jfiojxlb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3jurbpphb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3cysuelhd.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3refkcpej.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dgjkjjqe.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pwtmvldl.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3nhbrbest.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3vjwlldrn.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3oavpzphv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3suuslizu.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3nkrxflde.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3lkhqxaap.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sgfftgad.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3klatluul.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3raxaydjh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3tjfbdxed.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3jddaoink.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3mhourlcr.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3isdzevht.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3pigsdlug.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3vqulikul.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3mhzmcddd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3epqmpgcw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3nwyjeiwk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3cyqrqdtj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3doikarqd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3oalicioe.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vzmjndic.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ptznfbnk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3bexlcqnb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3iskfaqbd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cjpxzzaw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3syffcsfs.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3adshhfbb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xlonevts.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3xwhamvdv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3aoudlvve.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3wzxckozt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3oqxfzkfk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3bgwwlonr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3mjrsukbz.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wtajewna.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3bygpgudk.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3yjornhcd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vcrxpzbd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3apxqxfzy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jewslslu.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3olnyqcux.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nzkegtcd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vogvwmfj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ubsymqpf.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3kegyfzqb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aalmdhbq.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3svvjgolr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3dsiscvsi.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3klsthpuw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3oegiknyu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3erytsikc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3opnzxgnh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3csedvvut.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vtlwibyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3raabcuaj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3quhkacfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3guzzforb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3lzenrgtu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3okcjgabh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3mxksincq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ocdqunup.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3lbgueryt.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bmerwdlf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3cebjpkhg.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ptpehiws.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3epmcvqgw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3pxgutegi.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3nwvqyjzr.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3utmyieyz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3mnonbdvl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ihauppty.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3nynywltw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3mnsjiiab.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hviukvpd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ddrdvhnf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lvywpjwr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3wihfgobw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3wxzefgrz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fgrspeou.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3eekaenly.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jknngudj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wpptqgzg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ndfaypci.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3voqpqumb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nmyduvry.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ycjphwht.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3devypwuj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xnrympsx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qbhxtjuu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zpxukjit.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wriqdhqi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3tbdfsptr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3vbuvmjzo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rtvukljl.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3fexhdmoz.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3pcvcrpik.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3qbqjwdgn.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lpncuelh.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3zytidscn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ouksoiwb.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ppsvwllr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3oyrchtzz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3uvplrmqy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dlultlwx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3dujistql.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3yzpunkek.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3wewwytpx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3pdokgirl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3lphsfgfx.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3retxvend.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbsxxihg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3fetcemfe.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3gzxfhdfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfswjsdz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3wotligqj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ibcnqnlf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3siafhvuc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ydofquzk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3vauepplp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3xhoosvyu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3mfujohit.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3qmzregqx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3waqgqitt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3eutsfevu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3krsvobxw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3qcjotnji.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3zrepptbw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3xfsqlxsh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3flypmbfn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3rhxamgdh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3qxofhggg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3edfsmhzn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3sfpgmiwn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3njcbyhji.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gyfvbpfn.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3sxmuzrvy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3msnoqfrq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jnyfcbvr.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gnbsjlyu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ngjzwbeu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zszcuzdb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gtictzbk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3brguzdvw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qurvheye.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bnleekwq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mekfgbzm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oqgfyrlm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pgzpruyq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3thdyqtts.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jsahyckk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ykuqbqbf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3eeiiexhr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qowoxogn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3jfteuanl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cqgahiul.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iahvijio.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xecnlpne.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3buvlmutm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvrnfphz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3pniphsrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrwfhoyt.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3agnaxyea.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3onlmcqnx.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3oosdztxg.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3whsdmnyu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3gyaodtyj.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fixsqohh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3gcdwhxmu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3oepgxjce.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3myyolckl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3bsyoctla.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3txgiuwlj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fjxvaonb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rjbusybf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3wozmrizm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dvflfgqs.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3vpmimpsc.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3dxyexzaf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bkppvftq.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3csgpnogu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ixrxuebq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3abrsvsnh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wzfdrcyi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3olvptiop.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ytrlazrm.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lwtqhria.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3apevgoxt.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gkzrvbai.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3wqwyahml.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3upzlqtaj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3uwwevfuq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3lbbwmgkk.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3woqqfbvn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ugaklucx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3jdbwsefm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3pwoqtxhd.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ezllbkwq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3nyvkwjtx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3zyiovwcs.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kxbhxzyh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ehlyccdd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uddhgvij.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uizogzli.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dorqdfzs.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zqykisdo.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3avilxwsh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wkabztzu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3udxlzdcc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3lxwdxwxo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mawzbmim.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wnuswnbs.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hvafkper.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3bmdnwvih.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3uyavhqva.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rwnwvtne.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fjrbcknd.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cjfvekau.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wjdaxcky.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3dcabxybk.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3oycklcsh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3arqircqj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tiaprkam.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3uwlolkxr.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dpzgsoxi.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3anlbzlji.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lzeqxyft.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3pohbhvqt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dggxqlfk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3acpdrvuh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pyamcgoe.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jxvfpqty.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3uqeyzcum.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bbqzcwro.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3yhtsfoqx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3adbrokfj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bxqhtrgh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qxekkghc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wigfqkhu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ypzstwet.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3niotjlqv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3hvpgotgv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kmvxsphj.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3swnormup.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3iodxtweq.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3belpnzqc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vdronwvq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wwggpmid.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xpvafskc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3lsrpehfh.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3hdeutgkk.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3lulnnzzb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3kcspmwhr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wrqvitbf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tsnqlryk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pvnvlzlo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wxsfpxef.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iuvifibd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3qwmfqxgr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uajdcrsh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zxowgdmz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3emawwgvo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3pmticchy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3sveasiji.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rzgdgcbz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ynkhkadx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3eiophbic.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nduqsglu.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wycnlecd.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zkeartuu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ldmmszlp.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3odsabgrb.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cwakidut.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3njzbafrr.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zvmtcwww.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3thyujwla.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nxedtvva.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3okxpupye.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xqhxwnpl.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3zmxxaqdf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3umatgijr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zrjujfym.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3exccikjm.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yfkyqtjs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3dvguqyqi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hwvlsqzn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3dixuukdh.html


<!-- 参考信息 -->