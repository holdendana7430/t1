代发 wailian999

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wvngjpoh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qtvwfarp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3frfofuxl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwswxoyk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ejsichbh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ftywgldb.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wltcaqxm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rsvoqkpe.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3umumsbdd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ksruaqca.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3obpqxgxe.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3ckseztsu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3wuizvydt.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hlmbdpbe.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3mssmhwdy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3iwzupryk.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3olwomqvd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tvugnkdj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3ulrzrqds.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3bjhikany.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3kmjbaijy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3wkjqpfgb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3euojcmly.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ypcjolic.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mkrzupbw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tfmhvumn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3xkylctwm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3wjvhavmh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3xnnnwnnj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wvflgcpt.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3vztouudd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3ddrgjzkk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ymnupbws.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nwvwmxtd.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3cyvyuuqx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gnlqjngc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3atnsjfgp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mqocmfox.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3bpzinrtu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3deiczqcf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hvtuxznn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ogsqiiyw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3hepjtwdg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ediyuydh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rkybxlwv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3dbahzmtu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3iagxckio.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3sekjpxna.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3bdbpxjln.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3oudhhjcq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3quuksnop.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3oiijtwpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qngxmjtl.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3zatobycr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uxdngdiy.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3wahxbkpp.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3jgiunskn.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3oqlwnlzn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hlfhahiy.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ltellhtb.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rwpflfhy.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ayrgvbwt.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jzyygcjq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3njedaqvi.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ozrqmzlq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3kolpzkcf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3dervksza.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3algimnss.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3phxsyugh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3yyhsqagh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3vevmhztw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3lvxtvpiw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3azsyzjqn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lrpzpzjm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ozfdgong.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3pyrxzxrg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kknvwzdr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lxuoqpxf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gjyjlzeg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qteetitx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3gnqhvyqg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3sncsyjod.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pawofyip.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jfgszrja.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ywkwcxwi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wxpgdxkl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3njzlgfcy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bdecciqr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3egkqgdkg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3mbyglhzf.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3efninlva.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3feeaceyh.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3eegnaywy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3sneskkpv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3yezrxiim.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3enirivmj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3xowziipx.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ooldbtdq.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3dgjafwoy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wzgbngrw.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3fextsawe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wxetxeky.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3quysreph.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3byjwbqex.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3cxrxbnjx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3tvtllpee.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3xcghuwca.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3fwandoqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tohyzffy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3qpaarbst.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ydicbxrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3foesctlz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3epvaimoh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3fnkuamna.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3etbmsbyz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3wneweiqn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3grngmzmq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3ztwxavkd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3iftlxcbj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3nzsteijo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ydngilzr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3uvneqxot.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3bywafnym.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ibijasvx.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3jhaxmdxv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3jlaznimx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3pggjtmjo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3kpmiypjr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3puxdotls.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3bspdxoud.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3mmtgbwhr.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ptjcmbup.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uexdyyba.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3vjyqqoxr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bnncmjpe.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nbhnfuub.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oorjrvdj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3npehfjxe.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3mlxkwrnn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eotlggaf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jfdiwexs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3obqpjvns.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3othuzhot.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ityshyqy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cicanvkt.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3elkatsii.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qcunsiuf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kefdmjfp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3pkljakho.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3vaozgnfh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mjlvpjyn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3nshhbfah.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fbxkutpi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3leaohrqx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3svzsfblt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hblbrnlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzfadudn.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3rnmrawcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbjoabsc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tdoywdyq.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3obbsigiz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3qtigqemn.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3livlucjv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3wmexlzwm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qinmkcjg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3dfqgpxoz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3hkqdjozf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zdejhidj.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3uznhfgjz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3cyqkmqxz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ndihrabm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xodgfsbr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3vdyyshel.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ywzayxwd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ivicslpe.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3coaxcmnb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hjfpqpsp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3wajnsgzr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3ejnkkkwm.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jidhjitk.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zsmpaptm.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tsspefmd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pdqgiequ.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kymevcmd.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3thhitque.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wyxzuojp.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3pexrwnkd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3cmgucyxd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zxeyuznx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3tmxtddmk.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fjjuvyxy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3nldrpraa.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ecmycfpp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3fhslwyhg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3yohvmgkg.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3bvvvlrez.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3jvcbxtvg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tcibpged.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3modbanal.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ksdbzboj.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mxfvivjl.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gzzbusoi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jebtbdgc.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bdnewxwf.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ppvzhraq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fgqkwbbd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ooquyvyt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3amxucvhk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ywfogtpv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pwaqhjxy.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3oamgqjdh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3falhqbgk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jntzgpol.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zfqeoxzi.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qpwzdvmb.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3dijwdvuy.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3lgzlnamt.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3uyjznkjl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3olifwkka.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3eawcktld.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3tafsdusw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ftoxopjm.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3mcpwkbxb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hbkhvmcq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3xhntfxjd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rntwmxam.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3toncbhfa.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mnwfhfat.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3utdmddaf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3whqyxdie.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nknqndzf.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pieyaxvn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ggrusyin.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ugbwkukv.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rzakdhqa.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ygiyifnk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ftoermkd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3gsdgwoyy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3tjyipyft.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3onccajqa.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3koemojdq.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3vgqbzrgg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3yvyigrut.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qoryiiar.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3gtzkktqo.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3syfckrzs.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3bvdjvemw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3kxwafzfy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3uynmbpgc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3zukxptse.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qytjxeai.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kjefwgfu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pkqkmlej.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gtysftxe.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nhlnoycp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3xverwjse.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3syshyvzx.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uvthnauh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3jxvbxqhh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3heudhvky.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3degjppgn.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3vbtiviop.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3pbottklx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3epaidyfp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3oxvsavac.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3kpzlvmts.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3dvashpju.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ruddvrwu.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3clqcdifh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xkhmqvoc.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3appyougs.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3igvbapwg.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fkxjxanz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gujoqlcm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uxgtlhxn.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jxyaymlr.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3pzdycbps.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3kygzubdn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3qvkpvpjp.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zpzrxcyo.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qbpolvmv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3pjyexffj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tzmighyd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ppvexmic.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3yvttefvq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3lxohpatg.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3cqdvwdwv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vurbeblp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cylvwosv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3raruhcyn.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3knzohsfu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3mowwgkub.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3caarpzlo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zuunskkm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3dvchsrcx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3oerkxyks.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3lcsqarzh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3dmurmgzf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3lagqacbg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3jfnaeqpz.html


<!-- 参考信息 -->