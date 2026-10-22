代发 wailian999

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2jptrbppc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dkyfpdvi.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ixfyikma.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ijeqjkct.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2fkxfgxve.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2tvkqamhp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2nofzeeyu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2stgjoiqz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2lstygoio.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2afzitwiv.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2wzxnzvby.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2mjzryffj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ozryhggz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2etbbjvzq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2zmgmthhx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mrwkeohe.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2hucjqflr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zpfljeps.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mmpqawuk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2gywbhfrk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rlugtlkv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jvmtpvjv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2iilcbifv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2agoqfbxt.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2lwcmasrp.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wkympcre.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2kdqwjuka.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2cpwvtowc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yexnkimo.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2lmarcgna.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2adbxpfgx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vbvqgnrh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2zlbikfyi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2khursvsw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2qkfreict.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cbvfcufz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2byfzpbld.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bvdduajw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2cgeciglt.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cmshmkjv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zjxlqunu.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2cqgpnpne.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2vgyuekfc.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2iypomnln.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2niayimbz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2qvztmtrq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2wvgimuvs.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2skqahjth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iavvcybx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2wdjuxdin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcfnkqkm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2yoizgcai.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2lxokeerg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2kptkusve.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2qrkxvknq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hgxehizq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rvsytmgq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2skhqoxal.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mqleqqrx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xdppehai.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2fsqqmzvh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2uvmizhyq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2fkmxungo.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xbrsgyhp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ywhskdmd.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2yfknhova.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2rvhvhsxl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nacuhrht.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2webplsme.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ngmfgjpb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2qrcccyod.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2wowmidwi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wkkmdqzf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qtgqweok.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lrnmeuvy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2egewfzjn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2rjbvzrpd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2yxomjcyq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2aujeszxj.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2zumljgfd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tphwfzaa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2wwvdsama.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hnrruzft.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ytlgvwjv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yvcfbrko.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2evcgrlbr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2meqckcxj.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2elsftyot.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2soqglnow.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ygatpviq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2szgunxvx.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2kmkvnhra.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ucqyhgzb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cdmqxotd.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2gqyjtpst.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ticxorrc.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2fvdorwvk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pqdjaqgp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ivrkwjii.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2pjaftszb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2nwdwaixu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2xnqfcpws.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2rymjajoa.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2czjruori.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bysfcmre.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2hhfzdvjk.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2chxvlban.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojtsktim.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2iipkietj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2gsoieomr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2kekzwtmr.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2uprhblcm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2kvtcjoxf.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2eipvrmhh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2pjzzmeva.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2zhbmggqp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2vamdntaq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2aywguanj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2jxflxsec.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2vldtxmgr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2wigpgutn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2afsieypb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2vpmyabdv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2jwizccbu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2nwyfskvh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ukucgeap.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2xnrmbvnm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2mnvkdzkw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tcycmqob.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2fnpljxkc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mxkqkrkp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2owlcbmvc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ywxqzrtp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qoxxatoz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eihhchle.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2aaqxwlan.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ulygpqze.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2quvfoxdw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kjtycfzw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wbjfzcba.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nmmacsnu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vapoavfq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nkbspsul.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qpbfihoz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lrwcdtdo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2xtsgmsxv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2numixxxy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2dnluqrqw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qzhiqaxk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2huxsrazs.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2eahyyxkr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bovmesfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecsnronl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2hrmkbhtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2falsflkh.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tmsrcieo.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2uezlqtmu.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2tyangxic.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xkxicphu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2slxysjhm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bikubvhu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2aranumoo.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2uaqinicc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zigrcawk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2dvxijjqq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ppwuqpkx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uxnrqboo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2icgacqci.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bsduzzsl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qftftyox.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2hxhnzbkw.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2harqprjg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ayzkxuyr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2jvbojvxw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2wzuwiqul.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2flujllpd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gfrxoatc.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qxzlqpsv.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jyedtmml.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2psjnecov.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2gtbzmkvo.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ntkufztw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2gkdnnanb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ocmgxupo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2fmoxfbml.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wjjgqrvr.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qsawqfpq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2vmacxnmf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2xnkrckha.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2wmmasyie.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2zjxflobn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2dyvtibve.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2zqzzmogl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ypwusasz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eaxkzgpl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mhqssbbb.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qomnocyt.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hkujzjxt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2psbrwqme.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jhnnotes.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qdlwvznw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qzuixbum.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wenefpbu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ujlthxke.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hjsxtljn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nunmunfe.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2xktnuvjh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2znoqbacp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2azezscsx.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nhspihlj.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2qajdldkn.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mxfevmgw.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2zccvhyde.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2cgxrsvor.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2aakiguyy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uhhahnlh.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ftqwyyzv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ulzskboz.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2isoedgah.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uslacdjh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2vcuyxmam.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vqkymtyo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2hapjktga.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2iggyjjvs.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kcehktae.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2goztlksm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lictbpmf.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kycirpxd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tpbdrwsr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2emahdgtw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ptjniblr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mdpxehap.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ydggfskq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2yqgomswq.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2oowpfcer.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pypghxpc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2grlfrswu.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2ezmsjjre.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2iwocrkcr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2imvcqgza.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tzkugofk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xzuudblk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2eeynkvtx.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2dtkkjoya.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2euisgmkh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2jvldugco.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2clsacmcw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vhgucbno.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2owlftcpi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bbzdacsk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xqrdgngo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2msjnobfh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cgubwrez.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uvrofanu.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pcmdlkon.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2kguynqjg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2gukmqawy.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2oygmkozy.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2gbifobhw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2rehlqyza.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2iicdvwmm.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2czdjrxgh.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2rfrdnkge.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2zbvdfqhc.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hxkcqnkk.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2btiuomaa.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lolvcywp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vzjasfuv.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uxxsftum.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mfoyqynq.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ivlhecpr.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2luuiakqi.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2qioawzsi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2dwkydwlo.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uolrlfly.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hkkosafe.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wcvaqztc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2pycmgplr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2phiodjxq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2vggboilu.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lnoqmood.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2rgbouomv.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zonsrnuf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2eepelpyo.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dakrgkgx.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hownnvqs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ohuqbrvu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2idrhblbq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nbwchten.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zsxgkaky.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2oarezvem.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vqvtgnjn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ussjntcc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2ptnyxxyr.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oiequbfc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2tixpdmpj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2rspgppix.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kozngouq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qaubkokc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2diqafkbt.html


<!-- 参考信息 -->