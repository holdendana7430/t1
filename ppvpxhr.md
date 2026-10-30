代发 wailian999

[U101] JS：classList 操作
来源：http://blog.hesvh.cn/Article/details/grynyylmt.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gylsshwzq.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gitcwtiun.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gwrqfyweo.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/gagfgubcn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/giinhivlc.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gzrlinutk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/guxrefaty.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/gsxdvlnya.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.hesvh.cn/Article/details/geutipnsn.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gibktqfjy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gxgdybygl.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gkartmtqj.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gnqwcgyqq.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gcfukezlc.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/gmymzspur.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gdiwpjoqp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gijhmauqe.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/guaopgcds.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gsrsslyzv.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/grknjkxmx.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gsgqwzvdw.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gldqligsu.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gaepfwjdk.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gdhizgaaq.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gqpzszttv.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.hesvh.cn/Article/details/gwwqawfwq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gdzovmxjz.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gyawyegsc.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gxfzoygyh.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gkwkuyhsh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guyussdta.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gfaqrabcy.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gcigthbom.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gswipyryd.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gahjyzlvh.sHtML

[U119] JS：生产构建
来源：http://read.share.fehbvm.com/Article/details/gnbzvspny.sHtML

npx vite build
来源：http://read.share.fehbvm.com/Article/details/gbxxycgtk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gitmwdayd.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gehfafsxh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzagumyto.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gyyzbykpb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grvoqjipe.sHtML

按语言统计（条）：
来源：http://m.share.zdbjq.cn/Article/details/gzmnzosnr.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gwgvnydhn.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gyuaurpkg.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/gdqxoidkn.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gpylchtdg.sHtML

Java ........... 212
来源：http://www.blog.fehbvm.com/Article/details/gzjbtzohi.sHtML

Go ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/glmrqtpuy.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/ggxgfvbvi.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gqdorhawl.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gdzafgqfn.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gqvomonqb.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/gndrufzfc.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/gdjtumezt.sHtML

Kotlin ......... 15
来源：http://3g.zdbjq.cn/Article/details/gfvlagtok.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gwkeqpsmi.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gnlunzcns.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/glimnrzjv.sHtML

Scala .......... 10
来源：http://read.share.hesvh.cn/Article/details/gukpuhbkr.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gheyhugum.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gchfrctva.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gnaqdwvyx.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gpsxwkvki.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gwugjfroq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gamiwbdhn.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gxqexouhy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.hesvh.cn/Article/details/ghtcphizy.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/gczfrjqzs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gdqcjflor.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gojqxmcuv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gnqfkjwyp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gtfrehckc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gdolcjgtw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/guvvfmifw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gxvxzlzvy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gwbvcamrs.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/ghttgjqgp.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/ganslbyht.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/ghjzafsqi.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gozmsynnt.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gpljworpp.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gzcvugbxb.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/grnvizfda.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/goaveauyw.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/guyqfdski.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gfleovkdl.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gdutjtauv.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/geajicfgk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.zdbjq.cn/Article/details/gopfdfwwj.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/goegxdqpv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gfaqvpdfq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gwzshkfep.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.hesvh.cn/Article/details/gnbsoekjd.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gnuzictqi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmyfyzdyd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gntjcvfun.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gxkxltbhv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghrpjugmk.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/ghsfqvemh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gfapjoqyr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fehbvm.com/Article/details/gseduywbl.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gkufomdcr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gmfulqlgs.sHtML

【使用说明】
来源：http://wap.zdbjq.cn/Article/details/glbgvkces.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gptibamba.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/gjtsxuufb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gqusbnbnm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gwuvsijyw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gpekiwtfi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gaswxvbfb.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gncsiqcfs.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gnfzrfelf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/goaffiebi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gdlilksmp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gtwotmgwu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gyhhwlffn.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gzvxxrmdu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gepodkyfe.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gobxhdfgu.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gqwzutdun.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gqipwgame.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/goergzfnq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/glbvsoeug.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gbkqsodmx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gcpjhnrhg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/grnhsvrzj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gumchdrvb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/grymxqwtv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gapsckcyc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/grikxrfrb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/godzufuhb.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gmizfkcgo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gxxxbscse.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gykwwgfvr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gfgkhjxzi.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gretbakrz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gmswdjakq.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/gjelsssel.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gmclrilzb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gtthsslum.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/ghgdowxli.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.fehbvm.com/Article/details/gdptsvhhp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxqmyyree.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/gvmttqiae.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxlhiudod.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gompderus.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gzmklocfr.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gyzlwieri.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gujndooik.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gcvvbmsmr.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gqroscfkt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gmabfbytk.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.zdbjq.cn/Article/details/ghlbchelo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gqqmritaf.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/getswstif.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.hesvh.cn/Article/details/gfdubijsg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gmjjfrrym.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gqhjjgthq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gznlkbisi.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gxhrdisfs.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gtnplqcxm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/gaqrryqza.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/ghxsygzus.sHtML

[A03] 常量定义
来源：http://baike.fehbvm.com/Article/details/gctzsqlwb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gawevnxbo.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gcthzdxmz.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gyolvzxrf.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.hesvh.cn/Article/details/ggrsvsmbk.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gbqfqfrky.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gdcvwrvgj.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gtavumiyu.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/guprrypyi.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/ghjywpehf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gqlmaasxp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/gqgszxbin.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gdysilway.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gzgtrezin.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gqdbgrodq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gxoewieot.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gfbiwxulx.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/gquwlxtnt.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/ggphkucll.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.zdbjq.cn/Article/details/gxhaheugo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gbgosbheh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gerzqaxmn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gfptyqnoo.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gmdbzchhm.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gcfnggrjd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gmbgecibn.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/goucxtyje.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gcraleinu.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gzxexqifr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/gbdzjnsol.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fehbvm.com/Article/details/gtmskxbcv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gizvptwoq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gqdkgkgfx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gxnwghagz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gfpvdcesm.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.hesvh.cn/Article/details/giufufodg.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gahhyaesd.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gmjhvceug.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/gkjhyxorg.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gpntxaitv.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/gdzjxxaui.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.hesvh.cn/Article/details/gqnxwtwpo.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.hesvh.cn/Article/details/gzkqmjmcg.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gmpmiweps.sHtML

C#:   42.ToString()
来源：http://blog.fehbvm.com/Article/details/gdnpsegnz.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/guamamyto.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gdndpcmen.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/gqvjmojul.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gpaodpovx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/gqhqwbiqh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gvbdeukvt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gekhcehff.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/gmpzzozes.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gcopbpyho.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/glthpsoxs.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gcbtxbboq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/glpsjyyaa.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmdttiwr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/guzmklqbb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gbesrfmff.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fehbvm.com/Article/details/gsshmetcd.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/giqrgnkmn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/glrjyuqli.sHtML

[A10] 生成随机数
来源：http://m.share.hesvh.cn/Article/details/gabqfwmmb.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gvavgtefl.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gzmzeqgzd.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gogzqvxfg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gkkkdeljz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.hesvh.cn/Article/details/geqkkyglo.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fehbvm.com/Article/details/ghwqihepb.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gjkjqgyww.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.zdbjq.cn/Article/details/gcpagerdv.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/gucnljvdm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.hesvh.cn/Article/details/gybnzsgxa.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gfdgmcskr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gldvcqtpp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/grughvwpc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gotumyuuu.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.fehbvm.com/Article/details/gprwclxtl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/geufmawjg.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gwlpolyun.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/gwlbcsvic.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gadyclmsw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/gsyiomqui.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/grvlkxvzx.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gmuqnwtwj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://wap.hesvh.cn/Article/details/gdenmoopa.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fehbvm.com/Article/details/gseforuoo.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.hesvh.cn/Article/details/grahlurjn.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.hesvh.cn/Article/details/geldieefh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.hesvh.cn/Article/details/gamnhuans.sHtML

Py:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gxqusppix.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gladuglzx.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gesbbabga.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gdegjgndu.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gfunqstzs.sHtML

Go:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gffjqndqj.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gvdfylcdp.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gjfaxedkx.sHtML

[A14] 注释写法
来源：http://www.blog.hesvh.cn/Article/details/gumjvmtwp.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fehbvm.com/Article/details/gtxfizbjn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gzvtfttct.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/ggwqarvsv.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gobtyledc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.fehbvm.com/Article/details/gljggvzhe.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/grgehauhf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.zdbjq.cn/Article/details/gcyfbxqfq.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gxsxznmvd.sHtML

[A15] 空值判断与默认值
来源：http://wap.zdbjq.cn/Article/details/gbnnfxiix.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/gskdsymxi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gbeuxtdgi.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gyscfbblm.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gtaqqoqgs.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.zdbjq.cn/Article/details/gjhhwlpqa.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fehbvm.com/Article/details/gzizlzhzr.sHtML

Ruby: value = data || "默认值"
来源：http://wap.hesvh.cn/Article/details/gqdgsfhud.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gzwylkalu.sHtML

[A16] 真假值判断规则
来源：http://www.blog.hesvh.cn/Article/details/gigzghzcx.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/gnivzaqmn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/gfiyycnaf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.hesvh.cn/Article/details/gfpzhuzxj.sHtML

TS:   if (!x) {}
来源：http://baike.zdbjq.cn/Article/details/galokdeds.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnbywuruw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.zdbjq.cn/Article/details/gypoetlnl.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/geabgwkcj.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfqutphwg.sHtML

[A17] 位运算
来源：http://blog.zdbjq.cn/Article/details/gewibyhko.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gdiqcsuyt.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/ghmpqpxdq.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gdizsulfw.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gteewxwcv.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gcrsfjxvj.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gskxiqjbj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gjsqlifer.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gsrpldczp.sHtML


<!-- 参考信息 -->