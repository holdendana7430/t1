代发 wailian999

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3slalbzex.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3enaugplv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nstedkhp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3uouyujcs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3qksyelzp.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3huznguhw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3incmsuxo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vgsezsrd.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3aytcbcot.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3sonslgww.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3myfbmlkx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3lzxtafxi.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3zusmevnk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3kgybgjtt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pqfbftmo.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3dptwiaxx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3fubkmcvx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3kurshjvt.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3pztotvjj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3xjcbqzpk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3axbfhdlw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3ecbxhpms.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ssyvhauk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3sonxjypf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3xkkeqwgd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3pxsbidey.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fhokssmq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3luwbmiqf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3myhnjpby.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lpfodubd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3tqtcjejf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3iflyfhsa.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3rbdnfaez.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dyaqhyjl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xwhpvqio.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3jhojjswh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fogvtlhk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bvrqcdvg.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3qvyfwjwy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xzgakwsv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3hyohzdak.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zszfjbma.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3fyqddrqv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ybnpangb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rfhaolcf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xebdbqje.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3psfxszsn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3cnpgancx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3unonfdkm.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3wqnpsvhu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3vpotwqwd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3zsumqhxr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3yvmiyuoh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3sfhgwjgu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3wqzosmbm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3dvchaoyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wigtrfxa.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3smvfdyav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hesbjrbr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ddixmvvq.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3huahlmtu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3zlylseff.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3oupzojxl.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ymfgyhxj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yecptusu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zqadzpou.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3azdistpw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gujnhwsf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3zdtdprlp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3aayxyrbd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3htbjtptn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3fmyloptg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3dvqlzyla.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lssjnbao.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jidekanu.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3hazladna.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3sslpdled.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wocswrbf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3vtmawrwh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3lmwgdpps.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3sfovagap.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tuylhrhg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ygklxwdv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3xjjeuyrb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3iqyzstln.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3gjkibjup.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3soubecle.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hpteglqn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ktanhipb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3svlyovtb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tkeziesm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ohpxqwbz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mtzxmlyr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ryepugxc.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3txxvwwew.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wgjnztar.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ysbyrfyl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3lgryonmg.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gumvckts.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3ueekccap.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3mxewyoes.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hipwuncj.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3mdpzklsj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sakcyzod.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3odobejec.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3odcvypue.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ahxfduig.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3azafwiur.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3qvoyuxmk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3qoxwiyob.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3hfqmgeyq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3bqcjakzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffnodekr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3zhnzbwnl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3dsvvbotj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rpyjnmqg.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3kwkochtt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3uwzryjvb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3orappjqx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3melsewuz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3seewkurx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3sqmdpizl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3rwfliwxq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3hoevvdbn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3sruvxbmd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3eqqbolbz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3ntheyvrz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ocaafxib.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3jotyvwkr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3mmwhehkq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3oftbhvdt.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3dvkahiks.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3pibwpcjj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3uvdnopfu.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3ykslhjbk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3iaatllmq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vvytzmtt.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3jwbarrlo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bcdvzdvt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3epjbxsfg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rgafbpuy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3lmyndjgw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nrsjhyzr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3indqdmrq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rhxhcpzj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gptudwty.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zoopyxcn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3phcysqud.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3htmjnjpg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nwduflka.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fmpmmtlc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3frlnbhjz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jrvfgnfl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bsqujbvi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fpizpxsl.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3rieaoycj.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nqneunjv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3goziwzoo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3egjqabwu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3weoaekta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mffsfnej.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3qynrrrmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zkyeaomt.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3abybeimq.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jhiqqyax.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3zkagamrr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vzalwlto.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3vmidwrop.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fexqlzzu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3yqwdcaqd.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3oeptqtkf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qpjnutem.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3uhqyhkdm.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3aeiqjxis.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xnvbqgaz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cpbuijoe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gyywtenh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xcvfbufp.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ikapyozc.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3dvizasad.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pjmshotp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ggshwqvf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3crcwqbhz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eskymwiw.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3voxlfaul.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jqjuyerd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bhysvrkv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dvvuirgu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3davorazk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cbqiryfr.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3dycemdsa.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3yzwoiyik.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3thwbkaes.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3mswvjcdz.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qvctipcl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3tzyxdmzi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3zifujdtx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3nqatxvlz.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3unyiryhz.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3ygxkwyha.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3isqnhrdi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3omxmskjh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pggjldfl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3agxlcrtv.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aglvspla.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vwkpdwwk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wxaykyvx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mzpulgvw.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yzwswhii.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3osdmvsmt.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3hmloyyyj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3elvayyoa.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jtntwxeh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gzeipxbq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3japyvowe.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3jvrqwbrj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3gfqkfmyz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3nxqvoxvg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jvklfnzr.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nblxmfeh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3xfdbvtyh.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hrngchbm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mucdxogo.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3oetzksng.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3xepkezix.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3cdywqytc.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3wyphflhf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rluwoxpa.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ashnenjv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pbzudwce.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3hlxzxtjp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ikmwkwbb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uuqukfag.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3hzwsxozb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wqdnquio.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sedisnii.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntgxqqfe.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3guqrchqh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bclkbukt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kedmkcrg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3fltpiepz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3jiqekfub.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3nmhkfnhi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dushqhsl.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3sgeueuis.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3gqbekkmx.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3pariopos.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3oeqjzfdg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kbbucpqg.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mhydjckj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3moewrfjm.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3uzxsczof.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3mnzzexqg.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3akfyztmk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3txrnbgqa.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kzrofqrm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rsdqdeek.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ydrfzsfr.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ojbkjjok.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3unhywbao.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cbdennfc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xjxspbbw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ffpvsyco.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3bnevftrb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3psybrsdd.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3irnlgcse.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3tmlpomfg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3jgjkglhe.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3smjzmkeh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3yeclbrew.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3msmultii.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ukgocvff.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3phdwvpwh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ylltclpf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vopyagmb.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aepnoufa.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lmpmumws.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pzpmnwxq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cicaiajy.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mtuyugxs.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ffhdedmh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3qxouodmm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kfcoslch.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tbjsfcoo.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lnslubjq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3jyopytid.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hxrnwivq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3tpwiqint.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gzyjaape.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3imtwchch.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ubxkpxek.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vrmfaeut.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3injkeebh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3oujqheff.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3fvwspyas.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3qkwmitqz.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3dmjooraj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ctxricmp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3hxfyhjai.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3urlnucvx.html


<!-- 参考信息 -->