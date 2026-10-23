代发 wailian999

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3pghthsrs.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fxfsfqit.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3oxwauunt.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vbvzzrqx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oviplygn.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3xykfyrpc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fgdjoszz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3keiyhxlj.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3izixebgs.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3rcqwhsnz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3btamkqfb.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3khxlgxow.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3rwcjzhrv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3nimziyal.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3iwnmuizd.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfremvdk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ebyuehsc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cvzkodma.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3grztstbj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3wihsncuo.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3qxberjzn.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3acwhyyjt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3zxpcgpug.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3aqsyfyjq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3vtwmvhge.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ibagvrhf.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3wjouyzkv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fdwvnmzd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3byjqzont.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3qsqdhisc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3hovncuji.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rfvfzvhh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3wpgpptuk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3szhkmxzz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3brwzwrcl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3cplviqmz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fnpowlqz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3yyxuvlmd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3hboeetkx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jzxrpekq.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3gjwuwryr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3potbnwfo.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wgqsoeuk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3kpwhfyil.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3majoeyhp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ocoojire.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3gwxrrnvs.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3augntgsn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3vkimvxxe.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3baydzvhv.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3yiporyct.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3modgmfjr.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3oxxuxwqy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3holehhsg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3eernsllt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tymvdxgv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kefnrgmk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3wzfaeyjm.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3vmddfobk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3nandrtce.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3fgwoewxr.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3onterwbj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ctgwhzyf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3gcdcqfdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cebbffyf.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3llycrzoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jssyeufp.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3kytpgbhy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3hapzfdzd.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3fkcvaeje.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3pxeghoqq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wyahxylp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3eyuppylm.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jcngzdgv.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3chlfufgt.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3algoloum.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3rwsqhszr.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3jkhcuilw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3lerouidy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3ungtuvdc.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3jwvvombc.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3ndnrwafn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ghgqyyaw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3yzcvkyqx.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3hkykkrro.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xufwbefv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3bmvllxga.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3ggzsgtja.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wdkapsnx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lzlquarb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pergfkri.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3udidzrim.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3qtfgejmy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3juilflwn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ofwhicwo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3bnzgartl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zpaslprx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vjlgpivd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rbdwujiz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nolstsow.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qfaxfcjk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ihywdjun.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3kwcmluos.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ubzaoyde.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3yrriuyrj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3qnareahm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3stiswgcs.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3rggcavke.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3mlmlkyuv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3itrnbmee.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3phgsjofh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vijzocgt.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3tvpfmudw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3txhlhbqr.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3yeeapiht.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3ailomiwg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3doddbanj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3gayvbmbf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ryihqqko.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3dkqosdfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvwbfwcg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3usemxrsq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ckmqztzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezvclpww.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3otxzpkkt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3svhoepub.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3rdpyrjtr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3whruksou.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3qbiqxujj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3tipqdiue.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hfffnfsf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ovgjlhch.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3fvcxmkgl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3kckxjrkb.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3bwmaqsji.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3xujxxvng.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3vaklthzi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3opaslanh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3kvlhgycw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3wdmmmnkb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3klratavh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3swxdsmrf.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3fkznivjn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3kkosqpzf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rdroctmy.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3djbnudcr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lmboqmus.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rdnqbees.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3apxcqdob.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xssmjsoj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dwcqdfpz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fehskapq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kxthkzjd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zzdmyusf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3aixzyqbs.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ibyaikmw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gqgpshxa.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pnyvdrwn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rlalidbu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3iosgljiy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3peztlcbo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3itetjlpl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jfksmgtx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pxnxhigb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3njpfazsp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fqbfhvdd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3bfixiumr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xlrwnibm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3guuwptbw.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3rjqpathe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntpweefs.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3tjxfyedm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3cccqqmjc.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3eceiotrg.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3psavxlpi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qmidazua.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wyhucchd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rtqwucgn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3yzebalfl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3wdjnvpfd.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3wvdapith.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3zikppakh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zdpoakky.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ngduniht.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3yorvzhvh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bcolsmqw.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3gleeyrjs.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3xhbpbkcf.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dreixeom.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3bhdtiibm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3btppjsbg.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xrcqayhc.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dcitywdf.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xepivpld.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lwoowweo.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xqnbbuny.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3agyhbopn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lfeayjpc.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3tbsdbmwl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3llavfdey.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3mntgxykh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3kfuwoswx.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3utgjvdhp.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3nfjcgmnq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ducpubfw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3apcapnhn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3dpmyshwb.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3hybbphmu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3kbihqcsv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sgvlvoiq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gwnrbjzg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3gkutmtcw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tpzyadjm.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hcjjqdhf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mantsqdf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iyuyandh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rdnczkpz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bscssmlv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3lfmgbnfw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3tynlbmul.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ctzrbfkf.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hsynldli.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3bgoxumhl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ktuyzmuo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vzermtex.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pxltpvyk.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ghbxmosq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3hjftjjvz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jbqtzvct.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3vqqimumn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bwfgpgaf.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zgocuuxs.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ugnuzkus.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3bdxffteb.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ptchijzd.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fyiiltqv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ouawkuez.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3hvrjepro.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ykgqyxeg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dpsusijp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lcseheqt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ittfridv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3impvijbv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3gswsvads.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jjaludzt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wpklbvox.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hscqdljq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uuzsxkzm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pveoepyf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3dpbovdff.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3jbpnncso.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rhamsedn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3mnqpebkv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3xmryteib.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3zfnckypl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lgvhlmph.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zwbscpjx.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qlqnvmyh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3adoyjsmc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3ckxiicyt.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3cpzxvekl.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3uadoedpm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3qptywvsx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ihkvivts.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uavgvqcb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tedjmhtp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3chqmwjlh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3rmnnfevo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3circtsna.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3muovqwjy.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dwtmbxow.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3tsxxugar.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3dwekcgvu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3yeoqncep.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3jonphnie.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3weivrhiy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3khpexdxv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3bskogtsn.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3gfobocdj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3xponvuqa.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gmbbzcyd.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tedafmfo.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pbodmvyb.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3byooeotd.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gkhghdze.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3epxlpxox.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zyqexamb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wflpeheu.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3rjbvwznd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ryfutfku.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xrkrofze.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xjakwtky.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gbedpkaf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3peaofxgv.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3tstqgdtw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3tldsjppf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3seplejvu.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ccodejyv.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3xugzsxpn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dptuvuip.html


<!-- 参考信息 -->