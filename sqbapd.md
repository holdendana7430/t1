代发 wailian999

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3vvrhbczw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3sfkjfzai.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3mgpjswbf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3vqgcnair.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mmnrqlsf.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3tdayitee.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3lumwrwxu.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3utoicdgn.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3fplzvnab.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3otawjrda.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3qxwefmjs.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ajhbwcbn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pqitkccr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ctsarxqr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3twcpotii.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qorezhjt.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uucmudui.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qxqoukbt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3xthapcis.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3fcrkflfs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3nkoujief.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3pjiyjpnp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3cznxbsmk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bxknwszb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3oihqycfv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3btmgnwuu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hvgkndwk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3edccuylh.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tbwddbnl.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ngqktmlg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3fjfaxeqe.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ccctqozo.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3cywxfiic.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3fyqewuwr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3uwbvdxdm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3eodreduu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3uyhssqte.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3qnmhkvfi.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3uowrlvjo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xzemazwt.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3oxmuukpz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3nolvwrig.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dpouygau.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3cwrxfjdi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3quseejzk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3sbzodxas.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3jmccsqmn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3agiaiujq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3eynvhfhj.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dofehxfw.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3fnpussjp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3lqxsagdo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3okljxqku.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3xbsxivgq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3enamucwp.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ztwupqlp.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vbwmtqoz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hgsfwbmh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3zdeeemgo.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qgvsphwq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3pthlqgzn.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3rexepcbq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ehemlnhs.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3fzuxlqgu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3kckablcw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3fkjohmbi.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3nbanzzvd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3kdxnnrqy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3cexavkgr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3hyuanvji.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3euaqrtjf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3qsnphull.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvvgomun.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3epfzidtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bfbjiuar.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3bqptamej.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3wxfjpmwb.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ybqgcsms.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dtsxlwyc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3fwhfgdbj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jqamvqqn.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xhdxhbds.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ugxwobjr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lolykwzz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3lwmqlvyu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ateufruw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3vhmohswy.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3lhchbxoq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3mtulrbjr.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3fqtrdlhi.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3xmvrxbgm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wuzqsmxy.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3fqevxlnb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3doowucuj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cpkjixqy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3hchxlxwh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3flcoxfxi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zelmbhhq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3sbprsmzj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lowlfuba.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ecegegty.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jtozcidf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3evfrorsm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3bavdktst.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ljhkoqwp.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fnumybpe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cmovvbhe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xkcsnygn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wrtwzmze.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3irxudxux.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3didahbfd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vcyzqpyo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3aflyexzh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3iqgauxlb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3wyxlowok.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3gtkmqoye.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ulobcfnw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dpxuihtx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3bbogdmgy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xvfkkltr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3axqjuxku.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tldxsfme.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3sosxbtwp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3dywombpe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3xdnilznp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3oqckiodk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3dqslmqry.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3nxdcmlpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zajqecgb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3upysfsoq.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3eezjbumc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmmclfko.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3bbwxfyme.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3qcteehvv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3xrxbuish.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ffrklbtd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3orvurokh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3jbkhjswb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3mcfdhozx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3raxrwjye.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3nlfdaluz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3evrykxoo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3jafqhvry.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3xyixyyfu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3chovurvj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ifhumayx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3soayaxql.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3dkjawwql.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3exwjmgeh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3bamvaaww.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3glsbuprq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3rhryfcsq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kfttojhd.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3xjarkycm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ytlcmsfg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zertcyvo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3btswtewd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ljdhuobt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3flmqztko.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zniimqhc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xmujgxgb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jsuaatkj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rtahhdat.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mmolnjaq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jgmnknhh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rehidank.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uttjzydp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tuaeqqba.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fhvxmyut.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3njwtdetw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ezmwhyyw.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qxhbdfoa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pdcekbjk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3ashtvcgx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zammuord.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3khzmpmkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlwqwrnh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3futhhzsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cljylqap.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3afnnmhjl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qohkqhlk.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3fqraalxz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zyoqatsk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3sqkddbxo.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mymrcqbd.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3tahyyamn.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3zqbampwa.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nrvnypau.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3cxqykoxr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3zcglpknh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vlooosgu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rjbvilrh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3xewkdbpc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xbswwdja.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3wgswzqsd.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3loiwspru.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hhdqfdmo.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3lokjacjo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3uwxbfhye.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mbwiykza.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qwopblrb.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tlxxiicf.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fzrzmbke.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3fuperhuv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mojbgufb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wkfekned.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3gtqhdoek.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3vwgkhotg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3upcpnjpi.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mwhswgcf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xtdxxdoa.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3tbsfiwtn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3xtrvmuel.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xwiintzv.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ujoqlpvu.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3hrngarcm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3cqujjwmo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rctuebsn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gasrooxr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nptsujto.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oqhbjimb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wxgzcvdr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ufgtolrx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xslxexyr.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zqyajzja.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mqamkwpf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rcczyiat.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rorlnyuv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qxhbkmow.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3duaalfba.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rsjmbsqy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3mpaeoqdv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3sdznmrrx.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wavpjndd.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mjhcuhke.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ajsxzeel.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ofnpignb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3psoqsfmi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3kblaobsg.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bfymxzat.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3vffazruj.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3bmmrxghq.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3gdtagrsw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3etpiioof.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3rrakwtvv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3brwburyp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3srtubyea.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xesfwfpx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3neptmvkl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3acpyylaq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3emksvtec.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3uobdvjzb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfgrfmnx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3efrkspis.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cftdmyyy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lxlebcpa.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gngpvbfo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3gmgamaxd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3artdyssq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pcvmhwgx.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pbvzxahb.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3avfnmcwi.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3liekrilm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hecjdzwc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zkcglmrk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dalbmjtn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ialdnmhv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3jcbtudbl.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3stfyqtgq.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3faxgmzml.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vnhgizdf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ansndnob.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yguazwbq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dvezuusb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qdllzgyp.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3xakjiajp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ofhbelaj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3swljthlz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3uhqinfme.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3zxkhwyit.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3fdnzazqv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jyrpwkdg.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3llwdtseq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3noyizcwr.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wtykpbve.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bdmdnkso.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3eaanfptf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3inzlirnn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ysspgqee.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gqgcgzpm.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rsaohmdw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hhozwqzl.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uxkujntt.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3euksctnw.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3caibkakb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eqotyggp.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3xzjkamla.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3qifhcwwp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vklsoama.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3uwipqvum.html


<!-- 参考信息 -->