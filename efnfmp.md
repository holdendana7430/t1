代发 wailian999

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2xugstdnf.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2puekxolh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ecbwpytf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2sdgptcxx.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2vhjxvytw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2hzhltkkj.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2umqwblfj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2nrmfzdof.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2emeamsfe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nprhhibr.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2eugewjmr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2tirknkjz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2clretlwq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2usgpukoq.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2qevmfmti.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2fcxvmnbd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2pipruzte.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2kdfbgorg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ucrfgtkp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2hmtfxycr.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2dgysoqxr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uswiismu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2edzzvqcn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vuopegbx.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2dekylwnk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2cfvinbpr.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gcueaoce.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cnofrstm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tfvagieu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2avuwvxfd.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jhrbdczw.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2iyykxyqu.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2cnaroozc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vgpsoehr.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rhceuqih.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdyucvuc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2sczrssvv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fjschnla.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wqroleyf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2mbhxdrju.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2xdhusxem.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2rsfyftgz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2acxwmidz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2sugzdnmm.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2rntmqbcs.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2nbmggtth.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ufctjnpx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2nhsxtnrd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2mhdwsfbo.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2rihpgneh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ctvqtpvn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nowbbfom.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2eojfggll.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ltoisawu.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vwphkxeb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2licreydg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pronxebm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2amnofeim.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2lsmwdult.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2zsngobfx.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2vfpdkjlt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2apffjsvt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ptptmpqb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2wswuzsbo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2iyqmlqdn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2xmfqjhrq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2pcqgcgkt.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gcztqsoh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2acjynovu.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nbmoqbig.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2losnpofr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iovqzcod.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zlmtybic.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ogilpwap.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2ccgxnpnn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2psynwfoy.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2gjoyhumi.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ilytijqj.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2bszpemuq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2llqnkqrx.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2jujyyimu.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2lnbrrlft.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2fthuwpwi.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xbywkjzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nhkvlygi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2buematpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fmczassd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2qvxzjgmt.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2nikbmxee.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2icsnmscp.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2dxupjdmi.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2osjovnbn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gzaaupnq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2yhlloawf.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ettanmmd.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xkflmfka.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2grkmnvox.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2uebhggwi.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2osjgzjld.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2mlswjhne.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2idcoppwn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ztagwzol.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2guwoxmeo.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wbftugdp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jgwymrcb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gpmkhsym.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2dllsmsvr.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2nbbdbwql.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ddbxfcii.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ezlwwwrx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2dzxohbpf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2brwlllps.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ansdahip.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2shwholxc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cujqcphz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2kudwufae.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mryslalo.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2xjuakmcb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yoghllmr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ulxgrecp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tiebrrxd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jevrclxh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2cpnprgcp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fwcehylv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ecjzvekl.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2gisnacuy.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kjhvrcqa.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ggsrxmqn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ntemeynr.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yddqyzct.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2akhvzmpm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2isqfxeug.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2dqepwlks.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2esassaro.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2xuahzxim.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ixjesqnh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2gqlfjskn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ldcqrpgc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2njdwmhvl.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2epcgybpv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlgcjsfy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2hrrlvmoj.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2roacxdzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fmygspio.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2xkfsyrql.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2sqiszatf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2htmqzzuz.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2noafwvjb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2lduiyecs.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2qvtahxrc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2fskctpzf.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2hsanboho.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2tqivimeo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2wssxqwtd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2tkhrpmjx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2gecdriwj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2rquptbqo.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ayhhpuga.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2uiczsull.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2fmedeezf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2kgehvugd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2pxwxqxkp.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2bajimefn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2vbfiddgk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jschnhej.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2bgmengfa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2suznvisx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wfalbjpu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fnpnnvoj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yfoaeizm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ssfvpzki.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2yhphnvba.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2onwlmukp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2edqwhhsl.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ulhhnqsf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ajutsiyp.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bbgcoxdy.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zcxsvsxs.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hehcuoyj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iysgwmwx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2dycvltds.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2hfdewvea.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ahptuysf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qpukrnrt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2riqgoiyi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2afvcmfpk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rqdpqkpc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2uktbykfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfbohlwj.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2lgbhmrdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wixaqrfy.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2spqanwvc.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2hupvohfp.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2pnzgnnbi.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ykzrqtqg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2pqowebwt.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jguwmqgg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mxhjyycp.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2cudnclqp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jinmcahm.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2xuokawcs.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2mpfrdfgi.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zibihail.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tgpezrfp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ycsyfjlq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hhhnsmld.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2cxehesef.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2lgroswjx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uhiunzju.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2hojnugam.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2hhuaimth.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bqzcmoif.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tbnophza.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2abnlwott.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ghpyztyg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2nyeteelc.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rqwhkhan.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vxlvphti.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xlktilod.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2eihyzhdl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2zulhtnlq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2uugatogf.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wgkuccuj.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ytryshyt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2laqdfbyq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2nuqlxlci.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2wgwsovdp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2seeseavp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2rpuujjox.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dktjskjo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2eymsyfxq.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gwuqpazs.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pvuxgsiu.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dvdbjkpi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dxcxzvxx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dpqymlgk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2zcddzvyx.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vojhpymn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2lzfikpnp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2lsabxhfp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2kdojeyaq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vjgbiknt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2gyglqayi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2rzoitxdj.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wazexbmp.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pmxtlhta.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2mygggxum.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lytohcbb.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2lsnqfexo.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2fllshlqq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iwhqrexh.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yuyqshtk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2lfhniotc.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vkhzopuj.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2usntfoyk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mdszsraf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2pwyykanm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2omwhncuq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ywphdeba.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vgdridaw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gabluwcw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2jjzladih.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2aoqxcfee.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2movgxzbd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lleznfwf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xckdluya.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kmxyakrg.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nbutpnjh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xjpjugsf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2kqxwtdku.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2lvxifadv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xxncrkvz.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2pxcmqkbe.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2bwghvyvh.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2wlbjcesc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2slodjfej.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kehvmzck.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2puypckyh.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2oexrabwg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ngrngtxl.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2rpmpyfij.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2mmrmchtr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2brruxwzo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mbxvkcxl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jqikxxce.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ohtpcpip.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lcefqdgh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2godcepmp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2asnewciw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2inwfrgmo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2lmbuzdsk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2vfkioecz.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2rezzwnnr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2jjwjeuql.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2uhadwyhn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gfxsclph.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bidsqnzr.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ghsftzzc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2mifcvlfb.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2plycutul.html


<!-- 参考信息 -->