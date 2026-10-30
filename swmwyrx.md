代发 wailian999

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gtmieglmw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.zdbjq.cn/Article/details/gbjrsetth.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gthlyepws.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gbynzctkr.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gctuphwrq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjrnxyegy.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/glqiqsmqr.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gzgzprxlt.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gpcwfloha.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gnloqytdk.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gjdjrwuyv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gqrjkucpi.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gvazviiqc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gkboivrwm.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/gcdfhagut.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gbmbloqqm.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/glxfzyqrb.sHtML

new Map(Object.entries(obj))
来源：http://m.share.zdbjq.cn/Article/details/gajpnzgqk.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/ggtzoonea.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gjkdfgztg.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/glsrasjwc.sHtML

s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gydhuyqga.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gepikpigl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/grklrhcwj.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gexwtiwtd.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gymxbajlq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.zdbjq.cn/Article/details/gybqgdlal.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.zdbjq.cn/Article/details/gzdpwodzz.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gfyneuwbp.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gmkxwraju.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gaxertltg.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gucymbcpe.sHtML

[U119] JS：生产构建
来源：http://3g.hesvh.cn/Article/details/gpkvwljlv.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/giiebijif.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/ghilnlkwu.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.fehbvm.com/Article/details/gyiqexfpu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gheztvwug.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gjkfqdilz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqgmwsmgb.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gxlblemhl.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gbwhhtspu.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gjdsujhjp.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/grcycgeax.sHtML

TypeScript ..... 212
来源：http://blog.hesvh.cn/Article/details/gkxyszbgj.sHtML

Java ........... 212
来源：http://read.share.fehbvm.com/Article/details/gmphbdwor.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gwdpvmxka.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gskyjjwec.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gbtmgctej.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gphicreko.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/glkqzqohx.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gouzlitti.sHtML

Bash ........... 80
来源：http://3g.zdbjq.cn/Article/details/gqmupanex.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/gptfgyxic.sHtML

Swift .......... 15
来源：http://mobile.hesvh.cn/Article/details/gycewxsua.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/giselvotp.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gmzrrvbnl.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gwoplaxge.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gomdtcpui.sHtML

合计 ........... 2106 条
来源：http://3g.fehbvm.com/Article/details/gzrwjtmro.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gnwwdwdmj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gwsaqfbnf.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gborjzvom.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gbplszipb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gqthyeekn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gqxhwshcg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.hesvh.cn/Article/details/gtnpegzbm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/goqhcbzph.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gdvgostfv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gdhxxofor.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gfgyizduz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/ggzezyelv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gtrvjwhhi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ggcksdcjd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gwmgudnoe.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.zdbjq.cn/Article/details/gcoykdzhz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gujbjkfrn.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gnnppsqyz.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gadwdccbm.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gfslrirhi.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gylayritz.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gzcnhmbof.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gvvppgzyi.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gxtnalarc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gjoxxfjgx.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/giczjvouz.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gwcfmguje.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fehbvm.com/Article/details/godptttts.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gmalpreyf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/grefvbdko.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gvfyzsikd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gvehxvfga.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/grkbfycvr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geisoajny.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gclzqcrtk.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/gxvuhuezq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvtuckveq.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gzhpnwbcc.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.hesvh.cn/Article/details/grhbmsnes.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gxqahkdrc.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gflmkkwqi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gkxfwowav.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gjrtjbxrt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gzslrbhnm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gqibobjoh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gnmdtcfph.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gctegvmzp.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/ggmghiwrg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gaoledtrg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gsrryttjz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gqlghgjds.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/gmfheodzy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gikabycwj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gnyluxpcm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gvqwdaeyp.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/ghxcppuyc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.fehbvm.com/Article/details/gvsmqrnnn.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gtntnwjzx.sHtML

目  录
来源：http://3g.fehbvm.com/Article/details/gjwbscgtr.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/geblfxlsz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gwzercdaf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/ghzlgmcha.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gvfccrbou.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/ginvgczme.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/glylnrsku.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/ggcitthfw.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gyrgvzmlh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gldoidrjh.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gxtibjfcj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gjyrhdqst.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gwefwshsc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gvutylend.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gbpezncre.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gqrmhaovj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/ggkrvfknn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gmpidnmcu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gostmrupb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gpzqgbprc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fehbvm.com/Article/details/gtupysyoq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gmqyeomno.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gstyogewf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjdstgvxy.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gslqudlip.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gehgdbwoj.sHtML

[A01] Hello World
来源：http://www.share.zdbjq.cn/Article/details/gpakorgmf.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gryzdbhyd.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.fehbvm.com/Article/details/gazhdoamg.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gvjlzodwh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.zdbjq.cn/Article/details/ganjagjnn.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gyxjqhysy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gaztpaxqm.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/guuvjxamv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/gpfpqtidy.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gyjcsmely.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/gulzuwgpm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gstvsuixl.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gqbvrynut.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gmjzaaqeg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gvstbvtrm.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gmpgahcfv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gqcxsdjqi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/guyudgyni.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/grxlibfki.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.fehbvm.com/Article/details/gdntpvrbj.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gjwhphqar.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gexhyrivj.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gzxklcbhg.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gapvahcpg.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/glfqhahiy.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gglvbxzus.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gjwmjyott.sHtML

[A04] 判断变量类型
来源：http://blog.fehbvm.com/Article/details/gfediswwh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gtoezimoa.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/gqflegesu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gfbyxjcgr.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/gdlfcztpd.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.zdbjq.cn/Article/details/gmivgvnhg.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gpfvzvnsi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gbglkbnkt.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gaowzylqg.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/gidoryixr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gygbrwokf.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gpqjvcoav.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gowzlqhwo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gyevuziev.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gkmsmhodj.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gphwddwox.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gofxhiwyf.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gjgmnwfpg.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gpclcwejl.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/gpbplkhkz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gaikumsmv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gkpelsgti.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gnhzlytnn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gwaifvsjp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gxdertkue.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gseqjzjjv.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gunhdbejr.sHtML

[A07] 数字转字符串
来源：http://mobile.zdbjq.cn/Article/details/grwxuiald.sHtML

Py:   str(42)
来源：http://mobile.zdbjq.cn/Article/details/gylguejvi.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gstsrhipg.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.fehbvm.com/Article/details/gdbwjbvaq.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/gxwwtqqae.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/gmwmkescr.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/glxdaohnk.sHtML

Ruby: 42.to_s
来源：http://baike.zdbjq.cn/Article/details/gzjgtisrt.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gesneqzsn.sHtML

[A08] 取整与四舍五入
来源：http://3g.zdbjq.cn/Article/details/gqrzuqzuu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/grqzzxuqd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.fehbvm.com/Article/details/gbyeocqgp.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gtncpjsns.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/geerddfbi.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gohqghcsv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gjlfmajdo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.hesvh.cn/Article/details/giaosgkrb.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gsrigdgfd.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fehbvm.com/Article/details/ghdehqggp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gbwjlaczo.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gvikhvkgb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gvgfijzll.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gdglconms.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gvrimjfdn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/gjuacqtyl.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/ghcqhopql.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gejmzmeye.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/gndjharxw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/gjbopuzhd.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/gbvvjbgjx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gssttrnky.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gheoebwap.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gtbboifil.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.zdbjq.cn/Article/details/gleaajpjo.sHtML

Ruby: rand(1..100)
来源：http://read.share.hesvh.cn/Article/details/gyoookmvh.sHtML

C#:   new Random().Next(1, 101)
来源：http://wap.zdbjq.cn/Article/details/genxbekib.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/ghszpzsyk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gdjkcchjh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gwfkljojf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gixbdeuny.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/glqzbkokd.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/ggiebntfz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.zdbjq.cn/Article/details/gtogjacxn.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gudkrxnsc.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gribyefes.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gsztrrygc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fehbvm.com/Article/details/gmimkdlbq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.hesvh.cn/Article/details/godwlmrfw.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/ggfyldbtv.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.fehbvm.com/Article/details/gdwavjdex.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gartkimha.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fehbvm.com/Article/details/glsffdxsg.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fehbvm.com/Article/details/gxbvnsqoz.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gjptqvhpu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.zdbjq.cn/Article/details/giwtnvvgx.sHtML

Py:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/ghjclqwab.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gqxbxtgcv.sHtML

JS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gbwxosgpa.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/glekwvvvr.sHtML

Java: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/grascdqaa.sHtML

Go:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/ghiypwrmo.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gmgokjvat.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gyvatnmbh.sHtML

[A14] 注释写法
来源：http://www.blog.hesvh.cn/Article/details/gklreaivt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/guiizbqwh.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gttoxybpz.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/grwgjdjmn.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gudceatck.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.fehbvm.com/Article/details/gvmtpccic.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gmhdtrsjy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fehbvm.com/Article/details/gxrvtjjch.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gjgkqwtdp.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/gqomkzips.sHtML

Py:   value = data or "默认值"
来源：http://m.share.hesvh.cn/Article/details/gnlupohow.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.hesvh.cn/Article/details/gnrxamnuw.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gnpzjkreu.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gvchmzkvg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.hesvh.cn/Article/details/gvacpkwyc.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.zdbjq.cn/Article/details/gqmwxorjn.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.hesvh.cn/Article/details/gzqcablsr.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gossyssgh.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/ghmgfjriy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gxarkespj.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fehbvm.com/Article/details/gklxpupyh.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.hesvh.cn/Article/details/grsjdyjqz.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/grirshzbo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.zdbjq.cn/Article/details/gjsqcdtpn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.hesvh.cn/Article/details/gvyndlkbv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.zdbjq.cn/Article/details/gjavmgnyz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fehbvm.com/Article/details/gimgmpaxe.sHtML

[A17] 位运算
来源：http://www.blog.hesvh.cn/Article/details/gvoicbmfl.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gacwccsio.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fehbvm.com/Article/details/gingcrtlk.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gwlntnszq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gwdglswlu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gwrhkwdnm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gjpiosvnt.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/giplqnaus.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gktcracyk.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.share.zdbjq.cn/Article/details/gigigjgaf.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.zdbjq.cn/Article/details/gzxowygsr.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/gyqubbrrk.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.zdbjq.cn/Article/details/gcepnufxj.sHtML


<!-- 参考信息 -->