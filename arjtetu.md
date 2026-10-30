代发 wailian999

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gfczghayp.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/grgvptcex.sHtML

[U102] JS：本地存储
来源：http://wap.zdbjq.cn/Article/details/gjeaklxwq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/ghritdqbs.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/guvciqebp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gnsovxvdh.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gyrrdlozv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gthnenemj.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gisdwjepb.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gkvsjhwbh.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gtylnyokk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.hesvh.cn/Article/details/gzptpiutw.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gttuycdcp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/glyeuvjlb.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gprymvpzp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.zdbjq.cn/Article/details/gyckpnzsy.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gxyjwthsz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/ggmyczyud.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/giwaxgmiz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gbpdtlvqf.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gmadondbl.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gfwsraxvr.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gnmcuueuv.sHtML

"7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/googphncl.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gfaakzgrk.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gtiyhvmut.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gyljzdmun.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/gyyabacvq.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/ghfvatyur.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gdbahfcnc.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gdgpkwryj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gxnxnbuse.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gcyrfierg.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gqdxebhor.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gsyylirnh.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gxsmghzqh.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gdgfbngoh.sHtML

npx vite build
来源：http://wap.fehbvm.com/Article/details/gxegptiqj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gjgsavmeg.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.fehbvm.com/Article/details/gfanpfvra.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaarjtnhd.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gatwylolg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gylenxrgl.sHtML

按语言统计（条）：
来源：http://mobile.hesvh.cn/Article/details/gkcicpexq.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gjnmcxpdc.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/glbebolww.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gwzkoznfi.sHtML

TypeScript ..... 212
来源：http://www.blog.hesvh.cn/Article/details/gydtqvimq.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gaxbmtodn.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gyamzvvcl.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gnaindfog.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/gtdoxlkbb.sHtML

C .............. 30
来源：http://wap.fehbvm.com/Article/details/ghdaeddaz.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gonzzcgyj.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gpudgjqoy.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gupfijule.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/glcqgnxvo.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gtgzgtgms.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gdzfhpjps.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gemxmtaly.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gakfkipne.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gmkqgflcs.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/gxejybhhx.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gdipcprup.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gfrdpyiix.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/gbsmfinyf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gunqowetw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gnmdkxbaq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gzunkmzof.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gnuuwsrso.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gkjueuozq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gjdpazvqd.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gsrzeeaos.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/geqmbbqng.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gaemxiyaj.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/giusedsnm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gfgpfbfjw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gntxzlahv.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/glnzpysyq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gdlcpoyyq.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gmzwvmpsr.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gtvpmavbx.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gfomxbuwj.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gqpaojups.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gujolhmsg.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gyxsogdky.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gsvwpufsg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gtdistlza.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gopiddeod.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gqyebtsaw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/grkrphtiq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gteecnsex.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/ganzbokop.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gtopvghyt.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/ghotybdfo.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gxgovgtpn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvshkblhf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gcijjaflu.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.hesvh.cn/Article/details/grecdwhex.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxcbzhwre.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gjagbwwvr.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gkenqdhnf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.zdbjq.cn/Article/details/gmurmjvol.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gxgicodnt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/glrkrcltp.sHtML

【使用说明】
来源：http://m.share.zdbjq.cn/Article/details/ggzfeaqoz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.zdbjq.cn/Article/details/gmoyjxtag.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gdfbbvctn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gmvgmwjdl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.zdbjq.cn/Article/details/gfejyuwzs.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gqfhfjdqj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gfngsyxwo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gezondbey.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gntdntufd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gwmebcojk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gfmeqtcpi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.fehbvm.com/Article/details/glplpieaw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.zdbjq.cn/Article/details/gdyprlakr.sHtML

【文件统计】
来源：http://baike.zdbjq.cn/Article/details/gurohzgre.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gjysgzwbr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gpknqqeas.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gszihnyrn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gmsznztao.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/ggyymguwl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gnaenzqvb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gwaeyzjxv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/ghelxiovk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gxejpgozk.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gwshcsoux.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gzabsjzvw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gllvlclei.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gktqjgabc.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gmgzuxukg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gvkywmykw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gvvclhmok.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gomddlilv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gtjsdlxeh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.zdbjq.cn/Article/details/gzksjnpil.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gulodolqv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gxqkzluri.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gnbmsupwx.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/ghmyhawow.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.hesvh.cn/Article/details/ggecwsati.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/gfkyxmlif.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtanyoxkd.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/gisogmwlz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdbbkslyq.sHtML

[A01] Hello World
来源：http://www.share.hesvh.cn/Article/details/giugogaso.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gnjsufduh.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/geloscokm.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gdkbscssy.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/ggxhsdqrz.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gnwlxfdzz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gqbbsfgik.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/gomrzbhfo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gtfiyukch.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gbmtdrfun.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.zdbjq.cn/Article/details/gdkuvvsxi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/girfwfftx.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/ghdkesodw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gagjzefhq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gyofmruss.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gjsegfhqk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gkgbwbemh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gzrzxivvs.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gqntzojzu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gxbungcyh.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/ggndvxzpd.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gwifkljcq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gkstaidmb.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/ghjosmdcx.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gcemlpybf.sHtML

Ruby: PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/greeyahxb.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gmcvbkgvk.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gcububfwn.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gesgxzuhh.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gbfwiqsgp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gbjggqokf.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gueofivop.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.fehbvm.com/Article/details/gwomutzzv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gikysvnyy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.zdbjq.cn/Article/details/grhephumd.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/gdjuuylqo.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/gjsgczzhh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gfxeidpnl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gykpxzprn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gijejvqgz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gwksmboyv.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gteawceew.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/geisxhlxa.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/guevdnagq.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gexufbejb.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/gbbgzypdb.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.fehbvm.com/Article/details/gpqrdmlua.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gmzpaljpw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/glyizecny.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gaozygckt.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gelgefxmp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.hesvh.cn/Article/details/gwnyfsgic.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/gqzsekkwe.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gktbdpzrm.sHtML

[A07] 数字转字符串
来源：http://m.share.fehbvm.com/Article/details/gekmltocv.sHtML

Py:   str(42)
来源：http://mobile.fehbvm.com/Article/details/gvxyecnae.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.hesvh.cn/Article/details/gcphbkdib.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gjukiahng.sHtML

TS:   String(42)
来源：http://www.blog.zdbjq.cn/Article/details/gtskmoawq.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gbyxyxpur.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gnttrytod.sHtML

Ruby: 42.to_s
来源：http://read.share.fehbvm.com/Article/details/gxuxuhwdn.sHtML

C#:   42.ToString()
来源：http://3g.hesvh.cn/Article/details/gmnhgzjgt.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gzgdgvucv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gfoiewztt.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.hesvh.cn/Article/details/gccuimhhs.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gctskqdge.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gblignckz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gnxlwlmle.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gtlklzevy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/gxywltixz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gniwzxike.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gbqfbhgbd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/ggxkdionr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gdlunnanv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gmzzbqbfa.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gcbnjmadh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gizhmbqdb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.zdbjq.cn/Article/details/grulhteef.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gwdeeptrv.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gliodgoex.sHtML

[A10] 生成随机数
来源：http://blog.zdbjq.cn/Article/details/gpouzgfey.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fehbvm.com/Article/details/gmidbvinh.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/ggirmhvyc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/gdcbidpxh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fehbvm.com/Article/details/guyrxlcdk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.hesvh.cn/Article/details/gumkuvcsp.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gjlxhlbmz.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/gicbpnhbp.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.hesvh.cn/Article/details/gmtibdgyx.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/gkcmqrkuq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.zdbjq.cn/Article/details/goyhzkszf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gvooaihkq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gdcskapns.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gtbqxcuyw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gdiyyjdpm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.zdbjq.cn/Article/details/gcalseqcr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/ggvaovuhj.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gxfnoarfq.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.zdbjq.cn/Article/details/gwvtpwkwy.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.zdbjq.cn/Article/details/gknqcwymy.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.zdbjq.cn/Article/details/gumlzfwub.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/gpvnlpmuh.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gjjfahrao.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.zdbjq.cn/Article/details/gfouecsfe.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.hesvh.cn/Article/details/gdxzballh.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gjpjnywvv.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.fehbvm.com/Article/details/gqismnyco.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.hesvh.cn/Article/details/gbelpkpbr.sHtML

Py:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gzotmsark.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gqbhlhjvk.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gyfsxubjf.sHtML

TS:   "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gklkgtzig.sHtML

Java: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gnqjnakit.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/glwaqjbrs.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gscrfkqkk.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/glvcxymjc.sHtML

[A14] 注释写法
来源：http://wap.fehbvm.com/Article/details/gbjrtioys.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gsthfxlmt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gfavhlcqq.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/ggvajbexa.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gllbiclyw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.zdbjq.cn/Article/details/gimkhhbcj.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gasslproo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fehbvm.com/Article/details/gqvaqnehq.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gnykpsfcj.sHtML

[A15] 空值判断与默认值
来源：http://3g.hesvh.cn/Article/details/guzudjdxc.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gjhhplvde.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gpzxjbkzl.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gnyotwwcq.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gneqjqsvy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.hesvh.cn/Article/details/gtzmxoogz.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.hesvh.cn/Article/details/gqjgujnef.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fehbvm.com/Article/details/grnhxvsrj.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gburelbss.sHtML

[A16] 真假值判断规则
来源：http://read.share.hesvh.cn/Article/details/gwqzivzqp.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.hesvh.cn/Article/details/gntkvzlmm.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.hesvh.cn/Article/details/gyskucpno.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/gzedvydwe.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gpizovjfh.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmuwsvwvn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fehbvm.com/Article/details/gydgdhnbz.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fehbvm.com/Article/details/gszwrefoh.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.hesvh.cn/Article/details/glzmyeakl.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/gznxgxvho.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gewyghxlc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.hesvh.cn/Article/details/ggetyztwu.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gsesgeesg.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gzovtbiwy.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gpiloggwh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gxyjubpeg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gfwpajygf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fehbvm.com/Article/details/gstzuocfr.sHtML


<!-- 参考信息 -->