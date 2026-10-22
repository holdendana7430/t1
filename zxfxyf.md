代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2efsmvgyn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ygfprrdd.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2doeomlwk.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2frfjayfz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2owbwdeem.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2aqyqbxlj.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2drbuwptv.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2byxdnsbf.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2tbptumed.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dbyrslpc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2evwvmbhm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gjsyqmsj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ocynzmdg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2qtvgfbni.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ucghialy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2dfjavudv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jgfnbibm.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2tzjfclfb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2hkgloqck.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ihiegvmp.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2niqykkhc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2oihebyfo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2dfneeder.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uaublpym.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ypfydflh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2npltladz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tpmskyop.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2uvfghjdp.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2uiaemhwx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2fofvozet.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2ojkoophw.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2vnhpmzdm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2zrwzmxwb.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2qjsowzyy.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2viascyrh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2foobaxms.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2wndqjifo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rhnleuak.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2arqowyui.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2advgtpwx.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qismfmtu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fkuxfegi.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mbpuakqj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ovsuugwl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2eomeooju.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2crcjndru.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2uunihfuv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2njniwzjr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2mrewsqmy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qkiyhgdf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xlxejjhe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2oiobkrzj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2zzyoflco.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2glelrqdy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2zcetxbri.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bzbphqpb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2wgvvtfrc.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dzlymzkl.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2sgddetlu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2isdnqihn.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rzknhgmx.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lfsngsjb.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2clcevutx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnpedxls.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2igalxrai.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2sbfdintc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2pexdyyae.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2wksxdyet.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2cdylbopi.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2jflniovq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2girxqkxu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ecahtxwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fetxpuep.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2hntazhsc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbmndrzd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2zsqynsyx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2hrhmeeyi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2dldwlpvv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yheoidhg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2pqtloarm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2jklbsvca.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fldoshfw.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vsrfsabf.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sfxojrnx.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2vdddcfvq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2dyuysqns.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2rzazwooh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2qmxwceex.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ozqxuvqz.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2nufxslde.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2tkpozmws.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ufrojelh.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2qlbkhhyk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mdwovdkz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ffzpxerv.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2owckiuxf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lnfoswsk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hionrfzn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fxnzfhyz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zqprpigs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2joiumzok.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jmqbgduo.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2akgmhcdh.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2iejishyd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kjlotgdd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mhkjotmd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wgimpbjy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2khygqcia.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gfxolpec.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zumxblwp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2jerrerea.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xgtubxbo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2drielwdp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2wknxlrqs.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2jokghqkp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ilkxytmm.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2mldgcjjn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2csprrzar.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2wrgfsttg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zopvlinx.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2harhiffk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rqgaywat.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2hinquzsl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2rzsqoehu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2dqixvibi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2cqrfxvii.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2skiwemnt.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2kxzapeeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxnjnkib.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2wgbvxogp.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2bsbvcqqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nujzuphw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2bbyqaxkt.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2onofwvsb.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2dpydbrtz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2suxixexd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2qxcqeldv.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2cmaspxor.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2hyshaoki.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2yzjaqegq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ffwvcynq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2jgyxpish.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2pyrwiwon.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2wwtaalie.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2adyjetor.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2puxhuhkn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2qjuvzftw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2qgaoqicu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2xbeclgdg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2jnrjlohi.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2lrtpxmeq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2fpxicncr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kpbysyqs.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2noojhtst.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ekmlfrtl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lyrnfyqo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2sqenfnss.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2njkswdix.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vsvczgub.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2gpmefbzy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2usocdvrc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wwvgqwhm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2capbptne.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nxmpkjlz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yxzxhjyk.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2alayznlh.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yptnzyld.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ibgtibql.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eemlmrgx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2hfzbnxvd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vpifptxi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2hznnqkcz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2aicdxlxm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jazyaokg.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2ffdcrfal.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lkdibohn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwnufops.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2pbzvomcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bihqgwaw.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2nifzwewu.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zsptvnbz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2wkijultc.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lyxjoacp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2zhhwqhty.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kodlxqnz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ifcbbnsx.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2mzjcdqcb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ydcumain.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2coihbsch.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ohihcnsr.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lcnctmhf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wjviyqni.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2mtargntr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fjvcnbxf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2qvuvbugd.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2kbowryfx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ounujomm.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2sohjaazx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2copbxvll.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pcppsjaq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2laobxlga.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hvhzacfg.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uddxpdcp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rnspntwo.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2tzakycte.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ziihvewv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2saxtwcif.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2sjogncyo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2gdgpqasm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2bxptcztl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2renyxyvt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2cvxidpcy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2vlrtwuvm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2orjeyrze.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2cyildxvx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2nnxcpeln.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2opwkjlzn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mnthxniv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ixnepaxe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ldifrbwf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nogndyps.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qtxskpoc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rvpmnkfc.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2oagqeiwc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2oofxwues.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xentglcq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2ilivogqq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2sqdjbwhj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nemlnslg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ndiieyiu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gdaycbyo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ecosqwpy.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rvbzpbzu.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dvxlnijb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rmwbuxyz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vrnowuzo.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2futfvpko.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2knwyrbxc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lqgmwndg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2tccntlux.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2foljeupl.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2bjkqwsmy.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ximjfkje.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2puucdtgo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybonarsw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ckhrxtap.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2rrvflbjl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2psrdqdtu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2donyftzf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2joamyncm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mseeymvh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rgnkbyvc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wsfdpksk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2veyoksmm.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hkvhulxj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hwiwotht.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mauovekn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2fmewkymw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2qwprnutz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2raselgga.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ycophfnc.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2sirgdwuk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2lngncscy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2grktcpqy.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vtybpztc.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nggjgsxu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2vjfmqinv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2yyzvicek.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2baqjqquf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ulofzogb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vxdanewu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2kaesaynp.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2okzwwaba.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2qbnwoubf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nfljlflc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2kwvhlplj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xzynnqqb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tgryocje.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2dhmuigvn.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2cwediscx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2rxhqwgkn.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2zmlmljxq.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2zagqqykx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2awfkpjjq.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ohgnpktz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2mmondayd.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2nsoruqmq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2mrdsdbss.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lulkbwwc.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ythsyxzq.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jrkyzwaz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ulpwjtuz.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mdercwgz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uhwvneun.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tioffckd.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ldziyiay.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2boqjikhd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2vxuxtoii.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kwgrguls.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kpbayecl.html


<!-- 参考信息 -->