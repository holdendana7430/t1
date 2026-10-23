代发 wailian999

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fzcvongp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3emvfzbca.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3hvbziiar.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3itsidukv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3hknqhuto.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3qeauwyyw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3spiygvmt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3txaauhmt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3eiltgslp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3vuxmxwua.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qnsijshr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3alddlzzi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ubhgfksf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pdstlhct.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3stbiqapr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3jbnqkihy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xlfwscqf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yjvlofvc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3sambhphl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3tyvadbdp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3tmyebbmw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3lnmheusi.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3wovpeoat.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3dormxosf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3rgayaafp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3udnrgvcf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3deboysvy.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lqhpvxpl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3isobrjdu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pkndgvbw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3vconobhs.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3sqmzotvy.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3izlknbcm.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bxszbfgn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3nctcxzpz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jsulzwci.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kgfonmly.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3frrgqinx.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3qamtokqb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3rmbcrtjk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3bmpnbfzy.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ybmcrhlc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3bivubnuq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3pdedvzyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugcjwxcs.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3xkflnrwj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tmmxftsq.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3vugfvjkb.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3sbrsgofq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3sgaeoqmd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ieaecyts.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3cwfhzhiy.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3wjhfjswv.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3nfreisli.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3dkichafz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3uvoqxruy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3pwfdtbet.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3lohajpjg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3fjrekjbq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3wcmnwxps.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3luzlicbj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3hximmbnx.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3vynnbkmb.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rkubqknv.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hfjpknmm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hzjiegfb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3cronpyjl.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3mtixuynj.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3imkngely.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3slxaxklw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ohnlsguh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3mqvezxbe.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3zgqzdvuv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3kitlpvcy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vlpyxyfl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hwodjoru.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ndnefswr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zwpuhqdg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hunylqoh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3oczcvroc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3stfuxqbk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3gzffakfv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ogmnsqep.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ytxferlt.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ibmbtvhy.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3asijajcw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3kedoexmw.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3oxjqwhpf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3oecjonxe.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3soepvfhw.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3sgkzdnuo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nbabzzbs.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3utirqioz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hzfifkcf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3iqgfgvya.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3vqahlpqo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ffzjbzde.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3agtvrais.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3kllgavgm.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3hnacnycd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppsapkhi.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3iwltatdp.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3fflijyph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvmtdlso.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3eecqwelh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3axplhohb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3vlrzsxsa.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3axadwufk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3apwcmhni.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3joujzwif.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hvhgykon.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3mpdflzvb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3wrlyzzwg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3zkdqnmlp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3qjucbmrx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3pqqzofey.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3liywcpcv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3pjnuondo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3drvnorhd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3hazcqmes.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3sxpmafiw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3xgmodoud.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3zziddwbi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ozudeeos.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ijmssser.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3nlqidjar.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kkcfogkp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jlhaauvt.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3trvbrsnm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tpjmiqjw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mmemtjuh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3obaiexav.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3dkuwoxuk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ivvhavnh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dfmxshgs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qrkkmqzi.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3sratiebr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3eulvhmxd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yuxlhyls.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ikgwionm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xtytmoni.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ubjpckhj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jzvswkai.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nzikemad.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tkanfejs.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3bmdittio.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ihtjqlas.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tzxdtjge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzhmgpgg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3tqmcvtke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fydmmiou.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3tbdvmjnt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3oriwrhfs.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3tgbtbikb.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vxvukamv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3yidmpbrt.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3cnyrubgr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3lakxccjf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3cliolbhf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ohytqsir.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3pdokgbjw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qrzyfvkx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fpogmqvo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3knwryswi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tdcxhxyd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ibpsvfvz.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3xopixkcg.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3qdmbfotr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ajrnkgmf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3nrpqymby.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3muysjizv.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gvfubkmy.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gqvskgfh.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aybvpiyy.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xanghyfo.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ytxdorfv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vclkrajp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kysntwmz.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3eylybtal.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3mfnctmkf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xrjurmdd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3dtfzktdu.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hdwpzdwv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3hunrgsyc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3mcamxfhb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3yxmvhnsf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3svbaizsj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3aglmexgc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3oqwugutm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pitgkbpl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xjjutzjw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rwytsdxy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ekuqtbrv.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rgatlefu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yrbvntkp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hdfqfcua.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3dsppciki.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3maxartqc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ygmvnifp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3scsejchm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3vozwcelu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kpeuariu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3qaaxecwv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3hqsvfrfs.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3zxyynppi.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rxfbzgrz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3csylojfc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3zdxbzzvd.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ueyahhgx.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3owgccwzp.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3pglzvbsh.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zjuxayjx.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3nmwsxepg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3lfcfakaf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ifphultg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3akvggbim.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3umgojmnn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3byoscicd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3vfcprkqx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pqybibdy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wkyoclas.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3cnbdgrgh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kgxktzhr.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wkptjvgz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3siiitdag.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3itryqgvm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hekktrxw.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gbndqylb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yeorngmb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3vqockgbm.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3jpfsejke.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3devtclyi.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3oibfwblx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3tawzvdke.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3tepnbhgn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3sznlmcrs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3cogomrsb.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3snkuwxdb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3xgsrhifu.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3lxuvwgvk.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3dpfnvwsn.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ajglozss.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3pvefzbqx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kfjqksag.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3brechpms.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rapaztgz.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fwtxdaep.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3dhjjrded.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nbkgygyy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rhklugkp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3pwhrbazh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3vfbwraus.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3xcwyzhau.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3nqhzonqz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3arlttmyn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3adjxevaf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3whllfvib.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3gigovzqf.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ulnhxhnk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3clmzzubj.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hcqbtpqa.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3cvumhonb.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ynfzxvls.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ntgufzjr.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hspevvva.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ikpubfhc.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3plaovrmh.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gymkshkz.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3vigxxdku.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3fbwrhshx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wiyeqbzq.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3oebecmmy.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cufozpfr.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3ulwswebe.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3shkiipdl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ceynirha.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ubwplltx.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vbfooyur.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3marfxxzl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ydjsvbxl.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xgqkpfng.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nqlncivp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3jhbpcdmk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3clzckhlk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3iirovkle.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3lgcamgtf.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3muzqkcji.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3jtxuakps.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3cfxnhutj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3xrohmreg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3kkrjjtti.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3yquhfhnd.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3jcdzoabi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3unjcycxe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovpgxtke.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3lghktsns.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vzbmideh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rxncqduc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ydgdjidr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yjhfsgxh.html


<!-- 参考信息 -->