代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2higakjrp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2jodfpbnt.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sfuxhndn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dgmujrqw.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ctyvcgcn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2vxzgsruz.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qbntscov.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jdpzhypf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2cnonsnoc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2nbmshoon.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2bacbzczs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvqgygfk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zhdmgigt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pnxvjhge.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zwibrdss.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ivhpxzlo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2kmoqthvu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2seztkvpy.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ilyipbxe.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2pzifmiip.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2zjtftjnz.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2pdgyolqr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2cewzokqi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2squzurtl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2xoddnpot.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2wpokaerb.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ocycjdow.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dlmfilgk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2snzapuln.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bqruimef.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qxjlnqiu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2bdraffhw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pshscwie.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jjrhdezv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2aoohacbm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2kwbupegw.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2hjxeswdo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kmhsydfu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2xxwgkncf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zqfuaobv.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2vdtzafwk.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2icehwyxy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2fgremthp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2unndghgo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2czdohgbh.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ibwtbhum.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2cukgohwg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pstvjcej.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2evzwscdd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uzepfgwy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2oinfgxvg.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2geybtgha.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2kyzaehxd.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ygnluynw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2jdmuozzc.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mvouixbd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2bdfyxwcu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2hycvmmpa.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2haodmtcq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2vfzaazmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrkbicqu.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2lfyrraex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljxmfwzi.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2kttgzhvt.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2jglzainl.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2qhjljnka.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2meoepcjw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2nmunrhje.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2hflufvsa.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fqcuxvtf.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rcxrnhsr.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dusemgpa.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2rdhglqxo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2gcmhoadm.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2lgngjpod.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mfkbinia.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2bzfstibw.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2zqxdstei.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2yefrgtcc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2cunmgene.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ajomqbue.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yzsjxthp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bwefklpp.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2rlwkaccc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qlxgdccg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jfnhvrvs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2agdbdjgz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xazlljmt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2katzsrke.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2odpkzgsp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wkijvceg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rsbainti.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2jmqyfvgd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kpunflok.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sigorbqw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fmhyalzq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kcnyztjm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wxvtsfap.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2hmsmqitb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2syaajejc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2snnmoatq.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2jmlyavem.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2btjxspbv.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2kuodllol.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2kvolvujo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2syhxfgzr.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jjcqwbms.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2loosebfd.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2cufgddqx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lpxudxts.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2yfdghbhi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2qbceydwt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2nishscak.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2rxarmtxf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2tbjqhuts.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2kryovahj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lkceewej.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2bvtgtoyf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2jfdlxgkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mkzezudz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2iojzntpi.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2qasupuuv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2xgikctoz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ggkvtdgi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2plyzqnpb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2iqpbaybu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ofjdnfej.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2qyetixlq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2vgngjnyn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2wqjekcdl.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ykmmbqzv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2ocxyeisp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ncjkmdrc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2wiratgld.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2lkoqhfuu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2vkwuxzyj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2tepofgqq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2hbjwadcn.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2xellqahj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2tpjadiax.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gogyglik.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2tccbtdkr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jbthjzlu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vcrlbubg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gbjpralz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jwsknrtu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2mjotbipr.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vxddtzks.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bdvuuhir.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lafczyff.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bbosmumt.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2krixxlur.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2upgzkgwv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tyffvzvv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2elzlvgti.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kxvzyhtl.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ckyuaadf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2maffthjn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ocnaldmd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tmwicecr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2cfqcjhzn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rzzadmyc.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dnwaktmg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2epevpwjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhkdpuhv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2qtzmwamp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drolbwgx.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2mbyjtprh.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rsuziaim.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2tqctyhtj.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2larwqulv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2errrzkku.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zqzovuzi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2emtjmbji.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2ddrbfxww.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ugmggbcf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ahldrkpn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2sqcbarpr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vofpqdtp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2acmfkgyy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uhuvqqea.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rxdgomrg.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2prwoskvv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2gmpdxoix.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nntleblm.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2txolzsxm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2nhsfafmx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fltodsor.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zfwwrbdz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ccajfqsb.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2itdoqgcg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lendbkff.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ovkguzsf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ssrember.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ivsjdcpn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2fkhlcohl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vakdewbx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2bxbwikjw.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2glhyytyk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ttgnceiw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ioavilms.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2rtipidbr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2hdheegcs.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2logsxucj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2rutzwiuz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pbkyreyz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ksatqpcq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rnxbiddk.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qrzvctod.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2evyygenk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gtihhfco.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vmwxzjqb.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hemfzbgi.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kiktepcy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2bvudirpr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2pgsiyhsw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vbsfkcud.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pymlbcvh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2iadfquku.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2fvssgqlz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ubnxbwhr.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pllbtvvg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2firmccjk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2bkxyumgx.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rffloesa.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2valvxhvc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2shfzyylc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2bmpszxsj.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ejalzrdn.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2pwhmalsd.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2kglggyld.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bqnxjlcv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2zewabtcj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2atelbtrj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2rmfwtxvz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2amubvdsu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ewbjovnx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2qhuybvpy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jjxrjuyj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2galupcjc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2haovggkx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mndtortl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jizhoxlj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jjpbkbrv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ylvlwfrd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2rplkaudb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2mhrctdgs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrdiizbd.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2molxauqa.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2wuummehk.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2myovqews.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lkzkllot.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vqsdjuds.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wapivovn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2injamoqv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2gdfjultd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2enicrule.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2uwviaquq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2guykkyow.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hiborpbf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hdwfyseb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2erywtdaj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wqytbwnl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2uqeqpfjg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2khzduzel.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2boomoqzp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tfketaot.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2wlkmzjzu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2vborhnck.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2dijkfkam.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ulnxmave.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2utwrhxmr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2jensugoy.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2bkpbvssu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2qdfhzbus.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2ytpfxogo.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2klpavbzb.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2euyfwzij.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zivhehlm.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vjkttaga.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ejuufwbh.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yciihmnb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2edvawzmc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dyseoavw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2mudrmgfh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2qztqvbkc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hvperfwz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2yyyeiima.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tnfpoffc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2fofifuon.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kcwgzujk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2earvxmqm.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2majwglhy.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hgpwphku.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2qkdfrmbv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ltcaxcqc.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2zsorczit.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nebhmwnc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2rzvwdzyt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2huyksqku.html


<!-- 参考信息 -->