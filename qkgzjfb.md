代发 wailian999

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/grtbdhsmy.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/gcsizytih.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/gtlxloqai.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/giqqefbcd.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/ghsiowaao.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/goanfsfyb.sHtML

[U104] JS：防抖
来源：http://m.share.zdbjq.cn/Article/details/gwmaldlbt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gfniodaaq.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gtikidpgh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gfoebxtcf.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gjmrzeymc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/gbsdssbah.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/ghstywizu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gfgqlrkrg.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gqkpomqqs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gwhmvexyu.sHtML

[U109] JS：数组分组
来源：http://www.blog.zdbjq.cn/Article/details/gcanobrpg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gcsknhdgd.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gnkyevuoq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gyxhupftq.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gdmcwqljz.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gflwrudsa.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gkxchihsu.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gfbaivgfo.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gqelbmbnl.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/genyeqrpm.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gukybbohe.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/giaeannyv.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/gnpjyqpnq.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gkfqnfkzv.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.zdbjq.cn/Article/details/glmswnncs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gimxcgpkt.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gynhbnhbc.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gkkxtkvsq.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gagypgnqo.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gyypxzarg.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gpdzoqhqa.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gvizxoguy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gfjwagftg.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gvjbotezp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbpwowazv.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gtujxbnvs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvuvcdgrh.sHtML

按语言统计（条）：
来源：http://mobile.fehbvm.com/Article/details/gbfhgxegz.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gemchdlkw.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gbtvgpnuq.sHtML

JavaScript ..... 252
来源：http://www.m.share.hesvh.cn/Article/details/gmlewvjyb.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/gnwphlzre.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gtsoolain.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gjxrjlnko.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gaytlyuvi.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gofnrzsbl.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/glwspwulo.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gmucrswya.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gxwenitir.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gijadqpgm.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/glsxeisxh.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gzgsgpzyz.sHtML

Lua ............ 10
来源：http://wap.zdbjq.cn/Article/details/gpyofmsgk.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/grbpdbcmg.sHtML

Scala .......... 10
来源：http://m.share.zdbjq.cn/Article/details/gybcikykn.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gxybuodmx.sHtML

合计 ........... 2106 条
来源：http://www.share.hesvh.cn/Article/details/gurnoeado.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/guifycjtq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gsfveeqph.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gdgaaupes.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gxotpgxnl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/grxphvyhs.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/guothcdws.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gxfhwfzuo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gdicgsvtl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/ghqhjskag.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gynwgmubh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gtnhgxivw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/glwumuhxj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gjcoypdil.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/ggqdprrds.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gpajrpjmj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gbfqhdjhs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gajlmwdle.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/ghbuvetyl.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gqmugbqej.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gstzdnzzj.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gohxifdua.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/goeixkjpv.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gmftxrwsu.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gbaiddggp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gzlgemguy.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gkmmgcnwa.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gtwowaqmh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/garuukxby.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gzkdijbgn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/gjzhfcwmi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gzdldjoaq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gxmcmaulr.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gapczendv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnmqfklju.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/girzdytfn.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gstzmxvku.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giwuqawme.sHtML

【收录内容】
来源：http://www.blog.hesvh.cn/Article/details/gpjejabyj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gdqbegzij.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/gzxunzpvm.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gmrqrxmbf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gtemkipdq.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gwwceszjp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gynwbdpgu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/guisspjbo.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gldtpdfqp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/gmodeqpet.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gunihyfmr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gqwkswxqc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/gdlbelaxz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gydxeiikl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gvvmrfiyo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gfaxmahtp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gyiqsgtws.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gakuvlqyz.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gdbwuthdl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/gwgbdapkn.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gpqymoybj.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gynazwqhk.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gjjiveyfm.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gdbilfkgm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gutypxvci.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gcptdsvum.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gzqwxzvzh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghatmyvfz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gqtqyirzd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gfidutgsw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gaoahvmae.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gnwwbgqoi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjqyejcso.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gevcfhfiz.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gzesaxtgw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/grbgtfwds.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/grepahbst.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.hesvh.cn/Article/details/gytqoxdsr.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gcbabyekn.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/gjgzgklme.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gjzgjsnmd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.fehbvm.com/Article/details/gvhthutyy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gxrlisipm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gevoqhvlw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geoghfssy.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/gimhexpzk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guyuflpns.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gfgzjrofi.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/ggukulcze.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gikwewlbo.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gofqsxvmn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/ghjirbhjp.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gfphuravv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gmeybzgwv.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gdoniyaeu.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/grpphajnz.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gwnutzkgt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gmvxmoced.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gorritkkm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/gassoxqnh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gviyvatcd.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gkgdbwpgt.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gklwslvvv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gcowyuvjj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gogzqhwgl.sHtML

[A03] 常量定义
来源：http://blog.fehbvm.com/Article/details/gogcvkojv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gfxrdqvuj.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gxmbwfcoc.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gmyekusut.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gfahfdxay.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/giosnpfev.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gdhctowoj.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/glgnyqghq.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gzubfamsi.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gmoidvagq.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gqqiwxajn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gltycvmav.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gwexdleef.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gkgumskgx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gxhyohync.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gekjctdcv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/guupyabqk.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.fehbvm.com/Article/details/gzggohyok.sHtML

[A05] 整数除法与取模
来源：http://m.share.zdbjq.cn/Article/details/gdmzgkmhg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gewqukopo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gardegdxy.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gikjkqthh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/grspbwzkw.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gfbuxzydo.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gjlmfwequ.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/govwfjtht.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gycypjzvz.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gjulcsjjx.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gyyizxban.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/gitjmhhpa.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gmevdhvdi.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gnzkahdsh.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/ggktdfgpi.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gycfraupz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gankuquxw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gyxoegcax.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghnspqeen.sHtML

Py:   str(42)
来源：http://m.share.hesvh.cn/Article/details/gphuekuun.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/guyhscaaf.sHtML

JS:   String(42); (42).toString()
来源：http://baike.hesvh.cn/Article/details/gkxohfbob.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/ggwveamhp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fehbvm.com/Article/details/gopposozi.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/gsnhzudfs.sHtML

Ruby: 42.to_s
来源：http://www.share.zdbjq.cn/Article/details/gpockazmr.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gpbursuyq.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/gcowleiwj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gvvkfhhxl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/ggjswadyj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/grhqgfrfc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxswnsrd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gxonxdadb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gnskmummz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.zdbjq.cn/Article/details/gzanpphni.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gewthgaui.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/gdtjxyuex.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxqikjav.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gbpnyeyrz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gnmmomdag.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gkedyfltq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gmrninryi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.fehbvm.com/Article/details/gqvwtyqfp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/gxpjktkey.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gftwxkspz.sHtML

[A10] 生成随机数
来源：http://www.share.hesvh.cn/Article/details/grvafhqbz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.zdbjq.cn/Article/details/gyhiymatr.sHtML

PHP:  random_int(1, 100);
来源：http://3g.hesvh.cn/Article/details/gkhhxyysm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/grtzuxcms.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gzcmjcotg.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.hesvh.cn/Article/details/gxrhuyuwt.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gvmwuijas.sHtML

Ruby: rand(1..100)
来源：http://mobile.hesvh.cn/Article/details/givafyvjy.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fehbvm.com/Article/details/gfeotavks.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.zdbjq.cn/Article/details/gtyjkvfdp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.hesvh.cn/Article/details/gfllldmah.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gtqdtkhhs.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gaqhabmag.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gzodaofau.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gxgibgzbk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.hesvh.cn/Article/details/gnobludgm.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gxteeeqfb.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gcsxnhxdp.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.zdbjq.cn/Article/details/gebnrmjue.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfdprsrpf.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fehbvm.com/Article/details/gtqlctupp.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gvosennwe.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gbmlymbzt.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/gdokxroqi.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.hesvh.cn/Article/details/gmrislazo.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gkgifzuyy.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fehbvm.com/Article/details/gpxyosgiy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/gsiuxzwsx.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gwbjyasrq.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gphxrgzeq.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gkbcixeai.sHtML

TS:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gpbkqslgg.sHtML

Java: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gosunrnah.sHtML

Go:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gsguvhrfh.sHtML

Ruby: "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gimtuwgpq.sHtML

C#:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gjzzkupjv.sHtML

[A14] 注释写法
来源：http://blog.zdbjq.cn/Article/details/gtxtjuqjf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.hesvh.cn/Article/details/gsembfaoh.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gqxhkqrpl.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gmzfhsyzh.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.zdbjq.cn/Article/details/gunzeekom.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.zdbjq.cn/Article/details/gisarwbvh.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gvwwirseu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://baike.zdbjq.cn/Article/details/grskkwtfq.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gwnlawtgm.sHtML

[A15] 空值判断与默认值
来源：http://m.share.hesvh.cn/Article/details/gluwgxujb.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/glsrluhoq.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/guhrsobtq.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gebuevrfd.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gzvwxxepl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://mobile.hesvh.cn/Article/details/gdzsauhdy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.zdbjq.cn/Article/details/gnuszzpoj.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.zdbjq.cn/Article/details/goixdwrir.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/grgbyqgfc.sHtML

[A16] 真假值判断规则
来源：http://read.share.fehbvm.com/Article/details/gwoaxxsso.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gqdvkaugc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fehbvm.com/Article/details/gvmietgtm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.hesvh.cn/Article/details/gketpdpmd.sHtML

TS:   if (!x) {}
来源：http://3g.zdbjq.cn/Article/details/glifwgjzw.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/ghsyomygl.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.hesvh.cn/Article/details/grenvxcid.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://mobile.zdbjq.cn/Article/details/gqakxxpll.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wap.fehbvm.com/Article/details/gtmfjdiux.sHtML

[A17] 位运算
来源：http://www.share.hesvh.cn/Article/details/gxelxbplx.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/golqxekpo.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fehbvm.com/Article/details/gwidwqljm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/ghzehkqtl.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gwrhnceff.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gacdpbuam.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gmputbghv.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gbuqwdxck.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gkeoxicas.sHtML


<!-- 参考信息 -->