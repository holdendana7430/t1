代发 wailian999

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ofhszpum.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fytgnlrr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2hdjkljry.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2dzzirmwx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ztiwbmwb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2imjyumfz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2iozsilzd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2stalrvhs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2upwrfkrg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2reiweauc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2wgvmtbzl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jfadjwla.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2tddcquhj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2phgjkhnd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2uohzdumo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xpdstpgs.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hzjsfjls.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mmfutizt.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nsgrrapf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2okejtyye.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fzyjsfva.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rzevqhes.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2stfsatoi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2etyrmcoy.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nkhhnvba.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2dgiiqesp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2kygkiueh.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zvdsqjng.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2bqhsifhm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wvlxdhus.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2rlkheris.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qjtljlzm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2fdbknhaf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uxyxesxo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2lzpybzuv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsslxelu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2vbbxulam.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2tllvaqdz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2vfrnjbus.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2tshhhrjc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hiopyssd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2brofrydw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2vqojrmnt.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2hivkhdml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyefjdhi.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2vwcotzpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqgfzzhp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2jwkvohsq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2dbvvaaod.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2xrivwenn.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2vcjrgpfj.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qdjjvsuz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ikprecst.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zfxswife.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xxqvrtyr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2nnowftpj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2nzzckcit.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2alxjsezf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ppflegiz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2gsnpdjng.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ezwkykxg.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2yuomhpzn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2mdmplopg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2mkzagtsg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2arugavlp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qimfiufh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xgjxgpji.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2soxmiruh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wbuxeihs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jguklrxc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dsydelwx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vddygxwc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2efrawdfc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2msfnxsks.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zhkfqtql.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2krltrnhd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lngkarry.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2knhfgvso.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hiuanssz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kwxqmlse.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ghewcnyc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2guxloztw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2egkeidph.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wbgbyhpj.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2vetssjff.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2jidesfrw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2nfrleiev.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ordgypup.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2hnhpokzy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vmiasslo.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2kxwvbylk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lpwhsaej.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2zmidyazr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tbdijoel.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2aeccnzrg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2lmmrjwyd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2snzdobzq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2urtxndqk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2vxvnjwqo.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2rlvwyyay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sevizjkp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2oborfdad.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2zbleuiiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkzghxwc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2dxjrgcjm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2lleugqkr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2nzewdlmt.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2sjoempif.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2enbjmkbu.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2lnxwgglk.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2kcxrydus.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2oxiynanp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2pypptmpj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ixxdntai.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2xomiequk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2xtoumbsh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2duvrlzdx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2jnrieaub.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2bjcvyeyh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2zlebffgw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2zwvgwtba.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2kguqwowf.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2atovwbct.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2lchovrzz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2daihwpyt.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ojrgpeww.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2alzprjeo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pzegkttm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lxtxlquw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lqsdfuwn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vbtucaxs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cjnpddoi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2evytvaeh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yaogoakp.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2inzmarlu.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2edlatqgw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yzwjsmnu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vnfnmgkr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zmvtfspb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wznvckrf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2uekxbqsr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2agfpyffm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tvwxugct.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nnkwdsar.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2rscynjxz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2isniqvdm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2uexdmzne.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tcuuzopb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oaoxrkag.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2qlunnpfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eirzbbfh.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2pkjzbmcv.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ifpoqojj.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2tsywfxap.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ylsiauuy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2xmuweisd.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lpiocdeo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2thycdnks.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2kzeugnxi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2zoespxzp.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ivifgyfn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2gvuvkflg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uvwmvyrw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sbxxgpxn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2nsiognqs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vlxbvjqs.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2zhjjwrjo.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2dwccfjqi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jlegclvv.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2wakninja.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2lhoivyqw.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mpenpkvy.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zqovgcqd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fyjiflok.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xqtsgops.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2uwelizbf.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2cwoljiqa.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gaajqkrl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2fwzhojzt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2vmwxdrsm.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjecytfh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2qtlqylkl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2dyanapur.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2cpokmrqq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2knxzujho.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2fmroauru.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2igozoibr.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2wxdvdebl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2dnlzsulm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hzrbydff.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xogihgjg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2quwfjqdv.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2usozidnh.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2afqeapsv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wvomtmbm.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xihyvcsp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2whkapurk.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2duyiztyf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2jvpisptw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wxqmakbs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2iomwvjlv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2gxzomqmo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ftoafsej.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2jviutlkk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ifwtxmrz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2slvwbisg.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2kdnuoddz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fdovseol.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2nssnbolh.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tmlyrpkz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2pnagtkax.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yhaojjum.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2eizgnoxz.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mubbcrcm.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2mkmxpvpn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xdlmuwpx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2zyvotkii.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uwdltlyt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2xzkeqilr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lmkguzrw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gdkvclbu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2jowijmaj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jyuyxobi.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jemyiqgr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qdkqvofj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bpfzuyvf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fuyfmclq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bspdavza.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvurgvca.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ysekosyk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2wbijiqkw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gqnwswvs.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2xdqfbdxg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2yxunuadv.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2rikjzbdr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kygipixu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wnvkyqww.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kdtcvnng.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2wqqestfb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2smsgzaaz.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2xdddagaw.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2bbkhqmzd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qgqecbhj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ycspugyx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kfasmceb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2buuubyxb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ahnhkzbn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2rbrlyfoc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ntvshxpd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2twqvrhbs.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yfsptqra.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2yxwjbzkr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2mjgikyks.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ntzmvaqj.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lclzkcmp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2vwgyxqix.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hcgpzbdb.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2oyervkmx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2qqbnrtuu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2rupmfvet.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bujyheub.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hznilpuj.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vvvhygaz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ixgccgor.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xcghcgvc.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2myjumuhc.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2audsyisj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kzmtuenp.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2jqtugztx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2mqpzthog.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2utbcrngz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2npmspurg.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lzekwyib.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2gtjfzqij.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dzfgxbdm.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2zqkgcdcd.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vwrkehjp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2bnrlgyip.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ubddldum.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2syipreso.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gklomgli.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wbafrbpa.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2nzqtlazl.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2gofqehui.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2hybzzsya.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mrgaiijb.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2poxdeytv.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xxqhxlay.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2iiuordnl.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2msfjzyui.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2lbwsxdza.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2tbhznzob.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ukxvfpmd.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2vhgchtxa.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqeqkqdt.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2ddtnruue.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gtadcjys.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fsotfhoe.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cczjzdat.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bjwisbph.html


<!-- 参考信息 -->