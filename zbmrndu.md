代发 wailian999

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gfgmjkdls.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gctfktqem.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gscitirxt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gvvnqbmhl.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gysctagfe.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gcnnocqwx.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gimrgpqci.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gvtlnzzes.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gohyirhwz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gvljeyfkw.sHtML

[U108] JS：随机整数
来源：http://mobile.zdbjq.cn/Article/details/gvpuwfjyw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gnrdoiyia.sHtML

[U109] JS：数组分组
来源：http://read.share.fehbvm.com/Article/details/gvnhaogbx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gdwyguofo.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gzdikqbtn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gzbvpkmnr.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/glczpukac.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gsbncgkjy.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/ggmvlaomw.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gishymjqf.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gjgtcvigj.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfiybname.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/govalbtqn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/getkkjsgs.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gylpjrmql.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/guzagpgdt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gmaiozvez.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gyeluoelh.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gacgkorvg.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gmytfvwgp.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gfdhzxesz.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gdltckcsa.sHtML

[U119] JS：生产构建
来源：http://www.m.share.hesvh.cn/Article/details/gsisbwvwz.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gklgdpzgp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gbhaboswe.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fehbvm.com/Article/details/gdcqrzejz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gannowpxv.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/ghehtzynv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gptmgtlyy.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/guivgutwf.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gzyovbjks.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gimizirxb.sHtML

JavaScript ..... 252
来源：http://www.blog.zdbjq.cn/Article/details/gyxvuxlwd.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gwwltasao.sHtML

Java ........... 212
来源：http://baike.hesvh.cn/Article/details/ghclipppg.sHtML

Go ............. 212
来源：http://wap.hesvh.cn/Article/details/gsceuvheq.sHtML

Ruby ........... 212
来源：http://3g.fehbvm.com/Article/details/gcxebsbwo.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gszyahvtn.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/guhazegfq.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/ghdmdguup.sHtML

SQL ............ 90
来源：http://www.share.hesvh.cn/Article/details/gjyhetmcf.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/glegjllbu.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/grbqcgozx.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gncwpfspo.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gqoqhmwid.sHtML

Perl ........... 10
来源：http://m.share.zdbjq.cn/Article/details/gspiusenj.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/gzeeokxlm.sHtML

------------------------------------
来源：http://3g.hesvh.cn/Article/details/gxeyuyzys.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gvzdmlbqm.sHtML

按章节统计：
来源：http://wap.zdbjq.cn/Article/details/gpnpyvwth.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/grhfezjjo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/giobthmjq.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gxsbfokzu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/ganeimita.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gdtphsifs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gnugjzwxr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gglxsokqj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/gueqrozgo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/garznnqvt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gcaowvuaf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gagckurbz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gguhhweay.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gaiycqlet.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/glvqpohbu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.hesvh.cn/Article/details/gkixspeid.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gxhtdrqco.sHtML

Q SQL 专题                              90
来源：http://3g.zdbjq.cn/Article/details/gjshofgov.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gsmwjvzrh.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/gkazndfqo.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gmfvxkptc.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gcpredkwv.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gpcregonf.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/guqfrxjeh.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/goraweosq.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/gydnnxaxt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gtlkgzqxn.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fehbvm.com/Article/details/gxyjujbdz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gngbdqxmq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gjnxejcwx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gqadgkjmv.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gcfoyigaw.sHtML

—— 文件结束 ——
来源：http://www.share.fehbvm.com/Article/details/gwvugrdzj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnojlpqod.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gsnpriqlc.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gqebiptig.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grsxchpdx.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gzsedkynv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gcuirgcrk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gkuwnzgnh.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/goleqvnax.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gfymlvgpu.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/ghtkpumye.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gcxknewaf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.fehbvm.com/Article/details/gihgwztrx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/gpcylfrns.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gvbqskseh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/geffdhnxm.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.zdbjq.cn/Article/details/gyrhdjjos.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/goqeogfra.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gtkhzhbji.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gihrmbbhc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gshkoawnq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/gykvnseeu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.hesvh.cn/Article/details/gbuydumle.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/glmmiwzjh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gcfrksfhx.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gckecgmvh.sHtML

目  录
来源：http://m.share.zdbjq.cn/Article/details/gigqumqqb.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gwpwzrzxd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/grgisiqsi.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gwqcqazdy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gyfmdcflu.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gkfinjicj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gnfabvbjj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gjgnyuxte.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gucbcajsz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gpzlrwmds.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gcdegjybt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gmzrqsyqo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gexrjrnhn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gylojmilt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gqkdfkgnj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gfndlipjz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/gwabsedfx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gvxfprtof.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gcssbjcxx.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.hesvh.cn/Article/details/grirjaedp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gtlmevrpb.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/gsxifuylw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.hesvh.cn/Article/details/gftzdzzek.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glbdngwip.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/glblytuyk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnaljjzkv.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmmuruzjw.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gpfegefzg.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gwqsdrelx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gmwazkesf.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/gtkbmcowa.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/grgyelpku.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gengsrbyc.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.fehbvm.com/Article/details/guacujnaz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gwklgcbmv.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/gluzaaqcg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gevieowkq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gmcynqnwq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gfsmjavsr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.hesvh.cn/Article/details/gmiqkhhgb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/ghsewelpr.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/glkiomjqo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gvnzrtcif.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gnjxhpyiv.sHtML

[A03] 常量定义
来源：http://3g.hesvh.cn/Article/details/gyjuhdvht.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/gbqddtfsm.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gcrwxbwtj.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gxxuyumah.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gipjergcu.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gdehjyzzg.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gwknbbbrp.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/grvrxbsty.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gsoasupkq.sHtML

[A04] 判断变量类型
来源：http://m.share.fehbvm.com/Article/details/gcnjjzfav.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gjrfniimw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/grcwdsbbe.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gmmuspfor.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.zdbjq.cn/Article/details/gtvjkdxxr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gitebhmrj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gkofztfvg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.zdbjq.cn/Article/details/gkjtcoahw.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gbsomxgyd.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gawvlavrj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/giuxulmag.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gypvmgyyu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gntzjynad.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gxvjnlofl.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gbtswalst.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/glhmfbwsr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gnvpoddnm.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gasgkjagw.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/gzkpqlqzv.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gfmnavujn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.hesvh.cn/Article/details/ghgnlluft.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/giexuskur.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gpkiozupx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gjitvmdib.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gbbdlfdbn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/geyiuiatp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gywhmgxft.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gropmoujg.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gfvcrgnml.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.hesvh.cn/Article/details/guwfidonz.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.zdbjq.cn/Article/details/gtixctisn.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/ggpjjdrwe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/gbywzyfjw.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/ghpnnjnfh.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/giamotqdj.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/gyookbmea.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gziuqsnff.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/ggwcuxzmk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gcdxwpwkr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/geyebycxb.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/gyvxawgyy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gubsvztjl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gtlpxebrs.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fehbvm.com/Article/details/gqodzzeow.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gxomhpaek.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gjnytfqni.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqgyfkpiz.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gnoipnqzx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gtvwspqss.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/ghkeqjliy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gvelmbwfu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fehbvm.com/Article/details/guwxrhdqw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/gargmyguh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gwhdzzyzq.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gwlvnokfy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.m.share.hesvh.cn/Article/details/gaavasdig.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/gtmjcvdyx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gmbqvdnrc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gtdtnruvd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gxrrozyis.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.hesvh.cn/Article/details/gamuinrep.sHtML

Ruby: rand(1..100)
来源：http://www.share.fehbvm.com/Article/details/grfcodkyf.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.zdbjq.cn/Article/details/gklfrsoyc.sHtML

[A11] 条件表达式（三元）
来源：http://baike.hesvh.cn/Article/details/gxfbervkf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.zdbjq.cn/Article/details/glyhxqbrk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gdwfmataf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gmzqtouvg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gvkcdgmux.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gevnchuyz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fehbvm.com/Article/details/gifpzhaxh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gpldrjdgx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gycihcbyt.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/gwfslkniy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.zdbjq.cn/Article/details/gxetbcodi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.hesvh.cn/Article/details/ghvksrwkp.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gocaiouok.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gfoiifvyw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.hesvh.cn/Article/details/gmzpumskk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.fehbvm.com/Article/details/gcqflcxyy.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.hesvh.cn/Article/details/gyigrxymf.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.hesvh.cn/Article/details/gyaxxhxoj.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.zdbjq.cn/Article/details/ghinluftz.sHtML

Py:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/ggwlkgrnw.sHtML

PHP:  "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/ghipjofex.sHtML

JS:   "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gtfpnnhfh.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gmvrarogo.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gewkcgtfa.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gxkvioqhr.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gkfcxtvua.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gdxkgofud.sHtML

[A14] 注释写法
来源：http://blog.hesvh.cn/Article/details/gwolkyjln.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fehbvm.com/Article/details/gnokzeway.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gqiwetvqc.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gufvdlxjr.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gyvobjhdj.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.fehbvm.com/Article/details/gpqrgojjd.sHtML

Go:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/gwaibeofd.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.zdbjq.cn/Article/details/gtvdqqxjh.sHtML

C#:   // 单行；/* 多行 */
来源：http://blog.fehbvm.com/Article/details/gudxfnrwr.sHtML

[A15] 空值判断与默认值
来源：http://baike.hesvh.cn/Article/details/geentzdnw.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fehbvm.com/Article/details/gzkktegnv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/guyhluxel.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gxfgntmig.sHtML

TS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gmbagxrwp.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.zdbjq.cn/Article/details/gcrmdvtqi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://m.share.fehbvm.com/Article/details/gqqtprizs.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.zdbjq.cn/Article/details/ghmftlsht.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/ggxolhriu.sHtML

[A16] 真假值判断规则
来源：http://m.share.hesvh.cn/Article/details/gqrpfsikw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.fehbvm.com/Article/details/glrlfkcln.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fehbvm.com/Article/details/gjstfgoud.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://baike.hesvh.cn/Article/details/glptytxsw.sHtML

TS:   if (!x) {}
来源：http://read.share.fehbvm.com/Article/details/gwsuitrph.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://3g.fehbvm.com/Article/details/gksqngdwx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.hesvh.cn/Article/details/glfzzrsgl.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.zdbjq.cn/Article/details/gswctmviu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gawjvfvhi.sHtML

[A17] 位运算
来源：http://mobile.zdbjq.cn/Article/details/grfakcpzn.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gbwkcfkfo.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.zdbjq.cn/Article/details/gjsctuxow.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gfwjgmzak.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gnbswrvnu.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gecenvcfz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gqhddsgvj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gmsdsrtar.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gijhbmhoo.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.zdbjq.cn/Article/details/ganlgwzde.sHtML

Py:   ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/glfzcwpaa.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/grrxxtlri.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fehbvm.com/Article/details/gikbgleyr.sHtML


<!-- 参考信息 -->