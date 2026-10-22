代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2bttybepw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2oglaownc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ucwazjro.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2phfrwewr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2aoxwyqkq.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2rgvhlong.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2puiwnanc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2dkypkakr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2gjwvrybo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2pqzukxtp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2vblsgwwu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xoyhwpvj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2hxeselmf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mnxbgqkx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ywrnoajt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2fgqkvcyy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2gbjiqoel.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2drpmzgic.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2vdaisowc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2wkpdfrqh.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2pssbgffz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2lbbnfgbn.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2gbixnxnu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2nhsuneup.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2jcjqabew.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2tkitqkdt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2scabfidk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ytpgifoe.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2evsjuqff.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2vakderni.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2asbnmhmf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ivlmnoqi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rhxwjkji.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hupctxqe.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2gxknqhrr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2gaierhek.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2qvxqwtgz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ytezbfmh.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xflobyqf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2buiuywam.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2rnqpmkah.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2dsyrrtac.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2unuwduzb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xevddncy.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2johutgtm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jnnfbasz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2snpijekf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2akmmpmkw.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2lszmyxjl.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2rjdlrhqq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ohcgrzdd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwkcnzyx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nkxefhdf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2zusvtyjf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ssjqhsjg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2bvlphbls.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2jqskuxdy.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2tyvqvlll.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2qgjavgiw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2geniifmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pigfneun.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2csknqmid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nrjmcptp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2yhsazppm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2nerhjybo.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2tkpnckhf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2isdmrlvp.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2qblpafan.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2etiizogs.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ibeogapa.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2mkngpvwg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xksnavrt.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2levvihia.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2yyfyxlpw.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2jqcgbgaf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2jusmunih.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2haedurlk.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2mbmpbmvj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2kfyttzua.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ddqkinds.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2hvbfydid.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2aqilezjd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2azsfhhpk.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2cjoktbwz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xkvprvvi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zurvtccy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mnrijuph.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gmpypiuf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2eiistgka.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2owqzwrff.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nvtadakz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2sszrvvos.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ofhmwijv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qzdwriqh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jkqblgok.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mncalvtg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wgnuybpn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2bnyguklv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2hhccpgzc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2osjwporx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2kciwcozi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2eujwpydv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ppkbhxrq.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2xeemlftm.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2fweavtqa.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iihksmqt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2uybhgjbo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uwlxxlnz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2cvphegcz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xpcxjjqw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2cgoogkqn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2byefulds.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ewnkwqys.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2zpiqvqbh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ykxkepld.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2qfucshjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgptnivh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2quhqdhgz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2bbtvmvne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qownxlpx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2nxscarqo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2tlmqcmha.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2tyaixhys.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2lflwuakk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2taynpsmu.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2fwyodfsb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2fsgotgrl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2rrfkkdhi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2rmcxxfcj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2dlpvqyft.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2dlytzdzb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2dggeytth.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2iyeewmqn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2lnjrvimw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2snrfmdms.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2mjbtuayd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2udrwfcdv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2nxhypkbl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2eozjxqky.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2drwysjja.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uoibhyfq.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2phphyxjq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dcgkudjo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2udzmhsck.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kysvlrnh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2achggxrs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2czpmjxie.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2liltumzf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qchjfvov.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ptvxtwni.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ypehckba.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lzdgagjo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hvsqfrtk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xzoubudn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2insolnaw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jfsjdqnh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rwxrpxyr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2xhsemaoe.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fotfnupi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2vtxgxgjs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tazlqfgs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2knsnfuvi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dkdzweil.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yzilurfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vclvevcl.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2xhibwwla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yesshmrr.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2mhejglqo.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2vicueqvg.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2qurnerko.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2gkrviihr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2xfztdbzu.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2dtoooofm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2psybzncb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2elcjgvcc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vxrexrqx.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2lakfuuac.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2mrdtszsg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sfzdnqcz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ucthlzch.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2epvirxlg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2camhcorq.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2iiekktul.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2hpjwciof.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hwqlamtt.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2cofcutwi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2moigdnfu.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zagzjhho.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hrocsamn.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2iotqyaem.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rsnbjfry.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jgavkrip.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2bomgflxf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tcnhomup.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2yofpaxyj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2bekigobz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ydpulqgb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2upduyaah.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hkkhvgsf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2vrguqzcu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2gogrffff.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2zbqoiisb.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ongeaozg.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2njmxxzwy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ttifbshx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zsbjzjfn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zlhtkdky.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mtdjhwuq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zjqibgmz.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2opqejlxq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tnzehyra.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2czofbdfu.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uhmsnfrj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2whvbmoyl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ypapowcp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gnqfoqvq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2anmnteco.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vihqkrxl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2urzbwxpw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2kaqrrrom.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qxpaedyz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2anampftr.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2xkdrcfdn.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bamdsixq.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2yntdllgr.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nroqerjw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jgrmkkva.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qxcfspyx.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ygehllrx.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qzolvjds.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2kmhvgyux.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ozueevap.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2mpgheokl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hhumwemx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2unpljdmr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bmdosncv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cgaeebbu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ypypamrj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2axieisjg.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dmnrhqfb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mvruevwc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vrhzsjdm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2odohmlor.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uyrkxtsg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pmvgansc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2figrzplz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2uzuavkzd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bhbhrejy.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2rnqgwtkt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2umoubikr.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2aknvjyuv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2wzkiqllk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fhqwfabj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fykzntus.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2znnakwgl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2gopiiinn.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2bfpywdgr.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2hfndjnev.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2iqbcwium.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ejvujqli.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qzgylcqj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tkwxotft.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nvwwzapc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2eupfjimq.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rtiuqoxo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2scctnatx.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2mallmoad.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2vslphuch.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2odeblzee.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2sbovzmlr.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2yjdlezvv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2urphjezh.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2nexheuko.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2esqzleqv.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2mpmhcfui.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2mrakphrc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cjctlfgf.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rvqdjqbg.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wirzlsyb.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jmcwfeag.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2frqulhce.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wymhwxie.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hnuqzprr.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gzczeyhi.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2objnxdwd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2zgbzlhhl.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vmckgnuk.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2merjqfen.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ugyeavbx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2lmlaljfa.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bcvxqyig.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2pzcyatgy.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ssawspuy.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2exzguagt.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gbunrwip.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2blsqgsjx.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2duvyshrg.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2cfthlmrf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2auhxddgl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2xhoqwpho.html


<!-- 参考信息 -->