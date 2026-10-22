代发 wailian999

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ibpjejhb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2dhsfnwsi.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qajmbhxd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vivqxaxg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ftqjskua.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2iiipvktr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vbtvuccc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ijanyihu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2niomyyuh.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bpekkocn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2xbzkwido.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2svyuxxfq.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2htequgzk.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jzesfijn.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lrxsmmtn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2yakjibmh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2vonyxlul.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dbiigiav.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2qwfkffbe.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kghosvwa.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2uzlzaljm.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2eafaxjgd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2nekiwigy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wvfducwn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2powzigmu.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2bimrrxfi.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2yxvtrroz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mxqpsygh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2cugmdytq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2xykptcce.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vxbqdmrp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2cvsqujyn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cntszsbv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hjivthcz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2fwmklaoj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2unvahxps.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2velwfalm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zbrlvgeq.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2maebshxu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2dalchnbn.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2ygootcpw.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2iixkavxc.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2amvohrso.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cdtezfue.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2sgotfbpf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ympfpfbo.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2vbxztxcw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pvmnpgpx.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nxdnakoo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2audfimtq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2egbjozxy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oampxstl.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2emwirbir.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2xvbhmydi.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2hemuclgy.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2gawmolre.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2tdhwxjbr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ckpjpejw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2zzjcwvwq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2emgfcuku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ruvdgzhd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2rtjfebel.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhtdcerf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2yrndpajw.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2mnqbyyun.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2hpmavcet.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2pribhnqn.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2fyfeydxo.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2obsooizx.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2clmgkild.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fmybhria.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2dqxpeytq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2nywizfop.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2agkwqmcm.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2eopceqah.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2hfiywlwc.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wexpybcp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2mxpoowyg.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2iaamibrf.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rrodsbln.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jtpqqlqq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2genjwmfe.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zhfeismp.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2pvkrmglk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wrxkdfzg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ooykoozj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fgtszyvr.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2srivtncm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2rvtifjfp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2nmyzerrq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2odeastqa.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rolbvocn.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xkwpuekl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2usqhyihb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2vaghhmqe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vdbztgvw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ejhobrna.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ilbojxwy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2apyopjbv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lvlpiinw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2osuphkwl.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2rxszszzj.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2fgfsjdne.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2uvarmbgj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2vfbavawy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xbvuwdbv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2cialgoto.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jorvdhmt.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2mfdhyaml.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xivlakyf.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2sslrvivz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2iwnfjeun.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2udyefbjk.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2sbuaylkg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2thoptcio.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2kqvmxhwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfmgehth.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ttvicewa.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2twajhrhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2weixlkfx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2lrknavkr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2kdzlzhxr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2cojksgpq.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2yltjrrhu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2azoqresy.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2jmjilecu.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2wgqhjrgl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2wumdlydw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2tmgcxwwd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2seimtaot.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2cgumwlvv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2pocstuyt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2giyhmgtx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2qirmnmny.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2havqvgtc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2nylrmyhi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2fofpsokt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2bgdslktv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2msdujsba.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2cbzjwtvo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ocuiprrr.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2gjfexfbp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sjiyspol.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2dtebyedj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bmttzwhi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nbktbnzs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2xhvcozex.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gkmtflxn.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cgfgholf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gwlpxwuv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hmauielp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2inpnwpho.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bdizsjtd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kqpsrlbl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rjmibcqa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xcxaqfyo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ystynwbz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2snrwfxto.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gugnwvgw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bqtrfxvu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vhwdvzvp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zubbpaay.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tjttlowx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ikemdvbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbfyrrjm.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2fmdiwxfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfpidpek.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2gyzfkrsq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2menoguod.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2sfxuojjf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bsbuvamg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ocwlnchf.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ldbqsthf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2lduigwkn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2uhqxjkln.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xzyiurka.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2bocipvyn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2cpggwagv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ksmbohwb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ydfkbnfb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ouiesgzz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hneprprl.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2grfhujle.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2ozjjgrgu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xprvdxip.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2yoxhqymu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2vlnxzbsp.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fgztwqgt.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2elocsoib.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fjxdkqoi.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2akumosbr.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ylrwyyfr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qfngkxhi.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rsvyxvpa.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2rzukcnmy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2mcntltkw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2nitfsvwk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pihawhlp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zjztwnkz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2ofyuszbt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2amcgqlxs.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2crmsdbkh.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2pdhfdoop.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2mldfhdyd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2piowjtnc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cyllkbak.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ugrdzgxx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lqofeqcm.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vaslexgm.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zkzteenj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mtjuuufp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eaxhnpko.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jkfavrsc.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bwtlbcuq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2yrhhphlh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2xxlhzjsy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2krgluqpn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2tbxihses.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2hfppsjtv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2uoowlskr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tskaisnj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2zzweduda.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2wdqizwey.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xicbcjmz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2mdiykqnw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pculowbq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2gbeycupy.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2zfesjofv.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2bqoufgkg.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mqhydptg.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2cdvsgbgv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dxcrtfra.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2oodhdiiu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tlzacvya.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2vttbkbzk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2urylesee.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ldjdgaon.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2jjsrqmtp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kqrsgdem.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2etarhrar.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2doddaeax.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ikzrwzzu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qrigbmyk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aptkboyl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zznteezo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2fnloifui.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ghofmmja.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aaxlrzwo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2snjbxjng.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2wbmwrsrk.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2eajgswtu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2qlwdzwmf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lkpuhnnm.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fggyuznf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2wrrlinst.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2atcwiatv.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2lflrbaki.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2uipvroht.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2dlsqqemu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2favdbpwm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kkzextcl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fflsdull.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aczaqotk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2aarmxnsc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2apxsvjre.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fgqixyoq.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ddsnasar.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2mpbwplzm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ffmniukb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bprhddsj.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xezzzftx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2zuropwzb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2eenfocfp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2esbpecxe.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ojaxeklh.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2drgcxjvd.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eyumbwht.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rzgboqzx.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mymvwinr.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lrumgcol.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2flaqbgph.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nbycauty.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kqakzvoj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pxtxjzxb.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2iqkrpris.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2lxjndiig.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kduyyfmg.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2oyawujaq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2clwglvtp.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2esubxzsa.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2vwyrrtfq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2fxfftkne.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jfakosiw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2dpgdffgz.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zlogoqcs.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2fzulxbgp.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2imtcqfpv.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xrunojes.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2udnqqbia.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2xuzeasin.html


<!-- 参考信息 -->