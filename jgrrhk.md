代发 wailian999

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2dmidekfw.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2xuobwbql.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2btysevww.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmfcmunf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2oycllylj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hewusynb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sjwkrarn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2dcitskgn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2fxzlhbsk.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2olighacr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ysgiooxk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2prtxuemq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2htfuamtx.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ojlmijgj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2rrbtozvo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2npdscpge.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ldfygbyh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2iysqzfxy.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2wvpaxiom.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2selzdlxp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2syursvap.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ogfnokqt.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dvgjzguf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2lqebtdyj.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hchudhji.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ddiwwiso.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2ktwdhzqm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2grkezzfu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2lcdwjxuq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nkvylsrr.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2jqohcqqi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2dbvfmcvv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2gzvpslfi.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2bgexdvee.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2bcuqgfmy.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2amrvfzto.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jxxydmor.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uldghfbc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2esgzqcdp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2clgezyiu.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2kffkvhwm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nugeyhyw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2iaclwjic.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dutsbtxd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qytldlzh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2kthblshd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2grursqwj.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2kllvcidu.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2cnacnsgc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2rzopxnni.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ojcxhwrj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ugxzvldx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qftsraeq.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2xeinzgsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eoszxrdw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2pnhrvdlj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2jtqpfwpz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xyskdqzi.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2hkyclgdl.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2kdkvgmkc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2flxowlkw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zykccjow.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2enycfvsj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qlwiluwt.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2rvglnohi.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2yipltrwy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2htjdlzju.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2bgkuwzvd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2locpvxuv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2doyokllv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2yceynfpk.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2xsqcnxkf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wgjbgbrp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mwmyrorj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2wirubgny.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2jvnqkaaa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2gtgbujzg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2amyeupbr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pywivrfn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2yuhrrccp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2zftliuxd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2qevrphwb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rwszvckn.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rbmaiwlq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2plmaishx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2eucninjv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gfdvucqu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fikyypot.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kmeohobr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2iewojciz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ydwacqtl.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rhmcrecb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2cmrjwuhc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2lscilixf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2nlkjsoqh.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hmcmpbhb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2txngpeur.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vsvukmls.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2lvtdigzx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jmxirxjq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2iqofuxpf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wnjgeigt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2awliohsq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2nfspnrut.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2lxepzlcn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ftajyctx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ttbooylj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2lzyhsltc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yyykqkdg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2rbgpjqxj.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2tcaepxvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uajyktav.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2uybcouqu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2fzpjfrnb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2wevbmkxp.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2hlncqvvr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2okckrpnu.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2igmhjzqv.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2byyvjgbp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2crqgfvcs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2wwablzkz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2llyipvqb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2efdrbqyh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2vpllrflq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2otcogxbs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2fabhgydq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ayfwhbhn.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2pjwfucsi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ebabrcuy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2cqfprnoe.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2qlgajvzx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2wxacowpo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wcspquem.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2zlqbiagd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2spprygsf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qcydwkob.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jkjkwjvx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ukrafqwi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iogznfgf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2emkkpolw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2rohkjpfh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2skljxejj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wmffjntk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yemrqmdm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pgsnzhdi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qvgfkidx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iszomscu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2spcfatfi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jzyrvkig.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2bubawhig.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jwzmkbeq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ntyagybz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uzezjutp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2qxsmiwts.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2veiccxbm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tqjeibep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2reqpvpdu.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2neejckvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnspexin.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2buhpescu.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2afuhuczz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2hiqavqvb.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xvtuidqp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2ekbkpgeu.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vyunupwa.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2pfkrkmrb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2yhlhtrmc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yotkyydl.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2kftmxqpx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2gdkklelo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2qolvcqcv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dfmhzqfk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2kbszziiv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rlerdqxz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2sdawlhtr.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2kbjitjgg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2bydcfdyi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2yzuodrph.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2thxfnjvv.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2smvyywsf.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pmynpuwo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xbybiuxx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2njyitwzp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2zchojigo.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ykwekwgs.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2agxcmuom.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2dnuvkphx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2szhunraa.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2bhfzhwcc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tkvjppib.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2adcvnplq.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2eujpithn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2lfammgvo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2xurjsuyy.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2vhoecnfb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2anrifilk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2nydkyplm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xlxoezib.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2euhxkxpd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kxsuhvmm.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ctfhzhzr.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mccqykrx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jktkkixl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2txkatrvp.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zosjhbms.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vtwhwzcg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2dqlagkoo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2cwircxbs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rhqxfygv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2mmdqgkjw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2trplloio.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2dviheejv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qgzazbfw.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hedkebal.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2rrbxhhpv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2hgthwezu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2lxwmltjf.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ccovukwm.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2fprbhcyi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qxmyhogg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2leonenjj.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yvpevcgx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2dpeurszj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mvmcxomb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmukxksf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tqmlfezw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2oamqpoqe.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xapbslqq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2llhvejnj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2pxmuiuit.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jwigpdcq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qohzqvgn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qhgbjvpo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2trkzyyet.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gvpncojy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pqpkzlqp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2czuamtub.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2eyrjbabf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2wbiwsfim.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ajtqhwrw.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2dfpldadv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2cbrwozbt.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2gyqpkknq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lcdxltqc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jvzidlfd.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2xmyfzily.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2xzorhsis.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2nwtqwylo.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2gyfjrkjf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2utlsklrt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2lahtybsw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vbivzeoo.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ogvjuroh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hsqughsf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cdoviygk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2xezgysga.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2grdxjznc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bfeiirth.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yvxogxfy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2lqzzaddw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2aneyvqbs.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2oqczkwnh.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2rpedmlxv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dlirezcc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dckwgvsb.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2vqvmrvxz.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2yapayjav.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2obfajlmd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cpqjozls.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2unpolbuk.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iaedeysn.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pdcvcxes.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ttbfmkuf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2asuruuew.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aoiobozb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gmpwoune.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2qixqsrgw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2vfzmzedk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2nkkpfmit.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2acbiqpfv.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zgaibgur.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2cohckabg.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2whygfxjk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2bgbeapsr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2efaogiyh.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fckftupr.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zyzdkcvi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ignlneqi.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2uruotrqs.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2oadtxddw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2zkhogjnm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2exuulvzt.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2vfjosmio.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bhfsufvj.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2kapuutlr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2xexwipeg.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2fqswrfgt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jmjzqxtn.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2osdrcvks.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2azfhwsos.html


<!-- 参考信息 -->