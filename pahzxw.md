代发 wailian999

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2kqsomhbp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vzwydsgv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2klstsmjx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2armdrgdy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2jjrgngeo.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ajysxudg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2gzczpqyw.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2bokijgdq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2hcszcqpd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2tljjpkbw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2islasqaz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2itcbbzky.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2pzbkahhk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2nvtxetlk.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ngwdjjyb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jxxxwqji.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2kwoyyqhi.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2usycqics.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wuwgqkes.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2qfphuxhs.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vbeuijic.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gxvmfpmx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2aqaamzbu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2kgscnazo.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2jbloxsjh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2lnfavpgb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ggbdcgbc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2sshzatne.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2spxmtlhn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2juskojww.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2zphffzyp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ciacxwfp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2qsglozkj.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cbhvgwnw.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2eeexxdeg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2mksdufrd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2bdihburo.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2czamkmmg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xjjeamez.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2prdqehtj.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zahuspbc.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2yoxrtooj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2mtzwqnrc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2zinpsxoo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2pwxmxshp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2jokyqrvv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2cvrifexj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2dwycerfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kizsslvo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2dxdoqngj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phoeyhnm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2hrbcylqi.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mwqejqdo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ptizjrfy.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2snmyeyep.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nydotarv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2thyrqeno.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ovjbmpqu.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2oxsvpfhh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2vptqvrmb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2iemyhflo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2epjmndqy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2xjpyeuiy.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2efpfkiku.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2agadmqqa.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2iofwfuii.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2uoiqcobx.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2kexohtbu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ajgxjnjo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2thurwusz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2tswpwevn.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2kvmumyep.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ggkdachs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xvijgwqn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2evqlfuxj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2yitvucwq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2eglehifo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ubofsknj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2oifdhonz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2sbamuako.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vehgowpp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2oahuqpxo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ffmgsune.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zdxdlgfx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eycwvvrk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wvbfqdul.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2zdcacnru.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iweumlet.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2bnzszbvk.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2imsnfqbo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2wcknswal.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2fvfonuwd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2dnnrmsek.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ybrqfekx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ozwxmwux.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fjmvozgt.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2pyjwjppf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2larxvljs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2soelxtbz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2eziwwkbh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2qxxauhrg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2cabsioxb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2klqfkbyj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ufddtrcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgifufol.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2cttmdgbn.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2cdggtaml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2refpgcxi.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2yjtwclvu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2bfhchaif.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2agnqgthc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2lmcxoiet.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2kolfsxtn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2xrebmhrs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2nfnvyqmx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2rqphvjgd.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2nmgiepgp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2dguvaelc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2gqhdshru.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2dswogvmd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2nrsukcmu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2mnzuxlfw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ouepubke.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2grgudgrb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ywqbamen.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2prrfovbl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2wxsfszhx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ejiwmzcq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tfernrpg.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2xydnqixb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wjskywpv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2faaetnor.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2egkdaamx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dvwqwnwp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iqgjxsjh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dxyneyke.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2dloqpxyk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2rjjpnbmf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ogxnhywt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nojqgmlo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2sgohzfof.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qiawumyu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uoxdsyle.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hnnpnlwr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2jwtfxyty.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hknnkrtv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tayymcww.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vwkvwiur.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dsbeyeez.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vjhpvbru.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2uayjbsjj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wdufiuos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qnrsauoz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2gpniszpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfjgvryg.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2iyhdococ.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ppggftan.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2lzkojlbd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2uawsgngt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2qovnqjhs.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kpgnsrau.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2qjkmczus.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2lreqpddo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2stznprcj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2gddrxlks.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2fuaezvvq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fqstdwoc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nkhgiwag.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tmfmnlac.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kqpwofpc.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2aeisvluh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2uekxgiak.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2opyzflrv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2zxbygwxq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2wlctwlza.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tdfohizc.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dnbdrxrc.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oilvlmpx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fkwdhgoa.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2dkcfbcer.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2inuvutlo.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tecgixua.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2phpwygfp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2hjtsqyjo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzkhoxrr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2mhvdevtq.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ewyjwrnx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2jlhhxgst.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2lktwfbpc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2pfguvtfq.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2rnqrxspi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2wgmefbev.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2cnfddmpd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gpodlewt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cagntbva.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gijhkkck.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fkiygxkh.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jjhvyono.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hvampxqm.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ggdyxzla.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2bnygtgde.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vvgnitke.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2dpohxqkq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2eykdaimc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2dsiazolj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bwggench.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qfrqelpi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2aamyrjxc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hkyhtwfy.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lgzhzkkn.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iupoxdpt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2rcaqkiba.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xdhsvhnt.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ftaieaoc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lbrjspfy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yhkgwhko.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2acuujkdc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2bwyjotec.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2wepxqslq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pzlnfqjv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2wgsqrgom.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aaicebvx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2yoedrxto.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2joorjfdz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2butsjwzu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2hnyvqvrz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2skrnzdul.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qbworhoj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2utohfyxd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zxcwwjmz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qnbqeilk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cbflrdin.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yqkhvcuz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2sqryvlsp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2eklgddcy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ygsrsffm.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2vlqliimd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2hwtlbchc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2exrvfebv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gflhsrbk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2picqehbl.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kfxjauwh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2vmisdosh.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2btqteedj.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2yyulzmjx.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2yohoejan.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vvliyfua.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rdggfjvf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2znablrku.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rinfbxal.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oanbupnk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2esyxjfol.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zwywwqzw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lgyjdbun.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2gqivhvor.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2jbujcnfe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2yyztpsfw.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2yshewadz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2arkvnxwr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2mftahotj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ymudzafl.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2plcytmeu.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2mabbbhyi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qaugrndg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zkuqsebq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mxxmjler.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lqtlrgms.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2veowvfca.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pnabjvuw.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kqwadker.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fdhexxix.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zhmpjiti.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2eivnvaue.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2cpkelfcg.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dslfzpmp.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vfapekhf.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qtikosnv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2ffbvelph.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jfjzgaaf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2celklhes.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kxbbbllh.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2hbiqvmtx.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2yyhwuogo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lqotxukp.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uqmkjkeh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ysmxrzdv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2orgevmco.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2webszyzs.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2oubtzuhn.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mqmaqfpd.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ygminaza.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vktcpbza.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2bsozxwrw.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xcvltlqh.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2apmzysnh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2eqotsxen.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2inzdzavr.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ahgvaakk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2saphldmz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2gvswmxgp.html


<!-- 参考信息 -->