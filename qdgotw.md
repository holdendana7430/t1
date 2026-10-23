代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3wxggmkin.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3nzhtystk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3eksnxniz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qyodyfqi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3zskwxqoj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3vhcfnalq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3nppmfqwd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yvzpefge.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3qcemarmt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zenqdcew.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3cnluhbwt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3majuldpi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ctpgzgon.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3htbgkuuk.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ekkiwuml.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3icrpwyfz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wervcfnq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rrqlccmf.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3dbyepxxa.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ushpfkba.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3xzhqlwzt.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3wzkupjjo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3yklhpcii.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ufmeyezf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3iofokool.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3teaxkhdl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3vscanegx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xdrvtnte.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ykptmzgt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3szmmnapu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hatfopkv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3ineklopy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hjzsreii.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ctxhdztp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3qoyxtxes.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3swejyirs.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3kllyijtq.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3swisbluj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3hradqocw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3pbaxghuh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ynvxywyk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3njlxtmgn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3riksysyx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3egrpoeiu.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ofqnnzst.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ygveuhvj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3auagctfm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zbwxbvma.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pshzbeun.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zczfnlcx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zhfivvog.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3baxzvevw.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3psrozkfh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3jiolxufv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3joxghaoa.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3mmitepxi.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3popgekvo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3hnsllizx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ioileuwk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3aaknmlwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtfmisla.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3oatfogyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlcezlki.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3flmgunkm.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3yxiwlpgw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qrqxdlid.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wbmnotru.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zptpsnuk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rnlewskv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3vkvznhgi.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3leudziml.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vcvmvodj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3koiwckqy.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3qgvkckxs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3fmcgzazw.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3xipuvtrx.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ndibmtri.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3gcrajwqi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3tsahxefl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ejgizzmq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3zxnwpqnt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kvoabofl.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mciingqw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3xyazplsd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jvegjpah.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jqqpnhit.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sbwufkfe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3aibqvjxi.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ruowzqek.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3txzfyrhc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3soxpbgqg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ktjutahp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jcqrlkvl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uwcgvfll.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fedvoaul.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kqzwatnv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vjbmflqn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3gfgsoczt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3zslxjxvw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bodfsbdt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3cdvfiesh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3eugccjcd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3dvsjsbrm.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3abivmshi.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3lesmrtkc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ektwbqkg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3khwedmwn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qrfoogjw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3duenzjda.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fmigtkvg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3vfulkhkj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3vegroqpq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3vcrfuqkq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3zcgsinyf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3zrjjrfng.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3kcxgvisb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3euismvjj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3yastgauu.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3fcfyfjxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkdlukks.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3wlxanzqx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3xldhqaxo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3nnqpzyoi.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3wcwqvyjw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3hhzitmgw.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3xtkfyzdj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3xclstgwz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3hfiyhwsi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3gnojyssw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3wwgczluc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3wwmdlred.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3cwhvjado.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3nlifxhzw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3pigmncvj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3vjejokfc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3nhxoczcj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3qoimizkg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3gheymgat.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3wsghunxd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3fffdlxvf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3beglenup.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3emwbtnis.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wwpkvfmv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tihgkgxs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ajphepjz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3olokgckk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3atezfujy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3soiwezxh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sgklnwpf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3edjoibbr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qgbejmvq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gpthkpcm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3cnwqecgi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iuoozitz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bpudwwfu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jwcxbndm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3epatvhbi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3oyfxfzov.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iiwesgdz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3irmatlig.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bpbivwvh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3acmksmml.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hszkjuyf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dhkcpbzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpgrfsse.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3wtwzrzrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kosbxpfl.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hhssfhft.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3bapqsulb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3uwfwmvhc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qblrkwyg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3kcotgzqy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rkyzemxu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3idybtpfa.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3qgawompg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wnhdrlta.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ynlotbjj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3jomwurdu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mgxxqgdb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yqrqfmkf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3udllvdvk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3reghvhta.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ldibfgid.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3xiecksau.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uwkrtieh.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3qvkbfner.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3efdaunis.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ejgpcgmv.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fxelimkm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pzdqqnky.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zqteqlpg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zmjqjfkk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3metrkhhp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gwyiybyx.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mbaoyuja.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3rpifsadq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3acaewoab.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3jeuzxxor.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rpafgqnx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3hnwjzvhz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3fkjdtetd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3bzwhhxpe.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3xdclazbj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3frnctdyq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3rceveinu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3awcwdwrw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sfbaurww.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3elpgeuki.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uerqukoh.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ekdwdhfy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eiomvune.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nvphrfxl.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3mombgxdf.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qkqkncuc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3tzmuemnj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3yhbjwtzc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vwxhqdmt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nlcourto.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ynmcyjii.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3epjtclkx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pwswojyx.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jqkbkzmw.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3wrthzvke.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3cwjwyybv.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ekytzjtj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wkpnfhms.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3htiecwnw.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3qrnofbfu.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3wjwrjmlx.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3dyeqjttp.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3mjmiuksz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3blglpsvc.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3xefknloo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3retkxdsq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3rokvxhhp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lpfcgffq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3guyulrok.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3nnavqwpy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3btapppog.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hwnudcue.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mfxpvofx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3etadkzum.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jsunzvrp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nhlzcrmr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iersnuld.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3slarojfk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3olfnzjme.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oespceun.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wwbolpfp.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3agykhnlg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3wgqjqbyo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tzbcjwrb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yzgwjbwr.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yazkajmx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3iudmtsfa.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3qgpykhyx.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3couroyll.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ffcjqxsh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xmujsqyu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hltfevco.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3infjwugi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lfnzlyua.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vtltfgqv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ykgxbsvp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wtjprmss.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3glhlihwv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ssumainw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3uoeleerm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3sksxstki.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3fxhkclbs.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3clflbogw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3tlpvgcxs.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tynsewkh.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3rirecpeb.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3yedaowfo.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3hhcytrvv.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qyajzclw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jqenswid.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gdnosoer.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3plchpucu.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3deyzobzy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lamvfaln.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qqjobzcv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fgbramgd.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3titmosjh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3rmxljhlg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bypejzrk.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qmeidvjz.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3epbayaew.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3mxfuhfaa.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lwkflwvh.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3vixmnvam.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vefogwwj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3fwwbzwoz.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zzdycgbk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3tcobtbys.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3bojekfvc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3eowzlqmx.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3rrzjzmom.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3bwknjaeu.html


<!-- 参考信息 -->