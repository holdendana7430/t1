代发 wailian999

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gbfqokaiz.sHtML

el.classList.toggle("active")
来源：http://mobile.fehbvm.com/Article/details/gzbbuhdjw.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gbrodnorw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gohxuvfrp.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gkyisabah.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/glzcylslk.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gqwiyrnlu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gddlmgogj.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/ghpcmrwiz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gbpitmyld.sHtML

[U106] JS：日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gezfhfvfv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gavgfpycp.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gemvnnzos.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gapsgrbvo.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gzsmbmqnp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gvqbvghxc.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gtwtuglso.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gkphujvkm.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gtphbswol.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gjvpmflpd.sHtML

[U111] JS：对象转 Map
来源：http://m.share.fehbvm.com/Article/details/ggrikwjre.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/ggyotvecy.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gqlgejfqb.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gwuqvphqy.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fehbvm.com/Article/details/gsyfcvnou.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gdbyzjndi.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fehbvm.com/Article/details/gmqisstzr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gnrbvnayh.sHtML

[U115] JS：生成 UUID
来源：http://www.share.hesvh.cn/Article/details/grdipftis.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gzowipzbj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gwrbctehn.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gmdgdsevg.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gzwztwtxo.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gprhwmsdb.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gmduxhrve.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/ghrwwbdiw.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gmdebhmfv.sHtML

npx vite build
来源：http://www.share.hesvh.cn/Article/details/giyixnjnp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gyuovgbzg.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gvdzgmtuy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfymvtugb.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gxmtzkvrz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxzpdptis.sHtML

按语言统计（条）：
来源：http://3g.hesvh.cn/Article/details/gxidmeoqc.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/ggquowcar.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/giculwvrb.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/gxsccvjfv.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gtsqjehpq.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gduhnkoru.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gpwoeqdxj.sHtML

Ruby ........... 212
来源：http://3g.zdbjq.cn/Article/details/gtzpcanta.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/gtuxcymiq.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gzqvsquxk.sHtML

C++ ............ 30
来源：http://blog.zdbjq.cn/Article/details/gqgoftdxq.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gztoiivma.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gqnzyurjd.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gyrhjudmr.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gomarwvsl.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gbehhfojv.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/ghetxzkjo.sHtML

Scala .......... 10
来源：http://wap.hesvh.cn/Article/details/gvcnstdtj.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/grckroegj.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gqvayywmx.sHtML

按章节统计：
来源：http://mobile.hesvh.cn/Article/details/gjoufxufm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gwmwioaev.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gybqpishw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gdbfarwfh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gvalxsjfl.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gsiddbmzz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gsyafljjf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gczhzyzkt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.hesvh.cn/Article/details/ghgjsuiog.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gbzzqdges.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gjwazqbjb.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gffkjslok.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gpbqocubn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gofoxehdf.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/geobmzhde.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gxhgjbrjh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gaagezklx.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/giziiysfz.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gyllhbixh.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gbogafvuf.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/ghtdtwlzr.sHtML

U 高频实用片段                         120
来源：http://3g.zdbjq.cn/Article/details/gmiyljnlw.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gjxngumnp.sHtML

合计                                  2106 条
来源：http://read.share.zdbjq.cn/Article/details/gxresidsm.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gfxkrvxrf.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gagnjgmzq.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gtklczjvq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gdocrwhdc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gipvywtgg.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.fehbvm.com/Article/details/gfhzfgfjq.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gxujxjyeb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/ghcjqxhyc.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/ghvimgvka.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gszqaiisj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gfuiovdoi.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gveaqmcfk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gujvavavj.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/glaembhtm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/gjnkdcvql.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gnsjtgovb.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gbkwdtcth.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gjixtzptd.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gieykkrtj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gddzgolkr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.zdbjq.cn/Article/details/gunbsslxs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.zdbjq.cn/Article/details/gvcllilju.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gwgvjrfzz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/ggpvpqfos.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gthfyimkv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gwlmmpfbn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/giofacjnq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gzqtgmxin.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gdxrzmosm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/gmaizhrdn.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gtwbrxntu.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gmropuwlo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.zdbjq.cn/Article/details/gosyjwmkz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gmzuwqmnc.sHtML

目  录
来源：http://baike.fehbvm.com/Article/details/gsgpkbusw.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gfesppskd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gkltxuitr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gphfegrba.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gfvkkuydt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/glvmynetf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gqntgoigc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gylztogel.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqeyntget.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/ghjudvydd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/galjknusf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gpupxftyt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gqgqrpzyj.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwwtqsuwm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gdvqbibou.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gdozftigq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmcmnznlx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gfonghpvb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gsldeiqfh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.hesvh.cn/Article/details/gjknqyear.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gsigzagml.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.zdbjq.cn/Article/details/glrvhdsxr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gvdbhvnny.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmoxihoiw.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/gcizmcjcm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grdoftefy.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gfkmavauo.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/ggqsxttrt.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gdzjaxxlw.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gwzcwofog.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gpglzimuo.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gfjjzafrv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gsewqddbr.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gbsjyvhqq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gfymrhrwu.sHtML

[A02] 变量声明与赋值
来源：http://wap.hesvh.cn/Article/details/gqgbdhfca.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.hesvh.cn/Article/details/gostzmkrh.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gsadounns.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gzpglomhw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gilmecwzw.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gshbpmpvo.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/gjnidznqi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/ggusolfav.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gkzlcttlm.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gmkfecgbi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/ghrggictw.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gorvcsvtq.sHtML

JS:   const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gbzjbpqmk.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/ggcmxeecz.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gpmitjelf.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gmnadctuh.sHtML

Ruby: PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gmfulajsx.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/glgzkzray.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gftgrwoyv.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gyziavghi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/gzmhbmeyv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gzqaacwfs.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gsqzujmfc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gvxevbfgk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gkbppgmyx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gpzoyazuu.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/gaeixcmnr.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gxsvfalba.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gldknhoey.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gxoqmwplp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gwzppgdig.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/grvmgsjjr.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gzjiqqkwm.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gpvtzwpbo.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gbazyfzok.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gtldoefhb.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gkgjpkjbq.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/gsjcgqfrx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gvanxandd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.fehbvm.com/Article/details/glmkpcvba.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gblvuivon.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fehbvm.com/Article/details/gxztaghjp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.zdbjq.cn/Article/details/gfyrdgkje.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fehbvm.com/Article/details/gzpmiahvg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gfauzkmrx.sHtML

[A07] 数字转字符串
来源：http://m.share.zdbjq.cn/Article/details/gctvrzgzo.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/gfmeuceav.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/gyazdhhgg.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/gebbizoyo.sHtML

TS:   String(42)
来源：http://mobile.fehbvm.com/Article/details/gtxgxeres.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/gbglppvjz.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.zdbjq.cn/Article/details/ghbhevtjo.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/gktfkfmox.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gtptfmtcj.sHtML

[A08] 取整与四舍五入
来源：http://read.share.zdbjq.cn/Article/details/gspcaufqk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gudvjttzi.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fehbvm.com/Article/details/gzjldvsup.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gapxdwbam.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/gdgjifavy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gwgqjjgdb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/grkkwmbwt.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.hesvh.cn/Article/details/gfrsgfcdi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/ggxzyifvq.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/ggbwgaaha.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/ggdeaoepf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gdfoxnqvg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gcqovdbxt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gzuovghqe.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gyeamnfig.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fehbvm.com/Article/details/gtmoczcgz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.zdbjq.cn/Article/details/gucdoicwg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gbrghjxxz.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gvxixrfbn.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.fehbvm.com/Article/details/gzfxvbmsj.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/gkaaxrepu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fehbvm.com/Article/details/ghsrdshov.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gmrgbaeun.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.hesvh.cn/Article/details/guwtatbnj.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/gqamtkbcr.sHtML

Ruby: rand(1..100)
来源：http://www.blog.zdbjq.cn/Article/details/gcypsjeqk.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.hesvh.cn/Article/details/giqshgmdz.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/ggubbubfc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fehbvm.com/Article/details/gftuhbgrw.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gbjzwjwcg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/ghpfmgcgs.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/ggogcrywx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/glgjnjfpw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.zdbjq.cn/Article/details/gjkrvjufs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gjjbnilay.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gjpqilvzc.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.fehbvm.com/Article/details/ghurezpdm.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/gcdiobces.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fehbvm.com/Article/details/gpuovvdwo.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/grfcaidzh.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gpthuufmk.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.hesvh.cn/Article/details/gfucfgahx.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gfsuwinly.sHtML

Ruby: "Hello, #{name}!"
来源：http://read.share.fehbvm.com/Article/details/gadicttge.sHtML

C#:   $"Hello, {name}!"
来源：http://wap.hesvh.cn/Article/details/grmmhijrw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.hesvh.cn/Article/details/ggyrnnuak.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/guvahdmqc.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gwkbfzmwf.sHtML

JS:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/ghgaputnv.sHtML

TS:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gqxnhwzdn.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gqmpsdosu.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gmkzhpvbh.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gzzijihnn.sHtML

C#:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gesugcwip.sHtML

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/geecqysij.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.zdbjq.cn/Article/details/grzeogcmi.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/ggdqogcmb.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/gogysqrcj.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/grdotpewr.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/gnvmrtnbp.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gwbzarrjw.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fehbvm.com/Article/details/gcbgjdkng.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gkfupxyun.sHtML

[A15] 空值判断与默认值
来源：http://blog.hesvh.cn/Article/details/glsxtallx.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gewvndxrw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gyeklvkkr.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gltttsivx.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/gmfaooeoe.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.fehbvm.com/Article/details/ggotpfzfb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.zdbjq.cn/Article/details/gdeqbezia.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.hesvh.cn/Article/details/gisxalslr.sHtML

C#:   var value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gtcygknsg.sHtML

[A16] 真假值判断规则
来源：http://m.share.fehbvm.com/Article/details/gqtvdsrkb.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.hesvh.cn/Article/details/gsrseltym.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/ghqjulupq.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://blog.fehbvm.com/Article/details/guguswrqf.sHtML

TS:   if (!x) {}
来源：http://wap.zdbjq.cn/Article/details/greesoedz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.hesvh.cn/Article/details/gxuclusmo.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fehbvm.com/Article/details/gojopvxji.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://blog.hesvh.cn/Article/details/gzvvboyhx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcduwglfu.sHtML

[A17] 位运算
来源：http://www.blog.zdbjq.cn/Article/details/gwubzlaey.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/geqdqpiif.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.fehbvm.com/Article/details/guourfwcb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gurzdqcbs.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gzmavujfo.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/ghnjqnukc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gxpoyxjqc.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gykzzxbei.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gwvwmxwee.sHtML


<!-- 参考信息 -->