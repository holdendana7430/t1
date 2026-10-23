代发 wailian999

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3poxzmheh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tebtmqyr.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3gvpvyjie.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3wwtleqqy.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3fsuknhoe.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kihmpsjv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3xfyruygq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3zqtlgdhj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3gwbqexyq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3iqoxvqbd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3cmsucvvw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3gwgjgxmb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3urcpprjo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3hduqsrco.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3hircbxxt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3dlkepiew.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3rhwtsntf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ymezgtnd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gxnfhmmb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3apjkmtxr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3aazvsfxt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tcmowndh.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3dgbrkvls.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3ouofsyvz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3tnneegar.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wmpvxytb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3xpujgctu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3zkqrwpbe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jogaijcd.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cnajoqem.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3cwhprywn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vrotxibe.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3gjdijpnt.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eyymdjvd.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3zouhooiv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3cpvnhjtg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3iaxrnbmw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gijpylue.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3buihwnhk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hihsfule.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ziwwious.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3lrqkddps.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3mejnlszw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3upmsvpht.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3dyqfcwxy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3zxmfyhif.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3avzdhjas.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3mwlwtald.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqmhuuyl.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3cyzyaxip.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuojuhqe.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ccjkriit.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mdzshvie.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3qcvcwapx.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3sutvzxac.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3byxllemf.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3oqbxfygg.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ynthaqow.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3udezigft.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3xpgypmtj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3scwikqpb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3jalnukqg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3fwsoanoj.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3zddzaqcl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3szqrnznc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ammqcwgo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3javwbahl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3medfrksg.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3hfhuisvi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rjtnftjq.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vfkbovnm.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3jijcvnoi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3fpsfhfbx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lqgypcwi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ejjenesb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3vtzdbhnx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ynjeolqg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bjngthre.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3phkmexoi.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3avilmckr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ofpbvtze.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3rcmqxook.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zpgajtud.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lemxshqb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nbkhmhwx.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3vgdufxqm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3fdnobxca.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mppdfwik.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ofblhqrj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ufjkcebe.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3dsywzfly.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3brkfbgmd.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3hxljbpkz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hlsclnyq.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cwndjbpr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dsvhxkbf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3zmbngfrg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xiktfxtz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3xphqyvws.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3okljhisr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3pytaelwi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3mrmcjsiq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3vsrmltrv.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3xgtmsqvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mwiuwmis.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3wjiiuiiz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ocziivus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npwucyck.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3ywmdtfwz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3skfcakcq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3bpfiagfn.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3qkgyvaih.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3phatezcz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3plpeigfz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3wdxrwijd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3kvkpqghu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3rrsqyrvv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3csahrhga.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3zgdoqvit.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3wzkeqbjm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3vfgkmhhl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3chpgmkvl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3bwpvdnea.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3jjvhlpxh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3syggplnt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3jqtyngzq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3vfelllri.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3wtoglmou.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hpzzhiia.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3xkoyozua.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xawgcjwh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3srccxhbo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bpbenkcu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pkcsjawl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tcxckugk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3agyeurfd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ibqmsrai.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ubzoijsu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hocasuyn.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ctkhqazb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fzzzkfue.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yyzvzvfo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3zloinrib.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cqemmcaj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xsiacsqq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3jvlksklg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pzamevrb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3hmfjwuah.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3yqcghavn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3xpyjxche.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3olijuxet.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3eenlykua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kywzqfmw.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3vnbzankx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezqfgtlu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3mrfzsykk.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3zvijkodk.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3rhcusgvn.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vtjjheeg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3scghdcvz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vtevxokk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3bfuhjgcf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3elolyxma.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rvxbmhjk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3gohoczvl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3sbleplva.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pwaiygxm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bchxzobq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yfmwsbvl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ydfemocc.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3wrovqdho.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3mjnndqli.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3oxihgzas.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3xvwgcfwi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3jnygsbpd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3eihyafov.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mmwsgjrr.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hymrxnxw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fpddvpaw.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rdfhjtkj.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hihivaki.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wpzyimeh.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3srspxjjb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3yxihayyx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3sgrpuynm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3lranbwac.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jysqddio.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3cmzngxne.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3woblccuu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3bnsoqxem.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3jvglqpmy.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3hfsapgxf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3hmnwdaib.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3emtaocwf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mbmnkyjz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vwtzwflu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3avjtyepk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dqzlzyvf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kwtbthgo.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yfpbomin.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ptpajrro.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3foxiithb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3nehlpfph.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rjmnglbz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kpzgxiyc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ppzmlcjp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3byircmhm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3iqhrvzzh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3mavuzxuc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hedyeimo.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3qubglfnc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3njoajdir.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ptgbxwja.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3soymnmwr.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rpsvpeaj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ixyfmrrd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ggkknkas.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3eilktooh.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ifuscnfh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nxfmkhtm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ddqfqfta.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ueiujdzm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ihsnjdbx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3czaohvul.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cgwwuwcr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3etxydgrf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3unireewo.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3onfmmyjr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3btjaxmdm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gjzfschi.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mhkexexm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zfkhbbzp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cpjcewdp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3halsujac.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3qcuebpel.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dvrqammg.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ysqvtigm.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3izahlapp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3zeicpxyy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ciewmlpa.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3avefikdi.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3eyzszdew.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3qmnbgqdt.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3mgjdvmcb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3quqxfwnz.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3mnbsoaax.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3xvjtfous.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3whlfemak.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fsjqkact.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3foiblfid.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mtysqhkc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3tdfnllgd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3znvrawls.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zyfrukwt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3nkdwoppp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3hkifytoh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3yeejzfmj.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mlwugrfe.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3drlnucub.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ehygesfb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aoabspzm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zxmzmpmq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ajevqakd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3rtdydzme.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qbaxaini.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3urlnghwp.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3thgkwxtx.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3iuwcpykp.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zkcdmpth.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fyrctsxz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3eshcpwsb.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hlpcqlqb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ayboenkr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3bmruexme.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3efwytmgg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zfkhtlmo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bxpwnvhb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3chsmgdik.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3tflsukiu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3wxcetzqh.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zyceueob.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rgiviuvb.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3khqrwflx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3zaorftbn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wdchhakw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3quzmtqox.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3rdeodied.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3vhpdkkmu.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ogucvxnv.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kjgxkwrw.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3xxmiypch.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3dwewnrjr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ygmkgwid.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3qigegxet.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlimodej.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3gagktftx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3dqfjdoxc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3nhbcobop.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwprceky.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3wceobkav.html


<!-- 参考信息 -->