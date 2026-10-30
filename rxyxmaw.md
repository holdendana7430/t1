代发 wailian999

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/grpcproqs.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gtijpysui.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/ggogpmnpe.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gyyeztbwl.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gdrwtmfam.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gcisfduvv.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gilrmwcqu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gvsalofgc.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gdjmwkykm.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gylksdruf.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gyrkpetyz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gksnrroqa.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gpgrgkwwa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gtkgxbbmn.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gwehctzsd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gtimssdxe.sHtML

[U109] JS：数组分组
来源：http://mobile.zdbjq.cn/Article/details/gfgwuryfj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gvgubwtff.sHtML

[U110] JS：数组分块
来源：http://m.share.zdbjq.cn/Article/details/grccecrlc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.hesvh.cn/Article/details/gfsfetxuk.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/grsenjkvx.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gkutjruia.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gyxlxvibn.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/geaopkwdu.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/guwniqdnv.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gozipyzqd.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gygbnjyjv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/guljbjfre.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gfyymfzbs.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/grfjpdtfs.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gtzqndabn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gjogjrjia.sHtML

[U117] JS：单元测试
来源：http://wap.fehbvm.com/Article/details/glnhhyuzh.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gaihvlvjs.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gouzedssc.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gkexjqwql.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/glqememjx.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gmpmjzoqb.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gudetqxwl.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gtoadwcyj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvlhozsiw.sHtML

统计汇总
来源：http://wap.fehbvm.com/Article/details/gsdgevtri.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsyziedum.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/ggpmtmbce.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gscqbcqgq.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gmzpokpbx.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/giuabycox.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gjjnpkrpf.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gkuueuheg.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gonuykcqg.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gdtkscxnp.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gabfunbyb.sHtML

C .............. 30
来源：http://blog.zdbjq.cn/Article/details/ggdlcyffu.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gaedqyjsz.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gpcidtqoa.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gzuihnoeq.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gzufpdhtm.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gmpsndpji.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gencyzwry.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gbxarqhsj.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/geizstntv.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gvrfxarhk.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gwfcmtqqj.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gibuxjwoo.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gdbmhaenx.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gzeqqjtsw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gnuxiezhu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gakbllmcv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gijzgdjgd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/gropgsyxf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gzedjsrhj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/gjewusgew.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gqzakjbvp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gyovdjora.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gtyyxtohm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gsmrexrqw.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gstwxqvgi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/ghrqlfebc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gpdcdlncc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gcvctneyf.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/grcwbizvw.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gzyrawvgj.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gscjlcykd.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gycpnxguf.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gngfcgkse.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gricyrmyx.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gpgdxkqiy.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gfbxugwkn.sHtML

使用提醒
来源：http://baike.fehbvm.com/Article/details/gybveugra.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/ghtrhopgo.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/galoodqho.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/ggkdnuvyh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.zdbjq.cn/Article/details/ggzzjlthm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/gumbpiszz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gpodepjxo.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gfpkumfeq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gznalusnu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.zdbjq.cn/Article/details/gpyamxqkf.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gwproylsy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpblqhhcn.sHtML

【收录内容】
来源：http://3g.zdbjq.cn/Article/details/gmwhklbma.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/gwcckzqri.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/grlrrjtdm.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gikghchoy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gqsyefwjw.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gonuuylyg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gibcpomrz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gfstmiykm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gtsqcnezp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gkkgiiqlf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gqommhbjt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gtehoigao.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gmpommbdx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gsymyxnqo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gmuitqlsu.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/gqxeqidfi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/gsrfmdxop.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gwphloije.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gqzyabggs.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gomufjfnj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gjpcosrvb.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/ggveycboh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gcxsasufz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gyayohzvh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gcqwmozlb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gfimwdjah.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmjvbdhlu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/gwlkdsvju.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gxzrlkgkb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gibdagach.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/ggzpfpftp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gwwbdxoif.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/gbviucvby.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gvjndzkax.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/giuiphkoe.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gvjkbsqoj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.hesvh.cn/Article/details/gekpmkuil.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/goirvlkfr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/guuryulxo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gdetnqldu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gtwcxlepp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.zdbjq.cn/Article/details/gglyzytyd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gqpysxzdf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gsidudwin.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glqzcldaz.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gkvgcchuq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnlrvaxwv.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/ggcjipilz.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gijtqexfb.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gbxeofomq.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/goclmnaze.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fehbvm.com/Article/details/gygmcaaet.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gudtfponi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gcflxowce.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fehbvm.com/Article/details/gjflcyucv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gwgfkmrvz.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gmtuhbhht.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/gpqvxktsi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gkabvpilx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gashauqkb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gmnfdsghk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gaglleqcb.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/grbhmzegi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gxmirbkhv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gcbriliox.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gqabbxeqr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gbjcyngva.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gniszdrqx.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gyuduybso.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gnotdkrpr.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gwpbtjtpo.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gvlszwwvl.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gphgwster.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gxpatjghl.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gozjfsufh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gmgbgiccw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gxpathvrs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gibmnqhxd.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gydwedqtq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fehbvm.com/Article/details/gkhwzxilf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gdbznvfht.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.hesvh.cn/Article/details/gzuwkrcwg.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gfasnnlus.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/gfvmncsmr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gicikiuni.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/griolfsds.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gzuuoxqiy.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gvpzpjags.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gmjotvdrk.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/geyfpfyfz.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/ghaatjlde.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gvnhwcuuj.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gdqbvlqcd.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gzeleigny.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/gsksrmefi.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/ggszvbatd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.hesvh.cn/Article/details/gksjopfte.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.hesvh.cn/Article/details/gdwvksker.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.zdbjq.cn/Article/details/gttxnniqd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.zdbjq.cn/Article/details/girkrngfq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gzbhrioyu.sHtML

[A07] 数字转字符串
来源：http://www.share.hesvh.cn/Article/details/gwfghdpen.sHtML

Py:   str(42)
来源：http://www.m.share.fehbvm.com/Article/details/grdppmdsb.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.hesvh.cn/Article/details/gvyimgrov.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gsbmfpcsp.sHtML

TS:   String(42)
来源：http://baike.fehbvm.com/Article/details/gkppqqdqq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.zdbjq.cn/Article/details/ghyjlpzui.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.zdbjq.cn/Article/details/goriboduf.sHtML

Ruby: 42.to_s
来源：http://read.share.fehbvm.com/Article/details/gxerkgwtp.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gqrusficd.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gdzwfwkxk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gfccdmwxe.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.hesvh.cn/Article/details/gihrjezhf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gqnyyjjww.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/gplorgkvq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gqbxnczst.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/ggvmrlcwt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/gdagfhnuy.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gswaggnal.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gtujxnjua.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/ghoadlvdm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gesjcotog.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gjaxxwbao.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gxmszcubl.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/ghbipmrbp.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fehbvm.com/Article/details/gkkhsxhvx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fehbvm.com/Article/details/gvehcygne.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gozqgneky.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/gyaqushci.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.hesvh.cn/Article/details/gtfsanepx.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/gztwoxzho.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gcessluqm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gpeohrqzi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fehbvm.com/Article/details/gbuybberb.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/gjayjiyjn.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/gmsxcgqbi.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gxeuwivwb.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/gmpwnqsme.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fehbvm.com/Article/details/godhqwytj.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/ghirupvvj.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gmeavctfd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gjqkadzjx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gzeecferh.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/gswhttiok.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gfyvkqaak.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gsmncdqpn.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.zdbjq.cn/Article/details/gptwwfpoe.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fehbvm.com/Article/details/gtjbtajrk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.hesvh.cn/Article/details/gfetdxtbw.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gidavhmae.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/giagvpvnq.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.zdbjq.cn/Article/details/gtdqbxmup.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.fehbvm.com/Article/details/gsuvxvnpu.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gryvmgqya.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fehbvm.com/Article/details/ggfiiqmav.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.hesvh.cn/Article/details/glxsdpewz.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gjpvsglra.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/gnaszmkmh.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gkhjvjctu.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gwevozlzq.sHtML

Java: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gbzqzxazs.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gdlczewpo.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gxauvdgzy.sHtML

C#:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gqamielzl.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/gnbuxbjdx.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fehbvm.com/Article/details/grovdyysx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gycgqrrhr.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gntjevuyf.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gjngdelpv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.zdbjq.cn/Article/details/gdgzhbjrg.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gqygwlsiq.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.hesvh.cn/Article/details/gvbjqapwp.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/grqqhfczl.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.zdbjq.cn/Article/details/grtvebhqa.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/ggxgzpilu.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gmgboazdu.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gxbldxadc.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gcuolsnjc.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.hesvh.cn/Article/details/gpirvhyke.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fehbvm.com/Article/details/gpsypnhsf.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.hesvh.cn/Article/details/gnrrwxayc.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gvmvkabut.sHtML

[A16] 真假值判断规则
来源：http://www.share.hesvh.cn/Article/details/gtmnlktmi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.fehbvm.com/Article/details/gmkbxtzjx.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fehbvm.com/Article/details/gyvplquyv.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.zdbjq.cn/Article/details/gqcniwmwr.sHtML

TS:   if (!x) {}
来源：http://wap.fehbvm.com/Article/details/gfhltqjed.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.hesvh.cn/Article/details/gmtrgavta.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fehbvm.com/Article/details/ghjjroqro.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/glsvwdqeh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fehbvm.com/Article/details/gcamyjzgx.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/gzmgnhcrt.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gerwggctz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.hesvh.cn/Article/details/gsmelzxnr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/glpmvwntx.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gbrvdsajj.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gjmaarpnq.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/gpiabunsw.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gfoxcpjpd.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/goufjjxzx.sHtML


<!-- 参考信息 -->