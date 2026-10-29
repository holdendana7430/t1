代发 wailian999

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gxjtozdvi.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gzkodjzgn.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/grsoznfqx.sHtML

document.querySelector(".item")
来源：http://www.share.zdbjq.cn/Article/details/ghwlyfcdu.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/glmprdzra.sHtML

el.classList.toggle("active")
来源：http://3g.zdbjq.cn/Article/details/gwvuacgqq.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/gsylhwdpv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gnpopeybt.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gkeqrlomy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.zdbjq.cn/Article/details/gvwytenxm.sHtML

[U104] JS：防抖
来源：http://wap.hesvh.cn/Article/details/gapyvgflq.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.hesvh.cn/Article/details/gvfyzgvpo.sHtML

[U105] JS：节流
来源：http://read.share.zdbjq.cn/Article/details/gkyuucouq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gppkdyrls.sHtML

[U106] JS：日期格式化
来源：http://3g.hesvh.cn/Article/details/gfedvsjej.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gvapevipx.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/ghhfibqkd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gcqtmccsb.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gnumijsjz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gsodqixxg.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gqszqkknv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gzuqnvvfp.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/geoehctzb.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gntkhwwgr.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/gtiksrshq.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gcegbrbvk.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gppepwtts.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gaeqewwrh.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gtztdjdkp.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gdzjqehxu.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gzsqwrqbo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gzuouufmh.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/gloptwgnq.sHtML

crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gqekypswp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gedrpsdpf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gmvrxboop.sHtML

[U117] JS：单元测试
来源：http://baike.fehbvm.com/Article/details/ghhzhbgxh.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gavfcfznk.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gvzqobfqg.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gzrpqzpoq.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gnvtlecyw.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gvwlxaogs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gaqeasekk.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.zdbjq.cn/Article/details/gqhcxatyg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqpjwpijy.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/gztfdyihw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gayiycyqj.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gxwjdhuke.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gypbxlcfy.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gmgyntnqi.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gdoikruvb.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gerwgvqjw.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gitbaxhdv.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gyxjjthrl.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gioogvocz.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gykqufraj.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/grttowcnb.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gpeocoqvu.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gwclrdigh.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gnqrronnk.sHtML

Kotlin ......... 15
来源：http://wap.fehbvm.com/Article/details/ghzgjfcib.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/gnzcckkjg.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gzzwmhpwk.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gikanzasf.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gsvlsksfp.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/geuqxhjmg.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gessjcyqe.sHtML

按章节统计：
来源：http://blog.hesvh.cn/Article/details/gsevhprmu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gfzbsodpw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/glazalngk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gseomhill.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gncjhqhzi.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gvsbmxbia.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gjinowbdr.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/grjcxtssd.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gfukfqgvr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/goeukgrkx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gresdsjqi.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gwdpolpnm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gsqqgsghy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gdgmuiuux.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gdaxtijby.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/galsmjhth.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/grhoaacdm.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gsdjlvjst.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/gwglvntsm.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gzvgcovij.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gisymukzq.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fehbvm.com/Article/details/gyojckwks.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gczihbvmo.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gfycwwrzm.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gwadijdep.sHtML

使用提醒
来源：http://baike.hesvh.cn/Article/details/gfgyfcomr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/ghjpnafva.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/geadhgyxn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gimewgfdh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/gbvdoktik.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.hesvh.cn/Article/details/gkfiezwpa.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gjrjhiejz.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gikbfrpwg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtdwzygcm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gpkeahpdn.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gorfuxzzk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gynnoefai.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/gvwzsqmog.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gyhnqflsg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gymafivkz.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/gqrznibwu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gkhxdppvj.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/ghbcrbxdd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gqugxinlb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/grvynvdvl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fehbvm.com/Article/details/gdphdpbsi.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.zdbjq.cn/Article/details/gaokruztg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/gdnxfoyke.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/gmerfmwix.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/ghcrudmju.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.zdbjq.cn/Article/details/ghkxmhlwx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/glwpkjahv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gjfxgbxgh.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gywwflngr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gtnyiohxt.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gzlmweebf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.hesvh.cn/Article/details/gtvhkzuch.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gkrvmpxlj.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gvtygxsmt.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gzsxbqqtg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/garzmkcyj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.fehbvm.com/Article/details/glctgichb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gssqnjlua.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gwanhsaok.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gejfbjtwn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/giwxxvgkp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gldvjvrjv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gidbxsgzd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gyysjbszi.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gshnaydqp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gwshyxxaa.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gxldbwacl.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gbnnyaywu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gweuuofxz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gsuoujbrv.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gxfrvusin.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ghizetwoq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gqgvhcsfy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gadqkmkbo.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/geihwdjjv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/gkwonvkvu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/giudzmgeb.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gphfimrkp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnaoxewhw.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gkifencjg.sHtML

Py:   print("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/ghrpkkqtr.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gwkgebhca.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gmvszlijp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gzldruceq.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/ghrijlrru.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gfzwbjjnh.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gobyhfyey.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gfzshfmvc.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.hesvh.cn/Article/details/gksaxivmn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/gpnmikfuz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gahkjyvoa.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gtkgfzvwu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gflphwrrs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/genxsjvif.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gubbtbhah.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gzjuiwidj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gpckctlfy.sHtML

[A03] 常量定义
来源：http://www.share.hesvh.cn/Article/details/gjwifanhj.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/gwtikierf.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/govxhsdvv.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gfuokanxo.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gcjdqejps.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gmpmfhnrc.sHtML

Go:   const PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gmdvrnmjs.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gdtxaitnp.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gtvldsvkd.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/grywnyvfk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gugoxbylo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.hesvh.cn/Article/details/gqnulowfi.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/ggnktposj.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gsjsiysib.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gwnszcpag.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gpyvhcftj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.hesvh.cn/Article/details/gqtpkzehy.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.fehbvm.com/Article/details/gkxznorfg.sHtML

[A05] 整数除法与取模
来源：http://mobile.hesvh.cn/Article/details/girxucljm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.hesvh.cn/Article/details/ggbibaziy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gbkqbvgov.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gwhyfuyad.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gljhaybmp.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gsulsarvg.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gchphfyux.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gchrxshlb.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.fehbvm.com/Article/details/gfztvurur.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gxihmhift.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gbhchhgje.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.hesvh.cn/Article/details/gxgrtyxsp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gjcnztssk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gtlrmtfkb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.hesvh.cn/Article/details/gxsrqleev.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gsydgtgzi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/grvdkvypk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gnwrmdvbp.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggenqzcoi.sHtML

Py:   str(42)
来源：http://baike.hesvh.cn/Article/details/gsiraufhk.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/gavfyaisn.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.zdbjq.cn/Article/details/gqumhcmmt.sHtML

TS:   String(42)
来源：http://www.m.share.zdbjq.cn/Article/details/guareiheg.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fehbvm.com/Article/details/gnldlffvr.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.fehbvm.com/Article/details/ghowbexwe.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gwvqpcyld.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/gzyluuirq.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/gebeihoco.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gnodlwcgg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.hesvh.cn/Article/details/gkhmcmvog.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gnglrcslz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fehbvm.com/Article/details/gchxwcobf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gjohrhvpd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/giauhrfad.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.fehbvm.com/Article/details/gqrtycloj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gahnfqkqz.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/gbnkzrlow.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gxdwrsjvg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gohtauusa.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gzgyuivnu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gkwpnczxh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gzotndvwx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.fehbvm.com/Article/details/gatokqhcx.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gxlwcpkdo.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gqodhpaux.sHtML

[A10] 生成随机数
来源：http://www.blog.fehbvm.com/Article/details/gqzijyohm.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gujgweand.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.fehbvm.com/Article/details/gkjbhrppu.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gfiqubolg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gxadecacj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gljacreot.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.zdbjq.cn/Article/details/ghxppbaxo.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gcpzmeuby.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.zdbjq.cn/Article/details/gnxcqvsdk.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.zdbjq.cn/Article/details/gzoilmhon.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.zdbjq.cn/Article/details/gludybsya.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/ghurccmvn.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gyfmitypx.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gmmhcihzs.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/grbwfmnfx.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.hesvh.cn/Article/details/gnhvyvxuh.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/ggzhcxvmt.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gidshsceu.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.share.zdbjq.cn/Article/details/gxpxntoxi.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.zdbjq.cn/Article/details/gsqyotsht.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.blog.hesvh.cn/Article/details/gedgpxplt.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/grfrspept.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gptdafaio.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/gzfvjejjl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gpkxlgpkz.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gtrrlzjuz.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.hesvh.cn/Article/details/gmzpogbme.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/gqoreibzy.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gerwqxtjz.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/gwzrbmbfl.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gminwsyvp.sHtML

TS:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gqbafjmms.sHtML

Java: "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/gmoegxtiz.sHtML

Go:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gpcgwplyz.sHtML

Ruby: "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/gjjdkglil.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gomtalaut.sHtML

[A14] 注释写法
来源：http://m.share.hesvh.cn/Article/details/gzhqzrpfs.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.hesvh.cn/Article/details/gvozklmck.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gbutbpbcu.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/glteafuyi.sHtML

TS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/grgjnznwd.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gufmjvipr.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/giwnctijv.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://3g.zdbjq.cn/Article/details/gpmzjmjyx.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gyqglvpww.sHtML

[A15] 空值判断与默认值
来源：http://3g.zdbjq.cn/Article/details/gysizuynf.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gsluvoafs.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gjmqokdlx.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gjlpeuenz.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gjyulfjyn.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://blog.hesvh.cn/Article/details/gywywghup.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fehbvm.com/Article/details/galyqbdel.sHtML

Ruby: value = data || "默认值"
来源：http://wap.fehbvm.com/Article/details/ggfkzbznb.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.zdbjq.cn/Article/details/gooisqyjh.sHtML

[A16] 真假值判断规则
来源：http://www.share.zdbjq.cn/Article/details/gstjxkcby.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.hesvh.cn/Article/details/glmcpiviq.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.fehbvm.com/Article/details/gqzsjezpd.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.hesvh.cn/Article/details/gmgeklfbe.sHtML

TS:   if (!x) {}
来源：http://baike.fehbvm.com/Article/details/gwdqoavla.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.zdbjq.cn/Article/details/grricwcho.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.hesvh.cn/Article/details/gpjqondvt.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.hesvh.cn/Article/details/gsbuyaorx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gyjpuzlqd.sHtML

[A17] 位运算
来源：http://read.share.zdbjq.cn/Article/details/gbwpwzwop.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gthhvjhvq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.zdbjq.cn/Article/details/gzmedahem.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gkylxjnmi.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/gzfnjqklu.sHtML


<!-- 参考信息 -->