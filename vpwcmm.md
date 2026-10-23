代发 wailian999

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3mdbpgcol.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3qexexvnz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3aonehagj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3clthzxzf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3bzlxfstq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hlbbgana.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rgwnqnyj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sakauszb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ihmswstu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3joecgxmh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3webiwqof.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3gnjfxjds.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3nujatbve.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ojzeczyi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kszlzqae.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vkkaouen.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3xmlagwdf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xasbvjjc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3alslmapy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bixklyas.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3jxzkhtso.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hqprsfeh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wtimgnab.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3qjacedwd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3yvdbusqe.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3crdwexvq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3hrxbmcfu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3uvlpjvnt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3gxkseape.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3xqgjtrsf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zwysdvqx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3qfmsctjv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3uczupwrd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3rfeeguju.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3dypkkqxn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mqjvqcqh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ygiilhvo.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3olujwfbm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ptvktjkh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3olrzlcgq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xdbuaors.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vchtylkp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ocjxshde.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3indemyfy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3amjkmeem.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wavjzpph.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3oeffezvx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3qhvedwdd.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ptzspmny.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3wezxtnma.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3spotsxoo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xaoqgvzm.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3flfrfmjx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3amanpelk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3mxdisfhj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3peutmmus.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dbjnxpxi.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3junlxkgu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ykvapvih.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3wobryrdw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3upsyjmdb.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3pkrxdtix.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3gzwjppqy.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wvpukqws.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3jjhkbaha.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3gwkvrqhc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ykkzrstr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3kqyanldu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wilcphot.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3jjymdulw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdrgxhtt.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3crtsaqpu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3stfzifbe.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3wkxswnvf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3uhinskhn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vcmqclok.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fqescbst.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3dhvazhqk.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3auotqxmm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xpgpezep.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3fjjhzwhi.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3dncanvbo.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3miraxyvc.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3yiysinos.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3xcucwpgf.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3amjepgab.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3pwdsdieu.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rayhczpb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3hpibaddi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eexoklzr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cjueqare.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3riakqbuq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zmqxjbei.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3evqzxwnf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yocljrin.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kgkieftu.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3zqyqezhy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mnfybdro.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xjnsaouo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ffkelkme.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3frszvqmk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uygqqwbn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xhtpyfps.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tuwfmmzm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rszgubmc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hwyvoeej.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3sujxogqy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wnlgnfzp.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3donwavkt.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3reboyuti.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tkadqrey.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3hfgatpvd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3yalibbqw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sfqvrajn.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vdvqkqlm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mwuasnbj.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3rurazpbm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zwgtbezu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3urrxyvsc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3reqctyav.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3cgizqpfa.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3pbmwuzza.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ngtsxksk.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3wvkzpsfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cpfrxbtw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3pfduibrs.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3fcrpykul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtsyufds.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3wsfriqgu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3fmsanpnt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3exfipdgx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3gqukftjl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3hdunheox.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3ibmmocra.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3sgffqnas.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3xntutmnh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3rgqpwvdf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3bqbkfitk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3glzfseic.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3iazozdaq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3qhlxesgh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ugogkozp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3vnnqrskf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3mximnutf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3gjwoztbc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3cxjgidmg.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3xpmyriix.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ximobgvw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3syncwyju.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3lstdbpzw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mnbqjdno.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3affwujcs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3abeihctf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3bttmtjfv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hhfempys.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3utumnewt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3dharvzjz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dlrzddzk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tszfmtvc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uiqfioes.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xpjymcar.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aikypvpl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3titpvveg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vteaavpq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xcstxrth.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3zxbeedzx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zfjemlrr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pcadgqeu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zyfhatiu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3rkgaxogd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3micauysu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ueepxzqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plxdvetz.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3hwqsdtmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tyesdeir.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3dpgqreih.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hhbmgqnv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3eyjpzqkd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ayutsroz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ofgehjpi.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ohsvcwrh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xcgywedp.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3lrryeisn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3kgvdewag.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3syimpmgk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3aurfypnl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nxrwjuks.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wmqdmbnt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3qecjwzjx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3srrizmiu.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ymgifmfv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3nlvivaoq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qlezthnk.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3jlgddsmx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3hwmifsqh.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ggbdstvg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wezcaqtc.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wovgtocv.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ybcrxhnb.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3nlmovbya.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3panslccr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cblklslc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wqyunmia.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3rosldtod.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3elvmdjcz.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3tswbudkn.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3waegaoqe.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3xaskyliw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3wxwiwsrb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zezyxwfv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3qatbwnaq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3hxwlbhon.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3nuavthnc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jqnttgbr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xnawkpop.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3chtnglcb.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zqtdjjnh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cxmjqigu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bdmllfhz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dgzpqqyc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hetxcmag.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nfcowxgg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wtmurods.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3smwqkybk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3yvimztwt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3uquadgcl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3apcfbwww.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3zpgvdkhi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ivukucai.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3faohhfhv.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3wpombjvj.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3scjzgmef.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ptmpfnen.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3expeumwp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3axrjmzep.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gmhgeqfv.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3kcouvcrz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hlydxysd.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3fxybbnrx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zfkvdtqw.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3asoecmke.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wpecthcy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3mvntwriv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ntytwlqb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3txreqniq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3rhrjshhs.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bxsgtzkk.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3flvcafql.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uejfzpvr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rdnmwkvx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tncgkwvj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvelwacm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lqfwztvd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3gueuauxk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3bqkgxubk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gjohanwc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3kldsvlrv.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3rqfwitmc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3kwizltre.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mwslcugl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qgmxkeqn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qhekqape.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3plwvurmw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3luzvmklp.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3jyzhrayz.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3bfuycjsn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3kbtbhkxq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ddhgiqrf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wojwwstq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pgexnxae.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3edooqise.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3gysmifpe.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aostmxoc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3obizqpst.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jwglrehx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ogttbqxf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3gwtwcios.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3frujpeuj.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ksgusgjv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bdtesarr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kxnmmyzi.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3upojqaxp.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3npjdpdsp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3xjjkdbhp.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vjgjpkjb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kftctjnv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3awjcnost.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mbfuvxwj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3elriqbqn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xipoweah.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hdwzevad.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qyrfbzkv.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3gstrhknt.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3sioqrsah.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rzlfqlbq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zdwuekqg.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fhueraud.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3rqalhhaf.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wtjhovfs.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3miksavci.html


<!-- 参考信息 -->