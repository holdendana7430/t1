代发 wailian999

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3sqrxwkdd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gcgzorxj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3onxxgsuv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rxigzbdj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ajmfpcld.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3jjqqtrpm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lqsdvglb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3egmsuome.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3gfljeqeu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3wtmukvwj.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3dafigbmt.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vhxdjqkx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3liitljtt.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3obpsmvfl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3qeecazps.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdpvismw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3gpnhdbph.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vuypdhbp.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3jfzszizh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3kfhwswfh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3bxbmempj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hsighany.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3wbzsdbtt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3swguzxiy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3omjhadxj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3lqpyakpn.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3zplluqez.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3iyowborp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3xvmdmdox.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3zcalvkfn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3biwkizhh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lhmpwjdr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3bnokluft.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gabvrijl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3svjryugw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3mayyjomf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fadvisox.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3joeowxrx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3djrlzgad.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3guergjnh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3weokiauq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3trtzoupy.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3mxiacgbl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3gosdaylv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3aryrphph.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vqeqksed.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3gjfznggl.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yekplmpp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3hckuesth.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jxubkfcq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3alaqxzgh.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zfhoaxpb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ziuezpgp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3efkigwpo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3cjpcfrfq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxdgbwsc.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pewppyoq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3wjkbuwkl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xiiqkuzm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ennprfhh.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3hucotfif.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3yhqiikcz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3iowidxhv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3edbfnmnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehzeahge.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3boaguonh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3prupsjjr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3kofyfjga.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3bfempxai.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3munqwnrg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jqhqzwgl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nahcvuku.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hoxjfmzh.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3dtucruaq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vsannhzx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ybmylxue.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3bijjjtwg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3nburshzd.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3qsnxaysa.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wuwlqrpn.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3kzgommzw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xbjeesvz.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3oqcuymld.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3wzingoqp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3olwlvhhn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zzuyicsu.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3vugkknxs.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3oeljauhr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qeedlhlx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lxuewftl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3efoyeair.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3khbyopke.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ndrkgyaj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3mtwevkcl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3htkkzyzo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3irfrfebd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3liuraoma.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ufcukuzx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3edkzmoyr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3biplopfs.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zkkkpuja.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xqxxghbg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3zbyhtfje.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xodaqdud.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3exlfazgo.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3nubbiaoa.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3thrgmyvc.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ilwmxtpg.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3qoeyufyx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dwuceftt.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ebvkpxyw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3irqksjfj.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3hikamegk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ojfzrfhn.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ldfcakzo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3jjmfngfn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3wfumbjzh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3gzmtczrf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3oegmmeap.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3vdykchin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfwxaclk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3muzaipfn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3qtdandav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzbeeaoe.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3vpikihpz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ljhsqpep.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3fhymypfx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3zgpmbfwg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3polskktb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3unxlvaej.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3mqcqnegd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ckqzircu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3kkkwyrmz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3jdpriixv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3tjhcpner.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3zmxsudng.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3fbzwddec.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3rudrhrcd.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3gybjymex.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3twnmtdvz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3usqxpxvc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3nvqxtkbw.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3jiotxbca.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3duyeflmw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ktufifkf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3egweulqj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vzplrjtk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3evblulql.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xesvultb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rgfhzqez.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3hngqymcj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3xdrbxqka.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vpkrlccw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uhcbxujt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wqmrdmcu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qktykucw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ncgiffvi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wlbbedfo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kbcglxje.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ptiukhvk.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3htmsqaja.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qpqtwhci.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pbzypcan.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3xgyuanjh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pvuwelvr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xmlrhfds.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3rborhfow.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nmtkjfzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jahyalvx.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3wixxwcff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aoupchna.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lkhudxgj.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pnvpuutf.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3qharehao.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ijltcgmh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3sjfhahwt.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3etcpfuvt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3acqicraw.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3zsakzgkm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xhickszw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3eajopcym.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3fwhndcwd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3duvjvuzd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3furlgkrs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ucxywlut.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cvedteeg.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qbgirvvh.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3kkwygwwj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3shjovrzv.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3orzuuerd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3dqecmozv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fhjqtxgr.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lufyxees.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3venglhwp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dkqdhnnl.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zpkauxcg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3domonbuo.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dnzhrrnk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3oxjikajr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3jubhzmuc.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cocpyqjq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3sssliuhd.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nyotawsi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3dartpdej.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3almktnau.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3prwoplgp.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3tsbbsngh.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3qgbsedfc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3rruxhpof.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qhppcoqu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ymowztqp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ewqttczo.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qxsteglr.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3blwvemqe.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ksaadlxb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pbmctlma.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3witymfrj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3jpfcvvbz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wupafqya.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3njigfsnx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3yifmhpgu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dhkypgfo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3eyuulywk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3gmjytwmj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3scmapbpg.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rhbdkiki.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3glkjqntg.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qqkrukxh.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3muoigeyt.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3rzbjqecp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3vhyycylm.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gclbttkc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3reinbmoe.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3xnvlifps.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3nyrfxgpy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hrqqfmaz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3dvaktpzw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hhidnbtt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ldqxaqos.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bvmxdkzr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3flauntfw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3plavqqea.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3iemrdwza.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xwfngikl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dploclqr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulevkbjp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zlrfizmk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqsztnoq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3frqcjepq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ruhbddof.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3uvvyitfb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jwliukgf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qmxoikwr.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3dumbozsr.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3rghqiygg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3anmipjjy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qamwqlez.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vfwyuvao.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3tlurwmdn.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3kkndqwgu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3fycegcnw.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3eoouvpnh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ozdlzkpx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rkqnjjqb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zjkjezbz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nwujsves.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3spbflkhl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3vwdmmbhn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sfnwzgem.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dtbgmcgp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3jgyqchag.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3tomgorfg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3uekaofzg.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3grvtdpvo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3zobgldgj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tmyhnzwm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3panrfcqu.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3pgihdqiq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3forvthqm.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ucldchiw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3odmftqil.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zybfrvrl.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ypnffbee.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bzrickim.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3qjbhvsao.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pwoxhrzb.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pqldeezh.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cvcskbhn.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3lskngocr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3aafnjswo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hnlopwpu.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lgifsfqc.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ulqgeegn.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3sqboqjvl.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lpdhxbln.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3hvqnuuzm.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kpnokjux.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dvjuygqs.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3uxcocwhx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wuypweus.html


<!-- 参考信息 -->