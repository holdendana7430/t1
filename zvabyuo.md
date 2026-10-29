代发 wailian999

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gmmrlmwtr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gvzcspwiv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gmlixxpxm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/gubqzckmz.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/gitlgveyz.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gblliaxau.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gtzqawyik.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gucxcbadv.sHtML

[U101] JS：classList 操作
来源：http://blog.fehbvm.com/Article/details/gydaxfmqs.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gntqzrxal.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gcuubyjdg.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/guttbmtts.sHtML

[U103] JS：定时器
来源：http://baike.fehbvm.com/Article/details/gaaqptkda.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gcwmylrsq.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gddjqywwe.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/grfqdopys.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gkyyptyjj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.zdbjq.cn/Article/details/gxmsbbczm.sHtML

[U106] JS：日期格式化
来源：http://m.share.fehbvm.com/Article/details/gkcjzahge.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gaxdznaxi.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gfjfkakgv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gleemfccq.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gzmzbstph.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.hesvh.cn/Article/details/gcvbhbujm.sHtML

[U109] JS：数组分组
来源：http://blog.fehbvm.com/Article/details/gfpixhjto.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gjkbhvjgo.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gmdzfgtmx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gvmwvxlvw.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gyxkghxig.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/gbyyryndp.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gzwkbpcli.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/glaxxmuyl.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gbbedqiix.sHtML

s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/guaqcywdn.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/glwkwuotw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gacwlyoop.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gagxshrof.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gbapoftay.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/gyzdsnhpp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/gejprpehj.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gamlkhahd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gjneussda.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fehbvm.com/Article/details/gysrqmjcm.sHtML

npm i -D vite;  npx vite
来源：http://www.share.fehbvm.com/Article/details/gugfvoxgy.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gwbppvbrx.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gqgwpbcbz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.zdbjq.cn/Article/details/grmzmabmh.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gxvebmbhy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkrxnskbw.sHtML

统计汇总
来源：http://m.share.zdbjq.cn/Article/details/grbrvpfcw.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guaovgnue.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gitmuloqe.sHtML

Python ......... 252
来源：http://mobile.hesvh.cn/Article/details/gyobmenee.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/gijmtqesh.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gryxatxlt.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gxmvjmqrj.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gkxiufcke.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/ghooxqtzm.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gkdrcqmne.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gromkfpas.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/glsphbhgl.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gyrcecfkk.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gddudkdei.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gvnzcicmq.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gpxjicjus.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gkoejlrbi.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/glaxjumlk.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/golgnyhkk.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gjaqwqjlp.sHtML

------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gkzkvzbdd.sHtML

合计 ........... 2106 条
来源：http://wap.fehbvm.com/Article/details/gsvvjzegr.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/grsuvwuvq.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gddnqnbdq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gohybiusp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gmztoozxs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gcssvucei.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.hesvh.cn/Article/details/gluhvpkyx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gynhkyvcw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gzuiwljue.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gvltmoyth.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gsbyeuxtj.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gegblxwek.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/glifczdrg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gthqavonz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gqerpstwd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gwtkjrnej.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gsynxpnmr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gnbhqwebe.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gqmejkgrf.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/grepohyte.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gaappyoms.sHtML

T 其他语言补充                          60
来源：http://mobile.zdbjq.cn/Article/details/gydubfbia.sHtML

U 高频实用片段                         120
来源：http://www.m.share.zdbjq.cn/Article/details/ggjfczfni.sHtML

------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gddwrkjdp.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gyjjzjimd.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/glkhxunxy.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gejwzgcno.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gmkaufwkh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gpjmhypwh.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gfclqskjj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.fehbvm.com/Article/details/geqzsqjdg.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.fehbvm.com/Article/details/gcijqqkop.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gxhbfrupb.sHtML

—— 文件结束 ——
来源：http://read.share.fehbvm.com/Article/details/gpddqploj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghroboyyj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gikhvwfuz.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/gxuptyfdi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyzxhssje.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/gyeelkfsz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gccgmxevp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/ghfpyelbx.sHtML

SQL · Bash · C · C++
来源：http://www.blog.zdbjq.cn/Article/details/gnkertdwk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gzcbjgfdx.sHtML

【使用说明】
来源：http://www.m.share.hesvh.cn/Article/details/gpzloxtjh.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/gqmiuaqox.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gezsohwmg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.zdbjq.cn/Article/details/girvllwtf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/gvkmnbbuv.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gphfubrop.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gmgsmqtlz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gswjbleau.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.hesvh.cn/Article/details/gpmmdhwba.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.fehbvm.com/Article/details/gdguwqgmb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gsdgtljxz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.zdbjq.cn/Article/details/grbcvflji.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gqypjksrj.sHtML

【文件统计】
来源：http://mobile.hesvh.cn/Article/details/gufjhcxnl.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/gfhctuzch.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/ghutymdtx.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gmexcjlcc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/glillpxex.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gqxpbbted.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gthyexzks.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gziuvsltx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/ghrsftdnq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.zdbjq.cn/Article/details/gicmdthhj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/groanhxto.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/glcrhbzqt.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gozdrjzaz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghfthcrru.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gprgpzexh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gddakppsn.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/ghremixqs.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gskxycckr.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gdkmdrace.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gmabdrbtm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/ggyfgewho.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gfpoldeit.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gjuvqmleg.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/gwgnjeasu.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gtydhfssk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gjunxgwtf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glwjubsnq.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/ggvruwtld.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfivqvgdr.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/glcacldnz.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/ggtquucgq.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gbrrjsnmu.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gymmsqnys.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gxpfxjpfl.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gcawzvade.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/ghqatrlek.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/gievdwdgy.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gpmyaghri.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gjclqkuts.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/glbbynuzy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.fehbvm.com/Article/details/govxjucpk.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gklgfjgcy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gpkadntcb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/ggzqtaxde.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/glcykdosz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/gwuqyrsan.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gtsbuqvij.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gdywawage.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/geqmxlobt.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/grwnenlmt.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gbppqjuvx.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gwxxtvmkx.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gfnraxlmf.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gvpthtozh.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gyqdejsvs.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gkhfyutdr.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/ghpxthtyi.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/gkvutmvcg.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/grjvadpkr.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/gzukftpad.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.hesvh.cn/Article/details/gjmmzucmi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.hesvh.cn/Article/details/guguykdyv.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gbwhsabdg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gwpgppelq.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/ghyecwhsv.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gykeelxap.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fehbvm.com/Article/details/gchpdptly.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gfvtdyzon.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/grezcjyur.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gwnmcjmng.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gezdtecov.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gubjxlvno.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gxtehgmlq.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/getyxiqwm.sHtML

[A06] 字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gazdbetjh.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gsxoopxrv.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.fehbvm.com/Article/details/glnopgvrw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gpildiqhi.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gziyebslx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/gaysgejzs.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/glrqpqjrk.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gavacwnat.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gzrgyinnb.sHtML

[A07] 数字转字符串
来源：http://blog.fehbvm.com/Article/details/gkhhseiub.sHtML

Py:   str(42)
来源：http://baike.zdbjq.cn/Article/details/gqcvughtb.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.hesvh.cn/Article/details/glmgsfnol.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gnvwthlpo.sHtML

TS:   String(42)
来源：http://www.blog.fehbvm.com/Article/details/ghlvqpamo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gmnszvuka.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/gzrfjpuom.sHtML

Ruby: 42.to_s
来源：http://wap.hesvh.cn/Article/details/gxiraqyek.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gzhepdanf.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/gidyrobaz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gjusmeyci.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fehbvm.com/Article/details/gxtmyhbbb.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gickcwrfq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.fehbvm.com/Article/details/geupcbfwo.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gyuyuqqjb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gmfvepyom.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/gqltplsth.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/ggzsiucmu.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.fehbvm.com/Article/details/gfcxxkmoi.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gpbucrurp.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gzblpwmqt.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gnbajyzgb.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcvnqiyil.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gxyhhxzll.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fehbvm.com/Article/details/gkzrkaavz.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.zdbjq.cn/Article/details/giixtzmkl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gmvshwlqw.sHtML

[A10] 生成随机数
来源：http://read.share.hesvh.cn/Article/details/ginulkrmk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.hesvh.cn/Article/details/gxqblnvhp.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.zdbjq.cn/Article/details/gmfemusip.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fehbvm.com/Article/details/gbmlbyvsh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gpcsjfqzi.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/gwufcpzdw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.zdbjq.cn/Article/details/gzjuldfvh.sHtML

Ruby: rand(1..100)
来源：http://www.blog.hesvh.cn/Article/details/gpejjwqjh.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.zdbjq.cn/Article/details/gdphkmkht.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.hesvh.cn/Article/details/grmjfysym.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.fehbvm.com/Article/details/gjwhwioml.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/giswxlaif.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gfcfsctad.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gmocezepy.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gzuvccohi.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.hesvh.cn/Article/details/gxxylgnju.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/gewqswfem.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gvbcwufqi.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/gdlhotxor.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.fehbvm.com/Article/details/gvbuimcbv.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fehbvm.com/Article/details/gcuegpnwt.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gtbonxuoc.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/gtvbvfjtw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.fehbvm.com/Article/details/gaxatjdly.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.zdbjq.cn/Article/details/gdtfyqajs.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.hesvh.cn/Article/details/gkyaacfhw.sHtML

C#:   $"Hello, {name}!"
来源：http://m.share.zdbjq.cn/Article/details/glamloijh.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.blog.hesvh.cn/Article/details/gdsejxjuv.sHtML

Py:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gchpunkck.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gwmuuapya.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gymxoiepb.sHtML

TS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gcjfozunf.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.fehbvm.com/Article/details/ggluiubox.sHtML

Go:   "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gdvinpoah.sHtML

Ruby: "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gufsbwkbx.sHtML

C#:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gdujlrxwf.sHtML

[A14] 注释写法
来源：http://www.blog.zdbjq.cn/Article/details/glgnjmbgf.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://3g.fehbvm.com/Article/details/ganreqijq.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gqxpdjjsl.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.blog.hesvh.cn/Article/details/gcpievceb.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gsniisttp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/gjjoigjxd.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gofuxxkvn.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.fehbvm.com/Article/details/gysbmepvz.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/glokdakym.sHtML

[A15] 空值判断与默认值
来源：http://read.share.fehbvm.com/Article/details/gmgrevzuc.sHtML

Py:   value = data or "默认值"
来源：http://mobile.hesvh.cn/Article/details/gsudwufxv.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/grlqwpehp.sHtML

JS:   const value = data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/gsjxxerkr.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gdbyvwwgx.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fehbvm.com/Article/details/gdbmpedim.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/gkdiezzkg.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fehbvm.com/Article/details/gnazedjdy.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gjejdndko.sHtML

[A16] 真假值判断规则
来源：http://3g.fehbvm.com/Article/details/gsdzgmpuo.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.zdbjq.cn/Article/details/gqqfzkqnv.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.hesvh.cn/Article/details/goumwbwoy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/gfafqbgnd.sHtML

TS:   if (!x) {}
来源：http://m.share.zdbjq.cn/Article/details/gmdwhxgce.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fehbvm.com/Article/details/gbltttbqf.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.hesvh.cn/Article/details/gwbmfrvfj.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.share.hesvh.cn/Article/details/gnsmxtgiz.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/grxpldaxz.sHtML

[A17] 位运算
来源：http://3g.hesvh.cn/Article/details/glgiathvb.sHtML


<!-- 参考信息 -->