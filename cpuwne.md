代发 wailian999

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3zrybbbvv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mugjmdkc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3szftatpv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ocjkbiph.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3uomxjcjq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hooiakgj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pbxlivcr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3knzxabnj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3iqbnyubn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3iodhuyuq.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3lyrhkyft.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ufvhvvsb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3isfdvbvr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3dylqytxb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3jdtaciyw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pdxzjjum.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3cohapfzu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ugcykceu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nvhxktig.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3eofuksty.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pjypmitq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ajzaufos.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3azpeijto.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3sygolwty.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3hlekbskr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fhoozybv.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3mjquutxh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3dfkwmyrf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3tupsuhwt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3qqlykiwp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ycvtkjjy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tlddeogc.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3qwxovyji.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tskhyrjm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3qxodytec.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3crjrrcde.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3xtrltdsw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3axrbmiii.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3zzsbtqki.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyrqnpod.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qswtkyvf.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3hlcjgngv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3kkqsmmpi.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3eyurspqz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bhyjjljv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ngvhuhjs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3kexnacod.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3dwwdibqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjwipzun.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3egawlbxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmxgmtdc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3jsqzlkjy.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jmmlyuhy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3xjyaewod.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xrsciuye.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3kyoqhqee.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3gbjodkyh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zstffgem.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dpdlzxcs.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qchycsbd.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3lrretdch.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3vtvxmbmc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3uequmqls.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3vlhxgwch.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3iokkytyj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lyzvsldg.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3eekuleyz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ypylphig.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tvgpkkgx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hdkbsbxb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3pjgpfsjm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3wxnbiciu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3prsjdksa.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nosimpbp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3elaoxcac.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zikjghrd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3bodckrpu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3hwndvami.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3aufqosxe.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hvhtrjtw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yiawaldb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nxqrvuhq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kbwphxbs.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3byvpgpvd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xhcrjphp.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3luzhdpxy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3gjuenwli.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ndnoksep.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3wsrebgxm.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ywyaidya.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fltuugjr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3mjbjgsdi.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3jtjiptwg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oopomczf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3zgmlolec.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tafyeptx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3gsmkgmkc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nrnqufgk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ommuzpux.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3xkgnteac.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3aoynpgsy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3qluwhjsw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3bcsvidzb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3prwlhicq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skrjesew.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3uryaogau.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3uramnbhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avzrarmg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3qvlyxfsl.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3qpeaoxig.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3rhqknmot.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3suldtrwn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3rxxsbqqc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3mmsajufz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3tacrliwu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3wgchbjfj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3uihlmevx.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3daydixcw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3gnqfpuat.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3rhqiucea.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ewujxgxg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3nmfkrswy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3scdemftj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3okxhtsdw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ybijggzs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3anljojkw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3uhglnoqg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3wopyocre.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3giuoskzw.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3viophkpj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gpywbjhj.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3agmtscep.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3okbvumxy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rulbvvde.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3yzaekoqf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3mtlpaqrt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qwoqnivy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xwfgfuqb.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bwrrgtaj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vgkpycur.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xzfxeafw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xvnqynto.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dbqrsqob.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3oydtqchg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3inpbqahu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3incckeby.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jafodudc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3oyhwrtle.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xbvhgoxm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3yybmbgtv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3sxdimqry.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vfrwdmqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nebwkalb.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3xhotzpsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zadmssda.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ifxzwnbr.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ydfnlrtt.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3wmgvrhxk.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lxftebus.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3xrgytynw.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rnnxfiuq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3oorbsuuz.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3drzqbojz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ewxupztf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3nakimywp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3rkjlhyik.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mdqkckfb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3suzwrdaz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yypporoi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3njhxuqcp.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3yjmrlrmu.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3tavggidy.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dlvegchv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3igxwicof.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3omkgkedz.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zdcbpgps.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vviyhlkj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fdqjdfnj.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3szeejliq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3lrahjpgd.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3nkhtpwrd.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pssqgray.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3hrjrmvho.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3vwktugni.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jdheuihk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fflkhteu.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qgeconsy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3xozocaqp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3sovjfflq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3czxkmymo.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3gkujtket.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3oxztnnfl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3lsxsuext.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fiyvwwmr.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3eyhwnoyr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rdbbaznv.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eoephgpo.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cazwqkgr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vlviwpgt.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bbpwplwy.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rajtxiqr.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pfytjxbn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jsiqoumn.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3oxbcpgrx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3omfljkgk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xbghuizb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3xcdumsfp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3yipdijiu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xknglagb.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3mslbausc.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rmzahuvu.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3zusreost.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3qzdzofsm.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3qgnvxqpm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vyacptgb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3lcnzwxeq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3onuwrtiu.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ycaofxmz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ouaqpsob.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3atniwmba.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3psezucnp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3biosjqzv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3znvropry.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3yuukphqy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mpdyvgcv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3uqvzbnex.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ntcjarel.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3sgxalfds.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mikzprxf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3otslprtp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xxlbfmtc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecqveldr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sqgnrxxa.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3yxtvsfqi.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3eadvntep.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vpnacoiu.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wgvauzdj.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3gxrtcavy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3jvskwboz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pizayxws.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rnsvurdl.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zjvzsxns.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3irywnxxs.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3skkhsbsd.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3saqwczrn.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ikbwlfmf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bbwisgsc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iccjyeqc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pvycchrl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lmtgkhgf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3emdtijfx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3nphsxayn.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dwvuimas.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rissjcxa.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3robdwbjf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3xxlpgrjv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ygomyhla.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3scipvrhh.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3czajucpb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lsgpauae.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3quypdrlr.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3fcyxsmae.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3awkizeke.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3moxretsz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rxcxapfa.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3upwhaysn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hdpwaaua.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fxnghqhe.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dcppihfd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bigbirsz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mbnoedpw.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wjmwbxat.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3jkshrydy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3chmubhhr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xsqmfxgq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fekveyev.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3sgauikof.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3sjjwyfnx.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3adfvdonu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3nlzbjwjy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ljcjluuq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3mkewoame.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wseipztd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ecjwaari.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3smlbaamc.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3plhdccrj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3dayfffmd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3futpftiz.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3eglagspi.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3twqqauop.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3kpcmgkvz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mmabqqia.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3tdxbivab.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3ccfivahh.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxikewln.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohdzsocl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3dtomhsxc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3gpdgzzkv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nupyyemj.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3mqycnhxh.html


<!-- 参考信息 -->