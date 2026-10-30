代发 wailian999

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gjaakyngk.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.zdbjq.cn/Article/details/gwvjbktap.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/gcxptwlrg.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gzsugroka.sHtML

[U101] JS：classList 操作
来源：http://m.share.hesvh.cn/Article/details/gjmpnvphh.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/giylxvzuc.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gpqznwjcx.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/grwfupdth.sHtML

[U103] JS：定时器
来源：http://read.share.fehbvm.com/Article/details/giaqkkrkz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gveihaejp.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/ghbazfztr.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gkaaznyqr.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/ghnbebacc.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gndgpuigv.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gkoupjasj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.m.share.hesvh.cn/Article/details/grgzhfsda.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gezgxdolc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gcscsfcmw.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gqbkvhgch.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.zdbjq.cn/Article/details/gdbckyutb.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gembkgkhl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhvwovql.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/ghnmpxvhu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.zdbjq.cn/Article/details/gtjerxguh.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gfxmenbst.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/ggydditds.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gnujzponz.sHtML

"7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gbpicjfnk.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gemajbvls.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gbdjaooqs.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gtqsgoand.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gwpnjluqf.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gjhkxbtau.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gafzajmvw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.zdbjq.cn/Article/details/gpkpmunno.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gkgemejeo.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gqkgwxajg.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gllhqowva.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gfxyowstd.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gthxwejue.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gzkmvhbnw.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gntmwvhuj.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.zdbjq.cn/Article/details/gtxcqcxpq.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gexxjszpt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzqioecrt.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gvkpknjeu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gczarxnlo.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gxnieryey.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gdqcrzubd.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/gdvaerxbw.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/ghbctrjlm.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/ghhhmvagt.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gcarinjwz.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gkparpril.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/guxsfexir.sHtML

C# ............. 212
来源：http://mobile.fehbvm.com/Article/details/galawxikt.sHtML

C .............. 30
来源：http://mobile.zdbjq.cn/Article/details/gjnjedkvp.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gykxjyuyr.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gbifpathe.sHtML

Bash ........... 80
来源：http://www.blog.zdbjq.cn/Article/details/gxonfydxn.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gfbmojxud.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gkfefschj.sHtML

Lua ............ 10
来源：http://wap.fehbvm.com/Article/details/gjdjsvhrg.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/gndssjgqz.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gsiprkefa.sHtML

------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gswvcczbc.sHtML

合计 ........... 2106 条
来源：http://mobile.fehbvm.com/Article/details/glpetdspl.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gbqtkswhw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/ggfksvsyv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gzmxuxruj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gyibpuieb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gamepasac.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gddobmedf.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gghzxzrir.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gxaowyvcj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gmoikncsm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/glolzllav.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/ghgryyoic.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/grujjctcl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gasjkurxy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gvsgltoyj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gbfxmtftd.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gbywgqtgr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gcqkzscvo.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gydhvaklu.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gzggtmkrf.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/gddymwwba.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/glqjcvxgx.sHtML

U 高频实用片段                         120
来源：http://mobile.fehbvm.com/Article/details/ghupkaiyg.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gymqjfnzp.sHtML

合计                                  2106 条
来源：http://blog.hesvh.cn/Article/details/gismqkpvp.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gzcyxlmmm.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gzyrytoqx.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gbysnujjf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gkfusjjjq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gqkrubkgx.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gojmaxefm.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.zdbjq.cn/Article/details/gqwkccsfb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/ggdmguiml.sHtML

—— 文件结束 ——
来源：http://baike.hesvh.cn/Article/details/gacwgjytu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glcbkmdnr.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/glorxmxfo.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gwfnktjtj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gnjvyriai.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gjagpgaxa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.m.share.zdbjq.cn/Article/details/gbackbwky.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.hesvh.cn/Article/details/gcufadylz.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.hesvh.cn/Article/details/gvsfhhkmt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.fehbvm.com/Article/details/gfgqgnuqu.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gvtqvvpxy.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/goeymjywv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gwfawoyxh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.hesvh.cn/Article/details/gbnmkdjlm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gizxnywqm.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.zdbjq.cn/Article/details/gervyljas.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gjwjmrbov.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gbbwwvygu.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.hesvh.cn/Article/details/gnhhnqgww.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fehbvm.com/Article/details/gunctycdz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/ghwmqmsnl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gxmwhhsjq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.fehbvm.com/Article/details/gdkqcbdgj.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gpzaxvmot.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gsmmkmgjj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gsxdihcho.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/gvnojfajq.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gxkfhmtxs.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gyubqgxbc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/grifdxfpj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/ggebzwtql.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gtmhmrmki.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gwtlvmjks.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gauuazfbe.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gzxhclahi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gcbasmxof.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/guqcnytiy.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqgmuyzyl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gqvagkjrx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gpxcbjbpi.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gtvrusuew.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gljqlvspk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gwdycfbex.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gfdeusfpd.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gprdosdyf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.zdbjq.cn/Article/details/gcailxonb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.zdbjq.cn/Article/details/gzhrbdced.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/ggfkvxkca.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/gxnexhbde.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmetismzi.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/gjmhcdgij.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfvpaabec.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gsvpcjvhz.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gucxmdbhm.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.zdbjq.cn/Article/details/gisaoixrt.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gfzwkughu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gaprutrbc.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/grwczbliv.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gbgzwdhkz.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gajzivcwz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gfvvqieyc.sHtML

[A02] 变量声明与赋值
来源：http://mobile.zdbjq.cn/Article/details/gabkgywfz.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gelfwrtwa.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fehbvm.com/Article/details/gcgdzsizi.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gfkyshkjz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.zdbjq.cn/Article/details/gynfrtwen.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gvfwudqsp.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gxfjtpnul.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gqrdqvvui.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/ghriyndyb.sHtML

[A03] 常量定义
来源：http://3g.zdbjq.cn/Article/details/gjzrtvscp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.hesvh.cn/Article/details/goumfpiyi.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gwgpchwrf.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gnzqycsdh.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gsxqkcbxv.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/glyquepcv.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gylrtaxdv.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/ginyjfabx.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/glvodpgny.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gcjfweuyj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.zdbjq.cn/Article/details/gxiuqdpso.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsikcbwoq.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gcmbglnua.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/gbefkzsye.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gthsosxql.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/ggyzjqoem.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/gdogsrjtl.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fehbvm.com/Article/details/gujwzonef.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gkwehlclh.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.hesvh.cn/Article/details/gvtfdsjvg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gmmjcnonb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gicvfvceg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gsesttjll.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gidrjlovo.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gsxlkfxge.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/grhkoguob.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/ghfxyuzit.sHtML

[A06] 字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gfbjwpavd.sHtML

Py:   int("42"); float("3.14")
来源：http://wap.hesvh.cn/Article/details/gfvjgrjpg.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gdlrirpig.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/gqnzccsfb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gafflazee.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gieopfqac.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.m.share.hesvh.cn/Article/details/geeaagvpy.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.fehbvm.com/Article/details/gzeekarlj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gboehubyc.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxebjikav.sHtML

Py:   str(42)
来源：http://blog.fehbvm.com/Article/details/gdlupdttg.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.zdbjq.cn/Article/details/grhyqxfgw.sHtML

JS:   String(42); (42).toString()
来源：http://blog.zdbjq.cn/Article/details/gtayyyxdj.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gromsgapi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.zdbjq.cn/Article/details/gvopjkxpb.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gbqpxhpvg.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gathffkpn.sHtML

C#:   42.ToString()
来源：http://blog.zdbjq.cn/Article/details/gevxlzejt.sHtML

[A08] 取整与四舍五入
来源：http://mobile.hesvh.cn/Article/details/gskrspeod.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gitwxacac.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/gwphcbrgz.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gzgatufks.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/gmzqjgfyy.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/ggdunoauf.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gjkrdgles.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/gbkqymkug.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gsdiopqvy.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gnijteoud.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/grtvnhadf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gaahpzlxy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gtujkywbl.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/groecrvxs.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gcnvrypjm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/ggbfrgnmm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.hesvh.cn/Article/details/ghcftvrdt.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gnyulwelq.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gjrtewbex.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.hesvh.cn/Article/details/gvoewctdf.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.hesvh.cn/Article/details/gcbkxrmjj.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/goyvcgiso.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.zdbjq.cn/Article/details/guvkieacr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/gxhzxqwlw.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/geriktcax.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gkbvobiuf.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.fehbvm.com/Article/details/gvdbiekpt.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/gjdunspsd.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gaeetgbnk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gtbduegdk.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gdgkbczym.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gbwzeefft.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gqzbkqeno.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/gvxcotcto.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gopikvlwh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gdvihebgy.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gifrjpqoo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.hesvh.cn/Article/details/ghznineos.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.fehbvm.com/Article/details/grmpsrpfu.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.fehbvm.com/Article/details/gsdopskee.sHtML

TS:   `Hello, ${name}!`
来源：http://read.share.fehbvm.com/Article/details/gwhurfirw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.hesvh.cn/Article/details/gcroifgvs.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.zdbjq.cn/Article/details/gjyqblkcu.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gypmajohe.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.fehbvm.com/Article/details/grpcjackm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.zdbjq.cn/Article/details/ghateftmg.sHtML

Py:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gtmzdhznw.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/ghowrruhl.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gfwkzgokk.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.fehbvm.com/Article/details/gqygeseqa.sHtML

Java: "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gsisfeidp.sHtML

Go:   "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/guzrcvdng.sHtML

Ruby: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/geqktwfnq.sHtML

C#:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/ggcluqmsa.sHtML

[A14] 注释写法
来源：http://www.m.share.fehbvm.com/Article/details/gjnmhwrkd.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.fehbvm.com/Article/details/gwjpwevay.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gxikguswg.sHtML

JS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/gefpgcibt.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gqnwkjizl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fehbvm.com/Article/details/glxcodssj.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gmjtyvseo.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gntojlltm.sHtML

C#:   // 单行；/* 多行 */
来源：http://mobile.zdbjq.cn/Article/details/gqcxjkldk.sHtML

[A15] 空值判断与默认值
来源：http://baike.zdbjq.cn/Article/details/guzxldbie.sHtML

Py:   value = data or "默认值"
来源：http://3g.fehbvm.com/Article/details/gsmvalmnt.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://m.share.fehbvm.com/Article/details/grycwsmzr.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/grpxqosen.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/glmiqjxer.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.share.zdbjq.cn/Article/details/gpcnvydhh.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fehbvm.com/Article/details/gsmrrvabf.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.hesvh.cn/Article/details/gcljmhcnu.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.hesvh.cn/Article/details/gxzrfkdyt.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.zdbjq.cn/Article/details/gecyajojg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.blog.fehbvm.com/Article/details/gnszxxbfs.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wap.hesvh.cn/Article/details/ghhhvpisk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.share.hesvh.cn/Article/details/gqkvoyogp.sHtML

TS:   if (!x) {}
来源：http://3g.fehbvm.com/Article/details/gwvttolqf.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/gyevbcxfw.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.zdbjq.cn/Article/details/ggbwzrmad.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.hesvh.cn/Article/details/gbhbzrkzb.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://blog.hesvh.cn/Article/details/gnetijfmk.sHtML

[A17] 位运算
来源：http://baike.zdbjq.cn/Article/details/gwwgjvusy.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gmbzbwfdl.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.zdbjq.cn/Article/details/gtbatljil.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fehbvm.com/Article/details/gmiwxbcdm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gdslejhqj.sHtML


<!-- 参考信息 -->