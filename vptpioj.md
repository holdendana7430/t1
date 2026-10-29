代发 wailian999

[U97] JS：并发请求
来源：http://www.share.zdbjq.cn/Article/details/gluhjjwlc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gsspjnqmt.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.fehbvm.com/Article/details/gjhtvixqj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gcarvvteh.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gnoiudlgo.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/gmtxjbjdq.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gxouvytbt.sHtML

document.querySelector(".item")
来源：http://blog.fehbvm.com/Article/details/ggudfaohk.sHtML

[U101] JS：classList 操作
来源：http://www.share.zdbjq.cn/Article/details/gjremswir.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gblnftbkh.sHtML

[U102] JS：本地存储
来源：http://3g.hesvh.cn/Article/details/gdrkojptw.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gnwvtjhdj.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gcmspixgo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gfrynhput.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gqawkwapc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gawsjfnqs.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gzaismtpq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/ggxsrrbdj.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gjzrbxtel.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/ggwcxehaz.sHtML

[U107] JS：数字千分位
来源：http://blog.hesvh.cn/Article/details/gohhalxqa.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gyenrzlqd.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gmsxvcnsf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gkomhuqid.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gwulnwwvu.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gshqsagjb.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/guwygzvsl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gokvifabz.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gbpzembia.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gqqovrsjy.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gjoajvkcr.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gmbrxjkvy.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gxwearavr.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gaswlsidr.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gbottzkyz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gmvtcoibk.sHtML

[U115] JS：生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gzrtalvtv.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gapujjzcp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gholghhgj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gfzftcvdx.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gfhhnezqz.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gfjlejkmv.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gcvoahvtk.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gsnhwqxmv.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/geglyprze.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gdyvqnncs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.hesvh.cn/Article/details/gqrcchucd.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gawrrzehm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grmrvdmsk.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gatxzeyas.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzoijsadc.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/goroupzso.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gbdjsgjdl.sHtML

PHP ............ 252
来源：http://www.m.share.hesvh.cn/Article/details/gmggvsefi.sHtML

JavaScript ..... 252
来源：http://m.share.zdbjq.cn/Article/details/gwmclniij.sHtML

TypeScript ..... 212
来源：http://baike.hesvh.cn/Article/details/gzzibfmhw.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gfceevmoa.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/geqzpmxyw.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/ginzbkxij.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gxnlhjbjv.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gckkrmoxy.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/garhxbuls.sHtML

SQL ............ 90
来源：http://read.share.hesvh.cn/Article/details/gbinbumof.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/geznzpkzp.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gnmecbbpr.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gesxhkbqc.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gdypvcalr.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/ghuxecasw.sHtML

Scala .......... 10
来源：http://www.blog.hesvh.cn/Article/details/gwcdrifwn.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gvdsbhjuj.sHtML

合计 ........... 2106 条
来源：http://www.blog.fehbvm.com/Article/details/guamrkmtc.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/ganximjec.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gqzbyjrgd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gnzverkls.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gzsiudirq.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gwhotzjof.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gnvkcrxhw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gvnxuvgqq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/glhujgfaq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/ghqglmvty.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gbhhzdtfj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/grniiwlvg.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gxbhxsjvd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gufnhxbij.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/grmwdxsnx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gzuflrzzp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gmoavsqin.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/ghctvgtuh.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gpuwprdgw.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/giaweygpv.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/gqwghtopa.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gbhagkwev.sHtML

U 高频实用片段                         120
来源：http://mobile.hesvh.cn/Article/details/govghmehw.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gymucgfvs.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gzhfqnagi.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/glgvadoyr.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gdgxnvles.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gimtskxdc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.hesvh.cn/Article/details/giqbnvema.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.hesvh.cn/Article/details/gzwqzcsgt.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gzxmnsxzn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/glctpdrnd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/gntahhagp.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gtruftstd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gazjxoytv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fehbvm.com/Article/details/gngwtnejn.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gcqjxyuus.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbmkpuuvw.sHtML

【收录内容】
来源：http://www.blog.zdbjq.cn/Article/details/gvpvqzxmw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.fehbvm.com/Article/details/gxeakuube.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gkgotxcbl.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gneofspmu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gomhbvsdp.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/ggshcmwoy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.zdbjq.cn/Article/details/gafmapwzp.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gnzljuaeh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gfsrartxg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gozxkeosn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gorjfkqhu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gxrafdbzt.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/gxoxygkal.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/gogfbhmkf.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gladmeaeg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gpnacowxf.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gdritlnwy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gexgsbgpz.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gghsotapv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gcyoktfvq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gnavuenho.sHtML

目  录
来源：http://mobile.hesvh.cn/Article/details/gajjoikta.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gfatmphop.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gphkxdbze.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gxevodvjy.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gezcmlsth.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gxhrrsxpy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/goobvunil.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/ghmzzegdn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gfdvasrdi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gdklyavcv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gdgjnkvpb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/ghyhlrlda.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggleniian.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/girszlzse.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gzcervfrv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gncpkluyp.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gveztwjta.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gcdsgcotb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gvkaeudxw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gimhcrmpm.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.fehbvm.com/Article/details/guvcypzlf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/giahzqbrr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gcqawxmfl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpzdmadkp.sHtML

A. 基础语法与类型
来源：http://www.m.share.fehbvm.com/Article/details/gtgpljwag.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxmpghpqz.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gleludhqz.sHtML

Py:   print("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gaoungmkf.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gnrpeeyhh.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gokffqfcx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/geeivjplg.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gdwobgkgy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gvhewaawl.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gypvnvyzv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gcyelatxj.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gbjxqcnfc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gzdzngelw.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gocprciui.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gkoxrehzb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/gebmuuzlt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gouuhfkgn.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/gylvrvasc.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gmjeofken.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gchagtizv.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gfbekijiy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gkvfjzebw.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gxdsqelic.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gdwdgevtt.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gjdaqyual.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gukqgixbs.sHtML

Go:   const PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gtjikxyne.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/guhpftlbx.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gseafjkcn.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/gfjhesxds.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gzhhldhiq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gyziugedw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/gdqzayecy.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gokjvqett.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gvrsgjwzp.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/ggtamqjnz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gwuxhnols.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gegpsssol.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/gggsrytna.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/gxqthyzyk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.hesvh.cn/Article/details/ggofdqdpp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gtirkxkrd.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gyelmubhz.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gxxsdeuso.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gnvwkfeor.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gspeovpso.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gevzzoztr.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gnizwslxf.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.fehbvm.com/Article/details/gbfjqnjse.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fehbvm.com/Article/details/gowygvxhf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.fehbvm.com/Article/details/gfecqzuze.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gybplcuhb.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.hesvh.cn/Article/details/gzmbsdlvp.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/giggxbpyu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gdkoogeba.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wap.zdbjq.cn/Article/details/gzwupnacq.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/gozytyyxx.sHtML

Py:   str(42)
来源：http://3g.hesvh.cn/Article/details/gwespydvo.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.zdbjq.cn/Article/details/gzcmnyhlw.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gzafjnkrs.sHtML

TS:   String(42)
来源：http://m.share.hesvh.cn/Article/details/girnddymc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.zdbjq.cn/Article/details/gmyjemznz.sHtML

Go:   strconv.Itoa(42)
来源：http://www.blog.zdbjq.cn/Article/details/gwteszjxf.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gleqhuavd.sHtML

C#:   42.ToString()
来源：http://www.blog.fehbvm.com/Article/details/gncshqcot.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gmgubbmwn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gjlmmspav.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.zdbjq.cn/Article/details/gfjimujzr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gwufmjbfr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/glahysirh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/grylukvfe.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/ggbajpiim.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/gtleedyfz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/ggxmjvfok.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gszmuaanu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gymdlssam.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gdhcwyrpe.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gtjdqdbyu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gepjfxhnx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/ggmwldeey.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/gktinkwjk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.hesvh.cn/Article/details/glbamewki.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gyhopbyos.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/goenyhhyv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.zdbjq.cn/Article/details/gziniosmw.sHtML

PHP:  random_int(1, 100);
来源：http://baike.fehbvm.com/Article/details/galpmpdgy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gizjyhrsq.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gtkeehjdr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gwssgwdea.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gyvzswsga.sHtML

Ruby: rand(1..100)
来源：http://mobile.fehbvm.com/Article/details/gnhlghmdx.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fehbvm.com/Article/details/grxiyirrh.sHtML

[A11] 条件表达式（三元）
来源：http://3g.hesvh.cn/Article/details/gnremmxiq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.zdbjq.cn/Article/details/gxywdqnku.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gylvkyzkz.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gmpfakiic.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gsjnrjchk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gnuyhsnef.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.zdbjq.cn/Article/details/gyzmxnrqz.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/givyrralo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gjwzhoewo.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fehbvm.com/Article/details/glnuvyiir.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.zdbjq.cn/Article/details/gfvtxzbsl.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.zdbjq.cn/Article/details/gjihfpsxm.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gbhjwqxjc.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.zdbjq.cn/Article/details/gfeiyxpny.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.fehbvm.com/Article/details/getjqxmck.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gutrdxmlk.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gvmrrotzz.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.hesvh.cn/Article/details/gkqoxhcdf.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.fehbvm.com/Article/details/geomvbqhx.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/ggxhvfwcv.sHtML

PHP:  "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gnucvpume.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gcxxkdcju.sHtML

TS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/gnmlvrsxh.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gxmsdhimy.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gtypfkogx.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/giukfnczg.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gkanbswip.sHtML

[A14] 注释写法
来源：http://wap.fehbvm.com/Article/details/gmcojlydf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.share.zdbjq.cn/Article/details/gyokwopjx.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gwsrdvavd.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gfshtiktc.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gzccgpaga.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.zdbjq.cn/Article/details/gkdfviuqr.sHtML

Go:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gskyxraoh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.fehbvm.com/Article/details/gqseolnze.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gbnclgjxk.sHtML

[A15] 空值判断与默认值
来源：http://read.share.zdbjq.cn/Article/details/gtipidqcu.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gvgfsfesk.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gcpbfumkt.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.fehbvm.com/Article/details/gmydwbiay.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.hesvh.cn/Article/details/gaqquftsz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/gxzrcdbno.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fehbvm.com/Article/details/grtktgekq.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gjpujalgu.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gzlesroto.sHtML

[A16] 真假值判断规则
来源：http://www.blog.zdbjq.cn/Article/details/gdfvrvikd.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gxspdjbhn.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://3g.zdbjq.cn/Article/details/gfhhscfjx.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fehbvm.com/Article/details/gxxaqaqpe.sHtML

TS:   if (!x) {}
来源：http://www.share.hesvh.cn/Article/details/gfvcxxgfo.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.hesvh.cn/Article/details/gvgijblfa.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.hesvh.cn/Article/details/gprolbvfv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gpobwkrpc.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gvlnrorxl.sHtML

[A17] 位运算
来源：http://baike.zdbjq.cn/Article/details/gmqglhxov.sHtML


<!-- 参考信息 -->