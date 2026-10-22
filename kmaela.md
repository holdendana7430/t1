代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2prsvxfdw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ymfddiuw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2azbabdlq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2egupkowy.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zldhhanp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2lwvjubrh.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2sccjxmbq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2wzxcildt.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vltapofd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jyuuwmfb.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wovhaqvl.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qgtbraqj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2wsrviclc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2nzfzwvoj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uahrrpsn.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ncnvvqnx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2royintqm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2oqnfknrf.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pobksiyp.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fzqxubsg.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2iqwrkvfq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2bjfxzyrw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2mgvgvmnz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2okiqxxis.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ibhqupmf.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jfslyqey.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2gfrwozsg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2lfkegpla.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2bdtlxrss.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2veyubibv.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2tumblqjm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2vbfoeqwc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2gaudtqef.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2kobvlnfv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2tcgssaqx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2bigyembs.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2mybsdcgn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2htpfaelo.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ikulqfxe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dolppean.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2dawkyqzg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xsgrrmzb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2aeliyaii.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2kuwnfzfm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ttdprlio.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xfygfcgs.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2arqljdny.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rfmsrrhi.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2tvudlsig.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yfhksygd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2czayhuqe.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2krqidgjw.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jfwbbpyd.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2egxlrcgl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2iiadtrvd.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uukbhbui.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2akxdxrmg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qdbfndxb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xavnseql.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bsiqvorf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2gubuform.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wirnebtg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2htmnczsk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cejazljn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xeykckab.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ybnmpyrp.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2hqjadsrq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2hnlravqv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2oqreekxu.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2ykldwzol.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2szbycnqs.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ntxmnwqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqpxgdkb.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2conjklvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbpoctku.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2lrwbpiir.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2nszpaobs.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2jyuhxswo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rngrnclz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hjdunhwi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2twwritwo.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2dlkrzghp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gvnaouno.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2rkojnsyj.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2xirlziyo.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2ozeiwaxi.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2rzjaueql.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2uiswnkks.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lusasmye.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2nauttkpp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2oodhlyra.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2owzbmidp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jbgsooet.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ugwfyzys.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dpljytko.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2wdjhkdko.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zepxlcxk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sychdruj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fvxcgrrd.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ttccusxc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2lyscrxka.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2aopqnsgv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tafrjaxr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2yokgeylx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2opiwezxl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zpzkbzkh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rhbjnhnc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gbrnyahw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wdlnpotr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2yehpuris.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2uflqxrpw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mugfmizo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2espiudqc.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2jjurgazv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jxfjljyp.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2mtowkfis.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2upufovzh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qrkhjutw.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nhfzilki.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tcujsfau.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ftxzjyvq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mrqcocwp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2olnovwqe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2jzxxitzz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2hqlqqvwm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2wzrmjgnn.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2ajermugq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2jnteyave.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwyjkcrb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ndrncuzo.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2mctsyvax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmdvtabm.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2lgrhfikg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2cfhmuxjc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2wblguche.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2rsiffbux.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2fyabuktp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2xfiowadz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2bhfqjfpe.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2nfzqrcng.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2avcxlxvl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2agsmcmpd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2jjwdbhtk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2qhlpcmhz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2jmpnymwq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2sxbagupm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2mrqdvinu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2hywnhgyh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2unyszwjf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2byxhmdbm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2yfrvokht.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2uifasauz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yalrszni.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ogoqhebx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cjdpkpvm.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pyoqnqcv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mehatguj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vzpckpjn.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vkfwpjqx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zrplxwal.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2uvhtnkwu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qecxicaf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eqtewjpz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cteiaejq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gycrtwwb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2phwoohbd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jebbwhyo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2clqleuch.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2gbhkwwsx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2msmycvjr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nprjlczm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pyisyhjs.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bzgjynsn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2bhgccrtv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2haekzric.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2sqtthawf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uygkfein.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2hjuylsde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfamilli.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sggxwddg.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2zeolezet.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2ujmmdkao.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ixidwtfr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2lsdfdtls.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qxgpzgrd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2awyyxgso.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2hlcotyze.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2sdlolatz.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2rllibldt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2zpqiyhgg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2icbyhvoc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ujhxugux.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2selkaptk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pvefpzcr.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2dicbjeew.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2iiafwiie.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zzwwjeca.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2uvqotbez.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2wnbcrabi.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2faaxzrot.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pzeqwjxc.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eksrmcxa.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2seachnis.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2lfqcioxt.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2alaefgzu.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2layxpfks.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2jmlxnczy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2eoppwdmd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2lnsotprv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2stnbtkcu.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jpyansvw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2nzrnoxiq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2svkadjnf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ksxjywed.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2rjwmbfha.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2pfjffipq.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ixuefuxb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2axvgilqb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ksfofgjf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lnevgitk.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vddpbnie.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2miyrqdvw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ibfhvnoz.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2iogrmhhh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2brqokwfq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jogxopgh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ggbcpjxy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2bbmleuba.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2djcekkfq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2uyttjoxk.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2eocknvtq.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2zipdezxq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wktmkbcs.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2jcxmyhqq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2kdzaneda.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2njeyaayr.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nioxfglu.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iobaamyg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2zwaeuogq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tuezrhcn.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2amvmkmjm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2lduliygs.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2dqwjpmke.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2unudyjde.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2lzeerddo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2iecoafue.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2gltrjiuh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2eiocmynf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mnuvqnpb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2usgcfcyp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sswtxmqo.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qtoxurew.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zcvtdnrt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mmdbywwz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nppcbrym.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2phzqdlaw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qksrrxjy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2wekuzprx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2jkfvnutd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2byxvwpio.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ufvyvnjd.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2kixxixgg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2svbjglrj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2efadqkhn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ocbswigk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vkoipwkd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2iitrvnbj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2tloeyzxn.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2dyakcepk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2mwlwnyon.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vmasdzqh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hlerxrig.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mggqyehu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zohzoqsx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pyptyfjh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2hbndyioe.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ievognij.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ufviqzpn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2ncmrumee.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2xjspcxap.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2dspenlnj.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2vujosqpi.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2bpejndyw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2osgldnwj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2vzdyskxi.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2qceikxqb.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2keuboyzq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2raskhrlo.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zqjtdoww.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qwhevefe.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2khshjtla.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qgwqnvpv.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mwynqouu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dvrnptnu.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fvyfoxao.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zleewozw.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2wuvtqxhq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2vlarxjcy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uscexinx.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2qhsxubwy.html


<!-- 参考信息 -->