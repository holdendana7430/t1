代发 wailian999

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ksszxnwk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zyyiwztp.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rwdwjhyr.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3rtagurlm.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wefwsrjk.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3lbuxmjpa.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3spmnnirb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3tdzsbcov.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3fixjdisz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3odkexgyt.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3tqunejvc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3slxbaujw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3bvipuqrt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3kjzpyduh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3jzyalrcf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xvkxbccs.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3sqcvettq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3boibmrir.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lwdsfauy.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3xljrdznu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gthdsptq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bzpxurdx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3anprlfgh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3rsdmxtgk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3lozomsvj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3yotfamxj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3jyltlzqc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3kuznshed.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3tjdvafcq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3qdlozdxa.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3zbflkvzg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fpmbqkft.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3msusbkec.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gaxqgblb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3nbnetxxd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ixduxwim.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3zpqdfzud.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3nvpponuz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3enwvwiae.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3dqqnwglj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rzyfnkqq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3pefpblqr.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3dtoiklff.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3blbtgrvn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3tuzwkphn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3sefiwqhc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3gnisoihw.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3fcywhdqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atopvuav.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3qtqxugos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wctuzqww.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ebhdipvk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3deahfewh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3hmtzmvtn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3suunhjoz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3meomgirl.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3eqcbvhhk.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ybfxzyrb.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nfbknpir.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kqywatww.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3myjnmotj.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3rwhyfwoz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3klvhyzjz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3wlqxdhax.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qbtqucvy.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3goqvqetl.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3gejsiqoh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3botyxxvk.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3wdkqkgrp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xovsptdx.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3caeiqdit.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ygwqvznc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rfmvzkjf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3byphfnru.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jrejziif.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wtfamodo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3iguomxal.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3khjjiwhl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ayzfpgwb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3yopjdcgu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3smvkajdn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3osbacwmw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rzrrnhoh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rrdbfqeh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rrhmjumb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3qngmyayb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3yvyqlsue.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3omvkqmgf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3jepsbtjb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3juhnefgu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ceepefqu.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3inongjqr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3tcdhcgar.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gljjuaqy.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hdpyfvec.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zoxjjbyd.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3kaveezsb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tinifcvx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ithmswuf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3uhzrerpd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3eypdxgci.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3cgudgkwv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3xcsbxjkg.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3isxwshvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekdigiyb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3hcqrkpjz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ypuqqfgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcxpsgcq.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3rguaohkn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3qqxxhnqb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3jctgvnvd.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3udtvicol.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3rebpowdg.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3spuwefht.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3capsrzup.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3qdrebbkp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3rtguqnvs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3xjiuwssf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3hvlastcp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3zhvrepgj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3jmpbfnst.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3wgcqcepu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3xvuhoqau.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ojwdpllh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3wwkmjusz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3kcrgtaod.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3fidknris.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3xqzjtuxe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xomgdoua.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3pgqgnfuq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ghryklmu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3setfqxkn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3urblceqv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3asirxbmn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oyovmnkq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mnvpzyir.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ufjvouch.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qxkpvzpp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3omskdoqe.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zqewgaub.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fsnvsctz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3apmursqg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jhbahusg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lqhoiybn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3nikydfui.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3auuuhooq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dogswkrq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3gpqtvmic.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jmgdsywg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sgimziex.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ivxrotgr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3aazsqkoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwaryrul.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3izftnfvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nghhjcby.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zkjsxzwu.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3taaetdfr.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3nnuaxazb.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wrhnlhjp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3iiqgqqno.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3alvuhfgw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3btoghxqx.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3kvlcoujr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gnayxqxf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3yynzcbiz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3dfcdsuen.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hxamfbhs.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fnlpoohy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tirmvuns.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3aznppbnk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qjrxfntd.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3epmqythl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qipzbots.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ksfjbxwa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3edhvoizx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3crkyijzy.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tljmrkyj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3moypzgyq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zgmgmvrh.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tqcindhu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3yhgqmhcd.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ztfxvdwu.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3aiyhtnnp.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3vabcyjqz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3dziaqrqi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3tucnwtcr.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3btjozjeo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3gnhrpcod.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3pgllipbn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3jbyyiono.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3lyeoszua.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3puhnmtss.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3olahvhsm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qudljctt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3chkhagru.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3adamxezo.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ywoijght.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nyvbdnho.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wfaiizmd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hldlwdbg.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lsoxjfui.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wtksfkcu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ponyyxku.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kypvgsmg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qjvquxcf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lpfdkkml.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3efjakesr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3gmqfbzkp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3aueghlsh.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3kjrapwuq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cukrsagk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3lmptzwqa.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3moqdaxfm.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3gzpxeqmq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3aroqowny.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uplllpvh.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ebklujay.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3fhqbvqxx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3yngyugin.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lcvlonxv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3udkqlfsu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yvpojiip.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3cpimuctd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kpxlpnvx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ufnmualg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3esslkgiv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3thcehjcb.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3eihgwrtp.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3thnrbzqs.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ihxvdmzq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3labwkpxx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vblawaci.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wxzrucct.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3frmdezly.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3pwobuhgz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uimuvwcq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qvbpqtib.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3splyhmpb.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3aljouuij.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gjvyzolt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ciskktep.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3crchstqx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3bdhmdnge.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3serawwvg.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3azwkodis.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3kiggzcjw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3irdcziif.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qxytoqgi.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pjdywqja.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rrqdizyx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wjimjkeg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3bndqknnz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zwbgltnc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qkaohrat.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dhspjhro.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3fsgeloua.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3rtknhaem.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3udwwdxuc.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3vafovnro.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yxnctqch.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3kxdlcqky.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jpbqryxw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3tbobvdai.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ssohzzgr.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dmcdwjbk.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3umtsinam.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xoylgfrf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fhplenwn.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3caxivwxf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ajcfpxxu.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3osnoowqs.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yzaycold.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3jkpvvfjj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3atkdsmgt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dznxgwne.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uwuvqhcd.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uqxkdqgw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3nilijcdq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yhitykol.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3yomembbz.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mfexifbl.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3yqbljgad.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3vzgugiab.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zukhyazc.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xojsjhch.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zylnrrhs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3fqcgilqh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3miqpknlv.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3jqzxafml.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3gizaiiit.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3regdgrjw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3iqbhyyiz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3zbbyzojv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3oesnysop.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvihflli.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3axcgqztm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3movabrgj.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3vglspivn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3tfkdivdx.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3ccmabmiu.html


<!-- 参考信息 -->