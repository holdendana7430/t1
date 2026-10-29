代发 wailian999

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gghchugfp.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/guadcozae.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gunlodzaq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gjhrbggay.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/gjqtscity.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/ghplbctjq.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gedbjidez.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gavtorrbi.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gnidrupja.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gggidfsgm.sHtML

[U106] JS：日期格式化
来源：http://blog.zdbjq.cn/Article/details/giwqvcnvt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.hesvh.cn/Article/details/gwmjtpxbp.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gohsytgti.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gobnwotya.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gggxhugqo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/gucnsbirx.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/gkanvbzqp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gcivwaztf.sHtML

[U110] JS：数组分块
来源：http://wap.hesvh.cn/Article/details/gbeprnrqu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gjzglpvsw.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gezeypdgc.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gznybvhve.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/ghxpeyzct.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ggptriygh.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gauhpscxf.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gsevczngc.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gomchnnje.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gntfnoiuu.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gqsnxoukr.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gzztvvhoi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gmnfuymke.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gfnfccgvn.sHtML

[U117] JS：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gsewxipml.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gcfuutsfc.sHtML

[U118] JS：开发服务器
来源：http://m.share.fehbvm.com/Article/details/gwdhajlgy.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/ggykknrvn.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gqphlmsug.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/grsbiqmuh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/gfinkxbwf.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/grghgeolj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gokzypztc.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gqwvjpvqa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggtchrvee.sHtML

按语言统计（条）：
来源：http://m.share.fehbvm.com/Article/details/gbxuurazx.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gsjumfnpv.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gbqzxnezs.sHtML

JavaScript ..... 252
来源：http://www.blog.hesvh.cn/Article/details/ggkrazhei.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gfpgprqhm.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/glmcwfqpe.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gytjyshsd.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gdzkpazio.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gjsoivzwt.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/ghcnbdquy.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gntphmssw.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gprphnubh.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gibuvdirw.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gwyxauqrt.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gdxpzluqo.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gsygfqzcy.sHtML

Perl ........... 10
来源：http://wap.hesvh.cn/Article/details/gztyzdyvt.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/gfbjlnsfx.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gxpkkuelr.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gaybtrxim.sHtML

按章节统计：
来源：http://www.m.share.hesvh.cn/Article/details/gtzyevokq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gmyjvksog.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gnnsbzvyp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gewujdoln.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gmizpsrgu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gvbnmfxbs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gauoecusr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gihfyyihm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gohxayyxg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gauafjmbh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gsjnulaff.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gvkfwyasj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gwzdrvkim.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gdqwqcprd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gtwvjlbtq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gpwkpleaq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gpeyynjbt.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gwrpcgaev.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gfgwlflfq.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gwpyyezjp.sHtML

T 其他语言补充                          60
来源：http://blog.hesvh.cn/Article/details/gpeceoufa.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gnjohrqna.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gozdxjumm.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/gndgqvnir.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gmbebpvvf.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/guvhnvpvm.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gqcvhzrpa.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gmwrjvpue.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gjfvgbwiu.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gugywbbgu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gcpoyulph.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gnqhtufnb.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gygckenxk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqxalkdbb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/guznpjlae.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gylysaxsb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gqansevdf.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/guyqclbfj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gcdfjethc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gcjgqhehr.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/glbkazgpu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gobhwkyle.sHtML

【使用说明】
来源：http://www.share.hesvh.cn/Article/details/gzekfooum.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gndzkrmug.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gqlvdynhr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/geoeiuevl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/gvfowxlbo.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gxzqzbszx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gvkulfvev.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gkjqwejqx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/gyyywhigw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/gdrqcssgl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gzarhshba.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gevahvdjd.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/glryvisga.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gniextana.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fehbvm.com/Article/details/gycrinmvu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gmxeedgyn.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/ghkzyoebh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/grgqmixdh.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/glgurtcgv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gymgbrefz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gpzurbbia.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/grbmvqhqs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/ggsjgvmia.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/grxhtqqow.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gqsdqkvif.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.fehbvm.com/Article/details/giapjpblf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gltdxwdco.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gjpvcowbe.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gomfnndrs.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/ghykczamf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gwbmndvnp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gatxuchcg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmstwdvbp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/glwrcanhv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwfghhwfz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gosffupnu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gpcxmunkw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gouaxhptn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.zdbjq.cn/Article/details/grluvwwtr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyamqlzjk.sHtML

A. 基础语法与类型
来源：http://www.blog.hesvh.cn/Article/details/guwcghdlo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaubzopmw.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gibdjvbzn.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gxklnmerj.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gnvwtuyif.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gshikfets.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gxsfmiauf.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gmfdhnfbf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gbmupbysp.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/gcbyjhhqr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gbjpxqcoh.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.fehbvm.com/Article/details/gecbfqfyd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/grcmmtigm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gzdfeutrs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fehbvm.com/Article/details/gjutauagl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gluggsnvs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gxysqjlhy.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/goxvfvwjo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gkuvxyocm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gvqnlzjnk.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gwvurkeic.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gkrgluotx.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/goqjrkvxp.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gouystxps.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gczyuljsy.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gnuuvwvvf.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gaytaswuh.sHtML

Ruby: PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gdknmuvxy.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gjmsfwvus.sHtML

[A04] 判断变量类型
来源：http://3g.hesvh.cn/Article/details/gbsudpqvd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gatyntwyy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/goeopmvqh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gpybhlfkr.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gccsledyu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.hesvh.cn/Article/details/gtgsmtsqz.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.fehbvm.com/Article/details/ggargsxle.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gixfjfsbg.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.zdbjq.cn/Article/details/gfcqkskwt.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gwgcntuvn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gihfeomza.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gkmvnqyyl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gkvlgyjhl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gwokmuszw.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/giuaeioar.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gjeaopoyh.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gowhzohdy.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gmnsodlhx.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gzbzsssks.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gtzgblrjo.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/genqdared.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/ggfjiomci.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fehbvm.com/Article/details/ggtqypngt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gwfphacpj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gphcgvisa.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gaqgtfxpo.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/gfndehuqr.sHtML

[A07] 数字转字符串
来源：http://read.share.zdbjq.cn/Article/details/glvnpieyy.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/gvjnpgnai.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gvoknqafo.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gnvhpxrag.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gljrzwaam.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gefdaazsz.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gxgusvlha.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/garumszop.sHtML

C#:   42.ToString()
来源：http://baike.fehbvm.com/Article/details/gynpfybyu.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/ghhwmfbtu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gwnfzcdir.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.zdbjq.cn/Article/details/glnqfzrxc.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/guqqgwjaq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/gfgiqyexr.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gxfizjsip.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gudhefjxe.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fehbvm.com/Article/details/gvkwmnalz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gmsapnsfl.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.hesvh.cn/Article/details/gzcraxawk.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gwyurhhud.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gtyzhzywy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gjvkrivap.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gglbhxlug.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gkoryemqx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/gzhpxytqj.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.hesvh.cn/Article/details/gstmgvvev.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gaazyuyxr.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/gvrivcwfh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fehbvm.com/Article/details/gzqdszsiy.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.zdbjq.cn/Article/details/gatrebkup.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/guodthuwl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/ghdmxolyc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.zdbjq.cn/Article/details/gfykeeicb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/gdvgcokvw.sHtML

Ruby: rand(1..100)
来源：http://www.share.zdbjq.cn/Article/details/grutmiawb.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gdxkecpqh.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/gzyjmkiwt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fehbvm.com/Article/details/gslhfbftq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/glsomnsfj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gueuvgfoc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gvdyuzump.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gtinhqjzi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.hesvh.cn/Article/details/gvwlsmggv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gxbujgsin.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/ghgrnxzrc.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/guamrdeto.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.fehbvm.com/Article/details/gabosgtge.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.zdbjq.cn/Article/details/ggrngmzmd.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gjqvrupyu.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/grgbihjbn.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://baike.fehbvm.com/Article/details/gwfhxfcqg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.hesvh.cn/Article/details/gplwtkfwe.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gzegtbrls.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fehbvm.com/Article/details/gbtypbcip.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.fehbvm.com/Article/details/gqyodywnn.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gxpcscvkf.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gyjtchzxa.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gurpwmqav.sHtML

TS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/glvpobudc.sHtML

Java: "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gypufnzzq.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gekxynrxn.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gwgihkpqh.sHtML

C#:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gkygqbpwq.sHtML

[A14] 注释写法
来源：http://3g.hesvh.cn/Article/details/glrxuecny.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gjtkcfnbo.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gggupoylq.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gffroxlor.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gfoqpeztd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.zdbjq.cn/Article/details/gnnczmlmv.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gpycnvyqy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.zdbjq.cn/Article/details/gbyfvqofw.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/giotnwthl.sHtML

[A15] 空值判断与默认值
来源：http://mobile.hesvh.cn/Article/details/gjkyvmdci.sHtML

Py:   value = data or "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gpazjfgaz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gshdnncbo.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gcqnbpkul.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gjymglgdj.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.fehbvm.com/Article/details/gnvmsntgy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.zdbjq.cn/Article/details/gnocweurr.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fehbvm.com/Article/details/gwdjkubtl.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gtvgrvfou.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.hesvh.cn/Article/details/gxhcpfcha.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.zdbjq.cn/Article/details/gnlnkusml.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.zdbjq.cn/Article/details/gkplaolvn.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.zdbjq.cn/Article/details/gdlnzzptu.sHtML

TS:   if (!x) {}
来源：http://baike.fehbvm.com/Article/details/gtoaojtva.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.zdbjq.cn/Article/details/gzsczvdfi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.fehbvm.com/Article/details/giiqalsxf.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.hesvh.cn/Article/details/gwuncvgoy.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.hesvh.cn/Article/details/gyoyayntl.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/guvzermvw.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/geylatnry.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://3g.hesvh.cn/Article/details/goveyammi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gdmyejzkw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gtcdurghd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gquxezefn.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gpeprluzc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gibukyvsc.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gjkbxgrzv.sHtML


<!-- 参考信息 -->