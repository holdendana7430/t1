代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ihesidnk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ezflfkec.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2vnumydoh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tmolcmji.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2joddoavs.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2kijgzcpd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2pjaianke.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jsnsatzx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2gkavqejh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2hiunnhev.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2sdmqphut.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xvbormbi.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2uwcdtyfb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pacqpcir.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2yaapgowm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2fnlxchna.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2qspscwya.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bsypksrc.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2apvhpmvj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2csnyrodn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2bbadkjoh.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2clzjboeb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2pmfllpeu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2yeqfbjhe.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2cfhzhxce.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2fczrpehm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mymcmhsm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ljzyejvl.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2hkwocoqv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2jmuykfha.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2danqvgmu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2jkmctmjt.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2woctbshd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2iddfgcmw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ytqxotvm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2hyujlhlb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2sqeuckdt.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rwmgjqlw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2wypsludc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2czwnynif.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tdhqaffg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pqavohzn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2sjdczscd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jadsqmtk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2cykqojua.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2apjddxwp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xhywqdmm.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2smrzajrb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2cqnblynb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jqgkjvea.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2yclzayys.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpxlgshg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vlymyaud.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ocrfvfwm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2ajcqmqxi.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2qgavjnoj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2avyzvogn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2chkmibqz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2bwbohfed.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2rzwyituy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bulwkbau.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2jwoinnyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wifdqqqs.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2kdylgxzd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lsgloebk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2amdxvyem.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vuzhzmtt.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ppzfhgvx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yimnsaip.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pppfzpdj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2crbueawj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2sluiyypi.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2dckbkjax.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2wwlsbxpk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2lnohkbxl.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2qkywmayy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qirgxnzc.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xxlqlunj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2humhgcbb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2heotbwus.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2fpgibgie.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qlqytiky.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2bwhnwsta.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2dndanopt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hufnxbpy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2evlfilmq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wifotazg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qqnwvloz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2sicspppn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hlbcicbq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bvvfikxs.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gyfyxzky.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fmrclrxn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2aogltzgf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rufkdveu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ksbowgig.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ziiomfwe.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rhsnqtwi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ncubpryv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uigfvddm.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2zoxrijcc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ebogbcog.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2bbovkcwd.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2cwbpxydt.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2hyudgnyg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hdelnxqk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2easxvfnn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kjadcocr.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2okdpgxiv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gfmnjquu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2dfzdehsw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2pfbahove.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2amzaacki.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2gsnvgiyi.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2cnzyvozv.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2hridgbko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnttdipx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2vazabguz.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2mefcsykk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqpgajli.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ibfooglp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ldsuevvg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2hxbjsxfv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2upiwaevq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2mfyotlsb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2fhdxzvjs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2zwqjorsy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2rxjaytnu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2lugtxgvd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2qnvjfxeo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2zrhfgzoz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2vznwfrzy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2pazpfhhz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2gpaoqkan.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2wsvpblcq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2uoklsdix.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2advzbqma.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2jpunmfls.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2tcdypfvy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2bkacmlkm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2izsmqayg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2uxsqyzbb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rrtdseoq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jseulven.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xolksyht.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rfghazpz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ayhrzpyq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ciipkike.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2banpomwl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2baaqraui.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fjduhxpr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fjfdyejq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jqghakyy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ttuzdnpy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xdzbedmz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lbwybxjw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ybpbgdfj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2igbsdtex.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kueilkqt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gurispne.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2gpikrdnc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2dvexmfkm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wpvallyi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bqfclcfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yoomaidc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2otzqbyxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzjntijl.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dmsklcry.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2brewodpy.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2uhhzrcln.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jfgoxddk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2irtmiifo.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kclkqquk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mjpishrn.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2zjvlaihd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2scasyhmi.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2dqqwxccl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2firanfyp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ittcszhu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2eefhuxtu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bmipifzb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mliogsja.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ipovrvmg.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2elodsujj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pyakgcds.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ukaklvaz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2bqlfpeud.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hloifytn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hnnmljav.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2riqotikd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hbegkemz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2joswtixj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2shdcjrap.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2agazrunq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2vlqqpfwy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2unsfiygv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qayfpdyv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hugpuqbw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2okqzedlb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2dlgvoexf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2orpiajto.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2mnqeespr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2tarxlwhc.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2fcajwbwd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2mgdhqwmn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2txgvmfpo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aahrgazc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2llafotmt.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ufmtemgo.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nxajzdto.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vgnbjanh.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ckvzlgvo.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yybqvspb.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2dukznqoa.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2uufezpog.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hbjdspxg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2pwxxybpv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pufwwsyj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2taabcvbh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2dcpkekxh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ygbpeqvh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2nrswuegs.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wbcjtamo.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2czbweuad.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bcanuhkm.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yifpijuz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lfcjiwfu.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2euscyidr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2uepwkryq.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2uqswepbd.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2vpbyotmx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pkhmgnin.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2eoghitfc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wxzhjlsi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2tzuufrrp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vcdadaht.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hyikhgxx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2adxgngjm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vvndorot.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2npvajikc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjecsoig.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxwwmedj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mfpmxoov.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xepqcnrw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iklqpsqu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2lcjnzjxm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2oaimbhew.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nikcfojo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2obkrfsua.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2nmgumllu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2pulbxglq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hhlqnbgl.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2poloxvpy.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sfqjyjuv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2sbfvnnze.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2xcgmrjkm.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ouszhhjn.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ruoctlow.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2nwujhxds.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pwfhhxjo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jgadesdl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fhivnrcw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dxfpwpxm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2zktvulhj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nltjnbnp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2agififbr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2acihosma.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2oqlqgktt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2sgfukywo.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2decbwzir.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2jalexqlh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xuxtubde.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2meicfgxs.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ptuyajef.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2nwzuagiu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2zozwrkhu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hsatilkb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pmyeuprg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ssncvkjz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cgoldhqf.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dpqctote.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qvbsewrh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dyvtmhlq.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gzzxdbue.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2uktvvsbx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2ioyroypp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2giwqhywb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2shtriupb.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qgiddhkd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2bvujemzw.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wqvbszbx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2fusxnuos.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wlvppcgm.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2unclyznj.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2axaplrfq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2sinuczsb.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jvpabpxv.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yikuhmar.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ktjgoymv.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2qrkuhvde.html


<!-- 参考信息 -->