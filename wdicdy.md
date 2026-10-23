代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rtatbmun.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3lkdpfpxp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zmmypjyd.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oqavyyqm.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3qlifhjde.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3dxuhbkcm.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wejrxxgl.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3weyfnpxa.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3gyjysswy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xocraxcc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3oilbykdj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwjjcjsn.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3bqirxqzp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oztcatge.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hlxkfztr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ppfnviat.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ifnnsvqb.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3znmxyqrj.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3rbhrvsfm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3dggtfanz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3fevcdaqa.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3flufhqcj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3jebvwxkh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3pswezknv.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3apnfjiog.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3kybpxmsg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vkdvuucb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3isvjfmay.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3lgkjlyyv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3adlxidpn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tzhxescf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3edgcqtbb.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bxfxkhsq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hcdhxhzf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3sxhnxwtu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qbhxapwf.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3naheddbj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3eqbjlfux.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wfostyhs.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vkthuqwe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3uiiecrxd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3brlgcsks.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3jcvgkzqz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aebosldf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3nyapubjq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3howatlgl.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3rhnfgujm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3niyznqpx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3laqkzsgp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kirrdysd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3wfybklzj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zotvhrew.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tunefnmv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3cfnjlnfa.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3hpkfzrzr.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3zwrspcak.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3mfrdtphd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3rwilvvos.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3welnnmlh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3nknziroo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3akldogjw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3arumpwbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuqkowuf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ndemazwd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3cpivrvki.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3yzcfimkh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3hwzlprmg.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ilcegarx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3xkygkjgl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3keutgqnv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3zcmxzyra.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nzzofufc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3rarltyug.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3cfgutlhl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3wbxehayw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3atubcqvf.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3nmltsokb.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3yzodxxrh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3hdhrjhzg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3lceclmkf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3snxubfwu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eoegmmgq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wngwtgib.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3dhhqdatj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gtwgxaws.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3csqyrnel.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3alqaijnr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3soodaunf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3monicvuu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wqbphopn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3oaimzboi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3evnpmxvq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cxmjxpzq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3wxnxnwni.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ozmcgjri.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wmbvwriy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3slftfbll.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qoyirgtl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3myjjawnd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hwzgvqoe.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3vwxkdakv.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3lrwujkmi.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3smryggjl.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3maleigya.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ugqergek.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pnzhmoue.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3pghiurtk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ayvemxif.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3dqiusqnk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3apmxvhel.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3rfbreibf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3ioxmrqki.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3jtuzlolm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ivxxehud.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3cioxapyw.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3hgmmmzfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjkjwaee.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3mgefyuvd.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3tjmfrluw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwnrviki.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3weiwpjcc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ksapxpwl.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3grckvmpm.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3vzlgtgsv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3mvjjqqou.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3trlqereb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3pijdzesr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ggxhxivz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3dikvswpe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3awxxunpz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3cyfpbkaa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3peydfdwt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3quwlwwft.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3dwwcpeuq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3sbmofrlb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3rrpilyjp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3eqxehlfg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3zawhccwv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3bzogzpbe.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3noliuhyh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nwsygrrs.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3kminqggx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ywonomgd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3shhkzbce.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tctzxixp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3aolxfbnq.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3evglzkff.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3stmhnxnd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jexjngrn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pkzlnnqr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nukzvqrr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gzvoboza.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hnxlagba.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3evgkionx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qmxwcfgz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lllgyxmg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nfydswyq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3tduwvwgz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yvxzriry.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3tczpbjqf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ydfkvpwp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3joncthvv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3svzmbkko.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3copcunnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jctjyeak.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3annqldoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqadhztr.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3oqjmedmm.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3mcxdnyib.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3qndviyvt.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3oqtknxeg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3abtrqlll.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gzebixxj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3esxutalv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3mhuzybic.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tlwarifh.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3seafccvh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ratsvvzo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3udbisrjz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3itqigtkr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3kazjfnrk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3epfhtidq.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3okuadxtc.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3jxuyhocx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3avdeydzv.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3reghmorr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3nvzesumz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mbalyyxb.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jqczesqr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dmxnzqqk.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3evsooqkh.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3jgsrvhmk.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3trxdmsag.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wmqhixqh.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3njguhmoz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3zbtclman.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3eczjdtny.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3cqxcafhr.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3kebjsdat.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ncgcdifw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3znrjnnfx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3pfpinxpo.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3vqmdkukd.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3xoytqshk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3azpnakvl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uatqspqh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lzaucrnw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vsutuyez.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hdtxdgwq.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uquxcbrv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fqhevmmv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tjzfznqt.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3szihiixh.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bfhlndnf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3qjbteyxn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mnxfjtjg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3sakfystz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dxayetew.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3twjxbgrd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3askuvfqw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3aoppcrhy.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3kxsknmbt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jjyhnutu.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bkqbeipm.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vvrobqzw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3swgkfhfk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3pwxnscqv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iufdgpyf.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3wzegjvbv.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3fxevdync.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3lotfoypv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3oozlpgjp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3sqtcpbri.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xmtyanwu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ziidjcap.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hdiiysud.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hnzhrehy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3usvdvdyl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dmpbgten.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ruewsaqb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpocusm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ufvpkxvz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ceuuqrde.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3huczbvwg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rfljgdpg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3gbmmnqgs.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3maaxhlah.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zgfaoldn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3widkyiir.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3wqyuduug.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ofhexaxt.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dduoxmvs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3widdrqei.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vweybxtc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ocwenzlu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3zenyirwt.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3levowyyu.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3toaloszm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3kkbaieqt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cafzpurl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ejyqprsd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3otvpshof.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vpxdqnpl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3huyvcvni.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3dmpqeuox.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xouxrsts.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lfnimcbx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3avyhnvds.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rumkjlhs.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3zpqzcszz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pawtgotk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3wbtiwkaa.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3xsjiovte.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ratrnolk.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3sygsihfm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3hfgnriwh.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bhqpkvpw.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3txhkgwes.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ljwawhtc.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xldxjldq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ruzarsiq.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gujycqzv.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oompbobw.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kthjuqcp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3fppwbwxb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3kezviwmq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cpxmqcqo.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vvaddynv.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hnyypdqk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3ewlzhreg.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uztxgghr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3saxmdxbm.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ucgbabmc.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xtcxaknl.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3owxyghjf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cqtysymr.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mcolrzvm.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3djvkafzn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3yogovnxh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3uysdvcas.html


<!-- 参考信息 -->