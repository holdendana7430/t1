代发 wailian999

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gtntqzrlg.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.hesvh.cn/Article/details/gilwenpim.sHtML

[U96] JS：async/await 与异常
来源：http://wap.zdbjq.cn/Article/details/gpzabthlu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gnrefwuqo.sHtML

[U97] JS：并发请求
来源：http://baike.fehbvm.com/Article/details/gzdkvaylp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gnhxcxaoa.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gcimljtsf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.fehbvm.com/Article/details/gpwohfbjz.sHtML

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/glgseupcu.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gsofpigfu.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gmomkmljd.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gqurdupyd.sHtML

[U101] JS：classList 操作
来源：http://www.share.hesvh.cn/Article/details/gggaghubp.sHtML

el.classList.toggle("active")
来源：http://mobile.zdbjq.cn/Article/details/gygmzaryn.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gnaemtxzp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/glrarkegq.sHtML

[U103] JS：定时器
来源：http://wap.hesvh.cn/Article/details/gxdyycnsf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gwjgdgasg.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gvoxnnrws.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/ggaayzeub.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gklfsvikh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gltwhnzbi.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gfrwuxadq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gswesrute.sHtML

[U107] JS：数字千分位
来源：http://baike.hesvh.cn/Article/details/ghbtgykfk.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gjfwtfajo.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gkzjjnjuf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gsrqkszjy.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/gpfamzmqv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gjdcngvkn.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gjifqbbls.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/glyacksdo.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/gblvvqsdd.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/guytidqlk.sHtML

[U112] JS：字符串补位
来源：http://3g.zdbjq.cn/Article/details/gnhrhihfu.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gwfwklijs.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gnqambotv.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gezegbxon.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gvepzjncm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gkhnsfaxw.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gytxwdlyl.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gzvhzwiag.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gxsexjvff.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gmdsgwxax.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/girbmnfvo.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.fehbvm.com/Article/details/gxderybgl.sHtML

[U118] JS：开发服务器
来源：http://baike.zdbjq.cn/Article/details/gmmtxesiu.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/geyijyeqk.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gkphyxrbe.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gincyhlvq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/geqndkoav.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gotrxzzlb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcypjomss.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/ghdwfkzwa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpcjgiuas.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gjmnglqvr.sHtML

Python ......... 252
来源：http://baike.zdbjq.cn/Article/details/gpbtncklj.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gyagpiiqn.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/ggmwhmmnn.sHtML

TypeScript ..... 212
来源：http://3g.zdbjq.cn/Article/details/gnpltqewv.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gvzrjouuu.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/grccayoty.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gdazdakvr.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gabrbsbvr.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/gqxognafb.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gmovaopva.sHtML

SQL ............ 90
来源：http://read.share.zdbjq.cn/Article/details/gtebnvekc.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gryjjrmkl.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/guvxahblf.sHtML

Swift .......... 15
来源：http://read.share.zdbjq.cn/Article/details/gktfmkknt.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gwygbpilg.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gconvzvrr.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gcfpwmnrc.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gzqgvftir.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gwpcakwwa.sHtML

按章节统计：
来源：http://read.share.zdbjq.cn/Article/details/gokixifsw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gxaakwvij.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gqazmtech.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gebjfwdha.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/glzywvbyt.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/ghowhgofz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gxzlkmlsp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gltsbfznl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gzpyqeawc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gjkthwkuo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gzcxrxmbo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gdqeijahn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gjbywgcvm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gyxoegwxm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/ghzhvhmfc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/goibzfxia.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/geaubgjzg.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gwcywqpqd.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/gbjmgbctx.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/gxwpvxfbv.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gtgtxuvga.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gcowzxlpa.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/guyzktvfy.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gdxibzitb.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/ggyghkxxc.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/gxnnuwuek.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gwcngajay.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gdkhdlpkx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gknctltad.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.zdbjq.cn/Article/details/goukxvssa.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.zdbjq.cn/Article/details/gcnwyjphc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gjfysxcbq.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gvhgxisqf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvtncigep.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/gtibsgnwp.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gsyjkdjkd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyvabokup.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gkzlxvdtf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/ggcmoxmbx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.hesvh.cn/Article/details/glquzbyoq.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gabbctjyr.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gyzvgkiuq.sHtML

【使用说明】
来源：http://m.share.fehbvm.com/Article/details/gkimeqdtx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/girbinwrk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.zdbjq.cn/Article/details/gmpajggyc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/grimznnld.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.fehbvm.com/Article/details/gxyyojtdi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gwdjkzlaz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gmexbnszo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.hesvh.cn/Article/details/gvbflowaq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/geyqqnzwo.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gnghazils.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gfbvmodre.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gysebdpei.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.zdbjq.cn/Article/details/gjxcxbgts.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gcmdlviyh.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gahgoyypq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gvadyjgvw.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gizvrufjr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/guevibisi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gtdftplfb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/glwyskuhw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gfjvojdlh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gkhedbiec.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gvxlaifec.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gjqsgsvjf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/goyrrlaxs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/grwkynxap.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gfxfqzjcs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gxjbbgsqs.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gzpzjhywd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gzhmwzoua.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/ghchsdrsv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gccivyqho.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gvzkcalge.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gwsuofwtr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gfhydmzzq.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gmqgvmvnd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gveqkcido.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gibitisds.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gssohpqna.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvqazhgpg.sHtML

A. 基础语法与类型
来源：http://read.share.hesvh.cn/Article/details/gnqlvmaai.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkshgppxh.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gbbpaedlj.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gggbtjjil.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gedeiqikv.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gkxzyohnt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fehbvm.com/Article/details/gpoeuhkeh.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/giayhxinh.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/glwjsqqhn.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gmavyxkij.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/ggfsnomcc.sHtML

[A02] 变量声明与赋值
来源：http://mobile.hesvh.cn/Article/details/gklmfsblb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gkgczzrvo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gvndzgnba.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gmiewhlze.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/ggpsimvng.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gxqzumksg.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.zdbjq.cn/Article/details/goyupklsf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/ghavzpvlg.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/ghhmxtglb.sHtML

[A03] 常量定义
来源：http://www.share.fehbvm.com/Article/details/gepqgkbao.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gjrwhlkjn.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gyknnflne.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/glabvygup.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gyqtdqzrt.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gogfrnxdx.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gcxwfgrnm.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gdrptibhj.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gxcxxctco.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gyzslowei.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/ggfxnfzvd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/gbvpetajy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gdisuajro.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/guxvwffsz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gnyrjdrxl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.hesvh.cn/Article/details/gprotyxyv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gbbadipgz.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/gnlvnlqee.sHtML

[A05] 整数除法与取模
来源：http://www.share.zdbjq.cn/Article/details/gtffvghnn.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.fehbvm.com/Article/details/glscmgqct.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gadipknzd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gqcizjbau.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gnwvvmbqf.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gcvidbveb.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gqkjyljec.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gteuzplwo.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gngequabi.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/gzzrthgor.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gcpgtneoq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fehbvm.com/Article/details/gumnmcjkd.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/gmklaijnv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gzrtcihpq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.fehbvm.com/Article/details/gvftnkgkk.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gkyxsjlhy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.zdbjq.cn/Article/details/gcgbbbvix.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/gkxkvtdfv.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/gyllduwny.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/gcdyzqkha.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/gyruzgmbp.sHtML

JS:   String(42); (42).toString()
来源：http://wap.hesvh.cn/Article/details/gfwrhbttu.sHtML

TS:   String(42)
来源：http://read.share.zdbjq.cn/Article/details/gifrlhqdy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/giyeaohpp.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/gtbwfdojp.sHtML

Ruby: 42.to_s
来源：http://wap.hesvh.cn/Article/details/gnqdmjpll.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gkybksvyy.sHtML

[A08] 取整与四舍五入
来源：http://m.share.hesvh.cn/Article/details/gadqqmwmk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gsdiakgnq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.zdbjq.cn/Article/details/gtmwejlsf.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gzwspoakq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/gimnzptxm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gbgzxdmya.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gifebtpzx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gjqdjciwo.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gujssstav.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gplkzevou.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gnprcprwd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gdwqlvbqd.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/geupbvbkb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gsyexmszi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnhioyii.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.hesvh.cn/Article/details/ghlwaxacp.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gzgzcynwm.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gjxihdqud.sHtML

[A10] 生成随机数
来源：http://m.share.fehbvm.com/Article/details/gwpvnbbtz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.hesvh.cn/Article/details/gipaooozt.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gnkninrlk.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gqbakowrd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/gwcxmfasz.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.hesvh.cn/Article/details/gxggzrsit.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.hesvh.cn/Article/details/gktzrqrvg.sHtML

Ruby: rand(1..100)
来源：http://3g.fehbvm.com/Article/details/gjbxzbquz.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.hesvh.cn/Article/details/giwyslqsg.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.hesvh.cn/Article/details/gebithslx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.zdbjq.cn/Article/details/gglcywnrh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gmbyaqcxd.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gatbwgrqm.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/ggfsannno.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gidsqyfml.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://baike.hesvh.cn/Article/details/gicugoiyy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gxpwtyauf.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/giflfoqkl.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fehbvm.com/Article/details/gauegennn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/gjvmafzkz.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.hesvh.cn/Article/details/grjjsaogq.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/gygzikmoi.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/ghpupsmbf.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fehbvm.com/Article/details/gfkswqozs.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.zdbjq.cn/Article/details/gerqjbaki.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.fehbvm.com/Article/details/guduqeekl.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.fehbvm.com/Article/details/gefmifjsv.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://wap.hesvh.cn/Article/details/gbmqggbiy.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/glwypzshz.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gusrrpyau.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gweatjbaq.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gvlqjbsxe.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gpfwuilxr.sHtML

Go:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/grxwtdqss.sHtML

Ruby: "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/guaydwyfi.sHtML

C#:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gurktvvgu.sHtML

[A14] 注释写法
来源：http://read.share.fehbvm.com/Article/details/gugndabdm.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.hesvh.cn/Article/details/gdfavfefh.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gijwluewe.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gqedsnnwq.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gypjqtfku.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.hesvh.cn/Article/details/gxydiwvaj.sHtML

Go:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gkheunjav.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.zdbjq.cn/Article/details/grgmlrzpm.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.fehbvm.com/Article/details/gepmnvgsz.sHtML

[A15] 空值判断与默认值
来源：http://blog.fehbvm.com/Article/details/goksvjgek.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gvsulrprp.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/gwhtiwkpp.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gbxxknahb.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gphdwjrcg.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.zdbjq.cn/Article/details/gdvttlgld.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.zdbjq.cn/Article/details/gebmbseuj.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.zdbjq.cn/Article/details/gbktjnamx.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gejvixhfx.sHtML

[A16] 真假值判断规则
来源：http://3g.hesvh.cn/Article/details/gpkhfrrgk.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.hesvh.cn/Article/details/gscpxoasd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.hesvh.cn/Article/details/gfgssmtnu.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://read.share.hesvh.cn/Article/details/gmsjusanb.sHtML

TS:   if (!x) {}
来源：http://m.share.fehbvm.com/Article/details/gdwdyviaq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://read.share.fehbvm.com/Article/details/gylzjwsfm.sHtML


<!-- 参考信息 -->