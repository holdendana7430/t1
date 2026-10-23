代发 wailian999

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3fsqdxspp.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rpusftve.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3kbrncvyn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fzkjlbds.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3uiodbsax.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tzjdaqdj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vvvtrfww.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ukaiwovw.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3yelnokgb.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3xtxefwdb.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ildmvofp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3wsbfaeht.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3yeyfbxqq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3lwlkizew.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3bdwtqttu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3qomqdcco.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3lauhzlou.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3sjxtzape.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3sbrtigfl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hrntftyn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3kxmblloj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lshlqazy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zycaxkug.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3fmtubjhz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gfeuwayl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yhadmsqg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3qylhfxgl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3idgqfjgu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3faecvnxd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3bpcimejf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3dkdmspxp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lcolgtma.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3iqmwxzdt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3dtyblbzl.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3gserdred.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wezzmgas.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3nxomntas.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3przmpohg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3rxbvcxxw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vckotecu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wmyrmawg.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3adzkcpsn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3wgpehogp.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzwwjlcn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3lxznhkqf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3jkgincdd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3nvhbjmfu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3nalsogyj.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ypendmwx.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3gskayxbe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3naluwhno.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3diucdmcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxnescis.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3wgriwgum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfuwqofz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3wpritpwi.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3mcbxpkuf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3lqxpgnhz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3hrppjvvw.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jxgukvzd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3gjgcanuo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3adijdshs.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qzbfsbte.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3smnlrbdo.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3zfkmhoco.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ctjztjgs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3zkhnxysg.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3rgxwoxdd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jfuaugvj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3rhmklzsm.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jslpxtpb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ogvqadot.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gbqvfbmc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zvsnbplo.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3fhpyhdgw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3tgmxqbzu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lyxblkdb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vlxsuujp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kzxwymzr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3uqmukpvg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3lnhisfhn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bjdzschq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ueqiqzfb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fcflozap.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kigiixcv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3agzaaajl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jwhglmlr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ocrdpqvr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ccygfvut.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3giharlmk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3bqtvxrwx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yumjvdkc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3efszcaas.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ubucjrzv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ituheoqn.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3oelnmvze.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3kpukmffs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ucsxjajx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3mpblaqjk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rjqrlwbi.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3renammsl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3topvcsfl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3cryyvljw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3tjqsmjfe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ikepcgbx.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3gmhqglgw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3vkfbjypm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3qdjwknps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwqtusum.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3xlxthtok.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3hdxdzalb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlllramo.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3akarrcyg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3shlxqjie.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3dqdgrtuk.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3svciklet.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3sgictdsg.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3odtkkscw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3sozflgjr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3pncqyykt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3aterqtcl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3wfdtpcqy.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3cdjcqvsd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3jbtfvzjp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3gxjvrxvx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3kzcowvzg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3dtqexpaw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3wxcgosyn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3yzqdaohh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3prhrgohr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3exceapwn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3giptsnck.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cywwlctf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3qjrajcef.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qmsgaovt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lnplwlnf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dkakvlgh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qwwqqnqf.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cgqimtzb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dvgrogzd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aqcmezuy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3duumivru.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hfzaupgj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fjifprln.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qelqqdqg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3efsmimij.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gsxerugt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bkuotoyw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3sltuwawz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kcrcituw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kixkmdum.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ooljjars.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3iowdkxvw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oqauqjpm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pndotdgi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mcoxvgby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgzetnof.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3uizmcnpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxddgvtc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ecerrzxd.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3jqjqukqf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3gucnxfyo.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zljdpjmg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ltgdmqhq.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3maplesrx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3opzmhktl.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3vgtqqftq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3lgdtkqhb.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3fmcsumch.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3vsbkeufp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wjdyctds.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kfbtcvzz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qelrsfew.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3unulslyz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ryfvssav.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3serbkbik.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ogshgvxg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3ktacrmic.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3qzbxqiov.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zxmpkqiq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vxlribos.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mxzmmgeo.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zmhrqlzb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ptpdacus.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zillrvnv.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pzfjzufe.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ngexarbx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3enpgbmpn.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3lomokodl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3yoczfszc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3magmaknj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3lkgleams.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3xssrlcqk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3zroslcuw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3zbnhkxwn.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3hzqnvmmv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3dlbaayxy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mvymdizp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wfqapvnv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uchnfnka.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vbbyandi.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kflnisnz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fyjolhvu.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vjtxgoqq.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wxqrtcnd.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kftoyzaj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vquvjwtm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rvokhrki.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3eweyamfk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3erxibkwq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3xtejzbsb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ulzyvara.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3zqlriwlb.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3senuxcep.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mvuwknlc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jrawizdh.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zdiauucy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3fbsjqdps.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bmmyqyda.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3mjdugjij.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ymebsbsx.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3woxricwx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3fydmxnab.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hwsuxezz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3digbfukr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vkapxigb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ztejjjoy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hmmitzoz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3arruxxtm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3kteamxjl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gxnoahay.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3cbhoupoo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iohonabi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bkszkibd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eaixpsbl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3spxawemh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mvmccabw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3txxrmskl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3monpfghd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ryuyexnu.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fcwlipat.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3frsnepon.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3aidyqbnz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lkkedqji.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3nonjuepp.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3gvskqrej.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3vexehwaj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3satgxpra.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3mrvblvpj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3rtaqxkui.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qjvfgmjt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ytxwkhec.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3paiwcapr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xufjlasi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tnwisbwq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3qkiuudju.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qdsqvgrz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gdpjmzuz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3sfjqmlap.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3dwsxpkys.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3jdltulzy.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3epimojhj.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3djyqiovv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3azmjkkcr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zlloktqk.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3grjpdmlg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3yqmztoak.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3arnafnku.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3cwvmlrnd.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ozwixetj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ndxbjjei.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wftcylcx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oncjzixi.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qmwqlwyc.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bclwrbmr.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ouucdrlw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ycwbnlre.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3pvwnlqob.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fpufxnhy.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gfnomtyp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tcuwsjpc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3exyerofy.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3iwkaznca.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3bnvjofqo.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ffenvycr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dgzescam.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ledumxnx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3lknbfqud.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rmvxysmi.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gbpcvgno.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3ysbjdgdd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ilucyhir.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3hclyzuuo.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3leqyghlv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3pkqqlnaw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hwtpgquk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3lfnzqyig.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3puzfimod.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bsfxgdkz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3eqdnbiqi.html


<!-- 参考信息 -->