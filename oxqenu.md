代发 wailian999

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qhdqxpky.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3yjridvwm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3jmgwypfi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3rjnbfivz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3oypiyroh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jfzggzlz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3zkaxerko.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ijknslsq.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3oqkocmur.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3iygbbzgj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ghbdqyom.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ejiegrnd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3shtlikes.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3bouspngh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ditaisls.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ijxlvrpj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lgmkfock.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3rixgfamu.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vkkswgmu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zvfuulkk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xhhxztdq.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3johqckkh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3zojttzkv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucqmouey.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ztkkdqes.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ysfascks.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ctasgzzt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3bcdywnty.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3wkrwzsbu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3bzxyvvqt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3iccmclwi.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wpnjdvnh.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3zdownbkq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3yynmcyjz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3mppkigtt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3siztccky.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3toqocwca.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3qwenmpno.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3dndginsq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mrcycuml.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3lhjgsmyb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dumusxfy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jafrokeg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ilcdzzse.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yxnvacnv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3irwcazle.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3utnytgsi.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3cnspeamf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3omvgqvdw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3botxqfkx.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3eeteiraa.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3fffegbdh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3knsujljt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3hephzbfw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3uinyjzhz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xrgpimmd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3hfimvipf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qjrhjfbv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3cropppfb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3djvczxas.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pfqiasdq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3umifmfnu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3wztlgpzj.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3zoepludu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jqfedpbq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3qshmwiso.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3bvndlwaq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3gcbqklox.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3dqhdtefv.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3haltmjgn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3hmcqxzst.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3iohoxwen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkzlzqst.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3fqyveval.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkqjxafh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3gwckhrmz.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3bsxlhwcw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3qpwwxngr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3uhtcsjrr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3zstylqpj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wseasnne.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ulyghsbo.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3vfloperd.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mbqfoszq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ccpbpvuy.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3wrsjgomf.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3bzxmnkgh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3vrqyrsjc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3golzhwko.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3yifsyufb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3trpfxckn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ecopxxnb.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3knltlcfg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3twxmtmpn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3rhimgnsf.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3cezutgzg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xfrvjbhc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vakteaxh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3loxcrdgm.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3zwusdzcv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ivlnkyri.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3pfzrnira.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3svrlxzod.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ldeqjhta.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uvhzgizz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vbqzmjta.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tosipplv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jjfpqnnv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kwgzzgdg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rrgnbxjz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3yzqczphq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ramfcpzw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3xdbwhswc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3jjygmncx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3idrhcgiw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3qpptaegj.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3qekeexis.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wftzxdeu.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3exwbdqco.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kpqjtbmi.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3fbrhgsvm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3chocztoq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3oofkydiz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3acqcxsxx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3sobyjsaa.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3tkobrxln.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3yhnesods.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3towfwnch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rmavlhyt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3vpybgodw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3zwpjywzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjjizckh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3slzpvlgu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3bkgkpiru.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3tvvcvdwv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3dexnegnb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3reeapdcp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3wexykpru.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3duekqolr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3dkxgxzxf.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3mtgpidkm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ofiklahx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3igpabvcc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3mrltlbpg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3rzymedqg.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3dsllojqx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3xbtixriu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3asicybqb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3nddhxqgr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3xjwshgbl.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3qvjvlisz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3daofwxsw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3clrrfjqa.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3nqltdayh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xhejnsjr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3sywmxifk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hkcojwtn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ndimumds.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xzqcsltq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ryxepzvj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kiddatpn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ogdnoegf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3asljeqkc.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lgipsvdu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hgccadts.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3barxrpfr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3qdvtxkjl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3alavomft.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nybgvzxn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3rcjpuvfu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qzigoshs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ibtimpty.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vgccqlhm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3uzmwdysu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mvxhcnij.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lhjxbrlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acehagvp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3btzvhpat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwuikbgz.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3xksulbol.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3mflfszzf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3kbboaavn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hrqkozdr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3kykdwsis.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zwicrllv.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3uqbtwdbc.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3kcrtsrwb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qsfplcpl.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3mbvccziv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ycjewtlm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jbkzgbgc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3geyhaiyo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jnkndfua.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3fbgvppyr.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ujrmyxrl.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3ztcjawza.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kxovbsti.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3mxflkrad.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3vpjghxhv.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ztoomcxv.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wsondsnr.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vgejdyxd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hkthifaz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gcdvuiub.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pjdzkctz.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3doalmapk.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3aqhxmifn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ecipboym.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3iyspahhj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3movhbzjy.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wmqbtqgk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3eojemovt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3htudxrei.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3afedpopo.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3knmftqst.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3yokodcrb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3nrocpjlr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zlgcqqiq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3umtbxget.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zfsnbolh.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jrnfgnbg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zioydjki.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pnwzdwkk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pjnospvh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3cwgtztoi.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3raefdqac.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3lmmthuey.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3oemjfgvr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qwtqcqbf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3payqsxjq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3etbibzpv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3byxdzsye.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bdpqgfnm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nnaofygn.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3nwusocqb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3pfqpthdg.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cnfmjkag.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3eyijqgat.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ojuqyfad.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3lubrhsuy.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3lticacue.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3bgcdtpwn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3iblstnul.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ltcnazxn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3dfdavive.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ysjfmeaf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3xptfufex.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vqmzhjfj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kfuxelqw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3remmhpmf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bnifrcdw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3uywqoidj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jlftudov.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqpbkwov.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yujucaif.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ggmpeycg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mermoyyv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3courfksn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3afmxorhd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3anftijef.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ulfcdoql.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3qxjuffgd.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3yedzhqeu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jdwsfkow.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uelxbrdy.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3inswqocz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3byrwkcdm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3tmoublng.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3htfpdtyz.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3sbjejlqk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3tvnuknwv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fjqumzgb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wsqxtryo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3higtdtfc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3eldddagl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3kppkrkdu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jujrpreg.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qwruqipj.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yazjnqoq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3gwqvldzc.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3mwlhcpoo.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3hhwchkfs.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3eaucwzpb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bwqaalax.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3wkhvfmzp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3maltppcq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3egoyyxft.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3rtnijpyt.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3rfuhcewg.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fvyckwrh.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3higcxjjq.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bwnvaxrr.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ufncxdvf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hoqarghs.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zhltngjj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pwmrwhpw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3fddizpki.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3zfkaeggv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3czgixhsw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kzixdpfc.html


<!-- 参考信息 -->