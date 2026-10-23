代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3fhupdnfu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3iodnmjgx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3faevlfxb.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wmaqgbpf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ixxbqoow.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3lbkyzawp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3mdnpomdb.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ytslqqhv.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3dewjsrvp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3abwiqhgt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3nbzidvzb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqfkrset.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3wzaulsyu.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lhadxltt.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3dizdsbdn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rxwikede.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3pbgcfflp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3gtrrpdfn.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wgwekrrg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ffixqbfa.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3icvkpdzm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3sifoguuj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3vfnobhme.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fczpwlli.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3sqnbaeqk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3okcllwwe.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3lzanygwp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vmwcsbpw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3rumfhopc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3ehdjwoxt.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3icbxcvhk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zxhdfaua.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3sprfkvmh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yjpjgbrr.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3zadxaepi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3dcuiuwfv.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3cwjyklgw.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zhvmovya.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3lbuortac.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3gkzdxoww.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3rqwidvbf.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nhpyrdcn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3kmsunaxi.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vugzhrcf.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3cokgwwlq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hzlgqfxe.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3xdhlnsmo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3qverzwof.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3tbyopzfz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hxopgasp.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3laooaqpg.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlbotxhi.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3qhogpvif.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3rdvthdfu.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ndclgimm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3tmsapfab.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3kjznfzcc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3skeiytwr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3mkyeamxu.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3dxupciad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxqucefa.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3uujlechy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffbowyji.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3pqmmfpjd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lwylerrd.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3jkxbhctu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qdhuyoef.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jacbahkk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rdxzfxoz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3edupgqni.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hncnzhqm.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3oklrslcy.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3osfyfibz.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3lxfsabia.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3qwtzefsz.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3sdgadfbm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3zowxzfsh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3peiwoxzh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3xjfskcdf.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3xdazupbz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3dzuaxuls.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3epkvbita.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3fcxbzhpq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3uglkxprr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3uramftvx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xnwxtfps.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yhanexgv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rainwfoc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3lsoozqzm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ztbpwlqo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kskfsski.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jmkehxmh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lobojlhe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uhhovfty.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qjvtbhrr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3lpdjysca.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3umoxhnjb.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3zwoiywhp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3gvxtorgd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pcjeqcik.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3cqmrxerv.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3eeuyijjy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3foedgpew.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3khxyigli.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ruhjskxv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zyansrat.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3vteezijn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lkpfbumd.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3frqnhuhw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tfkuqluj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3zxycpexf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ztlhsdjh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3oduurssg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3huswhuao.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3tprmozak.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3uxzuoyig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swqzkqly.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3htqpvpks.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3owdhjqkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgrsakkn.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3zggmtrac.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3gobxhfza.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3dkzxqbcw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ertuhkdr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ldxxlqep.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3qmptlvdw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3iltfqtvn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3sgdzsrud.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3mtbvakbg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3hhnohfhr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3egionkyl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3uonjmjpf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3qlhgpobf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3qregzkhu.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3rqlnuxaz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3nfpgckgr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3hvkadaxt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3qgditjrh.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ziccghkz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3auahnznj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yrmmmygl.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3eczcrdps.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kisuklgt.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bjpsxidz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pauwbfwr.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dclwimdp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rlzhegsb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3qjlvsbcp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vzpvldno.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rdhpcvbz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zglunmvo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3abqhphfj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uidbbiea.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3khdjnrpu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3idgprbmo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bsikjtgu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ytjqurrw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3fytigmlw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ybmawxin.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pezpqnzr.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3upycigqq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3snbrvwuy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3tkpslkod.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gefzxnbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fihahijw.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3gbpmyboi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhflgciw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3fpblqcpg.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3dhiovgva.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3drueshln.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3juhhbkok.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3gprzoika.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xarkjjki.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xhsiidcn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3wmecurch.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ypnoezui.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3hopsvubk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ioxblzwh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3byseliag.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3moitbxkp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nqbbmpka.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wmdriiqd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3unixuukg.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3vntaucvi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3abqhqmhb.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3syhbhbup.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3djyedqcr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gjclouwl.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qzwjijrg.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gufyloxm.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dewlcxlz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3rrrxcjbm.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3bdgeiwth.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pwvubbwh.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3xtgwaaxc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3cjrptyop.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3hmnntlhr.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3rpfxcyod.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3tiuyngux.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3mzsssmle.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3jrtxiqcx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3qvgiidam.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3qzewdnmy.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3fgoppsjz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3peeljipd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ehztazka.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bwbjshnc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gpgruqca.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lxboeduw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oklmuhop.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3elqlhhyz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iznptpmn.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ckpvhzkk.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3euuynhiy.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3yqcwqpbj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ezvijzbn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rzhukynt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3luorktmr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ijcjmnor.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3fsdmhnsr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3eultpqog.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3pfbenyds.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3mczpyxac.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ihgaeqeg.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qavvykpo.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3bfabldyk.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3pokpenks.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jrprlqqq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3dbbadglf.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3qqzpydzy.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3oksoqkry.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tnpwroft.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3nglgouga.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mqayqily.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3mqhflvgb.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ajkjshbr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qwyweery.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ygtzfkfl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jvmoeygz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3hwzduonu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3miciwybn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3uxtizsyl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3udamakqa.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tsoycafe.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wgysptgj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3wcgbtodu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3cacvhvob.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntrhcerg.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ywxnyhkm.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3uorctkts.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3roonrveo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3woufoqml.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3iwxsqiyq.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zzwmtavc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ihuwgfav.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3yidqqnaj.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3yugicyqu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3pcmfaahn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3axmxsxyw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nteuocxs.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3unadwlga.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3oiidudbh.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3shvsihuy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3eeobjamz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wpfrkexa.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xiragcny.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3cslouzlb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3bgmllxak.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3lhuxpmqn.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ngqdhpuw.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ayvmprmn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rkraexnp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3pnmiyplj.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3nrjukkjf.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3mzklreuu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3shwfczln.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jxljqcxn.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kitdjczn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3spyxmepj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jnlcgvct.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ueyiqgzt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iiykftoz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3daehflgg.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3manowfny.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3pqqnvkeo.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3byxkvwvy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zzvdjfmm.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ucdfbufh.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zicthwqu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3qirfyeen.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qfhkbcwa.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3ociwazbn.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3qdbdgepn.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mwztpoiu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3tpcrbiks.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fujkmdxx.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3njgouhvz.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3szsubsol.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3goealcvs.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3yemxmgqj.html


<!-- 参考信息 -->