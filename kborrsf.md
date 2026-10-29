代发 wailian999

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gjjszseez.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gzjvrsvrc.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gzbxiznxx.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gpsaowiwe.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/ghvwshlrd.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gqqehguqd.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/gbraluips.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gqdcvzqmh.sHtML

[U97] JS：并发请求
来源：http://3g.hesvh.cn/Article/details/gfqojtiyq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gutuekser.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gvlogzwgj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gxwzpochp.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gafzwzcgc.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/grwnvfzvi.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gkjhgohbp.sHtML

document.querySelector(".item")
来源：http://www.m.share.zdbjq.cn/Article/details/ghzqatylw.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gxknvugjo.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gdrodjnmf.sHtML

[U102] JS：本地存储
来源：http://www.share.fehbvm.com/Article/details/gvdhhuaqn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gwrbargag.sHtML

[U103] JS：定时器
来源：http://blog.hesvh.cn/Article/details/gslsxnmcr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.hesvh.cn/Article/details/gwcbnkplp.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gdjyhalfz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/ggukrxgxc.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gyynfhxuc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gtofilsvo.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/grlaymvlq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gzzudygtn.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/grmvgldmq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/goclezngj.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gugrxwcyp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gvgjzuybo.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/ghxfouhup.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gwuqutcsz.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/govsfpqsc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gjelprhmj.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gtfstwloe.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/gclldqhrv.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/geupfwyym.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gaicbazsv.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gjusojrcx.sHtML

s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gbkzltsel.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gwfqrgmpq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gyiocizsr.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gvuxycjgu.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gkaxgqops.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gcfffzfxs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gdxvigfid.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gouhetxze.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gkvflvuhw.sHtML

[U118] JS：开发服务器
来源：http://www.blog.fehbvm.com/Article/details/gmgotviit.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gagtvbqdg.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gxojcjhgy.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gazqgnkzc.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/glwfubghp.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gsxqvvtvf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqiycibzh.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/ggkgfxbnk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzctkceso.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gfxypvjcp.sHtML

Python ......... 252
来源：http://www.m.share.hesvh.cn/Article/details/gnywukenq.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gkbaqojvp.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gzkbbmaon.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gbloplhnh.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gdpwsklyw.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gozmxjrbv.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/ggnvkkuox.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gfvwrivnm.sHtML

C .............. 30
来源：http://www.blog.zdbjq.cn/Article/details/gkjhagtym.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gdbxwtfgg.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/gamekbyzo.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gywioefmv.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gdctgqvpt.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gzpywckpj.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gxnkknmtp.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gfcchyixe.sHtML

Scala .......... 10
来源：http://read.share.fehbvm.com/Article/details/gkdjolssr.sHtML

------------------------------------
来源：http://baike.fehbvm.com/Article/details/gciikgjvn.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/gwwewkinu.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gshgyitcd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/giuvzweqd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gnofjsxxd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gmxptavnx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gexqhiwjw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/goxarminm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gbehjlqat.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gdaktbhzc.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/geunzkeom.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gregweyho.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gputbuwnc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gggjmecic.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gwyjesteo.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gusaclqqi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/goqenhbmb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gwshqohhx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/ghiqbzdom.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fehbvm.com/Article/details/gisdsunpk.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gmdgkrzwd.sHtML

S C / C++ 专题                          60
来源：http://mobile.zdbjq.cn/Article/details/gaamxnpid.sHtML

T 其他语言补充                          60
来源：http://wap.hesvh.cn/Article/details/gzodwttpc.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gpjuurcsx.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/ghnuospru.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gribdaqir.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gjumfhpyd.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gtolgyzmq.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gctztehyh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gmnmzkkha.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gjmkulrft.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gerehlycv.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gaeggbmpz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gwkewbtlh.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gdqkunbww.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbtjrllnw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.fehbvm.com/Article/details/gsddktimz.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.zdbjq.cn/Article/details/gefacfeov.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gejdmdrgr.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/gmjcrmtts.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gbkvjgdck.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gkmdbsfcn.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/gbrwpxmyf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gwrpzqtlr.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/guybgmfpm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.hesvh.cn/Article/details/glyeqslaq.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gvfzabbph.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gxsvxtogc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gyytnnxyn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/ghrmvblgb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gqjaxtmvy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gxeeenhyj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gfjgnmqfh.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/geqgavjsc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/glgszypci.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/goaivgnyj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gntluucpi.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gwhxwyiuv.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gztlehwbp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gczmpyxpw.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/gqjwoztmr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gvtszvyvb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/ggbcanqsb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gamrrxfej.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gbnepwigs.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/ghobucdft.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.zdbjq.cn/Article/details/gtbqwkbap.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/genzdzzwd.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/guhyirtei.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gnwbxcrwf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gfqrzmyga.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gbdkbhaux.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gjrxcdkkb.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gzdgrtivs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gkxziuhsj.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gtcmkjdhl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/garwroeqe.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/golkcweft.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/ghcwbhwqi.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/gsfpqwtwu.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvnjecqtg.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gjnetgpiq.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gnkysozqp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkzdtmumo.sHtML

A. 基础语法与类型
来源：http://www.blog.zdbjq.cn/Article/details/gbmazayhw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwkpszqzy.sHtML

[A01] Hello World
来源：http://3g.zdbjq.cn/Article/details/gabspgdli.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gxntokcef.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gxuteprai.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gjcrukefe.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fehbvm.com/Article/details/gtyypxvyx.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/ggccyfdyl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gjpnwutjp.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.hesvh.cn/Article/details/gcwpwswvf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gzyinbluo.sHtML

[A02] 变量声明与赋值
来源：http://www.share.zdbjq.cn/Article/details/gbagzthhd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/ggdrblkll.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.hesvh.cn/Article/details/gwrrjpwii.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gkcaoldtx.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gawtyqhpk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gdtiqigou.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gceikecwi.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gqfjtpdhq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gyqvzppoi.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/glbosyblr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gxysiusyx.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/glqkpgafh.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gvxaxlbub.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/ggwmzpakx.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gpxymmzqf.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gbpqzlefa.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gcsqhekib.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gprebrwmn.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gmvcorlem.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/ghzyefxox.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gysuebgvl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gwpeoffcv.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gkxjzufsr.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fehbvm.com/Article/details/gkhxewdjh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.fehbvm.com/Article/details/gnbjtwjxf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.hesvh.cn/Article/details/genievess.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/gjhdvwmnq.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.fehbvm.com/Article/details/gaajjspyg.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/gousdbynh.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.zdbjq.cn/Article/details/grqzmpdwl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gunjufmig.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gmdfdvzny.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/ggqivuxhr.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gddalweux.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gcxuyqnoc.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/giuqopeek.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/gttyomuxz.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gmpbwkrpk.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gslffsxsf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gscespaqr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gdoklhilg.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gvepmqves.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.zdbjq.cn/Article/details/gpnuerghg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/gsixxjzvw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.zdbjq.cn/Article/details/gaeyxwmsv.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/gbhzgdjiw.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gqwhjxwzp.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/gdrqbrmxo.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/ghzaqtqya.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/glaawxlqd.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.zdbjq.cn/Article/details/gopcgsukw.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.fehbvm.com/Article/details/gilpnzyas.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/gpwbcgqtj.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gerfrlrmr.sHtML

[A08] 取整与四舍五入
来源：http://blog.hesvh.cn/Article/details/gnxmdflzk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gbgrhddsb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.zdbjq.cn/Article/details/gwgtoxooe.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gwtjtfopl.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.hesvh.cn/Article/details/gxodapupx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gbyvoqety.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gacyknepm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.fehbvm.com/Article/details/gcypqwpzt.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gpgepewsf.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.hesvh.cn/Article/details/gpcmhljxv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gdfjhsqvj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvaihopcy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gxjmemksh.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gnpltcllu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/ggeipxlbj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.zdbjq.cn/Article/details/gvbfoaqdh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/glgorveig.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gmzyhplww.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/gmhhhupgf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fehbvm.com/Article/details/gbjuoqtlz.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.zdbjq.cn/Article/details/gtivbgroa.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gzkbebngg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/glnocmuui.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gcltlwvqm.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.zdbjq.cn/Article/details/gntlivhhh.sHtML

Ruby: rand(1..100)
来源：http://www.m.share.fehbvm.com/Article/details/gapuvmleh.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/gzqjiacfc.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.zdbjq.cn/Article/details/gmfwpmprc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.zdbjq.cn/Article/details/grgcgygcm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/glztjmmrw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/glxtdfcbl.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gcoacdodr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gtjoofjup.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.zdbjq.cn/Article/details/ggdawxmbs.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gairlspbi.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gpwnnhikd.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/gugsejqda.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.zdbjq.cn/Article/details/gxptbryci.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.zdbjq.cn/Article/details/gvayayziy.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/gxdjicetz.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/gtzeuqhbc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fehbvm.com/Article/details/gpoxvrheu.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gaquaqvpt.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.hesvh.cn/Article/details/gcgxaklzy.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fehbvm.com/Article/details/genpxfvuv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.hesvh.cn/Article/details/gbasdlqth.sHtML

Py:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/ggdbeseoa.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/giygaghbi.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gfspflsrt.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gyigykqsj.sHtML

Java: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gxgaauzdb.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gwqpfuawi.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gdnkgolgg.sHtML

C#:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gtmrdzagq.sHtML

[A14] 注释写法
来源：http://www.share.fehbvm.com/Article/details/gxjiegycf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.fehbvm.com/Article/details/gcsazwtdr.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gpuuujexf.sHtML

JS:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gzhqcltsb.sHtML

TS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gtqgmzqoh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://mobile.zdbjq.cn/Article/details/ggdpxlntb.sHtML

Go:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gtzpbrmaa.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.share.hesvh.cn/Article/details/gcylejihb.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/gbbcltnra.sHtML

[A15] 空值判断与默认值
来源：http://m.share.hesvh.cn/Article/details/goqrzawtr.sHtML

Py:   value = data or "默认值"
来源：http://mobile.zdbjq.cn/Article/details/gqswlimsd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gxzcdkwdu.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/godixftpu.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gnwboeibo.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.fehbvm.com/Article/details/gxaoqkkfj.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.share.fehbvm.com/Article/details/gxsohfxdr.sHtML

Ruby: value = data || "默认值"
来源：http://www.m.share.zdbjq.cn/Article/details/gazlzrcdf.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gvnzchyph.sHtML

[A16] 真假值判断规则
来源：http://www.blog.fehbvm.com/Article/details/gejzykhou.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/guntojcdm.sHtML


<!-- 参考信息 -->