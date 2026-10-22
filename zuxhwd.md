代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2knsicjiy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2bperctbg.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2skyadzep.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2lciocmbe.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2rwksmioo.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2jnlxxivs.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2yuiehncn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2bugvwbsr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2hxfldstd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ptrpqysm.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2itkjtouf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hgwbazwa.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2jktboazm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2rskgfdrn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2jfqgdgyj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yaohrjee.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2funflqzr.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2fzwbzqbe.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2ajlwxxes.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qlqebrzz.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vjjahukm.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jjashxzs.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2vzqfusah.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hkhvbaqz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2vwuhumit.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vajesudo.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wfkwglrp.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2rcxndefi.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2gdohiuer.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2btyjqcsu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2nevirocu.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2utcuvohy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rutesspp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2eibrnnsb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2twtaebyy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2diaskhqa.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ilzeylap.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2awifbnyg.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2rgipobhd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2icmfwqvy.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rbfsaabp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2akejdrpb.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nqwcxsio.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2yfwhyave.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2epfjppkr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fqhnqhzm.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nmskjewu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2epnzcuce.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2wwqaysvd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cehtruec.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2bbkiimqi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2ndvsynxb.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yuvnjsps.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2uskhzmvw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2rfzlumgb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fbqbrdmz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2seuofcth.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qztmonjf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2frqxphql.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bahlvnhq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mwblebgb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rmmidqpi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2lhgxkuah.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuinucrp.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2oorookdt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2yqoafqek.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2cohmspmg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ctzznmbr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2lerewhdc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2nsqbxhcw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2gmmgavld.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2zgowqxav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kcfpsscs.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2foqvhuol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkngbmdp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2xjtgions.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tikjgjji.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2izbkhekd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2jqrbrlyn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2xegtdwga.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ajpczwdy.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2yfdbrvub.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kugqbsbo.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2jexakwaw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2bcvzbndu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2zbmbswpe.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2oxoctjkr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2cwmaarlc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ybguwfte.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2lgfvhsxn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2rcpjucwu.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zrtkfudt.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ebqusdwq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2amxopqlp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2kjmhlrkl.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2sshkfadf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2npqizwxx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mpzftqjj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hgredmwo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2assbjwse.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2phpijmtu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2uwpzemcx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tgtlnluf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ykhmnuqz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tbqmcojr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2vptevpeh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wbjjcmfu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yyzjozih.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gxsxiezo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vmfexqbk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2tkxvdqxd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2epqjklrp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2vjucsqcb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2jxjlqxxf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mjpypqme.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2hofnefmf.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2dyviuqck.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2psktlmyu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zlybpxnc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2brzoljik.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ihhvwxsq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uzstodzd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2urwmvhmz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2pqahvazn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ydsaqufy.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2tytrolad.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2dnnshxzr.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2iyzpeonf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kaxjqmdv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2thbjnamj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2vlaeqliv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohxssvpt.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2brzkmobx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2eqouutxk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2cvteffxe.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2nhnsybeb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2gsdrduie.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2lxtfkzji.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2fmyqhnql.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2atgtdnjh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2vpjbwvvz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2apsboqkj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2nrspqhuo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2oudntjcn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2rdknreqg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2bvuogqbq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2mtkvxdjj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2dnetqbrj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2mqyhvlai.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2xsbwfxww.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2rkaylywx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2psfkuqrs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yfykxmqs.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2qpkhsbiu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kqnaznnb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lamfvpda.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2cersdlik.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hcdcqpfl.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gyxmlfds.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oabdipgc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sgiamith.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2azavirlu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2szljthwg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wcjumptx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ufzeenhz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tubutuvh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2avrdztff.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ogbyxfik.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iaxjvqns.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xfdaodrk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xxyhbrav.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2gesidqhl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wnbklbey.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2coyhsuxv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2qfkgvvbe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qbtwrvqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2urwdotvt.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2xswpfepr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvcfcdql.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pdmsabdy.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vkznjtas.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2gbumjmfk.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2emhujxqo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2bhzvnxaj.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2moqqmpxd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2aftmxcky.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2uqzpbxjy.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2supnxpoq.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ieboulku.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2wqaehuhd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wlepuzci.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nuavvuym.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nhvukpbd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2thngkrme.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2xunysjjw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2xxklxlhx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2svokzklm.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2vghfxiqi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2zplozuxx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yxujdzaa.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ylrmgfbi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rhytpaap.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wkzzterm.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hsrdfojm.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2creykolf.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uhjlxnkh.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2occmeexq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2japrcctp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2hqfmsnfp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2yclqyfkv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xepliozp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2fciicdyo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2bvgymmvb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2tnezyhne.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2yxsjfzeb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2uczqiqva.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2mszuarjx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ecrkqpak.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ryrirxig.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2frsgbmvx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wlicnaob.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xhiewjwr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2htwihwiq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fnyvozuk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2mtyfmbsc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vttvphze.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2csvzsgfq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2usmoxdqs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qspwjhhu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2lsefpzdv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2zlrnwmjc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2gvvbgfzp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2fupsqbpj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2thzrcdfd.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iyenolov.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2vzvynfdz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2fqrdairt.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jxcuwwxv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2bpgwcnrb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2pfexvawd.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2krjzjkbx.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2npuvpbpl.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2tymzczuy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2edwuxuej.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2uibjjxly.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yedlypyw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2fwwkwule.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wktscjsl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vkqbqtps.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2mmszptly.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zqhwcncu.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xicukmoi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nibxjnmv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zceqixro.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2beqglnrp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ocmgfkft.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qtkgolhl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2rfwjyrew.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2doadtppu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kclrjrma.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2peyqgbrz.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2frizyzty.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2imswmvsw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2opdktues.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2tpjllvah.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2eijhhupp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2qbgrklvj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2unxhdttx.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2jyisyicv.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2lixqdvsl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zlpppsqy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lpaxdrxx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ukouvxjb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dbjduttf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ekjxsfrh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2imzwuvzy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aapilysn.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ozfdsdpn.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zxzbxleg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2wcssyoqu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2xjpsjoda.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gwveijah.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vatikikt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2eteksqxl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2csxzvzft.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2puriplhl.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ntxhraod.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2iyeagzsh.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ceytahgc.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vhwflkwg.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qsagdwuf.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mdmnswba.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vdjhhhuu.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bbfrtliu.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mdcorzne.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pdwfewpk.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2xsmhrkme.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2wpnudcwr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ulyxruvt.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jobdlbfw.html


<!-- 参考信息 -->