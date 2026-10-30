代发 wailian999

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gjrgfgdcj.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/geycqxsuw.sHtML

[U102] JS：本地存储
来源：http://baike.fanxiaobao.xyz/Article/details/gwfmqbjep.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fanxiaobao.xyz/Article/details/grbiskjcp.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwynrmmr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbtmunqd.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkhjbzrt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjfpjxcp.sHtML

[U105] JS：节流
来源：http://baike.fanxiaobao.xyz/Article/details/grtxdkpfb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gpaanhhvp.sHtML

[U106] JS：日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/gflkmfuwp.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyyfctaj.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjgynrvy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmlbtekz.sHtML

[U108] JS：随机整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvyygttsy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.fanxiaobao.xyz/Article/details/gjobdpsmp.sHtML

[U109] JS：数组分组
来源：http://blog.fanxiaobao.xyz/Article/details/gcnmiohyz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmrtuhvd.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gdcmexzcb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.fanxiaobao.xyz/Article/details/glbfmpcam.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggacmyyra.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkerlvjdj.sHtML

[U112] JS：字符串补位
来源：http://www.share.fanxiaobao.xyz/Article/details/gujeqlene.sHtML

"7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gntbioncx.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gokuzcicm.sHtML

s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvehcikox.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrkuaqef.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtuvanbs.sHtML

[U115] JS：生成 UUID
来源：http://wap.fanxiaobao.xyz/Article/details/gdgaysbfp.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gjnpdrtpq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getqoumde.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/glgarlrdu.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gjhoalybo.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnwwcskc.sHtML

[U118] JS：开发服务器
来源：http://blog.fanxiaobao.xyz/Article/details/guxpxuwsx.sHtML

npm i -D vite;  npx vite
来源：http://blog.fanxiaobao.xyz/Article/details/gbsyfnuiu.sHtML

[U119] JS：生产构建
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgwmywyl.sHtML

npx vite build
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyqlohpd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzofzgvgo.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gfngjitup.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guznjazst.sHtML

统计汇总
来源：http://mobile.fanxiaobao.xyz/Article/details/guehtmkqa.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjsllgnfo.sHtML

按语言统计（条）：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblksgcre.sHtML

Python ......... 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gessmdqcg.sHtML

PHP ............ 252
来源：http://wap.fanxiaobao.xyz/Article/details/gjqunpniq.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkedqacgd.sHtML

TypeScript ..... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gjguupcyi.sHtML

Java ........... 212
来源：http://wap.fanxiaobao.xyz/Article/details/gyaoyksmp.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrzctdmd.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gjevgdnhn.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gchqskdhi.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejtxaqji.sHtML

C++ ............ 30
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnyrldym.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gfrqurbgg.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/gryjvjdvx.sHtML

Kotlin ......... 15
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjvqnifz.sHtML

Swift .......... 15
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsufuzxbh.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gdgcqcrtu.sHtML

Perl ........... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gzcnedmia.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gbhzzpgda.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gjneukdsc.sHtML

合计 ........... 2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdlqpgmw.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/grpwrtzbq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gliofqdfv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtzkkufh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fanxiaobao.xyz/Article/details/gifsmnoes.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/glohwxljr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjkhnawk.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoaxcutn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/ggxrcyvfu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/ggukpotfy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqahfjey.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gkdplzytx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/goxfoychx.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/glrgqduwk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gutscgsfe.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxfrrubb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gasxogmxy.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fanxiaobao.xyz/Article/details/gvnqvylgd.sHtML

Q SQL 专题                              90
来源：http://read.share.fanxiaobao.xyz/Article/details/gekxluvdg.sHtML

R Bash 专题                             80
来源：http://read.share.fanxiaobao.xyz/Article/details/glxqwdtit.sHtML

S C / C++ 专题                          60
来源：http://3g.fanxiaobao.xyz/Article/details/galpksxvm.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/guowvcqcy.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhorwtpl.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/guvqchbal.sHtML

合计                                  2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gnhfkggwe.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmlopozz.sHtML

使用提醒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqevnfapk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/grviorasr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.fanxiaobao.xyz/Article/details/gbirzfowe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpuqowmy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjltrqon.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqatznkx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gfboywflg.sHtML

—— 文件结束 ——
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgbgihgj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtaazaahv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fanxiaobao.xyz/Article/details/gjalknafq.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxhsedky.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ghxvugshv.sHtML

【收录内容】
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtkdutvt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/gugikkopf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.fanxiaobao.xyz/Article/details/gxijrxegl.sHtML

SQL · Bash · C · C++
来源：http://mobile.fanxiaobao.xyz/Article/details/goszrflwn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fanxiaobao.xyz/Article/details/gxyklwokj.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gifpsshoh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gubgjvmcx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fanxiaobao.xyz/Article/details/ghjrdpdhm.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.fanxiaobao.xyz/Article/details/genabjjal.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fanxiaobao.xyz/Article/details/gahwsdgfk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikgbmhne.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fanxiaobao.xyz/Article/details/gtymfeihs.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.fanxiaobao.xyz/Article/details/grhpcxajr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gcoyreeow.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaapcwkj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzpguhzw.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcprszky.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkbbsaib.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/grwsohdzz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhdtiikf.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gcqizkwhk.sHtML

目  录
来源：http://baike.fanxiaobao.xyz/Article/details/gxeitfxag.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gxjivncsp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwprfbjp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjinymlda.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlqbgcgq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxcqcohq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopfbgwzy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gbfykklsl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdfhwlgs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjewkgms.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/glyuihipt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garwpgnqq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gayxqfxmx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwfthlqf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/guofhevbp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmzdrxbv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gyxilrjqm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gstvclgfg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/galkwuoap.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gjthztzkp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtmvmmhr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/gygljrjhx.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gvstzaana.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbuipklw.sHtML

A. 基础语法与类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyjzkbqr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gefsxnhac.sHtML

[A01] Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gmtmawwxm.sHtML

Py:   print("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/gdpbdvqaz.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmgbzhaw.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbuvmdir.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fanxiaobao.xyz/Article/details/giuqelroj.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gutcvyoiw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsksffzpw.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fanxiaobao.xyz/Article/details/gulmguufc.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljuczqdz.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsckcyur.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fanxiaobao.xyz/Article/details/ggsifnneo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkjnqstt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/gfnempkyl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gwwqrvnts.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgordtyo.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fanxiaobao.xyz/Article/details/gagkpskuc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fanxiaobao.xyz/Article/details/giapaptwx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gmhqxqrjr.sHtML

[A03] 常量定义
来源：http://wap.fanxiaobao.xyz/Article/details/gokysttkj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogbedihs.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilpnvyac.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkadmdmjp.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gaavxgohe.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbxdzzxy.sHtML

Go:   const PI = 3.14159
来源：http://read.share.fanxiaobao.xyz/Article/details/gragyuazj.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiggtnpm.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqzjfksk.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskxqnroy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fanxiaobao.xyz/Article/details/gmszunvkx.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gsobglttk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gafdjjytk.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fanxiaobao.xyz/Article/details/gftispgjz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fanxiaobao.xyz/Article/details/gxppjonws.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsdkicrz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujucjngo.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.fanxiaobao.xyz/Article/details/gjxofxbjh.sHtML

[A05] 整数除法与取模
来源：http://wap.fanxiaobao.xyz/Article/details/gujqrjlqv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzrdtmnj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gfcudvdbn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/ghlauvrjc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gxxuvzvbw.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gzijhagxl.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gcraprpap.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gddlufpup.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gqfrrazfq.sHtML

[A06] 字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlreqecf.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/gboyypozk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyzkmtpm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwufialnn.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fanxiaobao.xyz/Article/details/gyifbrjas.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gngwynfci.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoxdxiak.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnipawec.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnzvtsiw.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknfgmoxy.sHtML

Py:   str(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gsbealosx.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gagznflbu.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fanxiaobao.xyz/Article/details/guzguzkke.sHtML

TS:   String(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gcdsjxrcr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gynxyaanl.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtfknvlj.sHtML

Ruby: 42.to_s
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzdxigpc.sHtML

C#:   42.ToString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyjpdpyw.sHtML

[A08] 取整与四舍五入
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyiubpfr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjkcszcn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gozrdgqge.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gawqngian.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrithbor.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/giblmhqks.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gpxsnuics.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fanxiaobao.xyz/Article/details/gcunspvnr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/grpjrrdti.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gmekybdhp.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gcfdmiyiv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gazzbqxyu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/giigkbiam.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gnwrruqnd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gukdirqsw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fanxiaobao.xyz/Article/details/gndzyxjwh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtxthdha.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwnaytij.sHtML

[A10] 生成随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxuhausf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fanxiaobao.xyz/Article/details/gnffppwod.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fanxiaobao.xyz/Article/details/gvbmvokgw.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/gjtakdjfo.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyaugpny.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gzvevfirz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fanxiaobao.xyz/Article/details/gulikqtdh.sHtML

Ruby: rand(1..100)
来源：http://blog.fanxiaobao.xyz/Article/details/gexxrgxhm.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fanxiaobao.xyz/Article/details/grrtuielh.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fanxiaobao.xyz/Article/details/ghabulqmp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gmkdpsqqf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gcbsdjkfk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gkxtibcco.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvwlzusa.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbiropos.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fanxiaobao.xyz/Article/details/ghjsxfugi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqtvdxyn.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/grobhqpky.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gntdjdhgt.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdllqxuw.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fanxiaobao.xyz/Article/details/gpbfumaks.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmorkkjx.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fanxiaobao.xyz/Article/details/gveuonotg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecwohdib.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gszecaxwu.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvctqembj.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.fanxiaobao.xyz/Article/details/gygljyfvd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.fanxiaobao.xyz/Article/details/ggmsgrgxw.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyskkihkn.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gifmavwej.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzahrcbqc.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfgmoeun.sHtML

Java: "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gsxcgdbqy.sHtML

Go:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gymgvqbkk.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gzbnjhdqt.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzroaynet.sHtML

[A14] 注释写法
来源：http://blog.fanxiaobao.xyz/Article/details/gounminfn.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fanxiaobao.xyz/Article/details/gamgbhlpb.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrhrhzeq.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/glielcnuc.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.fanxiaobao.xyz/Article/details/gubfnobhv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gpetujsbp.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxdjkctg.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fanxiaobao.xyz/Article/details/gprbsjgjv.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxipbxcr.sHtML

[A15] 空值判断与默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkhbcpdh.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrinwsrb.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gvswckktx.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsrievcf.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gpzjsrgza.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fanxiaobao.xyz/Article/details/gkqyrkewm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fanxiaobao.xyz/Article/details/glldrdarh.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fanxiaobao.xyz/Article/details/gipavppbb.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtgglpas.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gronepnsl.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fanxiaobao.xyz/Article/details/gzvqtgths.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqybqxlli.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxfizmes.sHtML

TS:   if (!x) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gbgsygytf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjduyhofj.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.fanxiaobao.xyz/Article/details/giqkdwxlc.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://read.share.fanxiaobao.xyz/Article/details/gggbhclzb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/grbwpyrsv.sHtML

[A17] 位运算
来源：http://3g.fanxiaobao.xyz/Article/details/gjfffwtpp.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gptktupem.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gusviqwgn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gsfmojtan.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gmhivurar.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gvbavydmv.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gcthpjcsb.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/grjttrhok.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmxecopq.sHtML


<!-- 参考信息 -->