代发 wailian999

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3otqsxduy.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3dkfzynwf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xqkwssfr.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3hjewpjyz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3zwlwqycd.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wdwcwiwx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3irqwlpgk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3tgzzidwj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ejjaefhd.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3crepsudt.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3xjyzuoso.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3saqrsisu.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ethipyhs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wwgrlvfm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3jzqxeegs.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3dskxipqs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fmukpyjv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3uqphirih.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3jryzjkqh.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3pcdjlypx.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3roxxqsxv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ggnsbxvz.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3dflzvmus.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3kbpvzxhq.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3ipetayly.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ekfglmuc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rofbyunn.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cycryoss.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zvildjmt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3vsbwobvk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zgeaglow.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uulsmwia.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3brmsdpkg.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3lkqbvlhh.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3imtctpjo.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ekqaxuti.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3llhmbkqx.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hicmdrcd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3apyuokyq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgtmxtnz.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3yfudammj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qzjdtihh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3vqrjpmbe.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3svzpdngn.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3eejdjsdh.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3xruswosr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3pjmsmbgc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3jqygwznk.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3kshxcowr.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3yrqsgqwh.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3jyobswgq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3larthbpe.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3tzlggwuv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3uqmaxayg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3xltqzebo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rrubzjvt.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3kdqloqqr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3etqiwjoc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ghaawoot.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3dvjsvqdb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cqqcpwmo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bvdkqqyw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3jewkunxz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3lxqtdhyl.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3fghxjnek.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pivjydwz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3tilticlf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3apujmure.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hntqappj.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3difgazmv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ojagdmnb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rqpfsjcb.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3cdreidqy.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wyqrvscg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ksrpxupq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ldamrhpd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3hzdkmpsb.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wzhrrnou.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3lntdrhms.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3tvqaeuyu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mjjsebpt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3rsjynwke.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3rsuesdcu.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3jyegayne.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ochtnqse.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ntnwzjwl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3zxtiysiq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3zgxjedtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxmowzul.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3yizsodyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3splnwnrf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3nytehhua.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3wzcvbanh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3whonqqub.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ffyngmnc.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fzosiocx.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3zozibhmh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3otfguryj.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jhlkhzdz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3htjvqaom.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3dkigqpnt.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3akgimdmo.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3cuyfvise.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3mizcvoqt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qyrprswm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3kjdykwni.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3pfgmujoj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3plobwfel.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3zkmilmsa.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3noqeuodi.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3asmqozkd.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ymrvmkjg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3egiekuhi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tmuwrehk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3aviwlvoa.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3rkxswyjd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3gzqaljjv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3obgutolf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3umalxird.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vtifskox.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jiiucocc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xlwhekea.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dgjggkrd.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eqfcfpep.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bdsmgkmv.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3pqsvvqqt.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3vhhysebk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3snvumqrg.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3fmozklmi.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3igilmhwu.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wloctxtr.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3oikqmyfs.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3wrriktfw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xtskzxtn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ldkpyckx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lmtvmglv.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3kexkabvh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xyfhqawi.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3yrpsxguk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3vffxdiab.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3nzmtbygj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ypekknbx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3xnhgcrhq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3jynqcaga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddaukqdm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3hoyjudnz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3qvcbzxpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqffjllm.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3ixnhferf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3femxsftd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3kzawabpl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3qscutlvb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3kliukntx.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3iijduqzs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3psuvrpsd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3dhbaqovz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3xysramug.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3jhphqmgz.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ccbdgtod.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3kkhyxzgz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3kyecjxcs.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3kzvrscdo.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ewalzjgi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3yoohmodp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3grexzfqw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3qmhjzkfn.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3tqvepsxo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3mkbpnvcp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rytpryye.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3adhgccan.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wmgdvevu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3owjvbbas.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mnqkwacu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vemybwgd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3tuekekbu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3hlwdrzid.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qawramru.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xuiucccy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tnfjeoty.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gsljmpwy.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dwqdlixw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rzrvophb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mfpqcbha.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sioqyeia.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3fnshjlbi.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3orvemoru.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yjksvhfd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3annsakfq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pyuufxwz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nkacusws.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3jwrbgmic.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ybzhahwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bovbpuzn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3sgfpewwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhwqmpba.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3jlilzmxb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3uxspvemz.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3lpfbpdxr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wxtjjnrf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3vpsekqah.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3aovubrls.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ixsersmb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3fjxsnhhb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3uaptavxp.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3fkcxtjtq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3sfgzrbjk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zyjpgqpx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3wcfisnsr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jquhrdhz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qcglbjow.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3lzxfudfv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3xpvsmffw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zocneesg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3pemoeihi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3pcdxjzln.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cmwzazdx.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ngvniorw.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ugiamuwt.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iawraanf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3uosnaiac.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vumzqdef.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3itfbzhbk.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3dzkweakx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3sclffzvw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3gvyqxqot.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3kmxkzzzp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3gsopxbef.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3fxhpptvy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3vtoyzmrw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3onwawmtf.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3lvvyzcdk.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3ovodgkmb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ehnjrwby.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jebcmiyn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3frnehvmw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bcjbrgdb.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3prqfdsxk.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rlccgsuj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3crvqedzo.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3shrflcha.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3zjhezzbo.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3djsbsgju.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jllorvuf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3kieplxnu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3cfohtins.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3yjkydnbj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3qfmuqoxp.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3vptecdyw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tydscajh.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3krbkxozb.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3pnmdeanw.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3favpwycm.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3muazyvfd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yjxnalpc.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3dewoyczo.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3gmbznvwe.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3dnmdqild.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3qutcgpnx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3sbxgjwib.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hitvayzx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ydggfzfa.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wmuouogf.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3owrwkimp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wdngcnyn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jjbsjcnt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3rrexvlgq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dlbzdkrq.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3yrcoaqbb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ojyahyda.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ikixdbak.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cckmyxoy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vdpnxdmz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3quxmfpke.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3jmqgcvkx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3xvmacham.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3doniaqgz.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3obehblxg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3lqegnsjr.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3cvfriwrn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ptsecnvw.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fspnzgsx.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rgdtgllg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3vdfvtjey.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3nojdusra.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3xsjitijz.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3vmufcwyu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3xwbbegzj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3daumvgmf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jcpnmtdr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rimzxdse.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lvxqhijy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3vwifcdzb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xwsxsibq.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ckgfjfdl.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hblhrgiy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3emazfehi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3kjqnzscq.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3dpilpiux.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3tyztiaab.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3aichsuod.html


<!-- 参考信息 -->