代发 wailian999

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2eczfjnrf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ijhkfswu.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2jnakvigr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2jefzgwef.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ajatgasv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2fabgmbvx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2gdewzgaw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2fqqlczos.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ytzmkbib.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2hwgywuen.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2enrutbfl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2ubqfkkwr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2stlsolru.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2izcteyoh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2gfpdxfqf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nzmeztks.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2jxvodjhh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vkhuzryf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vbotktnl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2joyelafq.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2icrrbjiq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2thnmsxik.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2bogyhpzs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rtujndzt.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2saqclskk.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hmfbeplx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2cbbvjztc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2uslxreba.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gfisjasr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2dwxcxhbr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2kcpgfymf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2irwcgbgv.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2hqssgshj.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dzbsjtmf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2bxyhzwwy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lqxhpaxm.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2yvncnvne.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jorvamlc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2wlwodxxx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuvrpyiw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2bnoujafm.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qqhoiffy.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2pikfdrma.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2cwfkcjvg.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2zzcljqjj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2xpjihkbe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2gyojxcii.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2brnavzuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqqhaatf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2kjbvcavw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nuyvfgmk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2mqsyxlmg.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vsxekaxz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ypptggtf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tjduryfe.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ipbxzgnd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ayldtnfa.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kmsipwez.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2amzeemfd.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2qvumyyul.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2aipzwhjg.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2koyjnfgs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2irpetoel.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2qkqolyzy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2tffhrgvo.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2juqijpra.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2iiwguwqw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2algmhzxj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2nutdamrn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qirxsceb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2zztgoxtf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2bzwanuuw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2jfzfjnok.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ppjkrbhj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qblgodvs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wkshrwqx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2vywgpnwg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zeflkoux.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2yaeznihf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2yfrwanjh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2rmohxvuv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rdyoucno.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qufgfiey.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hzjuilyk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wjbplooo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2oydhpham.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2onjjoljq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nyadtwbq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2idcbeqfg.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xcbhznnx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2wwxjamod.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2lvwhesqd.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2cvizllhj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xdwkxiif.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2rafblgci.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ibcczhhs.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2juxbdfwm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hhsfntrl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ahzrmbmz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2enogpfpo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2yqbcblpk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2xeqbneos.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2iibsuqli.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2hertqzcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxcpuqfi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2pwvcelmk.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2vpqmrvcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2caamldgs.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2tjpezsqt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2higdfbif.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2uiimqmpd.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2mfhzstxr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2zuvtkdrx.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2hqynafco.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2zcfsbiht.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2ewfgijcm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2xceusnna.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2hscqrdkn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2xbfiyscd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ntljbynd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2vdackbvy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2edrmhawx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2pqptnolg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2yeioxzxl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2rdrcmscg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2pdtrlftu.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2nxlxixxc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2pvvmtkig.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qdckhywq.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2aifkzmkg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ndposiil.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zmrytquv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nemnaxdd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zoshrzym.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ltnlzqzk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pmpvmidk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mjesgqwe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2iyrwdsdf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hodrmyxs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2odqsmxyn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zgvzgsir.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2splvzsgo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bvuhbazi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kdxgkpgp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lukpcrie.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kaalhlnx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dflxugqx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2yyrweseq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fifpaszt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kqpmkcnf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2agcplmwb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2srrmetrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqiymbdk.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2nvrltosz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqgqnefh.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2muaeeoim.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rdtcovwo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2tslrxvvt.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2snlpjnuc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2laxbdjox.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ekwtbuie.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2xxqpuzsd.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2cybibexg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jhgmgsca.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2lhembgwh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ysxwfftp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zqlfpvgp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dxspecyl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xyzduygd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jtvdlndd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2zvdrlonn.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2fwmresug.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2egvsqqsb.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2baotkliz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2mvitaiei.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2caagirrw.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rvfxgeav.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pdriwefr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2msesprua.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2oopyygxt.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2plycibev.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wtuedgtt.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dmtusvkk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2qhcbpryn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tajdjyda.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xusrrtfx.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2azgmmoaz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2grufgigj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2fmrtpacs.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2dhccixrt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2xxbpensu.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2qhazahki.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2bzlmavvv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rkswvxyi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mqsmgpbo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lmgvjccs.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bfjleosw.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2grublzbp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lftnfnfk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2scnybrjx.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qbfxtpbi.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2elmlnjtu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hnfosivr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2kzkundyz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2pdtisjot.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nupfxuuo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2nqkemepp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2llxwztep.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ddkjedgq.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2dybcsglq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hyxrjvcp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2mlxihuuo.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2uzjgyijy.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zojdxuyp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ljvvykrw.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mxirxpxl.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2bmaalugc.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2pvrtcwlk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ghkmjxnq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rupxwdju.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2banidoqn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zywgchnc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2rvpbriss.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fmrhpktz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ikqsazzj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2suhhhuyc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2atvwbaxz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2donjtpoi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wfkihdrv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2abiixset.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cpimgyyk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kxdbepzo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fufvxuva.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2efdtscsn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2bpfyczej.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bhaqazym.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2gmazuwpn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2knqonehc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2rbehpagz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tlcixkom.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wrpupoul.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gmtkeoly.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2plxajnvd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2uaymrlpf.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2srdufqhi.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ukuouqfh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mcsbmzrf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wdhptozd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zldkphcy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uwfcsfny.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ubqnyevo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2wvwopxns.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gavhxnrn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2orbtklkz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2fdrjkxrw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2lzbawcju.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2vtkrpicp.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2atlxypsb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zrltbbux.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2lzzqgvuf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ohyiaife.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2wpuaikzy.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2vevrbkfz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2rcuxfoxg.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2oywmneqs.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gnurciba.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vhsnqpvx.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2uzcziqhz.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ujbfbwlq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2crsvoqaj.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2caovxgje.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zhmcefbb.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2xprfzaba.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2hgzebjkw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2miczuozj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ilzoecdy.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pjdgacqb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2tletfpdr.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eonzizbo.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2tzcojrye.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fpthmobp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2bplabeor.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2vhhktcjg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zlyibipc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zjvferjc.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mxtwvhqd.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2vtnacfxb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2dssowjgh.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2imtufoqz.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uqilxwfm.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2axkrcplh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qyvksksw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2xxuurtyy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2ihizlarn.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2pwezefvx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qgixwzwy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2owiufurc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2rohasykk.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqyfjxca.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ibjatijy.html


<!-- 参考信息 -->