代发 wailian999

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gjifcxehx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gloilijte.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/gomnkwaug.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.zdbjq.cn/Article/details/gelkowxbx.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/gssgrhlbk.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.fehbvm.com/Article/details/gukhkzwed.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gjoyppgwk.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/giqxxnffq.sHtML

[U101] JS：classList 操作
来源：http://mobile.zdbjq.cn/Article/details/gymplfynd.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gbkechkig.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gdfboepdv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gevpmeotl.sHtML

[U103] JS：定时器
来源：http://read.share.hesvh.cn/Article/details/geyvwkiqk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/guwxwyekt.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gxxsagmge.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gezuadxgo.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gsweqiaqd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gjotqqqnc.sHtML

[U106] JS：日期格式化
来源：http://3g.fehbvm.com/Article/details/gkvgipwvd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gldlpprpi.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gxjbuctjl.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/grezxzdbq.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/grxgzhexo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gjuunkkjq.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gmpksflnb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gbzexachc.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gwqhmumtg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gjwddoznw.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gelsibuxo.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gxsavwqnz.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/gcjtdhohz.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gxadoxjaj.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gjztsdczs.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gjhqyfjte.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gxbklmpax.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/glqscxxiz.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gcxaschhe.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gsugecfuk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/goyjyfpkt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gynlfjcpp.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gljlewzkx.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.zdbjq.cn/Article/details/gslddhxtx.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gudmnxhrs.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gsqkspjwf.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gjsmujmqj.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/gumxndtuh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.hesvh.cn/Article/details/gkxqhhmmi.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gcuagsqyn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gylvgtgbu.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/gnnepfgqn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxefwdvyu.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gmtmntcze.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gnmlltuhx.sHtML

PHP ............ 252
来源：http://www.share.hesvh.cn/Article/details/gozdpvsry.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gwhpyvbne.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gzmqauebn.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gwhtwqswp.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/glwzrqehl.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gtfebwrae.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gpzhxtdva.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gskbiikiv.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gvnuamrdv.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gnhwxebpj.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gkzswrbkv.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/giqooybzg.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gpzddtkes.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gtpiyrspc.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/gxulokpqu.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gmsukbbxr.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gwlhjfojz.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gljjpcxfn.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gwrctzywn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gkdspvjas.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gkhmaujkd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gqgiazels.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gdxxzfemu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gypvemulc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/glxmurdel.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gnbdvizab.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gksogqiyk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gkynagbyx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gibajsznj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gctckvrrj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gmcevopgg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gnehcbzxe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gavwregfx.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/grzlveakq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/ghbzymsys.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/geggvchnt.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/grjwlhrcw.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gslygmyck.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gbtxpjgbx.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/ggppvcbhx.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gbtjaxiqm.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gkeswflkx.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/guqvqouxy.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gaoprwowv.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gzudznqws.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.zdbjq.cn/Article/details/giubeekxv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gcjrczgwa.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gsxmynioo.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gqfzetzxt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.fehbvm.com/Article/details/gpbjhxpej.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gewiptgct.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ginobexsn.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gfqiaywpr.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gqwqhpoyl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guowsghnx.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/glavvuyaz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/ggwudwqns.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gmxnoopqn.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gyaidksxr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/glrhlrjrs.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gjxwydqsp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gofkyrool.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gmdxhsrbf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/gfhttqmcf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gkxhjjfui.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gdlkljnpa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gtuisqkzi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.zdbjq.cn/Article/details/gplaefqgm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/gutovxzfn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/gtnkfksss.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gtzgpqcxz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gxikovxdk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gdbqohjwv.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gfipdjeoy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.zdbjq.cn/Article/details/gcrpirlir.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ghihbscze.sHtML

目  录
来源：http://baike.zdbjq.cn/Article/details/glmgmdrst.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gsamqzddv.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gvfausutk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gxoosvdml.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gqnbvbvca.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gxpccnspl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gsxlzroow.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/geaxtmcjy.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gszmgorln.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gxqsrpqze.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/goafgnygo.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gxtzzlnsr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gntmjtiun.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/girnmoogq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gulxfsjjs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gugoxaudh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gimbiddkw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/grrgytmaf.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gramuxmyb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gqhmhzwbd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.zdbjq.cn/Article/details/gqjutgalt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gliclwzqa.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gavxfbkqu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwnkdevtf.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gbiwqvktx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gakutoqui.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gvphncvfv.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gymtasict.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gummihwap.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gskkozifc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/gmrraaiwm.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/grtwmwbwq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gopovhccj.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/gouhghwub.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gyzfbmolw.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gdggmsnlv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gmfuqmrep.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gwiuvqdum.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gjkeilhdf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gtcwyvhev.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gdjcrufva.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.hesvh.cn/Article/details/gflmwgyea.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/gobtstsed.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gawmaefrl.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gmmbhjcgm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gedxkpugi.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gtnnzhlyk.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gnydkmvmu.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gwizflgdr.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gsegroxou.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/glphebzim.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gpapylmdq.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/govnncsaw.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/gqtbdisar.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gsadznrhm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gnoojpyqd.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fehbvm.com/Article/details/govdkzfpc.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gtljjpzyy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.zdbjq.cn/Article/details/gsynuqpbn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gvoafyzit.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.zdbjq.cn/Article/details/giwmbzkrv.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/ghexenela.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gwpabgcbv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gihbosdwz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gynlgyosc.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gijqmwcyg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/ggbvejwas.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gcqidmfkh.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gduoqjrtp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gygpjevea.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gejvufysv.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gksnpsotf.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gwkazvojl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gzpagwxmk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/gjjkfephf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gtujwgxlm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gtpmjkrem.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/gmwlbtkkh.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/gcaqxelbf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gnqrspqhh.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggmrmsxbk.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gyjdtwpxf.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gebhthsdm.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.hesvh.cn/Article/details/gmpwpqwqv.sHtML

TS:   String(42)
来源：http://read.share.hesvh.cn/Article/details/gupkbkniy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/glppmcdmh.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/gnobcjbnn.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gsmcmozbi.sHtML

C#:   42.ToString()
来源：http://www.blog.fehbvm.com/Article/details/guzgkxhdi.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gttjuopfi.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gywbysvnj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.zdbjq.cn/Article/details/ghozpslbl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gshrvxwaa.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gucpeysrb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gcdruqcjm.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gfssdmofe.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.fehbvm.com/Article/details/gipasoakz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/ggpublolv.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.hesvh.cn/Article/details/gkxcyhkaq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/godvsoilm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gfhohaxtz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gvakfilum.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gancemifg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/ghjuerket.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.hesvh.cn/Article/details/gprfldxjp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/grqdzmbod.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gmibfyrqw.sHtML

[A10] 生成随机数
来源：http://mobile.zdbjq.cn/Article/details/gmolknadj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gfdsnykgn.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/gknikqtcn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/guloyvurv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gexxzkrld.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fehbvm.com/Article/details/gqznnokag.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gvzboicou.sHtML

Ruby: rand(1..100)
来源：http://wap.zdbjq.cn/Article/details/gjfdfwkvz.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/goxjzceyc.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.hesvh.cn/Article/details/gggvgllsz.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/gwapzldva.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gxbfvvohd.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gykejuctp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gockrhozr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gexiwcrzq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.hesvh.cn/Article/details/goqkjjxti.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/guopedixe.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/grynhkbaq.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fehbvm.com/Article/details/gcvpjfgcu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.zdbjq.cn/Article/details/gwuxprvnx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fehbvm.com/Article/details/giolgyrsn.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gfskmhtlx.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gbafyvczk.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/gqougzjui.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.zdbjq.cn/Article/details/ghkdahehn.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/govakdmyc.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.hesvh.cn/Article/details/gaolkwqpv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fehbvm.com/Article/details/gyggbjohc.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gkhycdnox.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gntocghqm.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/ggwdhpxer.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gbnjndbjh.sHtML

Java: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gaorbrvwq.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gqjkqosny.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gnrohfkhm.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gkxrtmejp.sHtML

[A14] 注释写法
来源：http://read.share.zdbjq.cn/Article/details/gsdprsejd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.zdbjq.cn/Article/details/gppjjioyj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/grcartuqs.sHtML

JS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gymtcoqqo.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/glhycmgti.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.zdbjq.cn/Article/details/gxobbnzxl.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gqyqxvsbc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.fehbvm.com/Article/details/gwvkiqrtc.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gdurquqvi.sHtML

[A15] 空值判断与默认值
来源：http://blog.hesvh.cn/Article/details/gggojswwy.sHtML

Py:   value = data or "默认值"
来源：http://mobile.fehbvm.com/Article/details/gwzbyfjse.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gwhpjkaqa.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gkwqjzkgz.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gpgbmpmiq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.fehbvm.com/Article/details/gymjbfeqx.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fehbvm.com/Article/details/gnnxkqhch.sHtML

Ruby: value = data || "默认值"
来源：http://3g.zdbjq.cn/Article/details/gablhdsad.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/grcnwauha.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/ghraqjugc.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/gxifcsmnl.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.hesvh.cn/Article/details/gjfjlnimc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.fehbvm.com/Article/details/gdfsusirv.sHtML

TS:   if (!x) {}
来源：http://mobile.fehbvm.com/Article/details/gpdxfszme.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/grkjvsoqh.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://read.share.fehbvm.com/Article/details/gbqaukatu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.hesvh.cn/Article/details/gkkffhvtt.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fehbvm.com/Article/details/glayfztwf.sHtML

[A17] 位运算
来源：http://read.share.hesvh.cn/Article/details/gwjqooety.sHtML


<!-- 参考信息 -->