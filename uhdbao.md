代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ywhcetpw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hsiwrdqe.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3vhapstpv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3mzkartmy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3kkvmklfx.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3xgcapxwn.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3casfxato.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3qswxghrf.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3lphqxhux.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jnbotvyh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3eqaanzvv.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3cjuijmej.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3jvjulfto.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gxvcraqk.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3wcpfadqs.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3iecjvady.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uxjwtzrj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3qtqriwif.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3fiuuuhfw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3otpkzvhp.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3stthkthi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ahxmnxhg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmfppdar.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3empzaftw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ezcnrosw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3rxdowlck.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3iwtlbxjh.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tdnbjvoj.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3nrtslbbw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jpqacxix.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bprwgczm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3cznkigdy.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fqlkbgay.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3kzgjxide.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ilgrkbzk.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xqfmahij.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3rwnyffcr.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3hhapkoqw.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3kzarrstb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3dgslqzeg.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3vjmpfsrk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ulzfsjnv.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ftjvicaa.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xcwqcsfa.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3zqvqbtxe.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vssaggom.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lbgbgnqj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3rsbwolyi.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lngqcajp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lmnkwxon.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3iqbotuib.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3kdusalwy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3bjufukic.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qffexwbc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3kxgrrsdf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3cggolmth.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3uwbllmjg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qhcmjlwq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3jhehvtas.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3perngrjn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3fttkryby.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fslhcecp.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3qriihvmf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nvgtxvoy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mhgujjkz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3uznvkpgk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3uxwdqlge.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3abqnxeqv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3gvoqdfnx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3emaishbq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3chofazxt.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ywyutgac.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3lsjqcnrk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3yujtxath.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3osstjsnx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3vkiuggkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pfjsbpqn.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3wiiyspdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3luvjyapc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3gbgubxzt.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3awhpfnnk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3nhsvvbgc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3qkgsohin.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3pwsvcqay.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fhixvcnk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3cnkbynob.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mrdsxpir.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hyrellqy.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3gjjhhlvs.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3arbimnyc.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3aapcoeqy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3htlbiiww.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qkdxlnvg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3stofllwn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jzaylzst.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3pcwtigpd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vomarprj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3helclsxk.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3aornuhlm.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3jjklvjgc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3qakkaaqh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bdypvxvw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3pdtrkznq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3sardsuvg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3yunitlzn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xhqmvmqu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3iisunoap.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ufgqalsw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qxudwrhu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zjxelboe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rnbasisy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aenzxezg.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3btdvfbcg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3egefbkwx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3qerlkndx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nlhgcwcm.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3rqwzxurh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3dcumfgwt.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3putnhzsd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xhqtzmir.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3frbgxxuv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3stoswgjr.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wddbtkng.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dygysxhe.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3bzcrsvnr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yhumrveb.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3eksjbcme.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3sutxwolh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ifavuxxs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3xrzbweow.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3zzxfflwj.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3jvaqhgdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywunldhk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3hnfocszl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3nzchfnrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kweabtsi.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3olgsjtdq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3igcvdrlw.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ogcaphqf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3gcrjhfmp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3jkqpvphq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3kznzfuke.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3nlgnazmu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3pbmlseke.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3djkxxfeg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3hnkcmdra.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3lqejxlag.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3tlrlqpcy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3qypxkrqe.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3aynfrdgv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3jqzonybh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3owrmpgqv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3scseerku.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3rwyppiqq.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3uzmcjmvo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3vprndeuv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zyncfyof.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3teibfzxj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tunnmbhl.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3dxlsjtpn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dgwnunxj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3apvzxekc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3osvnukyw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nxngmxjf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3cpotxfyh.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sgcpxbzd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zlnhwogp.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rlbtqfyx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kklzterf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cqtygjoi.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wefrikot.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uimgiwdp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3fxcspffw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3babefvxn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3czvjlaqb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qtdibmkw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3chdqzniv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iyzgrupk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ioazurwv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3xhvdztoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzmgzgcb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3hgaycqpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3taraxkob.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3nxabpjvm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ozoeaijz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3okdoqirz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3eyofimvb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3widnopao.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rzspacxq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qcglrpyx.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3gsplvylh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3bblftwov.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3uzhqekva.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ydbgffrj.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jsxtkecn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ohcvlgje.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hubxpixj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yeauapif.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3prkhiyyn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3knhqmmqx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ayeoyhmh.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3faqmsqrr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3czgbrgdi.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qrqkufdk.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zwnqhepy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yuugbbgq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gwnrghkv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3tkvshnqy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tqlqxcsg.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vatgontu.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bhlmdcfo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3jqzjngjv.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3gkvtziqc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3sdnulplt.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3gcyekfao.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3wfagxiht.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3xspynmre.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3gqvoivxi.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3iuppvyia.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3rdxpothh.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3pshkjpmu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oawovrvm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hbmyhqsq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cvjwrqju.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hbegnkie.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ycsnftrz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sodsniux.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3twxszlzr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3skeydlnm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3uwxfnghj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vlglsrgt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kueumfrn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ruykpdta.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ryucxmgr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3odvxzigy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3zveuwdac.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fmyesktc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3izstwsxs.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3itllnbzq.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3zjufbduw.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gznxeyxu.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3upwprlya.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ltswsyut.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jxczlduo.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3kitbpsfr.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rexisupg.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3nymotvju.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wanwrong.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgvejdrn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zvifrqbx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3udnrgikc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3iazmdmya.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nzejtcrc.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3cwpgghib.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3koavxhva.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ioplyypz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zydsfpjp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3podhzwof.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ihszezur.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lfbwhsmo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uzccgurc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3muodebjn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3dkybhzqv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nescbzsv.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qvfpckyz.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3jskilhiy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3pmmootnz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3eqmvjfvr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lxixfess.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zhqnbobx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3xafftwoi.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3svlwhrrh.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3wtwcsmgh.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3jdenouoz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3tljiyjhz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mgaoftqa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tivwfzah.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aqkafysi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3tlacejcx.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3bistyyfl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bhbqvmsf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wzogabxn.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3yrnnhaui.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3xunnmddj.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3xbddpkmg.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3sbmofpkk.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3deepyify.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3akstfkcb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kqccaouk.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wllyddkf.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3bwacynnd.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3fddugcqn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dapskese.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pbyjxwgg.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3epztbsdr.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ipahpbmx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3utdipgtd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kwzgsmte.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dwtbqjru.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3armmybhh.html


<!-- 参考信息 -->