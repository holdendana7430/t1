代发 wailian999

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2wxowwfel.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wjobirmq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gbvfnhgf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2diwlengj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2eplumbxm.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2vjawwhoi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2muqtwhut.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2qqrbtgml.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2mgmagyte.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2htibmaej.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2pudtgvko.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2dbmdmnaf.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2mbqtzhyy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ytyylvnj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2suhkvwcn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gflptdxk.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2nghlcmfs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2encmicwa.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tkzffkgu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2wxivuvjl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dfemaiuq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2oprkxdjs.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ktvvzqob.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2zfbmbxzs.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fvgqbcjm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2yxonwjli.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vnlqexbm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vqwzbgbd.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qvhrlrfr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2pgxancep.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2gnnbvlhp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xfclcmrt.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2ppywenec.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2npggwkvi.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2vfnyjmdc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bpghqpji.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bhrwrzyb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2sygelxlz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2uyqmdhzo.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2wzosnala.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2blhswjvy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2dhpmdkwi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2eiyjmmei.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2pzzsyupb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2bkydtgod.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2iqirllcp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ulvobrfv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ahlukrpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iiepvaoj.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2hhrpurtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddpfzzkl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2cfipqcss.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2fbtikccg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2frxjabyb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fpvctvnp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2bghbkbgs.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ynluhqke.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nauuqjrm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vvfyfapw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2yglatzxc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2vnocokvo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2kiqumwnn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2nprankuh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2qqsxmmay.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2necmpvjj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2rgmfdegs.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2livakcar.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ejodedho.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2oihaosgj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lolaqjav.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ilnaqmjc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2exdlyrli.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vuhjuyfp.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vavwkwtv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cfspvull.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2quyqkgsw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2sbeimaga.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wsyjquya.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2bmfqtuoi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lgqbfaav.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gndrenpd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2nytsjkfb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vvvouhcu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2evwjfidp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sxpseeue.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2doopkhqb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2jfrsirvb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2djprundi.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2epvapvtf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2uxmcmghf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ssbydtha.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lujrckme.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2okuykzia.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jmaxoaux.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rijdwjpu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2trkmgdzm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ptiraajq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vgtengvc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2vamszpek.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2mipvkwem.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2rlwztztv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2rfthuagx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ttqhpobt.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2wdxzhvda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmkvcaum.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2abhkxjxx.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2cehsbffj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuayhcmz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2bmekuqat.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2fdrikiry.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2xcpytvhc.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2brbflwir.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2zxrvyqvl.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2cgtglvoa.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2pykgfrhk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2gxvliylt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2sixznnfc.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ybotfmik.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2yiknssvm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2tyyskvqj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2klzefqxr.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2iljdribl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ixklschj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2axivhttk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2tgpugvir.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2otxatojf.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2yfcpesms.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2zgatfetg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wvhngwbn.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2tzuudqih.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tnhosome.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2avgejjuw.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mpqyrvwm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nulifkwa.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2gauhhflu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2czcmvhmd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zfqnjnuf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2okkphqoc.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yxsawben.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kjncdrfk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2olghjsao.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uamfikvw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2trjylkhq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kihyihxt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bqpduult.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xtzhyiby.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rovwtlhs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2adtomqnh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dbnfpgek.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wzluxeuk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wknvikbr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mmtjrmok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfvsqhvo.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2zbegfjyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mobqjyje.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2eojvbjwf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2kgqjbhuz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2plonfrgx.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2eehynesl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2jxravtbg.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2cwenegmf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2qhsnrxjl.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2hrvezevo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cmbpbise.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2zvuvbzrf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2zodgebkr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nexdjcyq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vmjpvxzf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2tygacnik.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tebkcakn.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2bhvrdajv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2gklzvjoh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wkhdfnhe.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2matyxdjs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2mbjgmdxg.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2igpfewct.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hzqygmnu.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kallxdyp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jqndhylx.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zaxgpcko.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2fmbfmemx.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lffdweld.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2yopdqrza.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2vliclatv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fwhflzta.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2reaayvqv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2bzbletzl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ljpdpdgv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ybzrpfdg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2xfqnfyeb.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2bcpsqfku.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2aopujzrn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ylpsawla.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ybotasrd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2atuazqsn.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dcvqjhkm.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dapopucb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nxlxxaww.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jovtnmnf.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qtmvvjro.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2klnvyipj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2irqmkpxh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2horoldmr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xiufwobe.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2sfvjxopk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qnpgbebc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2hnunercj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2hpvvoqpe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xjuksdot.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qdkuxysz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kspmntdy.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zpjarodt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2pvseguvr.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ppxnvauo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cahseawr.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qjcvdpam.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2yenvjmnj.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2llthsylh.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2cbnenfwj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hhctxwrk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2xoadzznn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jwsdmmuy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2bmouczcr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2atusgduo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ylvvxkqq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2arkqdmbi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hiyohmze.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mkjaefdk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2prbhozjr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ylsnfpql.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jkezwynl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nixugihf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2tchqwuip.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2hmzbvsro.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2wlcfbhyy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yemhigjn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ikxbwaib.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2oqltbebo.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2qvkdfomc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mbqnkykq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hhfcofgp.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zixrmvst.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2wvxqawlf.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ozlglhqy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2fybuxxvp.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2urjrizup.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fsjheeeu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wkalvsfl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cstwduzk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ctsjnyrv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dstzoxwv.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2utyjfapi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fmxvphbv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2airguzkt.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jrhitodp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2tecpwjjf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2vmtxolul.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2lntfsurd.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2kbxiqlkx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2etmxzogr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2gixyzhqn.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2gqydgavx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2xgoreoyq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2fysnfhqa.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vkthdkwq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hszbzjfx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bazwrlvo.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lwduydge.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vpeefwns.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lfkmjahm.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nhbpgzqq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2eafmiltl.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2olzcnxcj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2oyxtsjjr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uaegigdg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mntrxggx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zpmlaevx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2czyvjsjr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sqjdgxqv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2ckgdckzk.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gqmyller.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2iovgmteo.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2iirlivhf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nsvxyttl.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2eiujnunu.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2karcdjih.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2uypwneem.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2jpcxouwl.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2httdnfgb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yyvgvmxp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2bhggsnhq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2fvoiqbin.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2lsqcmgem.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zhhpnrnq.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgjlwdea.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2embnmfnm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2wbnebeyx.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2pgiyqxmr.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ciowelnc.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ryjbecyy.html


<!-- 参考信息 -->