代发 wailian999

[U99] JS：事件监听
来源：http://www.m.share.hesvh.cn/Article/details/gnfyosxck.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gobrvabuc.sHtML

[U100] JS：DOM 查询
来源：http://blog.zdbjq.cn/Article/details/gehgqnbgy.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gcspugxov.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gfycvsfuq.sHtML

el.classList.toggle("active")
来源：http://3g.hesvh.cn/Article/details/gzawszzxh.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gungxjsrk.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.fehbvm.com/Article/details/gqqkhfsrm.sHtML

[U103] JS：定时器
来源：http://www.share.hesvh.cn/Article/details/gswjfuotz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/gkrwjtzuw.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gwfbdziuc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gngypnico.sHtML

[U105] JS：节流
来源：http://www.m.share.hesvh.cn/Article/details/ghszvffph.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/gltivuhps.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gburgzrnt.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gzvrgtwfd.sHtML

[U107] JS：数字千分位
来源：http://blog.fehbvm.com/Article/details/gykhpmryr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gkqpeynkp.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gmhqlzljb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/gvjwssbse.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gjhlmiyom.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/ghntzwcsp.sHtML

[U110] JS：数组分块
来源：http://www.m.share.fehbvm.com/Article/details/gpnsomynx.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gczdrpquk.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gfbcsdmyb.sHtML

new Map(Object.entries(obj))
来源：http://read.share.hesvh.cn/Article/details/gdejljsdq.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gsodmlnjf.sHtML

"7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/ggherfxub.sHtML

[U113] JS：正则替换全部
来源：http://wap.hesvh.cn/Article/details/gmqrlgpju.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/glcpxupbv.sHtML

[U114] JS：JSON 深比较
来源：http://www.m.share.zdbjq.cn/Article/details/gcqwedajx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gnnbcnhwr.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gkcaeawqq.sHtML

crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/ghmchfuej.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/ghennnmcj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gknyezcrs.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gzhomjfmv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gebrhakkn.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gyzqnfxfz.sHtML

npm i -D vite;  npx vite
来源：http://blog.fehbvm.com/Article/details/gjktdkggs.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gqfkavjbn.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gnelgkzvx.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.zdbjq.cn/Article/details/gvafzscer.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gjpmajjnv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gozqvjxpa.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gitfiadth.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggpzyfzdo.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/geesftkrv.sHtML

Python ......... 252
来源：http://www.blog.fehbvm.com/Article/details/gqcwgiuxa.sHtML

PHP ............ 252
来源：http://3g.fehbvm.com/Article/details/guyiazpem.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gqcxrstro.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/ghmcytxkf.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/grbvynvps.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/gebtfjesh.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gxnldzkvl.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gxiqifibh.sHtML

C .............. 30
来源：http://mobile.hesvh.cn/Article/details/gpzbtkcnq.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gbqkziwjl.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gluglomuu.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gntcnocyi.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/giyssfcws.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gicvynlrk.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gvlivjkst.sHtML

Perl ........... 10
来源：http://mobile.hesvh.cn/Article/details/gruiaysyv.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gdbbgmhli.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gookbsoac.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/grfeifhql.sHtML

按章节统计：
来源：http://m.share.zdbjq.cn/Article/details/gxzkmlxcs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.hesvh.cn/Article/details/gktctbtls.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/getwevkho.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gjcfwhnvh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gpisecwdc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gognxjkyw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gkwdquxys.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gyxbgpywh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gzexumcyr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gjsgqoxkv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/guzjbmjrz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gpijgpigo.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gntseckfh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gkfswibpc.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gircejtun.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.hesvh.cn/Article/details/gwoaceglx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ghoczbutm.sHtML

Q SQL 专题                              90
来源：http://3g.hesvh.cn/Article/details/geaxakbcu.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gxfgryxes.sHtML

S C / C++ 专题                          60
来源：http://mobile.hesvh.cn/Article/details/gvshgyhij.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gjmbqlkmh.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/glmbjvypr.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gyskmmfzl.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gazbbumhs.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gahtkjgjv.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/gwhudqgrn.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/glygfpsgs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/garanxnul.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.zdbjq.cn/Article/details/grepbjvvr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/ggdaofiox.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.hesvh.cn/Article/details/ghgbrrmen.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/ghmdjvduv.sHtML

—— 文件结束 ——
来源：http://www.blog.zdbjq.cn/Article/details/gmnbgpwue.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gudtnensj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gewcqhprv.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/guafjzosa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnmnlsjaj.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/gjlqkqaqj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/gdbyxuziw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/ghmgcoqrg.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/guaqtubmm.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gcltcdnrp.sHtML

【使用说明】
来源：http://3g.zdbjq.cn/Article/details/gfuqhpvph.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.hesvh.cn/Article/details/gygeyfpmt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/gltacmikg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/glpnixsiw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gsxwuxrsj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gxoqrwwgh.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.fehbvm.com/Article/details/gocnptvef.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/gauszuclr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/gigqcslsp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/guaetprtw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/gywysjgvc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gesjqozcc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gkojfkzop.sHtML

【文件统计】
来源：http://www.blog.fehbvm.com/Article/details/gcdkgrqhu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gluudxaeg.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/ggrmsiicd.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/gscucsobc.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gwduecvjp.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gyqlvzjth.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gxdadohng.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gbvuuzodb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gfmryjlny.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.fehbvm.com/Article/details/gnvvokwcw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gjwejshen.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/grhjwuyba.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gjwicoika.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gdyxbmwre.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gpqeiqenj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gaicazgbo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gznwnoiiu.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gbcojqoua.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gpwncnvlz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gglcitdff.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gxkafxnmr.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gyvtsqutk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gpyzbwhri.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gyhrylqnx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/glkxuazgp.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gdjzadnmk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsdjfeesz.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gocnlitpq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjnpsjvsx.sHtML

[A01] Hello World
来源：http://blog.zdbjq.cn/Article/details/gpsvqukpl.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/glvkhvgez.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/ggmetcmui.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/ghiikoouh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gwmpurwfq.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gqcdwuymo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gaecgrukb.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fehbvm.com/Article/details/gnvokeuyv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gbxutyrmt.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gweovdlji.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/gbtcbzpui.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gqjsbqcow.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/ghpuzywxu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.zdbjq.cn/Article/details/gxqnzkgmo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.fehbvm.com/Article/details/goycjxfye.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gfakmekjy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.hesvh.cn/Article/details/gbygbxmhy.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gwjszlzov.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gvfqbcbus.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gwppvdhdn.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gmgtapjgx.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gkuwhsihs.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gkbjmvqhe.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ggtpjutat.sHtML

Go:   const PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gfqnhiffi.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/ghvyauxeb.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gghkinwrq.sHtML

[A04] 判断变量类型
来源：http://www.share.zdbjq.cn/Article/details/ghcegfabb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gserngsdk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/glheuguea.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gqdmjbqts.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.zdbjq.cn/Article/details/giytuswmt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.hesvh.cn/Article/details/graumfefi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gaxqmxult.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gevblfekk.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/ggnewgqxx.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/gjnusxnku.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.hesvh.cn/Article/details/ggealzzlg.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gbupkabng.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gveoxqlki.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gdngquoar.sHtML

Java: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gzvxqwxlo.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/ghxhyxalt.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gennhsmiq.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gbjgdggfh.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gjccwxibs.sHtML

Py:   int("42"); float("3.14")
来源：http://read.share.hesvh.cn/Article/details/ggdzyxgzq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/gvifatzlg.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gwxhnekdj.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gpmibfqhn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.share.fehbvm.com/Article/details/gzwihooov.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.hesvh.cn/Article/details/gjaktekdi.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/gdhrmddct.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gsyigidub.sHtML

[A07] 数字转字符串
来源：http://baike.hesvh.cn/Article/details/gipzrmxxz.sHtML

Py:   str(42)
来源：http://wap.zdbjq.cn/Article/details/gyjxnbrlv.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.zdbjq.cn/Article/details/gqfhnrwyb.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/gpduuakch.sHtML

TS:   String(42)
来源：http://www.blog.hesvh.cn/Article/details/gekrqsqoo.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.zdbjq.cn/Article/details/gdxofsqxu.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/grepclhkl.sHtML

Ruby: 42.to_s
来源：http://www.blog.hesvh.cn/Article/details/gnugopgpb.sHtML

C#:   42.ToString()
来源：http://3g.zdbjq.cn/Article/details/gmosalxsj.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gucjlhmcb.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gccqkavqp.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fehbvm.com/Article/details/gouygzasq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gjmyxdzjw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/grgavicmk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/gqspahdmu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gogtoopge.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/gctdzdfua.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gamhejgrp.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fehbvm.com/Article/details/ghdyneujv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/glzpdcxqk.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gyednciig.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gjmiqtfjn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gevgtpkxt.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gyacojzdz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.m.share.hesvh.cn/Article/details/grfjnlnwy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gmgiqbfnp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gecfnwxdx.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/gamoqbdej.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.zdbjq.cn/Article/details/guminksnr.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.hesvh.cn/Article/details/gvlcntzmg.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gzwhmkbiu.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gxnasxrdc.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/gqrctjyir.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.zdbjq.cn/Article/details/gbwuxbvac.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gdzudtbuy.sHtML

C#:   new Random().Next(1, 101)
来源：http://3g.fehbvm.com/Article/details/gxapehqir.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.hesvh.cn/Article/details/gkikjxujw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.zdbjq.cn/Article/details/guahubkjt.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gnwmmgbsm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/goamvgxqu.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gxjnjqxdp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gaadrgdgs.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/gdkoqpvis.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gydabnfik.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gytcrtppz.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.hesvh.cn/Article/details/gvltiowcb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fehbvm.com/Article/details/gbuafvukk.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.zdbjq.cn/Article/details/grtebqxdy.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.hesvh.cn/Article/details/gpbvhubho.sHtML

TS:   `Hello, ${name}!`
来源：http://m.share.hesvh.cn/Article/details/gbxvsbnlg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.fehbvm.com/Article/details/gdkicvlcv.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.share.fehbvm.com/Article/details/gmowykxra.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.hesvh.cn/Article/details/gjznnxvsu.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.fehbvm.com/Article/details/grhbebjtc.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/gxwhcavdj.sHtML

Py:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gdlpyjyvg.sHtML

PHP:  "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gfwwwrgxp.sHtML

JS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gyxlzbgbx.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gbdsfvnyz.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/glpofpshe.sHtML

Go:   "第一行\n第二行"
来源：http://www.share.fehbvm.com/Article/details/ggevzwwgk.sHtML

Ruby: "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gwdcohpgh.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gyzcioehk.sHtML

[A14] 注释写法
来源：http://www.m.share.hesvh.cn/Article/details/geunacaip.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://blog.hesvh.cn/Article/details/gsjkjyoxd.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gfskjjvyy.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/grxqgvzvn.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gngjladlc.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.fehbvm.com/Article/details/gqpmsqhuq.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/grwfdtqjy.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://read.share.hesvh.cn/Article/details/gmlgvoymr.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gctkqlgyz.sHtML

[A15] 空值判断与默认值
来源：http://mobile.zdbjq.cn/Article/details/gjfrqwjfe.sHtML

Py:   value = data or "默认值"
来源：http://wap.fehbvm.com/Article/details/gcyqkxtar.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gldcuakvm.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/grkuzfiuz.sHtML

TS:   const value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gibbjgvbz.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/gjdyxzagb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.fehbvm.com/Article/details/gjmetrchp.sHtML

Ruby: value = data || "默认值"
来源：http://baike.fehbvm.com/Article/details/grpuhinvf.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/glzxkmtot.sHtML

[A16] 真假值判断规则
来源：http://mobile.hesvh.cn/Article/details/gaaqsftap.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fehbvm.com/Article/details/gmvaniovr.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://blog.fehbvm.com/Article/details/gqmqygasp.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://m.share.fehbvm.com/Article/details/gsnznssix.sHtML

TS:   if (!x) {}
来源：http://www.share.hesvh.cn/Article/details/geoestyid.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.zdbjq.cn/Article/details/ggkwzomus.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.hesvh.cn/Article/details/ghnpokzvy.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.hesvh.cn/Article/details/gsiebuptl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.zdbjq.cn/Article/details/gopdjresj.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/gqnhseext.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/ghgqarndz.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://blog.zdbjq.cn/Article/details/ggyonvfgl.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gkdyricek.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gagxslypu.sHtML


<!-- 参考信息 -->