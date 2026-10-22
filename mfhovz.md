代发 wailian999

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2mtpfjiwj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2xccjxaiv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2zuzfeewr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ygjgyzgc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2tswkzfzr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2updveohv.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2acrkuugn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2gzubmkgc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2nhopmime.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qoisleuv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ejbcgenp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2nmuordad.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2kjqbcsks.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2oowujehi.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2vbgopbqs.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ddtgwarv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2onjxgkel.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2gimcsvrh.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2udqngqfq.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rlvvjvei.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vanxtawp.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2csnkvcej.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2rdbddzrn.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bhbrkrbe.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nnendpku.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2dahmwhkh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fkidnjxd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jnhbqcto.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2omevljda.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2yjwspkrn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2vsrgdmku.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vkfxhpck.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vhyrupnr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2lpokflrd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2yvhlgqhb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pkezpmie.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2rljqthmb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eviasyhv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ejnuzbqo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2rlpzyiaq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2pjnitadt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ssxyyxhg.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2qlitsiyh.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2zqjestto.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2oucyymsl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2uofypprk.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2tsnslzwd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2hzefcugs.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2akcpeewb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2zsaenvos.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2eylonexj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2mzzlmtpd.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2avjfowsj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2aognapvv.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2swxbjgof.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2iwsfpymk.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hxdsnryc.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gqmenvor.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2impuugot.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2tysggzop.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2kdgszqbr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2wwdetowe.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2dehvvgse.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2eebjhaln.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2cexxubtj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2mgfrluzj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2rsfcsogm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vhggxrvb.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2tbqvitsd.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yzupfvbu.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2bolinijd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2pdjmthvf.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ctdckcff.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wrfoeemd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2rkdvtnom.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxsgvwke.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2blhayzmh.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2aiafcxul.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2vbihiiab.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2qpyhkgiv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2tbwmffvx.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2plekcfdz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2njjbytcl.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2xhuphunt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xggkisns.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2euacwhjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzpxjtjg.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2xfmsspdk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qmyhqumr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2kvbudgse.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qwtmtjqv.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2nutyzuxa.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2tjekiwol.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2olyscrhy.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ekghwrkb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ckknbvlm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2lrampznp.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2tdedhpvf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2vhxfqvvf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2svozewvr.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2omwozvoe.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2pldthvaq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2evpakemy.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ljrdnhuf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2sblgeabo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2bwrwvzfj.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2azalegyc.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2nkfcqbvt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fsaoaxfw.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rhncgnsj.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2xwwnyirs.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2yjuvqoqg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ybvawmev.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2vgiodtie.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fmjznmug.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2uiqyubbx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zefptwrg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2tnjvxzmd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2njkcdjpy.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qzoowvpx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mpnzrkhi.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2vezuebpy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2lstjfyfu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wzodwdqa.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2tpooalbr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2rzfavpwy.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2dcavnhpd.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2udtxwbij.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2kfdqlibs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gfhksrla.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2stbzhspf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2frndvwal.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2cbcpjkhg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vccbites.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2eheucpox.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2jwmzpzyj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2pyydzzrp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2dxvmkuwj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2orjifggi.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2bqdbokoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bydxjryl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2qeesdyrq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2wglgkiwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cpmhfogz.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2fnnvxmxj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2robezmsh.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2gxghmvkb.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2hhbhyxjd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2pnkmzgba.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2mbeqxxtm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2gltdzbuj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2djpivbsk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ukrmbwic.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2gkwbxsvd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2lfygezvk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2sooxhhyj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2voodzokp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2lpqtljos.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2oyqqsjox.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2jensmcxn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2owrcrjkd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2mndjgobt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2xyaugtqw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2weedwwgi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2axvlnfao.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2avrjiqjh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lxhfmygh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2bslwnqkf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2livkfcyw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2tcyvozxu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2itnigeax.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2tnpgcpcm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2hecfwbal.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2okftzmql.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gnxipmtw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2frbfauph.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xsipwgsi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jzibwhez.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ldcdqugq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qyopgqrs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hhgqplne.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2pludbyhx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lpgpbjle.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2wmgsdgiy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oaqqbzbc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bnumlucw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2igqudypv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ykyfanii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncgbxbhr.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2tprdrslb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yobqbbzz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ibuukdtq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2yennrwcm.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ofejcjkf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rxlyytiw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ascbqjek.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gcggnzge.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2rosyykxn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2mpgejpqi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gpreyazw.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2vquqljrj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2nzbwhsvt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2etvvfxjh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rwlbkdlq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2ucpzofyy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mxnstjqs.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2gnpwzfnw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2gotzeamp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2sgufqnbh.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ycvlvpmw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2dxtrjvbs.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qazlokmh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vnhmcxdv.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ynmjvhyz.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vofplsfz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2btfohqka.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2xktdpmjy.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zgqlnmfn.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2oiwvczhs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2eiwvagra.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2folrptwg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2uvehmjkd.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2sevjicmt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2djqnykvj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2jiytoxfj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ryggyufn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2gcnlyfgw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2lvkyhrmm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2fwzhoclu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xabwrmyi.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2flcjvmut.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fqfuhoct.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eygtfjwg.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rubwsnsz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2iuidjuwt.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cdqabplz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lwjzevgu.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zpkvilzm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2vasubfex.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jbgibjmx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2elifpgkb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2tbdendas.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2jkyccywu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2soyhghpq.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2wmxmkhex.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ysdekhvp.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ktnfyqdh.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2axopaugl.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hejfetxy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2giytljce.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ckqwfwkr.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ymhuimyn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2gvpihxlm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2lrktglcm.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2lobwrdsw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gepotbqn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2oekjqpea.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xybqwgyn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2inlskhar.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sesynuen.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ygkpehvg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2ftvpmgdr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qwnwujlp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2vpbmlrpj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gggpexcp.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2poqelygc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hvdfqoqm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2efqwslxp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kuizkrfu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2fvfdpleh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2vkibbpaq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rlrlwypo.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2vureboiy.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2tpqwxoyg.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2puvtbrws.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nygmyvxs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2gycsllxy.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2rtfhhxcq.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2fzylbrbn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2pqmjzgho.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2rgbpuwmc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2xggtnics.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2fmpbhsyj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2paqoxele.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bpapsoru.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vwlfcdsx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fxofajvu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2sfopqjdt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ajtpfxra.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nhpylihg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dxkrfmvv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2fjcwxjot.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2cutcwaix.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ddaxukzw.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2mdbbeqcs.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kbwrmkvt.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2shxuqhxp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2mgtbftal.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2nkmarmud.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2xyzsuiok.html


<!-- 参考信息 -->