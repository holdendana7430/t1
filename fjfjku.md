代发 wailian999

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ksoucatq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nazkkjfx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2ukaxbryp.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fttyctuj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2nidrbyoq.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2icvziseg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2frhfoddx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hdykuvhs.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mzwuhita.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2sodxhfhz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wkaifumx.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2kcaslrfz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xidpcvgr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2zpktofje.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2tvgatptm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ihnsesqu.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2osxliitf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fmlilgmn.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ycigmwmc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2yglpaquj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2gseavbph.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dazvldbg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2kcihbkzh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2vmwqmjun.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2tkelbzkm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2njuenudk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2yyirlxqr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2fhynwchg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2nyyubhgo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2vjsdivou.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2pzrliwby.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nfmvhfrj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2cfcbywft.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2exxtzuxl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bskkaeyl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2mbdaogxl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wkvngnzk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zotuhnfn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ifmrkkrm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2zrogjibc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2zwtfnafh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2seecexps.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2vjybqpei.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2cipvqzox.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2dtuxuepg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jmaixpqt.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2eveojbof.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fkqhdbmu.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qcmkkwhu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jposguut.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xmefmjbq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2idmvcory.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2snkzfetm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nnthdtak.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2wrvwndlp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2lzexceru.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2jilgriml.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2aseyxrio.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2sjwsdelu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2vwagnvij.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2dkvpnmop.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2znpvdaxb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2pzxrvxzx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2mzlbvzdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzsxohsa.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2uynmbdrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ehhdjlwg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2nwooaaxl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2oqwzgtqj.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2yynconxi.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2viwcpyzr.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hxedqgeq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2svxgjyqd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jkqkcdqo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pjxziage.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rswvtgrm.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2kvekipae.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2uqgjvzot.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2empobcjj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2uyxvjcct.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2oxdqdrxi.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rqytuddv.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2guymecqo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ftcuemtv.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2spgjxziy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lkkltpqe.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2civopbuj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2xvgcfizh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hqbmudzz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dpfwxoyd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tjgehsrc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jfmfpllq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2hjrygkld.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cyfrlemz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qtycubtn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2obugnzhd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qbzqbbmy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nupynuta.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hxbannfg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2humttwzk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ihieumjk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2vdsygynu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2fvdubajf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2jcjdbsui.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2funzixoq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2tprpatvg.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ktnmjyns.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2qlovqcgi.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ejbfbqfm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2htkffxwo.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ujbvvmtr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dkzwqhvo.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2xyafaxtz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fmkclgzl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2qldlfize.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2sypbdwmd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ynoyaxaf.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2tqwpuxqx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2wssfzttl.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2yypwiudl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixolmyfh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2yhvxsheu.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ushweqnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prxlihow.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2fnamnlbq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2hbhclemt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2horcimdu.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2nzwbuvbe.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2otjleuil.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2bjfvvcoj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2hbwnsleu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2nxorkivx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2vamhofpb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2zfycpdki.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2sgjtcmgm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2bgwgqewu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2hfzryukj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2bvkgnzyj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2kjxpvooq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2zoionjex.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2sfbclrtl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2drtnytvv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2iagmvqwi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2qefsfrsb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xijovgbc.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2tbcjufsr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2oxuxrzco.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2msjccges.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ibggjwmi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dmlbdbto.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2szjpeqxq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2vqbilcdz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yguotupa.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2kdodhhxi.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zwvgvtjl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ejvbwjfs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pjhtovoy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pwlufehj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bghkmcdw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2myullpsl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bpiukgdq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2wxslilgz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rfjwvpue.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nnzwxubq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tjswpncc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bxhzwkuw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2pfcgazmk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2hshvlyil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hgidfdaw.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2tbeudviu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tekcaqlj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mqdmyjlq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2hqzybkvb.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2xwvlxygm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2niglyvpq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2shkrwyli.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kuthqeqs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rjjpbgrb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2vahniugy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2etjjytiz.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2dotikabx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2mkrqeeeg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xdykznsk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kucjikyr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2tekbuebs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ugiauryf.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2avxcytpd.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2hfmxxrao.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2odyvbzlw.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2zqkzefog.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2omduiucw.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2icheausm.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2drobwksp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cisymvyo.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nheoxrbi.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2fwbezopz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qlomssmu.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2otvwzmyb.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pnjwctwd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2jbdouaui.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2xbpbznlb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2fqfzbhll.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hdhvyozf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2jbklcvbm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2fwqasume.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2piwdfajr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2enwkrfmi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2hcmfgxxi.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2atlxinzl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ojpgnkhm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bchflogz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xbxhbwxc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2znodcudo.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gmzlvjsc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kkgotqti.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2heyzvexb.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xfndlgbx.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lapudcmw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2oiofkiiv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yawqkwyw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ayfizvnx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2npihouid.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2eqkfjgcu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2xqcmobnt.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2chizvozn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2xgeidziv.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2pwluyaae.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2iexdqncz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2eheqjccm.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ivtvyaff.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mdrulwnw.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2gyhwujnj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ahpmoqrf.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2bfwjevqf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2grxoqlvl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zydajnfk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2fjtptxda.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uvzfysmp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2iuucvzoc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jarmwnzt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wnfowqjn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2jqmjvepi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2atqqoehy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jzbjldfw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cymvijcj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fqrgisrd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2imlsyrft.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gmrlaezk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2llnwwrgz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2enhcgyje.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ldqshfms.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gkxgefcd.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ifjxdixg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2dpdwowsw.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2pdczfhrg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jwcqcxcx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2pvwhelhc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2shbcgxai.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2lbykylll.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ikiybevc.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2uzgkafdf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2qayueznt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2rvddmljk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pkoncjdn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fwrjprnn.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cwpqlhfy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gevzzqve.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2ribyceod.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ssqhawrm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ayzchbrw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2svkoyvdi.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2hluntbxs.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2grgaobab.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2zmlqciro.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cuvjurtt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2btlcyoyf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gbpxflov.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ryuyyjzj.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2yfvdsgel.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2dtwovsmd.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ruzegxib.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2scsirsbx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wwdjjcpx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bpydxyju.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ipjnyyjc.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gatlaauh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hvrvtrlm.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ffxhesqo.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2xzmctmer.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2fytatnwx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nqssfkfm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lpepupfv.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rcfymyti.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2wwboloje.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2urxgaqve.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2rmcsimmi.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2besevhgb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fvaoxybu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2bqcfzohq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gwjzpydx.html


<!-- 参考信息 -->