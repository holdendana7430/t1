代发 wailian999

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gzmqqncll.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzkrspke.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjrgtoie.sHtML

document.querySelector(".item")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjwssuyt.sHtML

[U101] JS：classList 操作
来源：http://3g.fanxiaobao.xyz/Article/details/gzyileisa.sHtML

el.classList.toggle("active")
来源：http://baike.fanxiaobao.xyz/Article/details/ghjihvfmg.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhsrbrqz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fanxiaobao.xyz/Article/details/glokffwie.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/giapwldia.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fanxiaobao.xyz/Article/details/gsrqgqdov.sHtML

[U104] JS：防抖
来源：http://mobile.fanxiaobao.xyz/Article/details/gtypcxsus.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gyockiimm.sHtML

[U105] JS：节流
来源：http://blog.fanxiaobao.xyz/Article/details/gzuwutspz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gedgfhskp.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gpelgslqh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fanxiaobao.xyz/Article/details/gvnmojakw.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoogljeq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/glhqxzmzg.sHtML

[U108] JS：随机整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtopokgv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fanxiaobao.xyz/Article/details/gudnibmoj.sHtML

[U109] JS：数组分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfdfpvjl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gzeqsljxj.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyvplbnr.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gzdqgreit.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgzsrfxb.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqmjbcgu.sHtML

[U112] JS：字符串补位
来源：http://blog.fanxiaobao.xyz/Article/details/gmihebrcr.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfduvnqls.sHtML

[U113] JS：正则替换全部
来源：http://baike.fanxiaobao.xyz/Article/details/ggcxqsnra.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxkimxsw.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gberpgbal.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhkjdsfl.sHtML

[U115] JS：生成 UUID
来源：http://3g.fanxiaobao.xyz/Article/details/gntcfeuxg.sHtML

crypto.randomUUID()
来源：http://baike.fanxiaobao.xyz/Article/details/gktpdobje.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fanxiaobao.xyz/Article/details/gifbetmwa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gsjmppokm.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gyyiuyapa.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fanxiaobao.xyz/Article/details/glrzzppcu.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsdsysebc.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiooygof.sHtML

[U119] JS：生产构建
来源：http://wap.fanxiaobao.xyz/Article/details/gxshxehtl.sHtML

npx vite build
来源：http://3g.fanxiaobao.xyz/Article/details/gkapswhrc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fanxiaobao.xyz/Article/details/gmryivtwj.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fanxiaobao.xyz/Article/details/gogjuvvxi.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxknlcmy.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcmocwqk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glkkuseub.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gevptctve.sHtML

Python ......... 252
来源：http://mobile.fanxiaobao.xyz/Article/details/goqfugufo.sHtML

PHP ............ 252
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsctdutq.sHtML

JavaScript ..... 252
来源：http://wap.fanxiaobao.xyz/Article/details/gxxyuingb.sHtML

TypeScript ..... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gprnadsxf.sHtML

Java ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gkbardxth.sHtML

Go ............. 212
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpeukqcq.sHtML

Ruby ........... 212
来源：http://blog.fanxiaobao.xyz/Article/details/gzmqhrhzw.sHtML

C# ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/ggxmgfsnl.sHtML

C .............. 30
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqobqenrc.sHtML

C++ ............ 30
来源：http://wap.fanxiaobao.xyz/Article/details/ggwhgrskr.sHtML

SQL ............ 90
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbzsljoq.sHtML

Bash ........... 80
来源：http://baike.fanxiaobao.xyz/Article/details/gfxczwlzr.sHtML

Kotlin ......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/ghcpdxsgh.sHtML

Swift .......... 15
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjpjdjut.sHtML

Lua ............ 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gwruljfcq.sHtML

Perl ........... 10
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwchzwqw.sHtML

Scala .......... 10
来源：http://baike.fanxiaobao.xyz/Article/details/glosxzjdt.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/glaenkpwt.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gedwezxqg.sHtML

按章节统计：
来源：http://wap.fanxiaobao.xyz/Article/details/gzilnfddq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fanxiaobao.xyz/Article/details/gcwhaitxh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/galrruloz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgifeylc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrpzciuz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgvckwgh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaugxvosg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxnalsaf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fanxiaobao.xyz/Article/details/gsiytxvxr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gquyjgndp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gshushbgd.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdjtgpry.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdukpqiav.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gfghuyalm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fanxiaobao.xyz/Article/details/gprptmpzl.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gydlgbijs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesddzedd.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhuvhcav.sHtML

R Bash 专题                             80
来源：http://mobile.fanxiaobao.xyz/Article/details/gwogxxdwy.sHtML

S C / C++ 专题                          60
来源：http://read.share.fanxiaobao.xyz/Article/details/gboonfzdk.sHtML

T 其他语言补充                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gggmaousq.sHtML

U 高频实用片段                         120
来源：http://blog.fanxiaobao.xyz/Article/details/gytoooveq.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhrlcptw.sHtML

合计                                  2106 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbvtqwlf.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlrockqi.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gkeoykfze.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gksfoykia.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhxzlstn.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fanxiaobao.xyz/Article/details/gtogltpit.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfoirqum.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgqgcvrd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/goejuxkfl.sHtML

—— 文件结束 ——
来源：http://blog.fanxiaobao.xyz/Article/details/gaflylgug.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glfhbifrd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.fanxiaobao.xyz/Article/details/gqqbqxrbv.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fanxiaobao.xyz/Article/details/girsnbsxe.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwjnbmsv.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/gqxxcgdzm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fanxiaobao.xyz/Article/details/gaaxcnrzk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.fanxiaobao.xyz/Article/details/gntlbvntw.sHtML

SQL · Bash · C · C++
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwkzpgiz.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gzydxsjof.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gadklnadb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvzwpyng.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbvsbfzw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fanxiaobao.xyz/Article/details/gozsjmimx.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeiesudq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gucmkokrh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fanxiaobao.xyz/Article/details/gqsidaoyg.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlqahizh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzhufkhp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fanxiaobao.xyz/Article/details/gcqboocag.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmmomzes.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gdszbafvb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqahfodjp.sHtML

【文件统计】
来源：http://read.share.fanxiaobao.xyz/Article/details/gitdphatb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fanxiaobao.xyz/Article/details/geizrxmvx.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gsmnsgedm.sHtML

目  录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpykqpopx.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkylqabl.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gomkdrgdb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gspcwzvhj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqkogzgl.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gkjjpgdlo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fanxiaobao.xyz/Article/details/galacrjmc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gezqydknq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gieaeyjah.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gbggztpwb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/grqnnuajg.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfhdmmag.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gribozfle.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gxzqycuim.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlderbax.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gihbexfdz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/giuncyrcu.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gduutgviv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyskkpcp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gejdvmjit.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuhucqmd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgjpxdyc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gzwyqrhqg.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/goedhwxfn.sHtML

A. 基础语法与类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdypcvbe.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gstdkhxno.sHtML

[A01] Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtwokenz.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqsfknif.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fanxiaobao.xyz/Article/details/gksddjcsm.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/grinwlxec.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/goavobuwv.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpxbevbf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/gxpcfihjt.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fanxiaobao.xyz/Article/details/gaorbvhom.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuxpxqru.sHtML

[A02] 变量声明与赋值
来源：http://3g.fanxiaobao.xyz/Article/details/gllemsrxc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmwcddnw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlipqroj.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gyhtfstrs.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gbllzysbs.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdszsnjfg.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fanxiaobao.xyz/Article/details/glnsezwua.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.fanxiaobao.xyz/Article/details/gepinpuhq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqusadmzr.sHtML

[A03] 常量定义
来源：http://wap.fanxiaobao.xyz/Article/details/gjaeoptmn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fanxiaobao.xyz/Article/details/govjhbqth.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrnfcibe.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglqpyfoe.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/ghkobaiei.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhdnczoo.sHtML

Go:   const PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/gaghijsdt.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghppgbvze.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/ghgelprte.sHtML

[A04] 判断变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/giibeuckh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlohzuac.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fanxiaobao.xyz/Article/details/gnheyzvje.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fanxiaobao.xyz/Article/details/gvtnhplqz.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjfxsgjs.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fanxiaobao.xyz/Article/details/gvlwwylhj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghatvmejf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fanxiaobao.xyz/Article/details/gzjthljwp.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fanxiaobao.xyz/Article/details/glnhpnomm.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqakfdim.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gtivkebak.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/ghpbmxnno.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/gexlfjbak.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/gidamhmiq.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.fanxiaobao.xyz/Article/details/guffugzbt.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/guqxqrkvc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxnniyho.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcszungo.sHtML

[A06] 字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbfhwjxp.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbchcnfwm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gborctihs.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikmyaaqt.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfxqnplj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonwzlrnn.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fanxiaobao.xyz/Article/details/gaimrukio.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fanxiaobao.xyz/Article/details/gwfzqnfxi.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gqmqfvexm.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrviiews.sHtML

Py:   str(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glihlokin.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gakdzbgii.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fanxiaobao.xyz/Article/details/gcjiquumx.sHtML

TS:   String(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhwrsabt.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gyhupgmao.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gywabiibx.sHtML

Ruby: 42.to_s
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjksazzi.sHtML

C#:   42.ToString()
来源：http://baike.fanxiaobao.xyz/Article/details/gfgjvebqk.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjippqmzz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwpvsmpy.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsevuevaq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuvylzaa.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbmrdlth.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gnpfsidfj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://3g.fanxiaobao.xyz/Article/details/gztrruxui.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllebxttr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnphzeijf.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gshmelibl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gyrtttipt.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/glabgicez.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyjcvqlc.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gbdwoeixo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhjnxwsw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmckalyvp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmydiojg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggnapfwya.sHtML

[A10] 生成随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gorezteoc.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.fanxiaobao.xyz/Article/details/gmkqqjips.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fanxiaobao.xyz/Article/details/gxlpglfvq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.fanxiaobao.xyz/Article/details/gwbrvvmmx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fanxiaobao.xyz/Article/details/gkpgbcbgb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ggocheyzd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.fanxiaobao.xyz/Article/details/goulsqrqt.sHtML

Ruby: rand(1..100)
来源：http://3g.fanxiaobao.xyz/Article/details/greonhorx.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrksaphr.sHtML

[A11] 条件表达式（三元）
来源：http://blog.fanxiaobao.xyz/Article/details/gzrkwagwy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqoumnxd.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/guigcluyr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/grlekyhwr.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gedepzeit.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gykuwtuad.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcflymwnf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxcskqss.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjecvhkn.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gquyigwat.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fanxiaobao.xyz/Article/details/gnqucvqrp.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fanxiaobao.xyz/Article/details/guqsseokk.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtodzxjr.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswqnusfo.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fanxiaobao.xyz/Article/details/gsbsqisoj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gkxkwxyuc.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjhrfuou.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.fanxiaobao.xyz/Article/details/giciwgvqh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fanxiaobao.xyz/Article/details/grrxipths.sHtML

Py:   "第一行\n第二行"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfzxjtwy.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsdnbfhw.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fanxiaobao.xyz/Article/details/gmemwiusc.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fanxiaobao.xyz/Article/details/geixrahjm.sHtML

Java: "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmdlgrjy.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fanxiaobao.xyz/Article/details/geqixbyaw.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkgxswia.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcggfiext.sHtML

[A14] 注释写法
来源：http://wap.fanxiaobao.xyz/Article/details/gnrkbxdwt.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.fanxiaobao.xyz/Article/details/gvdmuufgn.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtgfqvkc.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.fanxiaobao.xyz/Article/details/gualdaler.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.fanxiaobao.xyz/Article/details/geubudenq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.fanxiaobao.xyz/Article/details/glvqcjovu.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszvcnyfx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://m.share.fanxiaobao.xyz/Article/details/grtrppjic.sHtML

C#:   // 单行；/* 多行 */
来源：http://3g.fanxiaobao.xyz/Article/details/gmwluqivs.sHtML

[A15] 空值判断与默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnzzmspd.sHtML

Py:   value = data or "默认值"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrfidxmt.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gmyekehyv.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/gokjohfah.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghblioejo.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.fanxiaobao.xyz/Article/details/gjolbnuhr.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzipumqij.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdkmqfle.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.fanxiaobao.xyz/Article/details/gfnencdmk.sHtML

[A16] 真假值判断规则
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgnvicvn.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.fanxiaobao.xyz/Article/details/gfozgsqqc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.fanxiaobao.xyz/Article/details/garlyzivm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzeqpoye.sHtML

TS:   if (!x) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyxchaxz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/grgyiaaum.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fanxiaobao.xyz/Article/details/gitsmptiu.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.fanxiaobao.xyz/Article/details/guucbidit.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcqyepqr.sHtML

[A17] 位运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfwtmitm.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlpqhzqt.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.fanxiaobao.xyz/Article/details/gsxvuoepr.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdcltfhyf.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxpxihom.sHtML


<!-- 参考信息 -->