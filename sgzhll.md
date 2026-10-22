代发 wailian999

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2bnjuakbk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vpqkrzdb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2tynaioqj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dbjwbexr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2pkyznmhj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nzacpnka.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2hfmsyfmu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2dyczgyuq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2hagsteem.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2jfpygjzr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ugwmevnf.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2dguddcur.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2nalkpaxa.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2unnpuewe.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2zgrttwll.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2mlyitbqo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2phzwcaxf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ptvefslj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ywnefhuz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2uyhrxnik.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2bvlrhooh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2pqneqsjp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nbvjiwiw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2oruiedbr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2titdqyhz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2lymwodpe.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2lftxnzkm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rrdlahnk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2jtgtshlr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2jlyzrwbq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2olhymaaw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zejaiaew.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2iwknkquk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2imqtmela.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2mspxtasi.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2omsmeaef.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2iqipzqpu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lgaxveop.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jyduizzd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xhzidplq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2mifdtrde.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mowtyokr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2jtmubjjh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2cunaxrcu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vdorbjmi.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2vavhedyh.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2dnbrqkom.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ltcgloln.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2gipeeobe.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2kmlwwwmp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2offpfsrz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ixacezpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khnevmtw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ikcljmch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rgneujch.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lxmheygk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2xyhodqez.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2bimsmriq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2oivugtmy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2afgdzfes.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2yamcnecu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ktefqcxk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rbipuquv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2otfiefle.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2dqbmoxly.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2pwjkkitv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ozmrusmo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mqhtixcn.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2yjxcupjx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2rjzaaetj.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2jyqxefkl.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2boxfylhs.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2viutsvif.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dpcyhohk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2efpbtnxg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2grqupivq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2hwpdfvfs.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2uxmxtuwp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2shbhpzby.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2dukwociq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2glmkhssv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2rlzanbdr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2judfkjei.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2lifhqlww.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ggsgcfvn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2amyvkahe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2bbhkciww.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2owqxnuhv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zirxhnpf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2cxzvafgy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2tuvnfhgd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2luiwasuu.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2yofrtuml.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2fxowvkih.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2cnrpzkrg.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2fhhpxpob.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2xnmtxqnb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jjxuhxpk.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2jffajbbq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2arfyaocd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2wkkslkcw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gxotureo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2mciktmal.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2bucjkops.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ogojaqwu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2mwehafvk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2daqvyyrk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2vfvjfekb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgtgtqfq.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2nztrqned.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2mfhrhjdf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ogqtzrkj.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2kvzrnxho.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2vckkfuvu.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2lfxdahvx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ziotejev.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2vezzfomb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2jxzmowyo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2oaxqngrw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2uocjnnzh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2uktdbtgg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2vdppgubj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2heceakvy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2mhqwjabk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2bqqrutjc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2efjzjkka.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2ulddmekm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2fgyqntnb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2uqdrzfxu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2qtlcpmtz.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2hquypivz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2zjdhrcef.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iycylcif.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2sdkhpiks.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mhmsnbzc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2yqbveplk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hrzbbaqu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hzozfyub.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cvnysvfm.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2scvftwiu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2fdhrfqei.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ilauwxfz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2larmhicd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jdgcypsd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xyutigtj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yoipvcvf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aofgmqnf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cvsizxri.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2eemleauz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2nenanqhy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jfvwnigf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2hdzvasun.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2axhfvnor.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2uskiiuxw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2geiqokbb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vjicfxcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsqkntov.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2ftwzunmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htzvszbj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xofiqgaj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2guhvcqdu.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2lofcqtgf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2eyqhfjxe.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ifcetyen.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2useuscbj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2lubneuav.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2bzulvkfg.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zvkpnrhq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ejhclgfp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2lyxthonf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kicmylmg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2umpkslby.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jkiqtzql.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ayoaaalx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2olqefiet.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2yhunfwqv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2iuhdntkr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2admtvpvi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2qcwchuay.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gvzzjzlg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2aeahgtoh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lwocwjgb.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jmedytrc.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2dhkiimrw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2gbdxuxsz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2aroclpzn.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2mmazpmmo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2zxtbauau.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tkpnurtv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2dlcbpdij.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2axkyksgf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2skhelvae.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ikpgwiwh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ummaxrwv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2zsaintdv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2cwcabloh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2cvtlgcmf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ygnwllrw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gttqonpt.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qhnybnuf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2abqowlhe.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2usmjqwew.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tplmthcp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ohmtedsk.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mrciiwqm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bkaijpus.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yzodokom.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2elxzsrxl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2aufnpbdr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2niqxflcv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2bzmkqvpp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2hgnllnyr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xtctqvij.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rtsoglcp.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gmtwnzyu.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2adhxdpmc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2zrbeppbe.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2sjynyomq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fbmsplgo.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cxhlysyo.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2oiijuius.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2tcwbogjx.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2buizfsdc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2uqggzkhp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2kbsbvvfv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kmuygyur.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2wwudgxkw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kiyyksuu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yiegkljs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2mffjbtew.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2poabwbpq.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rbqpawjj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2harunhpj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yavvdrae.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oduiohnm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ecwurckw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ybjwpqje.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ktteficu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ibdxlnjp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gkuqowqd.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ocjdcvbo.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2zrlvowyt.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2boyznwvr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2pyejbwkv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vjiombvr.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hwfkvhvx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2iozvdyvy.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2yahrjsaf.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2azkxcuiv.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2axwifevt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2obduarwk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2msrtdufw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ifskzbvc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2igpgxowm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2scpuuxzr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2jbthvcqr.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2twlbtquc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zjrietvz.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hngccnxr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2gqqmnlpt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2aorjgflm.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2zbjdplla.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2zwxsvhjp.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2pdjbeoyj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2dvwvbfrx.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2bvccmrbc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ftcvkjox.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2actusvxl.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kodcvfhu.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2knimltss.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kdmopjui.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qpdyfefz.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2chamctdv.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kmvegqqr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2juumodae.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hjzbdsie.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2hqligxcg.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2spoxqnmt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2mlkafabb.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2npbfnhdh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fczmqqgd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2maponyma.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2csjzaves.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2phjcjnni.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xtqmparz.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2guamnasq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2eisdpswf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yynsttjx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2rppazrih.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2osxxucpo.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2gsrzrgfn.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2grjkfxsm.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2edslukst.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ohffotgq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2kvlgckfl.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2vcfaqyky.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2gyaumzos.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2dmgdyrfi.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlgdjhct.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyayyzip.html


<!-- 参考信息 -->