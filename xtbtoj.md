代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3pglzuxcl.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3baulllaf.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3kxpbiunx.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3eppgylao.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ixpecesw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3mezsiejy.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3shuowemq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3vmbffvlw.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3wrmngtdo.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3caqxtele.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rpgcukee.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rrnlcuvx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3yfetaoip.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3fzwantgq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ztlmslcw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ryluapsa.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3omgpikjd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3nugycurf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hocsdgll.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pqruhqhh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3dzqnymiv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3agchpwrd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3afidxbpp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxwcvpou.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3zrjxxedp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tmjkqpxs.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kruyelya.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3widywbtz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3etjxuecn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hrkguzju.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3inefzwjh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3yksbbxqv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rbpyjfbs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3yqwacvgk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3uoggyzgb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jcmtpdpr.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3elpozmlk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3frljggxe.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3umknaign.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3sqhlvgzr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3tajxwlxv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ancluxnc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lrylnhpo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3eaqmbvkk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fniaonuq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3oqpmhmkt.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3oevnmoaa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3cjvqzgkb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3izcuseeu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3aipgnbkz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3pgusregd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3ifrxiicj.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ejlppbxy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bzcswzxj.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3etvgovap.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pbtsdjfn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3wzytiohk.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3knrffgkq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3jvgrbysu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oiringxq.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jchwafzg.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fcjdvvsq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3sqwjdfeq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fwagvfnz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3drgarxkg.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3kmkkypeu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3dxhwrmnf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3kkrdhnvl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3thsoqafa.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3rkqvkjus.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3ptzcsnbn.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3aqheorzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqltkbcx.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3dftgikya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amrjxhrb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3dhobgzmh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3tqibzjrb.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3swmhvgxm.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dnptsajx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qqxhczzz.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3irfvcfhu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jlinnfjd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3isccwmmu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3dqkzfaxk.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3gfmtvjhv.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3fifhalcs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3vajtnbia.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3warcwakj.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3vlmebfee.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3fxtknxgr.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3izqkoqja.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rfqtvefg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3bracjkbb.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3erxgazqh.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3litnokdf.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3bbmzsmsb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jdhcmfsy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gyqgpgqy.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rcnzbllo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bclqzwce.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3lmzybaat.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3qhczqrjr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3oyhjlwfh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kbghwplq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jdnnagat.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3fwnbazsd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hicerucr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3olladpkb.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nhknoiwy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xihghuqv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3gdvooemg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dqetlkrs.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3oqpdasvu.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3wzybadie.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3xebrzzyz.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3pgpvhitn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ousbujuv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gkhtffhc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jfotktaw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uoupbvnl.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3aztrykdq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3oanxdmii.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3eopboyok.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3lubhzihn.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3uutfanma.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3kfocgxhf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3iugsxabz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3hgxsqndo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzpmoamg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3iqrjlvmn.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3oaszwusc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqlfwbim.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3fhacyalo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3byzuhexx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3dudevqiq.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3rfozsgoh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3pbrohznu.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3dafcbzfp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ibhsyvfn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3cyrnewzp.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3rhfqfbmw.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3pbhyzvqx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3gqflmnjb.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3rtfmmwcd.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3upcnomgw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3rlgfovgy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3rnkviruq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3teekrzpw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3pnieacoa.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3nbhjvbqu.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3vhcorkht.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3vtumulhj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gufbvkct.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3dsgtqkar.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mncxdepu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3arawglqf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nivaymtp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3xmbubzlt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3wcraflmj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3pleralbl.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3xopcugtj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3asuehzuw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3adujusmz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lazgwqpo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3svwtgrkc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aikanxvo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wptbhnio.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gbzkyyra.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cmnhhyxo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3tfaurlyl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cpxqscyg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3zntqdacl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qhhnarro.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3inmahtpu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pskgiorq.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xondjujq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3czbyjlcm.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3tdbwnmpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmczlmuk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lvfxxgsc.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3lqcpmwom.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3htxlzkoe.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3oginytzy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3nrjbiweq.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3iaxogdao.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3sqlvzubt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3teligwly.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xelbzpyp.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3jkfketdb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3gncaxmwz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3phvctlgb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mtgsrzfl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hicpvgcy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bzppzera.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3zdxmedwn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3yljpupku.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kouizmkx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3deptpwwr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3vnseqqdf.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tahgqshg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qvezoauo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ohtkjoeb.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hinysrqe.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3klxpsvmr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3tkaasovi.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jiebqguc.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3sckojhoa.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3dhbvciqf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kaxojdwp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wclwtaum.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3sqyhzgpl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3kaaueygc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3yjdqvgwm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ziyfveat.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3skhixltr.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3ewnyubhh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3zjbnncub.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3btwtobxd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bdekacyh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ffglqbzt.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vlualjpo.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vczzwtpe.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rvpqukgw.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wjendyos.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mcmuviyk.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xjwocwap.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3spmqmsyz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vxubgrda.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3gbngwxpq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3bfgtblza.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3rzofthqi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3wusiiarl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wxueyuim.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gqnaqfwo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iebsqqcn.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fqdrceee.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3txnyimmm.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3jbeeckdw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hiwlwlic.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3hmqivupy.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3wcuybpbb.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3pdusxbjk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3eohsffxq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3txbrqhhy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3pdctmmnl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gkhbwrtt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3yqexkhfz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pbqlvgvr.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xgbzhdvr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3odqkaxkg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ypliwapv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qoyksodi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lpadrsrk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ywddftbq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3biygbmob.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yoryyeoa.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xstekdok.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3luhflvsy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3blvybuwy.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ouiqbqae.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3grkdcqxt.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3cgizonyy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3gqbvient.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zdzsczar.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3kshnzlky.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ewbswslf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3krysvzyj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3tulgvico.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3mptceysb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3pxvdtybb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vwyzzoeo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mfbfvdog.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nbcrkojr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sycipdiq.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xnrbrbvt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3jzwltwmd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ynikinpy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vamyzjrp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3rxbgxsgo.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3slukvaah.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3rhipcubb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ojmzvqtx.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jkrygglo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3klsbamgp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tgaedzov.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3ihryccdw.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3lvfpmejy.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3xghdxwvu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3chgvxcfl.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vledekha.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xofyiwxl.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wkqjenmu.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xlbdngav.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nbpasdmr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3aowxalcs.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3yvrxpfak.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3avblzrif.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3gntspjjk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zolrwsla.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3amtojnch.html


<!-- 参考信息 -->