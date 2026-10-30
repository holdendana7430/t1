代发 wailian999

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbunpdckt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlqivtnh.sHtML

[U104] JS：防抖
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrkgrejo.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiglbufs.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmsumgon.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfojqybio.sHtML

[U106] JS：日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/giyqfpekk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gnpcwbyga.sHtML

[U107] JS：数字千分位
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpqsmwud.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggglifbrz.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gasvnzjqg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaqlptaj.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gutbdxmrs.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gunexyhay.sHtML

[U110] JS：数组分块
来源：http://blog.fanxiaobao.xyz/Article/details/gtkdpokvn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwnxbbin.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvxnfsao.sHtML

new Map(Object.entries(obj))
来源：http://blog.fanxiaobao.xyz/Article/details/gksoigcba.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/gndvmofvp.sHtML

"7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdykyife.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynrhyych.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gtnjuxedb.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fanxiaobao.xyz/Article/details/gyuxmtcxw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gfgkoylwb.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fanxiaobao.xyz/Article/details/goxygmhgi.sHtML

crypto.randomUUID()
来源：http://blog.fanxiaobao.xyz/Article/details/glfgcqrza.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnlduost.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkdxnctu.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gycxfhutz.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fanxiaobao.xyz/Article/details/gcdjqndwu.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goopnhnpc.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzvruddq.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/grypaccnv.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gqmqrvcde.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fanxiaobao.xyz/Article/details/gwqxbisqo.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.fanxiaobao.xyz/Article/details/guhefnnen.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gohiemoht.sHtML

统计汇总
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdptoyxmz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gwhpsgjlf.sHtML

按语言统计（条）：
来源：http://mobile.fanxiaobao.xyz/Article/details/gofalvurm.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/grqnergih.sHtML

PHP ............ 252
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genomfrms.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gfjxybyyy.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/glqnahnip.sHtML

Java ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/glnqyfdjj.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwtvcmsk.sHtML

Ruby ........... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrezlhxp.sHtML

C# ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtuwloni.sHtML

C .............. 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gakwqzhqo.sHtML

C++ ............ 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknnvzpeh.sHtML

SQL ............ 90
来源：http://blog.fanxiaobao.xyz/Article/details/gdlgdgnjc.sHtML

Bash ........... 80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiuiyyfw.sHtML

Kotlin ......... 15
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmpjitqh.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpqzzrzi.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/ghnhnqejf.sHtML

Perl ........... 10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdminwvyf.sHtML

Scala .......... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gecyapehd.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvazjndz.sHtML

合计 ........... 2106 条
来源：http://3g.fanxiaobao.xyz/Article/details/gcpevckxw.sHtML

按章节统计：
来源：http://baike.fanxiaobao.xyz/Article/details/gvuyplrud.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gjlancwuj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gvxqkaezy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gpcqhvfeh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gdbfhdldy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/grwtpbujv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/gezvcvzwj.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/ghvcafgiq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fanxiaobao.xyz/Article/details/gibtuqvmz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gwldgfxfd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnyajysw.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqvtplsw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcmtynou.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fanxiaobao.xyz/Article/details/gzbctuqsj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwzjbqpu.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkaavanh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmvzwfel.sHtML

Q SQL 专题                              90
来源：http://3g.fanxiaobao.xyz/Article/details/geayyqjgy.sHtML

R Bash 专题                             80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzqsgtbr.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgbsglnr.sHtML

T 其他语言补充                          60
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlqmkgty.sHtML

U 高频实用片段                         120
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvmyoeab.sHtML

------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoforesv.sHtML

合计                                  2106 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gozrtoiic.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gailhmywz.sHtML

使用提醒
来源：http://www.share.fanxiaobao.xyz/Article/details/gatewzgzb.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/geiagojgr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxahkxac.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fanxiaobao.xyz/Article/details/ganwyolcb.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpclvgkv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.fanxiaobao.xyz/Article/details/gincgkblj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fanxiaobao.xyz/Article/details/gcxwydrcz.sHtML

—— 文件结束 ——
来源：http://mobile.fanxiaobao.xyz/Article/details/gtughrhpk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaydcqzw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfygrnom.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fanxiaobao.xyz/Article/details/ghljzvfjs.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqawxjem.sHtML

【收录内容】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtazlasyx.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnbuoplk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/ghnuzzhgo.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gjthoftlo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzqynmgw.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrqiekel.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fanxiaobao.xyz/Article/details/gsqerarsa.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlsakvei.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.fanxiaobao.xyz/Article/details/guyedvppv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaxhceqn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fanxiaobao.xyz/Article/details/gggwjpyow.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgwmvlgr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpimceyu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fanxiaobao.xyz/Article/details/gbreugeow.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gchvwlpbl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqyvqptm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fanxiaobao.xyz/Article/details/gdddqkutt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fanxiaobao.xyz/Article/details/gdhyegbdn.sHtML

【文件统计】
来源：http://blog.fanxiaobao.xyz/Article/details/gnbxxqiwt.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvxgagjk.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvvaczix.sHtML

目  录
来源：http://www.share.fanxiaobao.xyz/Article/details/geqjnvxxw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fanxiaobao.xyz/Article/details/gfqbjsuyw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gvzkwtwkr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gblljfvgr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gtgpthyqi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.fanxiaobao.xyz/Article/details/giosoyejc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxmdfiuy.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gdtyoeorg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxsbtcar.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpxkkhok.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gceelgtlq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnqvpknl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaejndvv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/ggqdepljp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcblyfap.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gsvwfkqjw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gvrkstjmf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzhutkyc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtdpolod.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaeqghbe.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fanxiaobao.xyz/Article/details/giitbmdpa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gjliddxis.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/glucdxcuc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gcizdtiqr.sHtML

A. 基础语法与类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gelnhhwpl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grsomdomq.sHtML

[A01] Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ghzevbbrg.sHtML

Py:   print("Hello, World!")
来源：http://blog.fanxiaobao.xyz/Article/details/grciqwxnj.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbongqlw.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gadrvdegw.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxahepszf.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glehavdoh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcovgwfxd.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzfqmmeo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/gapgvmmqx.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvnthgus.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fanxiaobao.xyz/Article/details/guusifxmy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gutchvkms.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcevqjbxm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggphaqrwp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbllglylq.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fanxiaobao.xyz/Article/details/gojpnpflk.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltijsgkx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fanxiaobao.xyz/Article/details/govqtxwkt.sHtML

[A03] 常量定义
来源：http://m.share.fanxiaobao.xyz/Article/details/glkhljmfi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fanxiaobao.xyz/Article/details/gbyacpzoo.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmxrhhhm.sHtML

JS:   const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/ggxvzaeoi.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmbmrhkk.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ghthebvsr.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqciafdyi.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnskciwk.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxvuhchi.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijhwqocf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fanxiaobao.xyz/Article/details/gmblcybeo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gemflpxyq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcpvcelg.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gqpyruize.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fanxiaobao.xyz/Article/details/grrgzitfk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fanxiaobao.xyz/Article/details/gzhjudhkb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.fanxiaobao.xyz/Article/details/guwdwxepy.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoccfetu.sHtML

[A05] 整数除法与取模
来源：http://3g.fanxiaobao.xyz/Article/details/gjdepkkhu.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsqeijnr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gwbkdoqfw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gdejvanxk.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitgxczax.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxkgxynzd.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksloanks.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejxedfgj.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzmxxebf.sHtML

[A06] 字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/geyuusjwj.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqdiyyfy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/goeiaybjq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.fanxiaobao.xyz/Article/details/gtdxologa.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.fanxiaobao.xyz/Article/details/giqtyalzj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgfwisoz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fanxiaobao.xyz/Article/details/gjfizzjtc.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsqjxyam.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjjjaymm.sHtML

[A07] 数字转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gorrkmxlr.sHtML

Py:   str(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gwrrxrlhf.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.fanxiaobao.xyz/Article/details/grszwhxbf.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfeyjmod.sHtML

TS:   String(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gwgyooyqj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gbgnjyfqt.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gvonlodjf.sHtML

Ruby: 42.to_s
来源：http://3g.fanxiaobao.xyz/Article/details/gllrcptcd.sHtML

C#:   42.ToString()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrsaqvck.sHtML

[A08] 取整与四舍五入
来源：http://wap.fanxiaobao.xyz/Article/details/gmuuhtrha.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/ggfolsbzg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fanxiaobao.xyz/Article/details/gzbdbnpfq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/geedhkuvc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fanxiaobao.xyz/Article/details/grjufusoa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gtkrcecuz.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.fanxiaobao.xyz/Article/details/gyyznzpdd.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.fanxiaobao.xyz/Article/details/ghanlvpsz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpjdquzg.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gkckpcqkf.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaawumobr.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gycgyttio.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/ghiuifqyv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqnocspq.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpqpwqhb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobnrmqxi.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gichuquie.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkncekln.sHtML

[A10] 生成随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqadjmmj.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fanxiaobao.xyz/Article/details/gonnduafo.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxuqoebam.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxwtzbyu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gigmwrgds.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfqlgtan.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fanxiaobao.xyz/Article/details/gsttrhgdk.sHtML

Ruby: rand(1..100)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzppnyzlz.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtdjdssp.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fanxiaobao.xyz/Article/details/gwnhxonpd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdxjmsnx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgjklauu.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakprtkaa.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gniitiwgw.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzzuhmwm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gekkiyhmo.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxyixhpq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkjzlrtb.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrjjgbqu.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaafqqmtc.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhxkpikx.sHtML

JS:   `Hello, ${name}!`
来源：http://3g.fanxiaobao.xyz/Article/details/gdbmlamwj.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvpadiom.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnpjtdxq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gekotzpaf.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.fanxiaobao.xyz/Article/details/gsqdzxyai.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgzuyalt.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmievdcw.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fanxiaobao.xyz/Article/details/gniecpkfp.sHtML

PHP:  "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfyrldvg.sHtML

JS:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/gpotwnzwu.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/guhbjgarx.sHtML

Java: "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gusjhenoi.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/glrmxdvzf.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsxdvwsh.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gnwdecnkn.sHtML

[A14] 注释写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gudnronan.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://m.share.fanxiaobao.xyz/Article/details/gygwntanx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfmgzlky.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpibdlru.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.fanxiaobao.xyz/Article/details/gcbcugfob.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fanxiaobao.xyz/Article/details/grrulheax.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gvfhbzlfo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fanxiaobao.xyz/Article/details/geajhdyvp.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gcnevxftq.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmyyglhg.sHtML

Py:   value = data or "默认值"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcfykiyj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gdurmwclc.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/gguwpurgj.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsbpdliy.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fanxiaobao.xyz/Article/details/gujesvwcp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkljieawj.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhgsnbyy.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.fanxiaobao.xyz/Article/details/genccebsn.sHtML

[A16] 真假值判断规则
来源：http://m.share.fanxiaobao.xyz/Article/details/gykjpajlw.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://3g.fanxiaobao.xyz/Article/details/gfobvncpe.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fanxiaobao.xyz/Article/details/golmllavf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.fanxiaobao.xyz/Article/details/geggxinqg.sHtML

TS:   if (!x) {}
来源：http://3g.fanxiaobao.xyz/Article/details/ghakwnhsl.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gevrkfcdi.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://blog.fanxiaobao.xyz/Article/details/gixhzcznm.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdovixpma.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqnjghic.sHtML

[A17] 位运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcgjjcqy.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyyxopll.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozhnryla.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxjbkvvb.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gndztjvur.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/grptkcsxk.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/gjxpfbwyx.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxcqrycp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gljqcogjc.sHtML

[A18] 字符与 ASCII 码互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjmgrvky.sHtML

Py:   ord("A"); chr(65)
来源：http://read.share.fanxiaobao.xyz/Article/details/glgihgigf.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjhytlff.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gajqffhpw.sHtML


<!-- 参考信息 -->