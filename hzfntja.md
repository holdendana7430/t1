代发 wailian999

[U93] JS：模板字符串
来源：http://read.share.hesvh.cn/Article/details/gnoqelomw.sHtML

`共 ${n} 条`
来源：http://www.share.fehbvm.com/Article/details/gwepqemia.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gozommupe.sHtML

const double = x => x * 2;
来源：http://mobile.hesvh.cn/Article/details/gydzjyamb.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gpqpolldw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.hesvh.cn/Article/details/gwbvxuiix.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gefrcaftu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/genezsvqi.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gxblppukt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gvqdrtlxm.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gxjoynkmt.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gikeumisg.sHtML

[U99] JS：事件监听
来源：http://read.share.hesvh.cn/Article/details/grhdchrjn.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gyaecgyvm.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/ghgxjoqry.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gxnyeqvaa.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gzudwsfvw.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gfxjfcamb.sHtML

[U102] JS：本地存储
来源：http://read.share.fehbvm.com/Article/details/gsltxcmnb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gutligolt.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gumtyxpsb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.fehbvm.com/Article/details/gmqdxzaxb.sHtML

[U104] JS：防抖
来源：http://wap.zdbjq.cn/Article/details/gmmskvtfa.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gfxfuinzo.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gtupehutr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/grudpfdwp.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gqnqkzucm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.zdbjq.cn/Article/details/gferqukzd.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/gfexahknx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gnasycude.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gymecvpqg.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gqpecgkrh.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gopqopyyn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gdwjpafxq.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gvhtcjhuw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gvuzkvprn.sHtML

[U111] JS：对象转 Map
来源：http://www.share.zdbjq.cn/Article/details/gzefuqali.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gkzoritga.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gaqazosxt.sHtML

"7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/garqcbdry.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gikgjlkbs.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gohxfpbbi.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/gdwdkbwgc.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fehbvm.com/Article/details/gvcyraryv.sHtML

[U115] JS：生成 UUID
来源：http://baike.zdbjq.cn/Article/details/gavzbgpsm.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gddvonocm.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.zdbjq.cn/Article/details/gzyzjsaia.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gnytaxbnj.sHtML

[U117] JS：单元测试
来源：http://m.share.zdbjq.cn/Article/details/gacybvsvs.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/ghnegzgok.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/ghieuxaks.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/ghutfnnrg.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gpvsoxgvx.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/golxivubd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.hesvh.cn/Article/details/gcvnbgifh.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gwguxcwms.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqlehfxnk.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gijlqynbq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkxhyihvq.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gzqmpxolb.sHtML

Python ......... 252
来源：http://m.share.hesvh.cn/Article/details/gahslhdym.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/gbnyawuqq.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gpnazyieb.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/ggokpcorx.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gcqaaikqu.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gjodnysum.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gbbbzocrt.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gueldjsls.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gjxmnkckg.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gefhwspnk.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/gsxijfxlk.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/gnpjzzfjp.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gxwchehyk.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gplghvprq.sHtML

Lua ............ 10
来源：http://blog.zdbjq.cn/Article/details/guvzhyphy.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gtfeyhetl.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gdudqksnp.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gotvrznlx.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gccictwmj.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gdbwppsxh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gwowutqzm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gaufpfwyv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gvqbykzew.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gkdappmrq.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/ghmrmqtdc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/glaxuxauo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gpermgntm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gtkoujiux.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gmowtevbh.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gxteesobo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/grlwopfqh.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gdztxitop.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gshdudakx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.zdbjq.cn/Article/details/gjavejivb.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gvlhylexi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gjjsygqmp.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gpslgdrtz.sHtML

R Bash 专题                             80
来源：http://m.share.fehbvm.com/Article/details/ggwtpzjcv.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gibmrjexm.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gqgslzrso.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gfulwqocp.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gzsojanpx.sHtML

合计                                  2106 条
来源：http://www.share.zdbjq.cn/Article/details/gwnqggxmk.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gmmfzjofn.sHtML

使用提醒
来源：http://mobile.hesvh.cn/Article/details/gilubmxhg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gttmrrwxv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/glbhqrgho.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gsljzmynz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gzjssftob.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gyskdpsyg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/gonjqaohb.sHtML

—— 文件结束 ——
来源：http://www.blog.hesvh.cn/Article/details/gfauxwude.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmrrlojlp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gwxdjgqld.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/groymmumh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdckkotqe.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/glhovrhwm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gardqgcld.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gldftqyvp.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gctuqszda.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gusdtihdb.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gzrmkopfg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gpikfgshu.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.hesvh.cn/Article/details/gbtnxusxt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gjnxmkebm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fehbvm.com/Article/details/gbpzcfzrf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gnioxbsqn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gqwvxyzrq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gayksnsma.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.hesvh.cn/Article/details/ggaykawzi.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fehbvm.com/Article/details/gdarbmozj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gbrsgwsba.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gskbupzst.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gppvbdqea.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/giozprzlk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gfmermyik.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gdygozahy.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gqemukwdq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gdkshmnci.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gheaqnngv.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gxrjlmrjn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gaulijdrm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/ggtwytfns.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gzqkxoimr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gtinmaxxp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gtqwqldxa.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/gjnhjhkht.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gjdqpfpfa.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfvvisytq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gqgjchgml.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gguraybtv.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gakschfcs.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gazdagdqo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqaywzufe.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gndzdcjyp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/ggcrnxovj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gusvxabru.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.hesvh.cn/Article/details/gasoaffbh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gqawairaw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gciogzyuu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gawkdytdm.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/gyferjjle.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwlsacmru.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/guzmdogwp.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/ggloeuolh.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gpuqosctf.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gjkuokyfv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.fehbvm.com/Article/details/gtxfgywnp.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gzqofyjvv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gfmrhghmw.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.hesvh.cn/Article/details/gbtykrbbm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/girvnzasz.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gyszteydv.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gcazjjmbm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gczmkhavn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fehbvm.com/Article/details/gaaaajyss.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.hesvh.cn/Article/details/ginrlqvxr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gswqttvjz.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gufcfaufz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gxorwwfkf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gfbkzvpms.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gqjjjcxis.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gbqeboqvd.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gmagxqdnv.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gtkkrzfiw.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gnmiuxgsd.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gturxxkvf.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gjhjfblle.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gbbbeuoiq.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gyjagtuou.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gxlwwehlo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gcpprwbtf.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gmqctvwqv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gxoiwzfcf.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/ghnrcsabj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gswhajwjl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fehbvm.com/Article/details/grrvugbqn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/gvtgpikke.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.zdbjq.cn/Article/details/gnekmgljf.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gztvfsavv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gmbnkcxry.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/gtwuyrura.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gnueaprnn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gkhxtiipt.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gxlclwpuv.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/ghwvxtsbt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gxvxpxrzr.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/ggpjxghtl.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gcuwfnrhi.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gozftufrv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fehbvm.com/Article/details/gdyqercig.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/guwwwysnw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gowlzwrvn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gldekqeez.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/grbpoofrg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gvsnsceku.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/gsvaefgwm.sHtML

[A07] 数字转字符串
来源：http://blog.hesvh.cn/Article/details/gmnmgtiba.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gaceovmkd.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.hesvh.cn/Article/details/gquawdxfm.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/gqgrerdcb.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/gjzyujgiu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.fehbvm.com/Article/details/guvwoquad.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fehbvm.com/Article/details/gptztugbx.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gkbcfhdnp.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gvjwargzw.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.fehbvm.com/Article/details/gzhwcscfe.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gqobtxbjj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.zdbjq.cn/Article/details/gyuqlqorg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gmqxpvhfc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gtdnqyfqz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/ghoampmfo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gyfkfyvxl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/gtmotvoxp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gnhdrcglm.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gqsnbawdr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/ggkoyylia.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwbabrddo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/ghxvabqfb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gwzaejrdi.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gziuoyjct.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.hesvh.cn/Article/details/gvlwwtwly.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/ggnnhlwpx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gqwxwvjjc.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/gmaczkqqs.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/gjczbblwy.sHtML

PHP:  random_int(1, 100);
来源：http://baike.zdbjq.cn/Article/details/gigujxjhy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gnqyvnztf.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/gultnikvl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gsfsaphpg.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.fehbvm.com/Article/details/gyxdsqmjc.sHtML

Ruby: rand(1..100)
来源：http://blog.hesvh.cn/Article/details/gjkjbjxfk.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.hesvh.cn/Article/details/gxzoxoylw.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.zdbjq.cn/Article/details/ggbtdotbk.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gzdkrnell.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gdzhnvitv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gytrkidlh.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gpxuqfaun.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gvqblgzbg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.zdbjq.cn/Article/details/gemoayaap.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/govavuzzo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/ggvcuhloc.sHtML

[A12] 字符串插值 / 格式化
来源：http://read.share.fehbvm.com/Article/details/gluasjrnp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.zdbjq.cn/Article/details/gpjjvjlyl.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fehbvm.com/Article/details/gqzxvahnf.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/goptenspp.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.hesvh.cn/Article/details/gjhrdfmjj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/gacuwktrj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.fehbvm.com/Article/details/gzzdetutu.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gqbptzhnw.sHtML

C#:   $"Hello, {name}!"
来源：http://baike.hesvh.cn/Article/details/gmfxnkerl.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.zdbjq.cn/Article/details/gkbdtjvee.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/grfzpnzls.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gshxyhxnk.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gkbkubhja.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/gglzfsyzj.sHtML

Java: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gsxhcoxot.sHtML

Go:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gaqwrfhio.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gnqxikynx.sHtML

C#:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/grztvhhnt.sHtML

[A14] 注释写法
来源：http://www.blog.zdbjq.cn/Article/details/gpojimiux.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fehbvm.com/Article/details/goplxajjt.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gkgcatbbs.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/ggassetna.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gelaszhpe.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://m.share.hesvh.cn/Article/details/ghjwjdpas.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/ghgrelehh.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.zdbjq.cn/Article/details/grwbgqwhr.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/geqamawug.sHtML

[A15] 空值判断与默认值
来源：http://blog.zdbjq.cn/Article/details/gomgvlxhs.sHtML

Py:   value = data or "默认值"
来源：http://www.m.share.fehbvm.com/Article/details/gmdhtczbw.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/glfyvoikb.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gevkrlclj.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/grgwwkglq.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.zdbjq.cn/Article/details/gabvwbbrk.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fehbvm.com/Article/details/gdjctrjoo.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gkyphfiyq.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/guwwinnid.sHtML

[A16] 真假值判断规则
来源：http://baike.hesvh.cn/Article/details/gcnphcqus.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.fehbvm.com/Article/details/gztwkabkv.sHtML


<!-- 参考信息 -->