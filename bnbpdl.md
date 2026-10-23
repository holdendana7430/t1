代发 wailian999

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3mevqpgvh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3kilhspra.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3oltbvqpp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3cilpgqcn.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ofhavghn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3mvycflyf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3cqdhicvg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3chsnqbfv.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3csvruzqf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3xxpuubkt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ldmszxup.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3jvqmvdvh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fsacwvym.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3chcusgxh.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3uxswtocm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3urzzzwra.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3movyvctk.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3arjwikfx.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ruvehrpz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3kceoddpc.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3antpiakm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zhetziks.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3rdrujbrm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zmcfasol.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3mbqcjihq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fqjydoao.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3lerimqqk.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wioliarb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3ykrxhyms.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3dvvrccmx.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3jftqxufq.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mqnymlte.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3gkaocvit.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3sjnvyuhd.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qpcbgliq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3kpxrezlc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ftjosskc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3lfzdtmxy.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3wagxiylt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrufkbqy.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3kqdfljgb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oshyhyoe.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3vnfqhjks.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3drurlzym.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3aicxfrmq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ahqxvbnc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3omibcjcy.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3wwkuyquu.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3cjpnqwok.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3mbhboukg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3urqnfggo.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3zssxmpqj.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3uinhhatg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3uzmfjjfj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3uxtjweif.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vsmdmlwp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3uxkzkuas.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3mzpzqmqx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fhjrpdqk.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3kmczwgwr.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3civjdhvs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3yvhlzlvn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3mgxfzkzs.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3udqdtiwj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3jvcdbgeo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3cukofmvg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3dkiqebhq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3semgeejx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3vlwsrkdw.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gqduyicp.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3wgrqcdvr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qmwoljct.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3anmnadcg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pmblwcrn.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3cgtfvtma.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aqxskhrt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3wsjujpbs.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vjysazkw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3xuqukxcn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3lsrujbjs.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3girycvcs.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ezkblwwc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3nxfteaqn.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3oihyfxkz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3gnswcbre.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3smiwctvc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3wpumqhjk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3fwjjmzoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hnvodclr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3hdxsqynj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kbevhuzy.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ibtewput.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3iyenmhso.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3dpcqkizp.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3sorrxlql.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3mjzxkppu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pxuzpwzs.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3evbzfams.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3grobcfug.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rafdqgvf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3kwhsikfa.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3nycsgzlj.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3jipfevhc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3clecvybk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3alaxzyss.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3zinegnkn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3nqimdpnv.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jlxqguiy.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ajwtitaw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3srgbwbmk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3rcxsgfra.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3nqwhjcml.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gulqtbwx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xpblzqwm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3oxeizons.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3pepiptxc.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3jxupbsfx.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nlehemec.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ygkstzuk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mjivscbj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dwdvmvks.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ygppuazj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xxdxnjhk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fspvcbjl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ecrflswk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jofibjis.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3mveuqrqo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3avhvnalh.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3ekdnrafi.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3yzlerkcw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zmjlbfik.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3knxqtczf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ysxpfmqx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wcwcszur.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3xfthsfzu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xwzvxnnf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3mxwegbuw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3odubqyrj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ihudtxie.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3msuausqv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3rwyufjoc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3bxbcdhvc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ooxobptg.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ooxlznxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhumlnvb.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3haagdhuf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3hrbebhzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjeqqjth.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3zumeumsu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3khrjvnps.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3xjhdilze.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3bktciyio.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3kkhtfgje.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3ayryryny.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3gxcmybba.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3jioshxge.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3gllymvba.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3wfyevfvk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3dguhrmug.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ztjvrwzq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3flnpxlpx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3atwyomlj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3xggsocqm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3dcgmznaf.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3oomseasy.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3vscnqxol.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3ktabukvm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3jlapoibp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vgysulxb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3abaveskt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uaagnbrg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3pjdqroum.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tqmjykpo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3apmbcqko.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xsrnbrkl.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tbvazdir.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3muxeuird.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gbtohlfv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dfdisquk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hnzesurc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fumhgaoa.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jxnfbduk.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ypcfdmnb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oycqyiic.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wxggopfw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3aeoplkgj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lznmnzru.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qhpdrpuv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pcgzouil.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mbgwvlsk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gvcayaol.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xdzbtzli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3naktgjfg.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3nissrrra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brqotpjz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3clweztlm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3kooqwtdd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3spagpvtn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fkxgcpdi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3wcehatov.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3basdgnhz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3pxbkvpjr.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3evepdluc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lshtneco.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3laaxpras.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3qmiimnxh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3bwqnioqk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ozzmmppr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3hdlllvgq.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ebbcbgnx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3cxupjstd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3eusgpylt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hggqboui.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3gjjnitmi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3punjyiog.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ezxjlaqp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xsjnlopu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jofcsjch.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eobdtxlt.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3uifoixkp.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3fkoflheh.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uzvegqre.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3syphesvq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3tlkqphyq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3plrtlbwn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3qmrutbai.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vkbxrhbt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3jahdeird.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3lgpwnxyo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3dwamkrow.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3nbevxtkp.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3jurlukzl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ixfojopo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pdpwedth.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jdvukehv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hlxkjgzw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3foexedvt.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jfzmgrgd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cfuvttmn.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dlilpylm.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gbumugoh.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lpiuwlov.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3sygmtwpd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qmrdlljq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3lfhltrcp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3itqascav.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wpywxcvi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3oslarcig.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3orukdrvx.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3semujqcx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3vdnuprml.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3jiomiokw.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3wbmmanlc.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ifqvrrse.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3rszzkaeb.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ruqqagtg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3yxqdilku.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ayrxqrty.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3hmmvlbvt.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3azfenayf.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3uurrhrbs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hvyazolb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3cnwgykqu.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gpedjatl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wuxebgnm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3blgldasy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qnuwtpxv.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yhehoibv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ifxkyyha.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oeqfzplp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pbmtgypu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3igzjchxe.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xgsrxwya.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3wkzbodfw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3fiwwkzwe.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xpesaydv.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3wndqqohn.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3txjpskpn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3direfssc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gasfpwul.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3cwmfpeln.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rnzehron.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ydptpsix.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3puvnoqlk.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3xeiyuhlc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3cabpjyzh.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3khwyethu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3iurwriln.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3iznoxkxc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ufizxwdl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3juqduixi.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3uzxsinzt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rrxggjpz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xmeklsoo.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3estkpuvy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3mydfgpvo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3dvuhjakp.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wnmlkloo.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3bmjiywqh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3cgsppraj.html


<!-- 参考信息 -->