代发 wailian999

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uolzvdzv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2olftueon.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2kfwgbfep.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mvjluzwf.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ncjycbck.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2pejxwuwt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2hjlahene.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfxynqpu.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2lglkzgci.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2edlqohzh.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hwedzdwh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xtgpuhim.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2dypsusqu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2rsiconlp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2mebxdyjp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2hdtuilqd.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2esuajgmd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2bciilssm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2egvaskto.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2tdagycxa.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2qwhlunqf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2whwuuddh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2yzbohdzg.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hdxlkxbx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2rfryvekd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2afeeovas.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2btqikauu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2fcwuwoxh.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vnrokpeo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rxebaonx.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2hogdnmhl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2shvahohz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2gbbkqruf.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2yfsgdvli.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2lohtbsts.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2iedhcwzf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2bwiinbjh.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hkcoivjr.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2wlghxbtz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2imowhkpa.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2yzvlkluq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2foxaxwyq.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2hsdhkucw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bosrpqpa.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2sdrgjzcz.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2skoknmen.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2hsajtsaq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfwkqpsl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2wdpwjfbk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ponnczvp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zyfvkzir.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2wvqxxaiv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2sdjsghsz.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2etsedecs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2larpargw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2vhaiipdi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjgrkmck.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2cpftpynl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwpwptty.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ecqvnged.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2fihvhlia.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2hcmmawaf.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xzewqwok.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2iuqipsab.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2nplbsybw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qkabbtkc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wblxpyfh.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zspagywg.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2jbtvgylr.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2xrrcztur.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2buyypjjn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mldhussp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2wpnpelfp.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2xcklfmar.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2jaepmnjr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2rgcjrblu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2hhvmeaxe.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lrkoumxc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2qnsuhfbm.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ivdpsqws.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2jxypirfh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tzirodjp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yjeafmjc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2sblcdzjo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2vkdiimvn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2snjeagpf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fxbtgbqa.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dimifgex.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pyibcmqp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hatplvxx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xpwlgycn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iocwzojc.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2voyxhlon.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2nfiqnake.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2mekyivwp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qpmelfif.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2exedosmk.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2edlkrdrj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2fzdhjgtt.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hlxysoyx.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2eyvtmkiu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hctsipdc.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2foxjriod.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xgtlulvh.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ppbtcrkt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hvrictrh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2xkvyvvkb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2vgpdlsrl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2pwgbxlao.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2yizuhvlv.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2gtuoeswv.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2fujskeeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmnelstl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2oodqpenn.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2fzyyipgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbmlsspx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2emwpkmrc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2vgshykyx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2pzahuulr.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2xyzxcijw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2guoinhfr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2pjmcfofr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2bqkkxryx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2dwyhjspv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2jalxbqim.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2rafaprzk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2rdntnrkl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2merqitjf.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2kibgyjjn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2muuojkdl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2orbcbpsk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2rdmcxvhr.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2iulijlis.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2inbhvqnm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2bfjsoknh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ghppohgm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eqjoagru.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ooajlczv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eypkzcof.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fhdyuljj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2josdxjka.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zedibilb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jvcixabu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gwngeuhp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2nwgqheqq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ekzjnadq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yjtzavya.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fjblcerp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jjabkboy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ldyunruy.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zcxfmggu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2qfstuhzq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2sqainuxx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2laodhwar.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ydcuults.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eejmuwxx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kohhsgya.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eilmazlr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2msxomhoy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mnlmirvk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnnfnmdw.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2odotwlia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdheuhcs.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gqmqpzgd.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2kuuchtjb.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2borslhkz.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2teiavchb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2zhjgjrec.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2dichnepi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2powxdtkb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2psvhzkti.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2phnzsqqk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2hppcmvnn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2gpbwqhcl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xjlheold.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2blzxzqkh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2tjxiephd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2jtvwfrae.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2bbqcxmax.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2yjxkommg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dbnsnvgq.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2gfhkmuxz.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2plxyoabf.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ubdakvov.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xwdiabsy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qzoqtiws.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ccjlbsxm.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ugwdzoay.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2uluswsme.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sujxjgfr.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2indbbmav.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2zldpaaom.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qfsgjkvk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wabbgjcl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2tuttwofo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ftjgyjsu.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ifctonfv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2vnvpqtru.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2xwbnsjys.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2bfrbhzgy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2uvmqyrwc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dxecqynd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ohnllmbe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hupjavww.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pmqmftrr.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2izghjusr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2knaoincw.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fpzzqvpv.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2tgegsjvj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2cwjjxbdj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2kcirhagq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2eatamyyt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2krflftgb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pboofhlo.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jguldvno.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2rjrakube.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pyagfusn.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2fftxajgp.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wfpglpqt.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2aframqlx.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2lhoboykd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fxjgtpmq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ewpymabj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2csrbkzra.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2smhdiczo.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mbrofpdf.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2kyhlqojx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rmxbnpkm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2wsxfhaez.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vzwzyfbq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2hpldsdon.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2aivghxvw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rzvtzugb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2gidsykev.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dqlhhwna.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2ayqfythy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ncyjhvjk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvozyvak.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2itqwpplx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwwrpwee.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ntrdbuvu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2phjffexx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2kgkmjoch.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2okgyoysd.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2hrtfjnwh.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2juczwwxa.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2hyzuflzc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vsysywuz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2stlpxiqk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2muurdsuw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2fqpfrqmd.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ypehxvvf.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2pytydovr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2atykmupj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ymhlrscp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uwuzqysq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tgtsmgyw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bderqbfw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dgxvgcph.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2exmzotrx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mbcbahix.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ousayjlj.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jxdjxyou.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2iozjidzt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jtwddyni.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2grnmemqg.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mxenjgut.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xjrhvxhq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uymiksec.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2cxlrzbtw.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pquxzwei.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2nnzfoicf.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mdsekser.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fpzxuuto.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2duqqhgvx.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2npvctqnm.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2dcarhrja.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2oaetrwwa.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ahudemga.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zlhkfjxr.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2etyaoyoc.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2fgzwmwpa.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2blmjqrol.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ubuiclri.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2omratfrz.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2qesntlmm.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2btvllzxd.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2vecnsamb.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ddehirnc.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2ldrnuuex.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2aviheiav.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wyuctjgs.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ckvqwouh.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2shnpuaiv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2zlwemfsu.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2owkznzfp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2emirgwcc.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mrpmtuov.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2rrfjvfzz.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2xplddnrm.html


<!-- 参考信息 -->