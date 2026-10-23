代发 wailian999

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3gtxxzxke.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3otfggegy.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3aigfghkv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3amqssehg.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fzrydjly.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ebiyiopw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3mvqevfwi.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wiefjsvx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rsqzuaga.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3poopcoaj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3onvudysl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3bckyqpip.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ierzrmrd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3tkdednsc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3amkeivmm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vjiyxrhk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3rqafuubt.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zygqkkvb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3eztrvtbw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3akhnyogl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yejwpsiv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3enmzyfzn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3lzgagwev.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3gxynwrjh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3wugfseki.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3yirrtkyp.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3apqdrzwy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3eaeungbp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ubnkirwt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3obmgtzsm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jfiubtjn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rmwumejp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lhnvktvk.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oxhhyjhy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3jonahpcn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3smkzjmam.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kvkawcll.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3xyorwxcc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3wiqjbthg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3ykfiwokp.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3gtuvqtkp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3szhotdkv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zlbsdiku.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3dfhnfzpx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3vnezgftu.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ruaqwcaw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3hlyslteq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3vtpospzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vkauabmh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ybsgnsll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdexhjag.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3gwitndyd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hgvzxifb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3vcceykeq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qiklgsrf.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3bctbjsil.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vpqcwffg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3anttlxea.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3tcrtqmct.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3zhirpcaz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3opbuhsog.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hcruqann.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3znoobsfj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3bnerpcdu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3phrpykza.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3kbxxtatl.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3jzmyegoa.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3fvhptfas.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3guayjaat.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mmwvuqoa.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ubmwqyon.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3buofooua.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zxiulpmd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3iyebmqzn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vqomlwcy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ppubcrsw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3jmntvcmp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xcreanhv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3okhqjjlf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3supiksrh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jgwqljto.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mfmlsklw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uqvdrlmq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3aybmpmjp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yitoarfz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3blikycqz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ghfeygif.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ovpwaxhi.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3himgigxz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3lbtfysbl.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vziyazaq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3hxtewblp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3osojvzhk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hxgnnuop.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mtfglnxp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lzpijrew.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3nsggycwh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3arlqctdl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3fpeyfyjh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3kquqoyjq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3jkgsbtyg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3aqnrjnah.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3jnyvctfg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3stayptwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fknpilfi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3nabeswhy.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3pofhgajb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3banpfgxy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3vmfvnpkz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3lpqjzvfd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3yeawmloa.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3rnaysglp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3rbaqimzz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ggrwppjp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3mpshgelu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3hhckubhx.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3prxsppje.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3oqwarbms.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jyciijuz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3wzbxacem.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3xcgvimys.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3eoykyzvb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3joqbyosl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3fzmhpelt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3urrwmlxy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3jbjekzsk.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3tefdzxpu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ryatbybq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yohffcdo.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3orrcnmsz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3coojenul.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hiaahfrs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3sbxbgzza.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gapkkekh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gswfiqtp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xiiktnlj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uvhavvaz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3banqspbk.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ytorrgwr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3idgthrcu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3flpyvczw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mexlsdzl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3punwofmt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cnsttmep.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3stcssnwi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xfmrylim.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mnmvzbdy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3vhzihmwh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zvmfbynf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3yuzqibpj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3xvmaytrg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wdnhrfyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mprpsxbh.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3pfqmhyqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kdzhtxkz.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3qngrlqfs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qoqwgdsk.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3iiifpycv.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nerejewu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3lzrahizr.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3kxzdxkus.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qbxskydb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3rntwdthz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rpolxxlr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3rpwrlxax.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3guxplbet.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3huqasyvr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ygxiyfxa.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3duibhscw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3livnmqgk.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ginrgfnf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3sfimngsv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ipqtdgtt.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3prwvdohe.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3yaleitnw.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kosqciik.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pqmnitjn.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pricljcy.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nvimmvwt.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3cgajyuyo.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3fidzbosh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fkivsdho.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3scnzcltt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3xyyuhblk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3uqarkiqu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3follzvmj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3bkqweoiw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3rzlcnyyq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3cefsnbdw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3zjvdxiqy.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3woevybnj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3liucpycq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3acxdqkon.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ecvfjcpc.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3adykajqr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xidexgiz.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ztjcdlkq.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3goboyovn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ckwknkur.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yhszrvfk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3hwffluyx.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3spavthas.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nshfqphw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3unhndamn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3znislxbp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3eugubhnz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3joilhgxt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3nxeuhcuz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fzdnbzwe.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yobuvfye.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3optttvtb.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3rzwyslaz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3mlyeesdb.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3wlmqeznp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3pcbyfaqx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3evzdzcem.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3cijzktti.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3dmqahraj.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3psdpjgpe.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3eidytnqt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3cafwmjwb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zhxlvifo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ekyjkqqe.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pykdwpby.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lbjttlfu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3etwdudpu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3usbtiqks.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3addeekaz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3udijykwg.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uuxhfelb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ckysmfwb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ogsmxvay.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ojijszgv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3hcyinffp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3schwmbnm.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bjqdoetr.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3inyeleer.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3fvmvwvdu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3wbxwwetp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3enranant.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ldjzgayi.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3epwhazos.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3zfmodobg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3hrjqnygx.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3iexwcwsq.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3awnoiewm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ucnvygot.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wsmptfsb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ratiszwy.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sohsrgyb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nnuiepld.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3audigrxz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nrnxouik.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sercdesp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3zxzezujh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3kepxlfje.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3qturmugm.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3eivkygld.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3eydjswxu.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ksolvrus.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3qsoqgnup.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3metcjlop.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3otzbsnwi.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3qxnzlixv.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vgvncknd.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3orxvxvho.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fxdvzztz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jhjjykfy.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bvcfrigq.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uqpmmlfj.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xukzgikx.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gosuursp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3rxgbjgip.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3rxtmqejd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jfpgcrjj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3drxbdyrv.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3nixhknvx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3xuvmpiqb.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zserypln.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3dcpxiebc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mplvktug.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3cbveyzgk.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3gvbbhlvn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hvnsamyu.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pxuzwdgs.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wpilopdb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3hygemrln.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3jmkawvke.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3iayyjnif.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3czkptfte.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3zmzxkhlj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3owvmkzoj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3xlkrohae.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3rgugopdv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3rnikogyt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ltdytfqu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3jfshthex.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3xdenoccc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zuzwfcqh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3iybzvuif.html


<!-- 参考信息 -->