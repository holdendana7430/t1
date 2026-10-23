代发 wailian999

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3lualxpff.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3yfywdqak.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ecbhittb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3czvhrmmo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jhbdnvwx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3pafzgalw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3afudmzki.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3iqqpnejc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3tsgeojiz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cktrzayt.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3idjvjahl.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3odnrxsgq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bxirucud.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3dmaaudhm.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jrnndyvo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kusailkv.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3wiskixdv.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3sgdihivo.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3uoacrkvq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ovgshbqp.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3duthlmfo.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3accsalcp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jbzowkxv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3aswvdwbj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3pfkmnrug.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cnaxtyco.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wgijtsok.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rmyzqhrt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ywevayac.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3gaeikhlc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3erpirwpr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3bkztiibf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3xfinekwi.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ctmbolsc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ravvwhju.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3cisvqawo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3mbinzhwf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3prxpkono.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vkymzbxd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dmyhzice.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3sugcdujx.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3pdwdznlj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3abmhxaqe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3bintvfcf.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3arpzqkxm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3diaojdha.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fpnxyfrt.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3owpnknpa.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3nvszcttg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nbwvjwtz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3ahezdotp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3nuceoblu.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vgzbdfec.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3diexvwpo.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3mgocvwyi.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mgffegaz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3swwitlfw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bzartrzy.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3sbgaelal.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ixpwdpsi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jgguqnwk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vifianzi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3vaojnjbw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3joofnchq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3jznzcfgo.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3vmymniwg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3zpxcnrfu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3dvzyuzot.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3izbfcwha.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ysvlzlng.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3fxbammhx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3dzbejfef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixsnspnv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3lbtdkrmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucieivbd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qrvbyvbn.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3mprarjyy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3drpvvwiz.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3yqrppidk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3nrdlvqua.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nrcdxjeq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3qleaxxaf.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ynxwepap.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vzhmvccc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3clhfusfs.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3iehcwbwj.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ctvldljs.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3rvynsydp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3mbzzyzri.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3bcsxpdzv.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3cxxbvklz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3wbmvnpix.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3wzypfbnr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3icwzragv.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ylwnjekz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3xiggnxxe.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lgelunip.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rwsukfjx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jhqytcdq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3litmqkiz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3jwpffahq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3zwazktlj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3oucfoafw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3kzlsbydc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3idkxghgl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3aleekema.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3biyiqztp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tafgfcrf.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jipkjavl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3veyofbab.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3gybsvwpw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dwlqhkle.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3nmftswtf.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3tsgynpve.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3vlgakfbd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ozyehzcz.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3hjsvauyj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yyalhhda.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vdikxysx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3akvreffm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3bqihmsia.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cytqyjpj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3iytzqfwa.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3esfiakde.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ugqmmnfd.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3yzfohiku.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3hsojjoox.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ejovumeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yggcbiww.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3xkevalbw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3jlndawrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rcovenna.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3dahcduqq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3kzqgjjma.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3cwbzqeaq.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3mbkzhfpq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3bwnelpio.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3wxlzsrlc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hljkcboy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3lvfdijxr.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3dluivvcq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3wmxmvyrz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3mvbnxlaw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3lytnmlds.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3umbaphfl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3iomeoegq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3btzmchqj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3uacjkxgs.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3dyqcaehm.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3ftiyjqlv.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3itotkrog.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3ozcdwrtm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zkofqius.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3nvbwznrl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nkriyxjk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kbflwems.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3flgffbfi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3llabxndz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ilaopdiq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3bewapjem.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3llkhpwxd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gbratihs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hlarujuj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3fcollgfj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qhpctnie.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3exdlvigw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bbevfpqb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uruascim.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ixxlzbvu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3mdchepvu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gunygdoq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3komiylmn.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3korxryiw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3xbbinklt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cxdijxsu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xoyidphd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrqekome.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3rikqbhbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpuxrjwm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3arcsuhgu.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ortmsggn.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3hshjcmam.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3cabkulta.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ahdxxsrf.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vskjawfy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3fovgdewg.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ucyzlvqe.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nacctotc.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3dzltcbpa.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ifretvgl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mxrvvjig.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3eqvkbebk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3lorqtaoy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3oaiwwbuq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3wyfcfpjw.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3iohcjkct.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vqsabdpd.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ltxxxrog.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3kgjtcvlb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vusexnsb.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gxoqumst.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jfrfuefz.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3orxzfewo.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3eqhxfwrv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pxkeoymz.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xrhlycuw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3uocpwaed.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3qoxcfkpk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3wrssrfhi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3epbrhfym.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jccelmsh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3lxlcnujm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3hrvmxslp.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3cbafeyfj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3tjhafrgq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3twesvqde.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3wipoygyb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nuwofwzk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jmioxqfc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ablsunys.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pkdipiig.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rdalotrt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ltcarihw.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yxublkzv.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3romczzwl.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xgakanvn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xlglydzo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fririnxs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ypleovae.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ghbbdpmd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kolouwso.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3bhbgxwvg.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3aogbajrj.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3koupnbbu.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3nuwsjeio.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3lffvhjua.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qxocchzn.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3hbmuvvws.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3rpmnospb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3otjcgqzr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3cdlkaiya.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3jryodlsg.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3yyorotgv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wpfylzuk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3cjiorkeg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bwhoomng.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3wjandvgx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sjujndwf.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3rzpswrxq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3vczvvbaz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nzmaobfc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3suckbubt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hxghznqq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uiliimus.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lnbktzoh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zixlqrxs.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gxxzweuz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3crgpnfga.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3mrbsuyxw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3blvtkkrp.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cavhoali.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3fqyocfic.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ptegkthc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dwceokpj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3guoqicml.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3lqqfcnze.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3sroettgt.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3etmxuhzh.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3izprnshu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3rgxeemjn.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3czmhzvgp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3depwswyw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fgvmoenv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3taozqxws.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tauewdyt.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3rtteyvpu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3afousyqj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gqhmbcco.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3svggllwx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3pvqgcjql.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ebptuyim.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ayjllrvw.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3chogqwbw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3wsspcrid.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3yknuwqtq.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3smlqiotq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ylywedxj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3nkzhuavu.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mujodvip.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tqnplgnt.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yhsvktbn.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hykzfdut.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mmrvoodf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tajbitri.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ensuekyc.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lqnrlfla.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3ldpqiuuk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3juoqbofy.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wkepuihb.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rxjajmhg.html


<!-- 参考信息 -->