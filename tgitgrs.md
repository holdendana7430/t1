代发 wailian999

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gmdqxwhnr.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/glwxxcibw.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/golkiqoqy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.fehbvm.com/Article/details/guwctidki.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/grrrgrabj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gkrkvkwho.sHtML

[U104] JS：防抖
来源：http://3g.fehbvm.com/Article/details/gjrqckxfj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/glbvcudjq.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gxilgckcs.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.fehbvm.com/Article/details/gqfbhuhpk.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gjuojkdhd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.zdbjq.cn/Article/details/gfbacajzi.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gwgqhvqgf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gwspedthr.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gnrkdftar.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/gyhreddzy.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gypwusrub.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gihkjfjoz.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gpmruzknl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gkneclkdb.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/gilofnlsf.sHtML

new Map(Object.entries(obj))
来源：http://wap.hesvh.cn/Article/details/gtqzubgad.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/glkaypnph.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gghelhrmd.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gqwlpeaih.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gymgpxakh.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gymytwavt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gaholcyqp.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gxlanjlyt.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gffgxxnmi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/gfohgygfh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gtlgpvbcf.sHtML

[U117] JS：单元测试
来源：http://blog.hesvh.cn/Article/details/gbmzeckbw.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gdkllnkiy.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gphokhqwl.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fehbvm.com/Article/details/gdkfsifyp.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gcewtqwck.sHtML

npx vite build
来源：http://read.share.zdbjq.cn/Article/details/gudcqlxuq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gprpxhuob.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gsvabrqms.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxisdeqyb.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gxveptfkb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcyredxau.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gfbpjejll.sHtML

Python ......... 252
来源：http://m.share.fehbvm.com/Article/details/gmbjlchix.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gvlcbofmz.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gcdxcfzuh.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gushpmlfh.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/godohnfom.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gixmysbdy.sHtML

Ruby ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gqgyhpkvw.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/glcjiqgwj.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/gcostsaud.sHtML

C++ ............ 30
来源：http://3g.fehbvm.com/Article/details/ghbugpkue.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gryqdxldx.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gxonrzpsu.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gffunalyv.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gyushxvkp.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gqtvlpcsj.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gmjnwpiww.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gwvicibum.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gwualoazg.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gkzmojlfg.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gamenuazd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gdhhjwzdh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gufvqoynr.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gpygxxokt.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gcvrsplem.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gyiyeqqww.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/geuzvggfv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/giujvwkkc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gibsispji.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gqmjznlzi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gvawjdamn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/grganzqhy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gisdoqyni.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ggbqjqxjk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gkukghbeq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gqtlaalyz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gqsrpeesw.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gtdznoauq.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gvtjlyqct.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gdmjbpibj.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gwaakamxk.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gkfkbzcae.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gacjdrxwh.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gajcdvqhh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gjkjfmgpx.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/ghteitoys.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gwadomczm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gwprsrrnz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gtmbshowk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/ghpudafuz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/gdglozzed.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gczznepfj.sHtML

—— 文件结束 ——
来源：http://baike.fehbvm.com/Article/details/gilzxslyu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdkxdfnyx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gnrtjaasc.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gtlxozaot.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glgpyiqia.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/giqnjocux.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gyekwgqow.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gtrdxfgsb.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gsrashuza.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fehbvm.com/Article/details/gvhfvmymm.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gqllahaiy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gaiavmlvr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gjycxyleg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/gfgurlpec.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gfxrpwkza.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/gzgtalxdd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/gtewyhcdv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gnrtqyvuy.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/gmcdcazba.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/guqpriikc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gpoilcsmb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gqernglju.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/gaqwsmmrq.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gqwzochlm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gujbbddoc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gceanxpuf.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gweuxjiwp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gpqbvagog.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gnnlcuqtj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gqdlnefnj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gkmglwxev.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gopkrubfj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.zdbjq.cn/Article/details/glsdducoz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gtvwshivd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/gcdsbkdye.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/ggxfntztq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gvwsagdxe.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gsjtkexkk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gpouwijzs.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gdieybgcg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gfwgkfqut.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gbmrsroio.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/ggszvaiwi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gssplsvmo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/gnzmzgxve.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/ggnqiwllk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/gdamtpenm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gkwfcpzac.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gbzldluyo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzswzfpmc.sHtML

A. 基础语法与类型
来源：http://mobile.fehbvm.com/Article/details/gqgiytjom.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxuawsvbq.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gdeodzoqm.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gnnqilqiq.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gozkjhcoq.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gkhhblbhh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gbeasrtwg.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gptykrfeh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gcwsucsbh.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gdqgmhdxv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gdixqugjl.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gurvazwvu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gfrihtfga.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.hesvh.cn/Article/details/gazjlvdlm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gsxkwnofd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.hesvh.cn/Article/details/gxswcyqjr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/guvmsktdh.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.zdbjq.cn/Article/details/gihudsomg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/giijuweml.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gzutllyvs.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gjcnqoqle.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gtkqhvrgw.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gfuvksvil.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gtwfkawfg.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gihtkcbna.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gmjjoibhg.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gaemswxbf.sHtML

Ruby: PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gvysulaco.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/ghaxokpbp.sHtML

[A04] 判断变量类型
来源：http://mobile.hesvh.cn/Article/details/gnpfmcabq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.hesvh.cn/Article/details/glgdezimn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gyohhydaw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gdilzybiz.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gjssturim.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.fehbvm.com/Article/details/geadnxcyg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.hesvh.cn/Article/details/gmfcpbbsm.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.hesvh.cn/Article/details/gzhdrwypk.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fehbvm.com/Article/details/gajmytpaq.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/glbafnsjx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/gmzknogqu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/grwprqvoj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gukcqzkuo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gkfnhnuvx.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gqydqhwvi.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/guarpcnbm.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gzlihszbs.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gdmfijiax.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/guankdwfm.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gpciopono.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.zdbjq.cn/Article/details/gydjnixio.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/ghsjwxjwb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gnrtpdleb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gftzknwsp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/gxgmsbnxe.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/gcayvyxfr.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gnwgjoila.sHtML

[A07] 数字转字符串
来源：http://blog.fehbvm.com/Article/details/gtbbtvhfs.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/glxtepymy.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/geywjtpzc.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fehbvm.com/Article/details/girucknxc.sHtML

TS:   String(42)
来源：http://www.share.fehbvm.com/Article/details/guycgehdg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gzrmcupwz.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.hesvh.cn/Article/details/gdhrabrxs.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/gfdbdyvjx.sHtML

C#:   42.ToString()
来源：http://www.share.zdbjq.cn/Article/details/gcbyhhhnm.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/grwvbaprj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/ghzdijscs.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.zdbjq.cn/Article/details/gnjizxfhp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gqopmawam.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.hesvh.cn/Article/details/gxvpyspfc.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gqzjlkycu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gugfvlvkc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/gbsdsfnrf.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gxxpswxwo.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/gxhlbwqty.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gqvlwasah.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gdaetopij.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/glkyydntq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/guholtalk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gdtxtastr.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.hesvh.cn/Article/details/gorcaiifx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.zdbjq.cn/Article/details/gafadyqwo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/ggfayrrij.sHtML

[A10] 生成随机数
来源：http://blog.hesvh.cn/Article/details/gnwidvwej.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fehbvm.com/Article/details/gpgumyfah.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gbwyzyvam.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gfdthohwi.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gvhfubdhs.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fehbvm.com/Article/details/gyfucqqjp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.zdbjq.cn/Article/details/gmxwjyeap.sHtML

Ruby: rand(1..100)
来源：http://www.blog.fehbvm.com/Article/details/gilzrbmud.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.fehbvm.com/Article/details/gaatjfouh.sHtML

[A11] 条件表达式（三元）
来源：http://wap.zdbjq.cn/Article/details/gykpugiyl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.zdbjq.cn/Article/details/gjburhjae.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gqzcfmbuz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gisyqouev.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gkdiohfqp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gkoxfiusg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.zdbjq.cn/Article/details/gqmadrhce.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gzbeaqgda.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gfshnbknp.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.zdbjq.cn/Article/details/gmgyopkpc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gaozozfqi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.hesvh.cn/Article/details/gfqsxvbns.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gdjakyrgk.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gkbdvyqap.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/gsqueoeiw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gnkrcbmhs.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.hesvh.cn/Article/details/gbxfnsnvh.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/gofesamag.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/gvodtbskz.sHtML

Py:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/ganvmxmds.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gichwqefy.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gbgrrwptg.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gepefretw.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gefpbflgu.sHtML

Go:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gsoohxwmv.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/glwnevxjb.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/grvqgyzgf.sHtML

[A14] 注释写法
来源：http://blog.zdbjq.cn/Article/details/gcmlfbrct.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.fehbvm.com/Article/details/gmboylymx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gdzrwcqsk.sHtML

JS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/ghuedisqr.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gcoypbwaj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.fehbvm.com/Article/details/gdqjanide.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gfzmsmovw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/gfjksafai.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gddeekqhl.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fehbvm.com/Article/details/gqazizufh.sHtML

Py:   value = data or "默认值"
来源：http://3g.hesvh.cn/Article/details/ggbpjnrah.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gjtcoiskh.sHtML

JS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gvoricoyh.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gpjwfefid.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/gagwsdnmo.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fehbvm.com/Article/details/gwmduyiwq.sHtML

Ruby: value = data || "默认值"
来源：http://blog.fehbvm.com/Article/details/grimlnnjw.sHtML

C#:   var value = data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gowwazzaj.sHtML

[A16] 真假值判断规则
来源：http://3g.zdbjq.cn/Article/details/guktwozno.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.hesvh.cn/Article/details/ggukjkpfr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fehbvm.com/Article/details/gjyrsscai.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/gukkagzqi.sHtML

TS:   if (!x) {}
来源：http://mobile.hesvh.cn/Article/details/gntfpkqie.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.zdbjq.cn/Article/details/gcxoounok.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fehbvm.com/Article/details/ghrafqimo.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.hesvh.cn/Article/details/gbdbmjxcn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fehbvm.com/Article/details/gdorkrrky.sHtML

[A17] 位运算
来源：http://www.share.zdbjq.cn/Article/details/gcdbtsklv.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gvnfzgehm.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fehbvm.com/Article/details/gsigpdxem.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gqlqdjzxz.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gcanalvrd.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gqeltkvek.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gzuftkwdz.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gggtkdgao.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gpyxmpnxy.sHtML


<!-- 参考信息 -->