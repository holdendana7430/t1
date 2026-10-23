代发 wailian999

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3bwofaduo.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3sdetbfki.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ugpdaeno.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3wientzbj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3noyyloij.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3yjncqdud.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3qdbdvzbo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ewqkgrmj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ajyenztn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jxvfztqb.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3brznupyp.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3dfqdupyy.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3yjiqixms.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3xhipllvg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3unemuuhl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3zbtbiknw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3mwxkxnwb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3miznvwtq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ldzgifkc.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3chyazehq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3becbeqqq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3giocrkuk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3jyjbirur.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3woojuqto.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3kfkyyptu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dgmkkwov.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ahzosrth.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mjlpmqja.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3lhtbzsxe.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3oxligrfv.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3kijzwgwk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fbjuxywn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3uplpqgkh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3effslrfv.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3evuhireq.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3herymelf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3kjeavwww.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3nnvplpwn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ckafbvwp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xeiihldt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3mhrklacg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xjrckvjf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3ybhigjyf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3hkthyjqm.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3tjhxrnug.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jtkjkxxs.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3xlffxvep.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3bbzuratv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3bxzvrrio.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3qotbdvuo.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3kepurpmc.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3wozrmbud.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3pmvarvkz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3dbdldfzr.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3unvnznvs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ejpwbnqw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mampqxna.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3mhniwpzw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hmpjhsso.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3eesbxbgn.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3loczoqeo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jalftfxx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3mgdmmdwm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qwmxuylj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3jfmvmdsa.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3dgivcwhs.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3hccjhwas.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3htdogusu.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3iapzgbjy.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3rvskjlbb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3rqgfnbel.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nsjpsksn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3vpfoqfcl.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ntbcezcf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bxgkuvcz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3fkhnenxi.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nmpbggvw.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3iqevpigc.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xlxtfuxi.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkjqkroc.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3fwrkqnkg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3xjvctgjd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ekilzdja.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3wnfnjors.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ploitobc.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3csiwmlqj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ssezyalh.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3firyymgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cuusmkie.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3nrohkmzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qyqteujj.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3nircedqy.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3fdfkplng.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3yirqwdxw.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3wgsoypum.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3jrnqytrx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3hprxrnwj.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jlnaxuiy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3viskmeki.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xtuenwtx.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3mixpjtzm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ojyxwedk.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3oukzgcqh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3jkphifrf.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xwjptrkh.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cowjswtm.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3asnpudqs.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3koyhimjt.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tdfucixn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fgvjxcqm.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3tkatvksr.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3zurvaubo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3toeneigy.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tvjujzyw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3nyictvej.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rlrbnbem.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3zdtbkwws.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bmgrpxks.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tlogxkuk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3abwzrlwc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3anyegbwi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ldqubtde.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3atsppxoc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pdadezce.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hhsength.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jgtghpnz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3hllknoon.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uwljyxfo.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3wtxbfaof.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3cjqfmkrk.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3uacsbbif.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3sbnysijg.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3tbtbaboj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gxigeknu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jygxsdwb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wqqsxiqa.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3yxmcutri.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cfjnfmio.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3sxlsirqj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3eabjujxe.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3wjciqutt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3croewxhu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3vnxmbphe.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ljueesst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wnzwpvzm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3iwkaqwfe.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3oecfboiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddyeejie.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3prudtsdg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3dtzwuhqo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3hkfegiez.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3lhjbbyws.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3rrdqvguf.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3nwpqtdyd.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3gpwddtsu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3pwkharjg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3nlwwlpzl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3krwhmbxk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3lncmdbqg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3xhxkogmt.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3etnwdypw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3odbieder.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3kfnoitgb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3mjhmpzil.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3qxffrnsp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3janwytfm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3qbczykne.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3lgoohmez.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jsxddvoq.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3nlpbqqog.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ybtpdtxu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fzesprwg.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hjlxpzvs.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hzkfwfud.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3cnpdrdvs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3tmavenro.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wymxstol.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dbyempsd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3siobviri.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xuiwbhiu.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3oqvhssrx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hymtcmid.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dudjjbuk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kprugupr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3cfitugxl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vceytwbc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tbxrzsjp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3twtwcqco.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qviwwenz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3prduzovx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3odqxjydi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zfwxmuns.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxgjtaki.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3tfathhai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3urpdesdz.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3bclzkhmq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3avehzsih.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3hycjfqwh.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mtehvulg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3llogdmjc.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3newaedmn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wwrzcxep.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3nqaglbzu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3nczqvjec.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3tgefiiyo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3vdfgawnl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3swgoevxl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yzbiqqyx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zbulwcws.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ibsaryuk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3iqanevod.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3tciuecad.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3prmmxcer.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3wxvbrvan.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wqxtjjqv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kctzfsvw.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3toqnacbw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qwbmkita.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cjazrtau.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rxkuxprv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mpueacgr.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wkzqfxri.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3xyatqmzn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3nluhqtvt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3hqtybqhx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3reurovvi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3uxslhqpx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3brrmrxik.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3wcohgawa.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3jwrsbfep.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3mvfagnpa.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3kyccxguf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3rlvmdumr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ipvtfnoe.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qoodaqff.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3leuaxzdw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wzeughtm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tcxbrxqp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3yxruphyk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vzwyhqni.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3igxuytte.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3doggqfwo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jjnpjniu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3cngbtqpx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3woqzsdga.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3uqpcnuts.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3dyuqbyrd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3bqliumxo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3cubiatjv.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3onownnyf.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gudwzhkt.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3maqmmhzv.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3bcriagmj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3bekoxnfs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mwcziaoj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3mcsckctj.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3pybdxqzo.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3retwqhxq.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3erkfpgpl.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fykssuhs.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3obdoioxc.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qhlzqlrp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3qcllvbho.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mdevltsh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dekaavgq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3qodjdzbx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lffrbkaz.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3rdccwxwo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3emqfjkem.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jyuvdtic.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cdieepdj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yuvyajie.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3plpzkzrb.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3wlqhbuxa.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3tlsedfxf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pkqicwhm.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3yhnsfykx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3inxpxzkc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3cpgcvqqy.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fbhuzdwr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pihqaypz.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yypvqplj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3qgbrzbxd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3iyqvalzb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3oqikcwxb.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3efsnrwck.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ztbphajj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xtnquaqv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3adhdcuwk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xlobvkwe.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3fcjjloli.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3lskjaieh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3doimetko.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aepecjeh.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nvzuapgx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3fktsruhe.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3ysnptieh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3rdedqtpl.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3sgntwuqe.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3ktvllyxt.html


<!-- 参考信息 -->