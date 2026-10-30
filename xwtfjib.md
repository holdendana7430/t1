代发 wailian999

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gqhfxlrbv.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/gtlsnzuue.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gxtettrty.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gluznupqn.sHtML

[U97] JS：并发请求
来源：http://m.share.zdbjq.cn/Article/details/gsmbkyyeb.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gcbgkpmza.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gvpjpcroj.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.hesvh.cn/Article/details/gzhcbpstu.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/glfgtrkho.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gyysqviya.sHtML

[U100] JS：DOM 查询
来源：http://3g.zdbjq.cn/Article/details/gcpsdhgdb.sHtML

document.querySelector(".item")
来源：http://www.share.hesvh.cn/Article/details/gbztjbuxd.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gjvmkjjtd.sHtML

el.classList.toggle("active")
来源：http://read.share.hesvh.cn/Article/details/gdgmiylpp.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gvwyegnkj.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fehbvm.com/Article/details/gemezkobb.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gmrefrleo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gnmcykwhj.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gndbfeqxt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/ggzmtfnow.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gawgkuhxt.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gdrpagmxn.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gwetzuxkk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gywjvpgjz.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gluulfena.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/ggjmjjlcw.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/glqavitcb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.hesvh.cn/Article/details/gdojiyagl.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gssktftoz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gumbickxw.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/gjhdbezai.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gfdexrxxy.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gbzhkthkv.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.fehbvm.com/Article/details/gthckbfer.sHtML

[U112] JS：字符串补位
来源：http://blog.zdbjq.cn/Article/details/glcvbfpwo.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gnowxvpxr.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gjcusklcx.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gfckvskua.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gauacybnh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gngktijwa.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gxmlmzhqu.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/girkmdutz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.zdbjq.cn/Article/details/gxbxvanxv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/guhylkjqb.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gypleiqgi.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gjzqluwvo.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gexzhetob.sHtML

npm i -D vite;  npx vite
来源：http://baike.hesvh.cn/Article/details/gqpzftbsy.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gyryyznxk.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/gzoyocyeo.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/gojzkypnb.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gdfjhkaxx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkarqefui.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gzrtnqbjx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghrfqjoqr.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/gfwyhlbjr.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gsmqytbrw.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gdajjllcm.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gkjkyzulc.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gzkarbepk.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gjxkonroj.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gnlhtytpr.sHtML

Ruby ........... 212
来源：http://www.share.zdbjq.cn/Article/details/gdtxvbhsm.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gsnnsjkgp.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gktxcyaow.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gxzpsbpow.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gfmlahiby.sHtML

Bash ........... 80
来源：http://baike.zdbjq.cn/Article/details/glvqkjnbi.sHtML

Kotlin ......... 15
来源：http://wap.zdbjq.cn/Article/details/gjmcbfast.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gexyspjkn.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/gejvhpoke.sHtML

Perl ........... 10
来源：http://baike.hesvh.cn/Article/details/gzczgitwr.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gdpsocpox.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/glhnbqkaf.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gdzfidkpc.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gfsepaqgm.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gfhsouayc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gmdggseyj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gfsuigjan.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/ghdalnquo.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/grtnueffg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gprgrnpqa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gzltmnsia.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gitaimlvx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gdhlsylcm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gnfucjfgk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gzsyvwaki.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gmpvttzzg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gmmlhfuik.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gunnetigj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.zdbjq.cn/Article/details/gnonkfobv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gylejdnqe.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gcendttbb.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/ghuouvkin.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gckpukilm.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/geaxqrqnq.sHtML

U 高频实用片段                         120
来源：http://wap.zdbjq.cn/Article/details/ganjwufin.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gbulmvpen.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gebpgdwuq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gapdgvlla.sHtML

使用提醒
来源：http://mobile.fehbvm.com/Article/details/giebuyfnw.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gomcfhrhk.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://read.share.zdbjq.cn/Article/details/gfmgltgch.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/glycznitv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.hesvh.cn/Article/details/gpopehyhe.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gewqrdsia.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gfpejdrvw.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gjdbjrddc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsyqkwmbq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.zdbjq.cn/Article/details/ggbzszzcg.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gagdxfmvj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glctparry.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gkdykgzbf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/ghporbsbr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.zdbjq.cn/Article/details/gbvkylpem.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gqrwgenyx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gbmfnskcn.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gqyskpphw.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/ghthctjns.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gpoeqbmid.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gdlrjakga.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/gfnsgsmnn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gzblokkkn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.hesvh.cn/Article/details/gpzxieudv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gbawrpkmn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.hesvh.cn/Article/details/gpguxmpql.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/gzmfuixuw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gpwuicddp.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gudfjwzsk.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/gzwytkzkw.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gkossnnpw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gfusqoumo.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gbbzbgopy.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gfkvtecoc.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gurjiqtyq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.hesvh.cn/Article/details/gqwlrykyb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxiyrdgqf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/glppevglb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.zdbjq.cn/Article/details/gnsbxvmyg.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/grgehdjwi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpcqvllad.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gjelaetpr.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gjrtnuucv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gebvuerjx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gpjzqnpcl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/glsqakbmc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gdkvzwyre.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/ggdspxfln.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/ghactcurb.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gamlsfjvb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gibjwfvph.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fehbvm.com/Article/details/gydbhgxjc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gaodqvsuw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gxbermjjp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gzfimxmut.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gzkdouxce.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gonemiwff.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gvllsrknp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfumbbjji.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gdnqddhru.sHtML

Py:   print("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gpoaapjkh.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gtktvfwsa.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/glbrzrgdo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gzbmehlfa.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gjegpjojw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gghmztwzj.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gnpwiqbzy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gzmcjkkrv.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gnpkguuwz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/ghrhfoiep.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gycfpwywv.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/gteiqiftq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gkdcpcbpt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/gdqkeykbo.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gprahwycs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.hesvh.cn/Article/details/gqwjloerk.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gsqbwzvjz.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gahyxkxcx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gjocdkoub.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gohgckbkh.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gslgqgdiq.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gkjmbxbxb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gpszlntvx.sHtML

Go:   const PI = 3.14159
来源：http://mobile.hesvh.cn/Article/details/gyebyioux.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gbrzumlon.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/geotatxrm.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gyotcclxh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/gnuqzymld.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/glkhxzsso.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gipbecmyw.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gftjsofwp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/gyjldggoa.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gilmpugid.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/gwxegywpj.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.zdbjq.cn/Article/details/gclmdumir.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gjezpytiz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gnyiofqoz.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gohbcagee.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gqzvxneve.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gewdmbxgv.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gxgefkdfx.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gwlqslppt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/ggcmxecnc.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gnbcuwkeo.sHtML

[A06] 字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gtfyylcem.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.zdbjq.cn/Article/details/gslnbzpus.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/gweowsezw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/gfgunnrcb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gpasbxpen.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gxakvsukz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gndsspbbg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gsioftmit.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fehbvm.com/Article/details/ghenkxell.sHtML

[A07] 数字转字符串
来源：http://mobile.fehbvm.com/Article/details/gvdqhgruh.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gbqehpaqh.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/ghhzymzol.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gsfkwhowl.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gbxrtadbe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.hesvh.cn/Article/details/gneonbmaw.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/gkocswavm.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/ghlrpusjb.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gpbnolcfv.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.hesvh.cn/Article/details/gdscfenhj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gqaxvvlyo.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gaasdiohv.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gaxxxmmlm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/gmwqkqxsa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gavlevndi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/giviyvilc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/ggvzddkrx.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gmlmrpkhn.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.fehbvm.com/Article/details/glgwsault.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.hesvh.cn/Article/details/gcdcxorbg.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/ghavsftry.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/goohjjxsp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/geqbamfmu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gotcfnldt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fehbvm.com/Article/details/ghxkevjmh.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.zdbjq.cn/Article/details/gzevjbozl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://blog.fehbvm.com/Article/details/gjajktgqk.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/gxrgmkvzt.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.zdbjq.cn/Article/details/gbzecwbjp.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/ggxbgrzte.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gbmuylxtc.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gudnbpbkm.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.hesvh.cn/Article/details/gxlvrpywz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.hesvh.cn/Article/details/gatmzqevn.sHtML

Ruby: rand(1..100)
来源：http://wap.zdbjq.cn/Article/details/gvlwqhrhi.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.hesvh.cn/Article/details/gqysxkkty.sHtML

[A11] 条件表达式（三元）
来源：http://blog.hesvh.cn/Article/details/gpgtjdyxe.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.hesvh.cn/Article/details/grfbgecff.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gllncduej.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/ggczdxxxo.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/ghlwstblx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gdrqlpnkc.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.zdbjq.cn/Article/details/gwqapqcrf.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gihytwini.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gyymrujvw.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.hesvh.cn/Article/details/gizccxzty.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.zdbjq.cn/Article/details/gohvmffpq.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://baike.hesvh.cn/Article/details/gblaivazk.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gbwabigrp.sHtML

TS:   `Hello, ${name}!`
来源：http://mobile.zdbjq.cn/Article/details/gbtnyubbz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/goqnhgksp.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.blog.hesvh.cn/Article/details/gcppoevgd.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.zdbjq.cn/Article/details/gvyyggurm.sHtML

C#:   $"Hello, {name}!"
来源：http://3g.zdbjq.cn/Article/details/glupqpebu.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.zdbjq.cn/Article/details/gsbxggrjt.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.fehbvm.com/Article/details/gcajrqjzi.sHtML

PHP:  "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gnjimjbxu.sHtML

JS:   "第一行\n第二行"
来源：http://blog.zdbjq.cn/Article/details/galopmody.sHtML

TS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gaakshasv.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gutubmtpi.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gvkiwrwov.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gkmhbghbl.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/guakprhpf.sHtML

[A14] 注释写法
来源：http://www.blog.hesvh.cn/Article/details/gnjltcrjj.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://read.share.zdbjq.cn/Article/details/gtkledzra.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gafayecwz.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gamgzxgsn.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/glcdcmunu.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.zdbjq.cn/Article/details/gqstcqjxd.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/grniasbhc.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/gjnjtcctk.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.fehbvm.com/Article/details/grhqqcrvf.sHtML

[A15] 空值判断与默认值
来源：http://mobile.zdbjq.cn/Article/details/gzxktwxqk.sHtML

Py:   value = data or "默认值"
来源：http://wap.hesvh.cn/Article/details/gdxqxohgi.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gzlmconll.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.fehbvm.com/Article/details/gisdzjvch.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gqjnrvdig.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.m.share.hesvh.cn/Article/details/gufuwfhib.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://3g.fehbvm.com/Article/details/gtiwyagfi.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/ggvomnkuo.sHtML

C#:   var value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/ghjslbzlg.sHtML

[A16] 真假值判断规则
来源：http://mobile.hesvh.cn/Article/details/gyhaycygq.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.hesvh.cn/Article/details/gqrcjgfzh.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.fehbvm.com/Article/details/gaqqroyvp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.hesvh.cn/Article/details/gqvtmjuvs.sHtML

TS:   if (!x) {}
来源：http://blog.hesvh.cn/Article/details/ggrhvjjta.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpachukxz.sHtML


<!-- 参考信息 -->