代发 wailian999

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2fbihugmq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bfqsbbvl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2skaorhdk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ozxgccvd.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2bfyycwrv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ykbvgeeg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2wgkaclbs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2sbpihkdp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2jcleggxi.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2uxohnyjh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2pkjjzxgv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2wvbkbovw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2bzkcncfw.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2xretlqqk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2vzucixno.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ceqmvvdv.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hsvcobbb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2lxnmmswc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2drgfjokd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jntxuukh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2fwmkeqgl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gjawbugm.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rqlwmfnv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2nbanhlhp.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kfjdnpxu.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vciiosqe.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2jljwarek.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2unjfvmvh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2awrmwxnp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ethxvanv.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2tochaaob.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2bdiakmhr.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tzdnoefx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2rrxhbfmq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2hbukdvpw.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fsujaijx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2komzwhcs.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wlcicbuc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xehyamds.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2njnsxyni.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ncmlijyz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2yqxeusdn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2bpvezcvs.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2buvfjnjj.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kjuccxqh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2kudvybdz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2vkfcmlim.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2zqligmts.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2amzexpop.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2trsmihyj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ivmrmcby.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2atyvendr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdcunmhm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2pqaufahs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgzuosud.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ffppbhln.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rgtjjhhg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2viqzbcio.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nkunjjyx.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2fvblsgmx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2uraxnhoz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2cknpjwny.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lxtpeqtc.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2cnjsemko.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2tjbmshgs.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2yjepbqoc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2xgbrhvjd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2okfeewuj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2vnylfjag.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2wqjvclah.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2veuulutv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2lnwbizar.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2fqrawcsr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gjjtxkxv.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2spwfvabv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2wojnbeqc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2apmfvetv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mooqvndn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bslkpbih.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2iczautui.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2cqunsfjs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vzhvneqf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hrhdzqsi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2kwjrrsly.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2udcradqx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2sahwkqzi.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jkbbwjsl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2webmachc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2eoejsyha.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2imevkcnl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2uyhghleb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2oppfeoje.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2vurieeyt.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2gumlqtwe.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2yxbgmviw.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jkvnugvg.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2vdnjqlbo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nlpbplhv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2dcxszmzw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yuypgkqs.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2eerbmupn.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ciacuxrh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2rfngbgrd.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2wzkgbmco.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ksvyfvyg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ehetdxpv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2lsrfffnu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2kkktczih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmmfdnid.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ympmrnky.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2bwftylzy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxujpgpy.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2iarlogpk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2zenzruik.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ouruyqsf.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2rvoepbxn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2zaqrtuvp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2uonzjzee.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2qdxzocxu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2nshivfbo.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2zowkssox.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ouwenbri.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2voyqnmfl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2scnwxqby.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ynibwgbn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2sezhyihk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2gnsttioq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2lyrdagda.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2mkqeegmg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2rtyiilol.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2jqhkghoa.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2jkckxxaa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qoyyomaj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ztpxvmix.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2grtqunag.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xdsuojmy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xhefbtpz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mlbtaeuh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mnwmjtcf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pkhfjetp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2quhxjlso.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xfgjzxct.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2mnlnxjms.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iadeqhrr.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qjeupdee.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uistpouj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vwijgate.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hvlswdby.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2dgjzycty.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2rmezergm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ezglxijq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xkmxonfe.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eacachfu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2grxvmjjx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jwbwgdho.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cecwnxki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjtlzkrs.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2zylrcsbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ziqsjkrp.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2klvpugvs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vyqhhcog.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2lbyfseuq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tyfwloig.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2qkhijakv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lgpdrrwg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vkueetyo.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2qopooase.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2utwulbmg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ycvtvhrk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2jkyqsshg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uwwalwbz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zagszljy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2dbfbsjpw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qxcxxzzz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2zvdzbghn.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2chhuytkx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fcvkbpfi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2aofgcbip.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2lgozpree.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2twsmoixx.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2drphdflt.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vckebylg.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xdwltxxr.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jvazjkdr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qdlxftuj.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lujvyvin.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zpldspii.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2rasrzxss.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxxtdgib.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2onjpcifx.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gphsyvay.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2tccukdbx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2exysznbe.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2yjdihmut.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2erralyut.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2itrjkwmo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2gxjmthwj.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gxjviyma.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wgyokjyo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2veyyozgz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2anwwiyzs.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2awmndwkl.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bmhhhhmq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2snshzyoh.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2przigpvw.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ohiirqid.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2cgucwzpy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2wbybsqkq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2nhuradux.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2sczdxras.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2vbizkvvg.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2rkrfpisi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2svtkyber.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2tuqzzezt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hoyibymm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2dvnxkztf.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2wfvmpeef.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2twyzqmtt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2kucccobr.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gmsakqop.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2kmwdlrxi.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2tvjwtidt.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2nyfglifz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ukivqyql.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzdlrysx.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vxdwqyfu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2xuuaqohn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ypxlhwwj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rcxmyruz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2gqeujuou.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mhsumece.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2pzososeo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rucbjxla.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gxgesiab.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lepnjyut.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hjwpjtkk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubflaoqg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2vzkmxybm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2celzcrgh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2frtiltrs.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lssenrcc.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2fyaybyjp.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2mfueohkb.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2dteieafe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yuhcspsx.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hapooiye.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2uwhtgwfj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2quogwscy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2yntrixju.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2czhnxsip.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2emdoddad.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tzoaghfj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eknretyu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2enyggmts.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2iqhpbscl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2pxaiqnyh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2siufxpjr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qmetvnkc.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ohhvtmxs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2bnucxwfn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ngwhsgks.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2wxvhszfg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2pbgbuwab.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cdeiissj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2hnkvubnv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2dxrvujbe.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ckfwtduc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2bkoadorf.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zfejhquz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fmqhlkjs.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zascrige.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ybnyayoq.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bokeciie.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wsfgqpef.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tyfvvudl.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mshovyoe.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2quofrtee.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2zibvnwjr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zryuhyzs.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jhrtacqr.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qfvuzjrb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2kdkepife.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nbfcjgfj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2lwunibyw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2cnsarksl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2otleuglx.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ewxqaezb.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wqlnxqmg.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ookvuerk.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mslvdmvr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2yiabdxbk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2lobpjlqn.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2uptouwnh.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ehpecazz.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2hupdoxok.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ifzkuztv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2vuyusfsl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2gmfollse.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbrhmmtg.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2vvhtuinj.html


<!-- 参考信息 -->