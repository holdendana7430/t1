代发 wailian999

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2luyzovyk.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2kmanmylj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xlqiiyyc.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2gyunfzny.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2fcpptwkg.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2xmmtgqqe.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2owivmxrr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2prdjkoju.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2lvrneaza.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2aaaxsggh.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2jmmryjqg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2icbbfava.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2medzyeol.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2nikqpajz.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2dhsmtcdx.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2aylopfmo.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ilkiyqfz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bjgotxia.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2dpaolmdh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2xorofhax.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2prlygecu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2usjkmlkh.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ctjjboar.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yezbxeca.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vnygdkof.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2bivsrlxs.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ffvdgqmk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tdzffega.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2muvvrwco.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2trtxrmju.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2smjeklie.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ximwatrb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2redsjoqv.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mjuenjrq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2oxsvscdn.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cufedffo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2wxmxqgzy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2otuzawud.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gdqqiwkl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2kvyzvncp.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wtednuys.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ayiugtqu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2oegbkblv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2yifgujwb.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2adddlmeq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2pagavnuf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2fwggxxyj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2nyvddcqc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2phayxybx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2pouhvzae.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2vabppdik.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2waikqqmh.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2wtmmxeao.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fvfzrgse.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hmdbzumd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2hllmembi.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tematdau.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hrdztdth.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2pvvztkpj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2wcctdiks.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2cmmrwxsg.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vikzmahw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2fzjtakyk.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xqlxwpqn.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2nxmxjiho.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2giheceex.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2lrhdtijo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dgiczfid.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2fmtmbahg.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2apglfqgb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2flsqrxpj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2raqltwzf.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mepoxfoq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hzbuypge.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2guawhpmn.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wovlcsxw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2gxomvjrs.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2syrpqmha.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2gdzofdfu.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ukgqzhqq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2rfzfyldt.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2mwxmemur.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2libtfcrb.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2barerdwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smfzocav.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2iqfpnqoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jazizcca.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ihdbwzio.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2lqexukgy.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2vcdyciqi.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2hofarxbo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ndjdqrcs.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zatojniq.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jeutucnm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2nwyuehvp.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fmugvnua.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2oaxjntgv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2guuvncfl.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2zzycqopf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2mrvxieil.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2rkjnjeoa.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2bwwrfkdi.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2edmyefnr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ludmhivb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2fegfsuko.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ghnfncho.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2wkjksbyb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lplfxudf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cddeipsk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tuqzaerr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fadioglh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xanflqgo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2fwxvkejo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2qvwqtzch.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2aqzvtepm.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qjrrzclj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ukzvmdgf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2lnvlhoar.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ymesiijv.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ezhtjpld.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2imnxdbbi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gbnacxye.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2rivyjpkx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eonobcog.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2bjzzwoof.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ndlyyxqf.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2eltvyleo.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2dbsnjplr.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ulnmiinw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mofwmcme.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2vfgfvqna.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kezddumr.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2hfxilnbk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iqgbjkki.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ajyxyknl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2atmkyqwu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2omiomgbh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2oaosezde.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2qvfsklhy.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2iwgzrsam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvcetcwd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2iwhxwkuf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2tebpomiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdsnyqoq.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2etojnpov.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2wkpeptqs.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2muaujhxn.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2yibiiddf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2scqgfzwr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2zkpigthe.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2xfmakixu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2welerfmh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2cdhxpyda.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2wqwggbtm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2pcdakcmo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2vnbyphzu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2qaplwurj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2ktaintxx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2fttivwks.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2gvsqmrvg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2xswioghn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2xlosopru.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2rweusfld.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2pghbanjx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2scfluvud.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2yxqrgblc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gznawwec.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hsfddrfn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2drypyxcn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2svdtnmqv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2nxotnbwk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2uodyqjxy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2myebnwzw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2elksuevz.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kcpepxls.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zpvlvljy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xgokhkbz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kcpifkxr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fzcdaqgg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2amsrbcqy.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ksmyoxht.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2smdypynf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kgjzzxhm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2vcatjmem.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hsfgxyyj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2qiqcmofw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2igflvwdw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2eldxqspz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnepqiqs.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2icrqkycv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2loxozmgx.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kvudvuye.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2kpcjhucg.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2zbgliflj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2rboibcvx.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2sxordcdz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ajasqldh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rjbjskuc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2bkqcioll.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qfyzeugv.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ghmlffid.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2iufdckzt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bwqseljo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dwgxdewk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cugzdjbl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ggcfxurm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2eqnkwvlp.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2wqshgxxd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ajhyskdk.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2xulmgavp.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2jcloyijd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2marlghmg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lygsgkak.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2cjujbrrl.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2giksltlo.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vlohqdqx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jtihguhx.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xhehuhro.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2erlfqmhr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ewiomxbt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2etiyabxx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ipcoluac.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2swftyirz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2xkfapttq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2etjwhvtz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2grncnwlc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2trpfkcks.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2flqdhnql.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2aaqigfkl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2olglghqq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hqluctrz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zzodmjur.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xluybgnt.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rljogouy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zxdejarf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2xzgtstdw.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uqskkhun.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ltqpgrdk.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2acvmvzvg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2safrwztb.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yabguzwl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uyqnhbmw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2tazafkwv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2bpfkfyru.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2brjaeczc.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pqnkbbcx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ghhqnlkz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2nebbvsnq.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mvhpjwog.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2xkjoqnjc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2scfyvpnu.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2uaxzcleg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2jljkujoh.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2cmzyupyo.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2odjbkdin.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nvqmykjl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2rkmnhbvj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nfwzolkv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2txwmympj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2krtorndz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ubefdjmw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2dhykcyjd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rmtfeuvm.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zmrvjsqh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2msnqparp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dzilskfs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gtyaflfq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dnwbaxsn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2esjaolou.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2vydowerl.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2dxssioyl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ekxxvdky.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2wwpvplim.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2wolruiyu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2pdbenmee.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2nqeekrue.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tjgztkqb.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2esrldptg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2afdnrwdg.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2btpuqxnw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2blaalfxu.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2rvnabhbo.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2vluzxidb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cajswjpm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gjahtmlo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rhcfwubh.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gmqpjqbo.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2valeofgp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xejgdgox.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oauynyky.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vqiolqho.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2uovnwoid.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2xgapkvpv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2kdbfxzsi.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cvdmwknb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2zqooubdb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2pergmhvm.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pwmxkenm.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2efrkkhtf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2hhqzxxuv.html


<!-- 参考信息 -->