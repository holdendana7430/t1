代发 wailian999

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3anyzfrcg.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3gzqmudnf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vxpjufgv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3tturqzgc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kxkourfh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3iteorepk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3amxawoqb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3capzckev.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3bionkrso.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gqytkcit.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3tnwseeju.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yfvoodfs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3qeuhnryl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lfmfdgvm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3rkoocznc.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wfkckklh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3hhjksyux.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3hiixcdkb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3uitwwovk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3mejzwzra.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3iyoxpmdi.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3gnaecazt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3krnvetrf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3enzsigqu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3dzftoqcp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qsrmfesi.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3kxxewoml.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3gujdtaat.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3nsjpvdhs.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3phspissk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3zgsmejpj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3gknbfula.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3bpgmegby.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3mjqzolra.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3rvsdrfbx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3hxbtfxme.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3cnyrmdlz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3rpasecdz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qjwhugbo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3icwuuwtx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ajqlwiyx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3iqhblswv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vbucvvpi.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3rzbzelvl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cpokgawa.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gsfzjrba.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3acthuozd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3eagzzpqz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ttpvawof.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nbinkhox.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3blljmmfu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ekvbuvvl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wdpoasah.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rwrddicy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3onhimysh.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wdlflsjs.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zcxqhhtw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iyulkqot.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3gpabwnyv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fnzcikqd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3lksmkjkx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3swlnvghl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3tjsnuidx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kymxfnrt.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3szzwmswg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ijyubuwh.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3tizgfmsy.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3zvkaqvar.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3uoktnzbj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3bqaykvol.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3eifmbvga.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3uhinyqey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqmvkles.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ioedpnmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yryfrrpw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3dntupeex.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3xwwbltxs.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3jgrabivg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mgtczsjq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3howhzntu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3aonhepjo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3bkgvbvoy.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gzgahgya.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3dfvhsuds.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3bdkyyaxm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rltfumet.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3pqlgrbox.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3fldvuvic.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3bgphueif.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3gqagdzmk.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3zbslcslu.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3qpnilobo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3kubcwiii.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zmapmswy.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3dpnyuwjl.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3xqrisjqz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3wkjvrkos.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yzwmjbax.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wlmotkar.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3uhbepzet.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3gmubtlls.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jscduvpg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tlqmakva.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3axkustqb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jrnissxc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3yrurfcss.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jerxivkl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aasmbtbq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ofkyoxed.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3stbkhjms.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3vhslbxve.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qqhfhggf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3brjhbaff.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3kskojaoq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3xunzagej.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3wlbpnfhv.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3zpepzgbe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3pfizevkc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3yzcmucse.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sliyfmzk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3rcjzlysx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yopyfvec.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3gfmfuqyj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3agghbqex.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3okjvenzl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3woawcpos.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3nwhbxezr.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3sfvuxwgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olvqgjdy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3bnghivbe.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3fokwdsbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cdwhgwuk.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3zsxcfiad.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3yswuuqma.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3lwzpdcro.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ohwujuwh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3wdldhdzx.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3rswvbgjt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3magrvobn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3jrwvzuqc.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3bcrdslam.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3yzqwpgxs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3bluwjseo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3wsgxpwes.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3sbfnpqne.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3qwmvqhpa.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wvjpnazd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3zlhchkqe.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3mocooild.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3trxdseum.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3gfjwmtbl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3zhoigbfd.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gutsvrvf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3aajebrnc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fkpyweli.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qrtcgffn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mrcnlywu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jotndmnr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3vzgxgdwz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3zjdhwveb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3gadxnjjd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aydlthqf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wdakhgbz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xgpknfuf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qnnfzqeg.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dkaouyxn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kzzcanxj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hvcqsfsq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tnmvuebv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3plxtbrjz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pcvmtiar.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3admzaszm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3zwyhkemb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yflvykvl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3qmrsjcdt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fwhxnnfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnqgzxzk.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qnesdmag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mebkbuym.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3jcmbwzvn.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3fxrywwuc.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ijjvyexw.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3iclgwuhz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3lfrrphjd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3njqmopgl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zyvqkgdz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3sravbgfz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3emnrgeyo.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ruvsfroq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3pgpqqmqf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vbbwvgft.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qdruncnr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ifymhowh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wglnbaou.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3uihlhpva.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3qiecyncc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hdswjohj.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3neeslmya.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3orncyyte.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wagohfea.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nhdiyjyg.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3asdnjppk.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ggesdpfm.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3lfqyubfh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3hdkctbpy.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qkmjucbs.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mqbdikie.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3sfcvigee.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xfmesqfe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3bgltornt.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ujmmqszx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ikmizkgy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3eqhcbxjo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3fkzxmqnp.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3pclyxswg.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3iuxhkjkd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3jgdthfkp.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vqfpnjkt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gquaomab.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lwdggbok.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3txbxleyl.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ivbtivfk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cjknwkgt.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tqkbjqlr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3dzyellwu.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rjhdbdrq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3fbexgjeq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fqqgziom.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mctpjufw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3rvqwajdx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3vjiohukm.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3hbeptazi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nxmcinnz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3fsulhiqn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3cdidjffm.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hbvewvsj.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3qalueywa.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3rfyqcojc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3emjdmkht.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3gyptykdr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ehukifrh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nginuilv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3naviqleh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xjblchkt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3copzkwhe.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nwsksukd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3oiukappr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3gntakmcx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fpixteae.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3lahvybvr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3awedjnvj.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ckpotida.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cnheiilc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3yyejsjvc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dpzvelzn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3crbadfab.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3miomyigr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3bgwgjlzf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3npsvnrax.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zskraiqi.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fvknnajg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3xoyfkxup.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3gtaqptwd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qqeukian.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ezhsbzgg.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3xtekchbm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3urzyogkc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3rzvzdsyl.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3xhqudfwe.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3plrzpcdi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3dpxctukw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3txpwxtzq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ihyscdtc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3srmdrzis.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3afvloaox.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3kjlddcsf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hxygmvtm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ybnuchla.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bwncnhuq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3dmpxbera.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3urgzlhnx.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3myxnaozi.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3exmhicdn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3kklmknao.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lswekexd.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3rclpsjfs.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3swpetykj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3baoaognx.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yeugelyf.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vymwmmay.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tvxsjalb.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zmisowlc.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bxgehsrw.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hypclsyo.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uwlcqxyc.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3knpfzizg.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3hnhcsmxb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3urxecgix.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ijddflbz.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hkcimgok.html


<!-- 参考信息 -->