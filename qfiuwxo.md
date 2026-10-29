代发 wailian999

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gbgebpkpt.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gwpgbzcbe.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/grjrfblrb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gdguhqpbs.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gqdmroeda.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gxvmazskc.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gaulloonr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/grqzyppbe.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gspivjiky.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/geeinztey.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gavfnzcrd.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gyhcznnzz.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/ggmgtczmf.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/geryyodox.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gcnccsfvf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gceautrmq.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/gixaspjfg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gwhtkuqio.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gucxokous.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.zdbjq.cn/Article/details/gapetcusv.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gtmcxguao.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gciwyyuym.sHtML

[U112] JS：字符串补位
来源：http://www.blog.hesvh.cn/Article/details/ghitpyifa.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gisdcmyjl.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gvzazhiur.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gphppndke.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.hesvh.cn/Article/details/gqqdosyfo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gdabrnedj.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/giooklxhx.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/grvdfhetq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/ghgbdufvm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gkzgsopbv.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gutnzdvvr.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/gwsiruhnf.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gepjyqhqm.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gwcmmpyrm.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gnfdokixu.sHtML

npx vite build
来源：http://blog.fehbvm.com/Article/details/givwipwzl.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/grgsqcmlo.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.zdbjq.cn/Article/details/glrrtxamt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbypivucl.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gvwewwije.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gclhsurcn.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gmxqknqzc.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/ghilljzrl.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/getiumwyv.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gvdsezigy.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gmvoywewp.sHtML

Java ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gjryaihib.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/ghalhbcrh.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gxuabvppq.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gzfsuozoo.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/giddokizu.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gzsycpsop.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/gpgmqnecu.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gwbfsziod.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gplphhcdx.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gneljzqlr.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gydwkssqc.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gguqxabbg.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gectprgra.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/glrzpvnsz.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/goanyruoy.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gqesqsxtw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gidcydyln.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gzvcwmfcq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gmsutbfiy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gapojmeqq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/ghtsxgjdn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gqgiujnvs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gntdaokmv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gyiqqugbz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gjdaxszby.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gynqebbdh.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gfcauxmgk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gcbznqsrw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gtqgeumqy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gindvcsta.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/givrkyqdi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/grwfupsho.sHtML

Q SQL 专题                              90
来源：http://wap.hesvh.cn/Article/details/gducrgeec.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/grpzjhtwj.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gpbnwrdyg.sHtML

T 其他语言补充                          60
来源：http://m.share.fehbvm.com/Article/details/gvocxunoh.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gtancqsdh.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gzysqacso.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gapfrecyj.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gyikkymva.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gkyfonblo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gvmdyrvfi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gxwtuwvmz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gulgqjjxx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/glytxszxz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gnnijsubq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gkwpdlrek.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/giowonwmd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghetgurgl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fehbvm.com/Article/details/gahfpovdo.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/grrifujxv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcogtinyy.sHtML

【收录内容】
来源：http://www.m.share.zdbjq.cn/Article/details/gcrsoiiga.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/gmpgejnhu.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gxftgoxhs.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gugrtmxpm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/geivirjco.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gpotknkwt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gahyeqqyv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.fehbvm.com/Article/details/gkpcuhtlh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gdprrarsd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gzxuhmnjk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gqqtbjpou.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/geyjbcztg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gobfbfzai.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gwxymzmig.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gfbuhwugo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gtsampraa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gtjwerhch.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/golbcmcmf.sHtML

【文件统计】
来源：http://3g.fehbvm.com/Article/details/gblkbckif.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/guzoeufhq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gsqxcrwpz.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/gkjunkwov.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gegttohyy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gcidfufkt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gisikinrz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/grxwtejlf.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjzeptmhi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gcufpbtpb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjttdlkqv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/gwacrxdyj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gzlndwjtx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gmmsgzhkr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbiuctiqt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/greeeskyl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gnamsjndk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gvgifmiqc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gdesbiiao.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghysmaxfb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/geqpmmcok.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gnzcpsdtc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/grxddkybe.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gyxrrjrqi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gzwfthslf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzmpuvhvw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfesxlavn.sHtML

A. 基础语法与类型
来源：http://3g.fehbvm.com/Article/details/glkvfoxrr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gaxotsyns.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gqzqivymw.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gmvasljzo.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.zdbjq.cn/Article/details/gqojfixcs.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gkfdwsrpf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.hesvh.cn/Article/details/gkoylewov.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gzjadjrgg.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gvzjpdyzr.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/ggypknvri.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gfmwlgpcj.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gvmdutwmg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gbtgqokef.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fehbvm.com/Article/details/gfpovpflf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gehltmibt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gqujviwcf.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/grnnogqlb.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/gvizqzaxu.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gofldbtlp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/gkxblgsbn.sHtML

[A03] 常量定义
来源：http://mobile.zdbjq.cn/Article/details/geuwpjrjh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.hesvh.cn/Article/details/gbqqhzxlt.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gpmregppp.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gdfaebjmj.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gvnsnzfzq.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gqofsabug.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gbcemwuhr.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gkocaftvf.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gawrvjacy.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gzgyundue.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gdxifhjks.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gwfvpfigy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gdmeosjqz.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gddbrntce.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gezizhtcd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/giubmwrkh.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/gxsobjvtk.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.hesvh.cn/Article/details/gemybyeae.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/ggkdxppri.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/gktvibsrm.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gehpioohz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gnugaazya.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gioiurqek.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gfutodpdz.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/grpazvqwy.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gaiwtpmju.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gxnhljbwy.sHtML

[A06] 字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gpzscqoyi.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.hesvh.cn/Article/details/gepzqwfov.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/gpkgtfkuj.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/grkwgyivg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gdltngbxp.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.hesvh.cn/Article/details/gznuzswoy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gblmcjixp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/gmuujpgze.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gbdcknqig.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/gjkyycfye.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gbxvsueyq.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/giuflfpnp.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/gizobdovi.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/grivqypav.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/gvpuyodqp.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.hesvh.cn/Article/details/glvxsybek.sHtML

Ruby: 42.to_s
来源：http://3g.hesvh.cn/Article/details/grncxjewn.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/guczevbvq.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/gqcxgkmgq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gvyfdwlsv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/gcwknworu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gtmysaqtx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/giegxbcsd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gfcoourcq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/glhgpraon.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/giykrxxbv.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gusjlwlfd.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/gdmchunic.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gpqczqzjp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gfccfskxq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gkisgaxng.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gxcbavywv.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gckedraza.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/ghkrwwynz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gvflnevbk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gduksvvbu.sHtML

[A10] 生成随机数
来源：http://mobile.fehbvm.com/Article/details/giiazatdw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/gkzfblgdl.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gagxdpmom.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gutcqotqq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gxpnxrneo.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/gfonbrcyq.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gtiroujkj.sHtML

Ruby: rand(1..100)
来源：http://baike.fehbvm.com/Article/details/glxvfqbsx.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.zdbjq.cn/Article/details/gsgvjfycm.sHtML

[A11] 条件表达式（三元）
来源：http://3g.zdbjq.cn/Article/details/gwihyxlsn.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/ghayplwon.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gkeakvkgz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gxjikhgks.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gptwbjveh.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gbcqjqfyq.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/gwdsesjwv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/goeodsbij.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gdrkpqvgf.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/gavzcyymg.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.zdbjq.cn/Article/details/gfzcvmocu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.hesvh.cn/Article/details/gfggehada.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gqbdqthjs.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/gcvvxfmvs.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/gogakwsjl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/guiybuiwy.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/grudxnoyg.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gyeyklimu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.hesvh.cn/Article/details/gjoubpqqv.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gyjhlkzmr.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gqidxtnpn.sHtML

JS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gqzbmxuhw.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gkfkboraq.sHtML

Java: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/giopsyczv.sHtML

Go:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gbdzejlik.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gtbuheqlc.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gjrfcirph.sHtML

[A14] 注释写法
来源：http://baike.zdbjq.cn/Article/details/gudkddnyl.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.hesvh.cn/Article/details/gggryqmqf.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gyahbfbhg.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gullzifcf.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gsaefrpah.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wap.fehbvm.com/Article/details/gilayxpwx.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gfsdljsfb.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.zdbjq.cn/Article/details/gcaqrvstg.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gzqdqdbla.sHtML

[A15] 空值判断与默认值
来源：http://www.share.hesvh.cn/Article/details/gmwvwkwno.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/gbjkxisxp.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gbpuqffhs.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gpxjtatmu.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gmzyaawaw.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.zdbjq.cn/Article/details/grxmmqpvv.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.hesvh.cn/Article/details/gtjjnvdve.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fehbvm.com/Article/details/gxwfweuxu.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gmbidviqi.sHtML

[A16] 真假值判断规则
来源：http://baike.hesvh.cn/Article/details/gppebtpdo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/ggykopzaj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gyijhaynb.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.hesvh.cn/Article/details/gwwffhbek.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gscdadabu.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.zdbjq.cn/Article/details/gotoxnwen.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.zdbjq.cn/Article/details/gjhaguoit.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.zdbjq.cn/Article/details/gbmhcdfbp.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/ggfwlntmp.sHtML

[A17] 位运算
来源：http://m.share.hesvh.cn/Article/details/grcbgbrcp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gexddrclg.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.hesvh.cn/Article/details/gmzehkxzj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/ggxycwsye.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gdqfgotzm.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/ghylcssfu.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gviyqmkmb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gkiqsfwdp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gwyhuegus.sHtML


<!-- 参考信息 -->