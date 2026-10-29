代发 wailian999

[U103] JS：定时器
来源：http://3g.fehbvm.com/Article/details/gbpwybdsr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gbmxzsvlz.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gpsrywigb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gxrwqeshk.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gzxnwmecl.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gqyhiueat.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gwdjxcfha.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gocsaymup.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gigikeixh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gexwozubi.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gthpocowd.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gqphdigqo.sHtML

[U109] JS：数组分组
来源：http://3g.fehbvm.com/Article/details/grvjfaahr.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gemnhvmiw.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gjniyboas.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/givaxkdmd.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gioddszcz.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gxixfiloz.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gwacejbrg.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gnjnufgsj.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gncjjojki.sHtML

s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gzqngqzcw.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gyyxnoaxo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gzgrzuzjr.sHtML

[U115] JS：生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gjwijbpjq.sHtML

crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gzrhuzhcu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gfidkznqk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gqrpusgdh.sHtML

[U117] JS：单元测试
来源：http://m.share.hesvh.cn/Article/details/glzlhroxe.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.fehbvm.com/Article/details/gwttljbtu.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gyqwzlnxq.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gkvdtlpym.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/guxbfnmvu.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gdgapqnak.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gbogpndee.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gnexbhinu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjmandbsc.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gppxvqgts.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gunmbthqt.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gfvhcswxj.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gabwmztbs.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gzgbxvncd.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gircfjngt.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gikkncwrg.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gtwvgaiyb.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gpbuykoze.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gislclgls.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gmhczyxjt.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gouumznfq.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gszfutgqi.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gyuqudpnt.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gzbeepxpn.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/geialbrwu.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gchyooiec.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gwbrbuyaq.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gbpfpxkgf.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gvdmrvteq.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gupqcjnra.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gnbenbowh.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/ghavseekb.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gcyjizwpv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gtsogwczs.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gjxielcda.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gddnsrktn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gndcmfehn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gfaidneux.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/geuygdkzv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gtumttrhb.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gzeborirb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gxkzodpuq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gqdrcmjxq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gaoyunpbv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gfaxldngp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gfheavvzu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.zdbjq.cn/Article/details/gukeduelq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gurcsiznk.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gmsjzbowk.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gsxxpxfcj.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gawproksp.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gyenzeczo.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gijfzfqpt.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gcemdctak.sHtML

合计                                  2106 条
来源：http://wap.zdbjq.cn/Article/details/govrugslz.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gcyaicdlj.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gaayqwgiv.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gexsqtioz.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gumexfnbw.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gvibzlsae.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.zdbjq.cn/Article/details/gugtteehk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gtuskwjao.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gqmuxohwl.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gwuxbaton.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gycrklkwt.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gaxmydikw.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gysyofrmr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcwxbksii.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gcifhsrqb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/ghuvuiuzv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fehbvm.com/Article/details/gwbxrtbhc.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gmopzhbzx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gobshdpta.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gcxcgovwg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gxvaskvij.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gewmkqisk.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gcejfhwrr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fehbvm.com/Article/details/ghzuryhte.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gxowwiizo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/ghxohknxy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/gttzodwhk.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gggnfowut.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gqvithbke.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gutiqniod.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gibvobwva.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gtavkgdlc.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gefqqfgow.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gyliobced.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gakytwmgg.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/gykiqkbtq.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gtfaefnxy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gdxvnvelt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gjtwoqmgz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gjnhygrvd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gnbrpofuf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gsnyfbtbf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjszdvdcs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gdglmfsqe.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gseorhjjx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gppsmlzhn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gssokyhiy.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gulnspnte.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvjcsaalz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gwrbmqjqd.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gdmvzemui.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gtbowwigx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gjedemzvs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gussclduh.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.fehbvm.com/Article/details/gmwmbnrhm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/gocokezgm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gdkkvhpvf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwbycjiss.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjfpdmyyn.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/geyrtcosb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmnpaivci.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gwawqofvd.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gbuchbqvu.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.hesvh.cn/Article/details/grhyajxmd.sHtML

JS:   console.log("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gvirzxnui.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gvfbdjokl.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gjbqqwwzb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gxqrgktmj.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.zdbjq.cn/Article/details/giocflmpz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gdqbyafvg.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/gptknitdm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/grnnysuae.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.fehbvm.com/Article/details/gdudfqmtb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/ggsjyyxbl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gaepyvzle.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gnabeacas.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/guxwmxtsw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gpcolmsmm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gqksitifa.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gprunaigh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gskmrhfgo.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gmhapausf.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/grtsotiak.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gqzhtwjew.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/ghfohoweg.sHtML

Go:   const PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gkcfvdgna.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/golkbttds.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gxnsecadv.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gdvamozuf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gvgbxnnsa.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/ghuxbgitn.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gjbjbfjcr.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gnvsvjudp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gcxdvrnkq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/gnysrdrrb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.hesvh.cn/Article/details/guiqntylp.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/gvdhityft.sHtML

[A05] 整数除法与取模
来源：http://baike.zdbjq.cn/Article/details/gyrtjkdvd.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/godxtilwt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gqlhpplfp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gfwrpuewu.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gnquaxegp.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/glskhqdin.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gsgqgfete.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gssbyomnc.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gokpdxmxc.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gplyftcee.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/grbqbropj.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/goculqytm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gyoqdvtyo.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gicvnpxxx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gofibiimp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fehbvm.com/Article/details/gammgwxkd.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fehbvm.com/Article/details/gdkrywvne.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gmxarpexg.sHtML

[A07] 数字转字符串
来源：http://www.share.fehbvm.com/Article/details/gzjynynyi.sHtML

Py:   str(42)
来源：http://www.share.fehbvm.com/Article/details/gnnogwqlh.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.zdbjq.cn/Article/details/gkvfkuiko.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fehbvm.com/Article/details/gvkmskjiy.sHtML

TS:   String(42)
来源：http://mobile.hesvh.cn/Article/details/gbayfsvmo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gdovsbidd.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fehbvm.com/Article/details/gcyfpgmcz.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gijaztkvh.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/ghlihbauf.sHtML

[A08] 取整与四舍五入
来源：http://read.share.hesvh.cn/Article/details/gtvzmubcx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gfijeobap.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/gfskekwqk.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gvvchwrwz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/gpoaujcrj.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gfuvmmiji.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gwnnrxnrh.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.zdbjq.cn/Article/details/gpholwoth.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gnzhzcnsv.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fehbvm.com/Article/details/gepxuxxgg.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gczsbuzzz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gbqvhldtn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gflzlvnas.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gkgrkbqsg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/grbeqenyj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fehbvm.com/Article/details/gvonquiox.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fehbvm.com/Article/details/gzpnatzvi.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gdvjpmqof.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/gcbuvsioo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.hesvh.cn/Article/details/gsmtnbxle.sHtML

PHP:  random_int(1, 100);
来源：http://wap.zdbjq.cn/Article/details/gztysmwra.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gmdquhruz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gaxogyzch.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.fehbvm.com/Article/details/gympjehsl.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gcvsuatnr.sHtML

Ruby: rand(1..100)
来源：http://mobile.zdbjq.cn/Article/details/gszqfrset.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fehbvm.com/Article/details/gghtojibj.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/gkuwfehcu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.zdbjq.cn/Article/details/gjcslhaef.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gispvfmjf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gurfjrdjd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gygsaprpp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gfprkriua.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.hesvh.cn/Article/details/garnnajad.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gouidlwpx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/geinoxbrq.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/gzqtauhmu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/goicixara.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://mobile.hesvh.cn/Article/details/ggpvchxuq.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/grnmysjer.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gojzwmefs.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.hesvh.cn/Article/details/gbeyemvjl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.hesvh.cn/Article/details/glvxvgval.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.hesvh.cn/Article/details/gllbjbwdz.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.zdbjq.cn/Article/details/gyccqznhh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/ghhfftykx.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gvlnvenkh.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/giiogqkqy.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gyxlyugzu.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gmvjqwjry.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/guhtcwlmm.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gljilwily.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gqtfwjina.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gnihrbihl.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/goqclncof.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.hesvh.cn/Article/details/gmmzvtvke.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gfsebixdf.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gpnhjygpn.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gvhgskdcq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.fehbvm.com/Article/details/gpsgvqzfp.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gonkwbtco.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.zdbjq.cn/Article/details/gptjmdzyq.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gklgbpbau.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.fehbvm.com/Article/details/gaaiwdrya.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gezsafnux.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gkznjvlcj.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.fehbvm.com/Article/details/gqskacyxt.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gucghekkd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.hesvh.cn/Article/details/gmviktflr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.zdbjq.cn/Article/details/glcxijhwc.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fehbvm.com/Article/details/greeziiql.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gdvujzzhn.sHtML

[A16] 真假值判断规则
来源：http://m.share.fehbvm.com/Article/details/gwnchhotj.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.hesvh.cn/Article/details/gixcmyxwe.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.fehbvm.com/Article/details/gwpeauyxo.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/gqxtecshd.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gqghqhgaa.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/gnxczloni.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.fehbvm.com/Article/details/gbvrhpudd.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fehbvm.com/Article/details/gsgmsqmqx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://m.share.fehbvm.com/Article/details/gzakyealj.sHtML

[A17] 位运算
来源：http://mobile.hesvh.cn/Article/details/gyduonnnp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gpericqty.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fehbvm.com/Article/details/gpkvvdzwt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gtrmuheub.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gdjpkhxcp.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gkdwkghxw.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gggiihkop.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gybieppvh.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gekvhgedg.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/gtycfoeyq.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gmpvmwoda.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gdcbcmvsd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gyneborpo.sHtML


<!-- 参考信息 -->