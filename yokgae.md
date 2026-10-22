代发 wailian999

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2jxkpflhg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2bnvsnvon.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2usnpnshv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdlocejh.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2vgxywfbf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fweniedw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fidnuuxb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2pdnurmgo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2rupjsiwy.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ncoupfwn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2tnbqbsqt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2eswoeycw.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2aeifeubx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ibnxwdjy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ouecqqys.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2evjiwhsb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ozlkwawc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2czwtfhdn.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2aumdfpck.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jollrvrp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2gderyzmk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zuscrnzn.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wdyxehpd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ecouozwj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cebmcahy.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ovbweewo.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2djtwmovq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2oszcterz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2tsnbnabg.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xbaymvwr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2kdwliwsd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2kynggzdi.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2sksqgzce.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2wyqwkypc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2eedugamv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vjaboszp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2nizmymky.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lolnnzrg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2dvxhsnem.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zqhhiaev.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2voifpkck.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mojqssma.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2xywuqiau.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tatiikxi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zkfgmhso.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wroubxti.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2oxynlthn.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2gscgvofb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2gjpyexau.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2kbpgnzup.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2kkmjuuse.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wtuuftix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jvrrbnmk.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2vbwcgzgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhlocrjy.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2qixyoolv.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xetrdsuw.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ldowlqri.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2clpkpywq.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2dgelqvaw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2yxjfzhwa.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2tatrvrsi.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2uobuglak.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ddxycapp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2iudtbcgw.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2inmxrpmq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2rdvegwpv.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2kfdudtee.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2vwjskhwh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2csulzasr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2feplhcyo.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2zzhgkzcy.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wrioyqpj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cmtbxtlc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2skngvmvj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2zkrcqjyn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2rjjchhdo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gghmwtns.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2undpvzwt.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2kufjsiuf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2oxzrfmfv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2urpvpsmt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jeyxstmg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2legomrbl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2quudwwag.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2eiepftnb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wdsyqwfo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ptbzqwxx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jpebxmjf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ynccwhbu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2msghqqhf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ufgobcap.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2poxuddfu.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2xjtvztic.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2snsgsfpr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2sfrkpdid.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2utexqgqe.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uiwdkfph.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2uwcwgdgf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fdonrxpi.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2eaicxfid.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mxkeyjhj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2pxejiwir.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2vjrkflrg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2rdrrickp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2awypsgcb.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2cxdofgog.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2caaioput.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvfvcuue.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2uyerwrdi.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2fpdwckif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmlwbuqk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2cmxlpwxm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2vnfaandh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2dbcsyoza.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2kqxnxujx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2azccgurv.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2jwnwigia.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2jupjddzl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2nsfhfhaf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2tydsgruf.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2kbkcxrje.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2kkptwtxy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2gfabgfat.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2biuhscai.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2xmpgulqj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2vanhqmsr.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2summxivs.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2wqkuhsux.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2xhxazqwl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2lvdssrjv.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2rvqfrkci.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nhxnxxkw.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2nwcfrvtm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rgppawjo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vleeaheg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mjoaekdj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nibtvmpt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pgfcvpwb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2nlhpdbil.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2nvlhvjqj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2otmkahyn.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lppbjavm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ofauqdvj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pjbufkfi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2abffkknh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vdctwzzt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ceenxbiw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2dwsbbrip.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2glbdydsf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hwmmbejk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jjffyvzg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2dmkxljjj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2fyvklyyr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2vetvvwhy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2axmzxpgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uhoeokxb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2xjfgydrk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzqwnier.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wdmtbnxe.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2qokkxcrx.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2rstmghvj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qfyyxrdx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2wtptyfkp.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hafgzszb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2yjlpowon.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2wwqwcwst.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2fjeqehup.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2lrsxpjpt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2oxtbvbqi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dmqolzlf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rlkuyycf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hsqxelyl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fymogurx.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2vlkwinsf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2vjydssfg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vvwsfaua.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2cgcokciw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2vjrdmkwt.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rhvbcjzu.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gclninox.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ufwquxnw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aiewwltb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2tnwzjyvx.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2coezrewk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hisiviys.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2khxedrwc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2sbeolopd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2zykjwryy.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2rbgchhby.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xjmyeurp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2anscewle.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2pbwlvfmq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2tkoypzgw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2sdnbijcy.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2pnjnykgk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2fvuwehli.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vceljkwn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ximrivuc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xabfkdeq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gqtwxbkn.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wkaxzxjz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tbevjmvs.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2awzbmvny.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2vgywkiyc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2tngakhkg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gqlazynk.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2osgnhgri.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fxynfmom.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gljcdnlc.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ccxzbvca.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2gwufnboo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yopufoyg.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mgfnqerq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2dpzkqjjl.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2egdlwiyt.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fijucklq.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2jyfyivbg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2hsaqzqdf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gmtynffd.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2lpavnoqv.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2qvwxdqwi.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2varcxkae.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vycgxxca.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2njizsmld.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kkidszsf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2pjsfnqoo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2clpmohkr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2whufwdlz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ywwapips.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vddoltas.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hnlgnstg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2efptxmry.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvyuacwo.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2suulwdfe.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2twumsymp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ffrybnbs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2lnvwdcoa.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2jyhrnidt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2klbsnrlj.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qabpafeh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2pscbvohw.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2tzgpeyka.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rludomov.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hmqceliv.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2efnclctb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2dshkbpgd.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2dhtdvapk.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2cxokhezm.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2etfvzheh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2llslwvmy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fcvfsbku.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sbocumdd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fdykupld.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2daaykycu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2pqgfrqqu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ifvemkln.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2djqwtsvd.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2dgzbokzu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2owstnttq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ofwmtbnu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2yhnqipks.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bymqxxaf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vjstillo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2ukynqpym.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2hgnetple.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2vyvekaip.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2jeggywvo.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jhuwjdqv.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cnxlbonb.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dcbznyea.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fmnwkgwn.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fcbsnxcu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ymtyifni.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lbyfkirk.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tvwwwfej.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2sdbzgswm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2tqzrflmu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cqnonpef.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xregypsm.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wfjogdfm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2lxbocvku.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jxbtdsvj.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2cwjkzhdc.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hfnjelmn.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2voxyhaco.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2mezxpysa.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oeiltdvo.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bydfrzax.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yyhggvmb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2iknbduwe.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2cizpqtwy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zlxypfjv.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2gngpsmcb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2carexzgh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2ymklnrah.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2ihzjjprk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2taahhnri.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2bopnxcgz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxqsizbb.html


<!-- 参考信息 -->