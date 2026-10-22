代发 wailian999

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2wtawyetx.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2flaaizgn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2bqnswsxl.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rzublzur.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2nmgddspa.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rsthupez.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2xmtqyozb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cprcryam.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xfstimny.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2rmivmsbw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hgwgqjqt.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2oedffvxn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2dzdthcop.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2lpapyuim.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qzvkycfx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2agxijiki.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2gwsalnwt.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2qtfercxt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2slsplqyi.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mmjwhwyr.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2clrrwebn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dgytebon.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2plklejib.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2zjwhmpvw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2nqqdmxfe.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2cqxzwkhu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2clqvmcnh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2gfiljmrx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2fikrwxdq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2blfckdst.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ysnvdpos.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2tgchxujf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2sffzwdxa.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2geelbdsf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2eeqgcrie.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2svbpvmex.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2zbkziizs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2eowtcuvj.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mldzsbzk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2owgdtdmi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zdbekbhx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jlpttlcl.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2tgwdyuot.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2gdfgtsnh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2omqljomh.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cpxaobuc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2qfvokzhm.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2iozwfnop.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qckppngq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2mkzknpjn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2auzhkrxg.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zgzscdev.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2riwinkuc.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2goveaucr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2iplmzfcc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tmprhdyk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2lirrtmki.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ghwgexgh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2abqdgqqk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egqowsan.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ewwgwsao.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2xiopsbru.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2dihsbegy.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2takbbajd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2oaqowzis.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ilcoszak.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2advmkcgf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2cxmgzkcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ienamuwm.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2wamadleo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqcpcbqq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2bfdjhcch.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2uawucvns.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2xnaksucp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2whcbfwdm.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xvrrpuei.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tokyedtb.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2oyzagijv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ykznddmq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2uoscwvbe.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2vckcfuqb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2imijokxc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ydqreies.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ktwfjiyd.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2fvcbfzpp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ewdcwber.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2buylnhts.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ipstvnno.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2aivkouvd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yrdanzpt.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cekoatxm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lpqvelkv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2cnccxery.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dveydunn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gvovycct.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qckovnww.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2lzzuuzhc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2agqoflcw.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2vivtqlud.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ulycbyns.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ccdywixp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2cngywjrg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qiqnidbz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fxovwwld.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2pgcrdbce.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ncudaton.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2xjkwukxz.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2htbssxts.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2iolggxgi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2xmxrdhlp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2irgfyfrs.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2skdacqbt.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2pbhgqfzi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vkijsmcf.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2uilaocye.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qeounylm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2oynepzio.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uabapksm.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2kzvaerdb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ezravudi.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2xgqdwsac.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ejkbwfdm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2swqeagfk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2lkhixtfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpiblmxe.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2ucdbejhv.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2ftnzzypr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjlfytfs.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2pflbbnen.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2uywpzmbe.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2opaqnrdx.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2awedqrqn.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2xxfavsnn.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2dnavjahi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2vyghhjhd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2kxahimis.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2bmntlifi.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2zvusdlfz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ksbylfww.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2bazijkvl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2zkotbjom.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2tllxubru.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2zvripyzq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2qivohsrm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2izutituh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2zuxqqkle.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2qkxcjqzz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2qvymmauq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2bwygngce.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2ujbhkopb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zsooazhe.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2knhdcpyh.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2qknfexqd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yunfxupp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2dxomngtz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vdfokfyo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2bucnozhu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fpfmekle.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xlckbnxz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ihfggdgt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fsjjpxfc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2inecjtrp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ttvgnuvt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tcvwuocf.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2stcdacdq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ppyqjwvn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zwdxzrqn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2xbquhgyx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fgzbpbko.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pffaqduq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2uprmgsam.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2kpdbstcs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apirwzln.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2nqgrzzzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hazzcdtj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2owlsdite.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2iozgijhg.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2opjzrihw.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2cwhftykr.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2kwbowdxv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yjszculi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rxramgyg.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qljloczc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2htmrfstj.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2qkhmesto.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2mckyjpln.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vzspdzqn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bdymhxsa.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2jlljtxby.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ijljrkvp.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ucbmpzpd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2dptluhxe.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wehdbzlz.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2iycyhbhm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2nxrnwfnw.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2uepnljlr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tsvpvafl.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wfhvviup.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2viizfcit.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2mjbalckb.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2rfiniekk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rdnjssad.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2mryqmong.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2xgdlsbpo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vonqcdux.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2yippczte.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2lfunobdh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2bkyaxvgj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2xrbtupkn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2wubkleos.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2strnrarv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2wnrtvdhx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2lxebngdo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fyaammcx.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2olwioljx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ocucsdyx.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kggoqmpg.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yshtprlf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pdlsoupg.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ebtqfyuw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jxphjyli.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uelcpcop.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2toegylwf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2lcvczzgt.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zsmkxtdx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vtyxvcyp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2tzmtfwtl.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2yasmbxwo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ofciavar.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2hxoqhehs.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2zyrnlxsa.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lvfpqdgk.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2vzhxkvmn.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2uejwmkcw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ksoxxoxe.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yhtcizff.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ukvkweuv.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2mnppsmxh.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2hvjidgrb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2eumvkjse.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2kvkzvjxv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rbsgicfh.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2auianzjz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jpsoesgt.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dsohyegx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2kzzodgvz.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dmdomahq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bmaduttx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ykpaiqka.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ecradgwp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2couyirbp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pnglzjlf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkuuzbxm.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2axwvwxex.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2emzkmtcl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bjksxvul.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2kpsfxgjf.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2vbwllqsh.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2wsyqpzlv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jcvtushj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vtzvkhqh.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2cmjpemgz.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2mywtvzjv.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2jpvldwnd.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2xqvctdlf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2kgechyxx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2usbqplus.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hztjqsrg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lzzdmuxw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2txwzvpls.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2phxqhkad.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2vnaeagge.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2plhejnna.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bgdgltcy.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2iimsulss.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2xwcqdrcq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2rjymdrmb.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2dxkjtujv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2krcblpqw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2eypkpvva.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gljlptua.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2uftphxop.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2kutzptqt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2xozbxpxp.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ltpxdrsj.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hktnagsw.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2asjfnucp.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nvrjwiwz.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pwyaoqvn.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qrqlvnux.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bltrwqdx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dsesrqys.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2phbpiuao.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2sqhqfpfw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jmzqxgyn.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hqrcmaxx.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tvdguspv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2qaaccqar.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jglkgsdt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2hxulhbrh.html


<!-- 参考信息 -->