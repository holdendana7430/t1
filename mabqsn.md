代发 wailian999

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2qxpxgqqj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bqdktixi.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2uwpdrfsp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2opsdbcke.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2veizpxls.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2yptnzbkr.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2mqittkky.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2wmnscehe.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2bnicbctf.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ctpnuuyr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2jmlirjpu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2pkuciqer.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2beglqykw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fdwhkhag.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2dxqgthuv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ywmmqxlg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2xoxkmncy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2hexywvya.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2bypekhtu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2qhqlotcc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2wqupcpwo.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zgjtqngp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2vpskyxqr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2pmgqoatn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2znldkdwz.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rtgvrzsq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2himqhrre.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2odbzefcz.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2xrednlnz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2yyiffnrp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2xevdcgpe.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ktztsrbb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2fcahurqy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2qsvrvpsn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2frervdcg.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gvnblgxh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2ksvlndvs.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2nouefxsi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2minbedjf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2djolehys.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2rwmhazay.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2psdirguv.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fbogrmjy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2eofdiadr.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2jracdjjx.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fgagyodw.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2aypqnylq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2apuhydxc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2dufemcad.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2rwxfkrrg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2bdoktnfe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2lvpbjgwi.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2kuffxbwj.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2dqxxiopb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2hnhzhfoe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qznrclia.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2nvriootd.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ilpxvelw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cyiznqcx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2hyitudle.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dmcahxpw.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wrdscddy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xcbqdfeq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2uamcxtzc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2olighidc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2nyqaqkod.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2tmboecyi.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2avjrgkyr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2blbzpqvs.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zkwwomhr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2oikklndu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ofabfath.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jugvpmqu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nryppyaj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2iiwfpdcd.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bfntslsb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ulqdwxej.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2egohktoj.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2wyylcegl.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ocwwsnzn.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2fxbffaqo.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qtfapohg.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2pmgayvgb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2jczkffoq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2elxwdgbp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2qupisbcw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2qgmrhatt.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2nclfijis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hizyrhoi.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2ybuxjqjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gbjzfzqm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ezbvspdo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2iuigmwje.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ogyqeqsk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2qcpiwzxt.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2tzwwxndr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xujlwuxt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zihevzki.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bhgqxchn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2taeoxtrl.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2lggjsqhp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2oastaxxe.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2egvletnf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ihdquopg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2zmgovwuq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ozaaacum.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ezuauuyr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2bzlhvrwu.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2cmpayjsm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rxzinird.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2hwohehop.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2hwmhgqwy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ksidcvcl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2elynswyn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wsnsrpme.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2eoidenhl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ouvwzfzk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2kkazmsdb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lytsdbue.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2pyvrkppy.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uszxiatn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hbsaynpc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fmjcuiny.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vtzsasqm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sroizvef.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ytlagyvb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2pixrvlpy.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qwqrsdgb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2vkygwuph.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2gywczybd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2jpcwutvu.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2cvlrsgws.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2srolzzle.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2celynjss.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2lyjrqkqe.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pmjalvrt.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2nyyefyhe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xqccjykz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2hvairrgf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2rxgltnet.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2iokrphgm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2gvoqzojq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2foyddndn.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2bwnnieiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuhivhye.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2yghxvlqy.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2dblqietj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmnkzmfg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2gjspebcp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2uzdzajfi.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2vibtyzvw.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2zzogarfw.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2efhfuvhp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2acmdsvwi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2gdcxowaq.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2rsewakhl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2hovcoxxo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2mfxneatg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2plkugbdx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2iekiqybr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2pcstuxfa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2iavteqvx.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2uguwcrvu.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2jykalrop.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2hwstcvoz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2irufrvth.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2mbhmhtdc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2hsgpmdtc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mmfhccmq.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2eogydvmn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nxdhffhh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2raxqzxmo.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2atqtjcgq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ilhzccio.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2msbjomex.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2epyycmoa.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uyobbnnu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hpofseld.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2mnbkjyiw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sbjqqxhj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2icdvlhzs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cvtkqbkq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fagaybpi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bqhwrtux.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gojvjunc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2unosdiyk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yrgjkmtu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2oehxdrte.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ggxgdjpw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yeigpaof.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2lcupxnvx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2etlxinxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2meqeelzf.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2xwgheoax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuburcfi.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jiqiyett.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2pxvwgcyt.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2sslnhpei.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qeeejwmi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2mcsvckhs.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jqombqca.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vekvgaqg.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2ciijlhqc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2cpjcrmpg.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2jibqhnjp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2lzuoqctt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ntnicqcm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tesaebkg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nvxzyeum.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lyvsroqr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2jvevehdh.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2jyqadpsd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uqelqmcy.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2eowylcid.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2zcpilqrm.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wxmaqvff.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oviioyhz.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2atbcnesy.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mjbcxmlc.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zjrbzrih.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2nicfkcqr.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2elwfdqdl.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zbfstylc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2qlszznxa.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfzpwlah.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2bortasvi.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2wdzmrbog.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2hvknmxta.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2xxagifxq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2rhfiobgw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2qzsmsgms.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2jkcxvmgl.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2bhefvknv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2orvvjgbh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2djbifpcb.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lxqdlbpq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hncbkmcc.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kkmykbri.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vgwnygmj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2svdekjyo.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zuplhyxj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qpaxmoqu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2niconjwa.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2axlohdfj.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yztenhjy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ppsexcbb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2cmpnohdb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2ohitnjuk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ixbechbz.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2muhcdrjc.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zsddhbap.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fxqubuas.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nevygycw.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2rnbncwav.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2tuxpxuoc.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cehxacvk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2nvbavgfo.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2hveddqxk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ylivyqqn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xkjdhjng.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjmwvbpd.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dkgywinn.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2cqipifmc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ccpaavsl.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nqpgfbxu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2vaylpixt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wvfyhswo.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nuendusw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hsnfpbao.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mnpputzu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bltdnvug.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rzcodqwc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2whialbpy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2eidwxudg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2lfzqjaan.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bnxidris.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2npwoghmb.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2fyjvgiwi.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2dxkmclge.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2aydlifzr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ltqrlfdc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gxwilzgb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2xaisyvkw.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2fiutilli.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2rphykhqt.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ekaevwuk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ldcxwnkw.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2luymiafx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jfvzmrct.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2niufgcrm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bofudoev.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2dpormrnl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gbhdhbby.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fwmdpequ.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2zjmrwrcf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2oqovmrfb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2weohlija.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rwywvhmz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2iptnnvzo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2eqrtuoai.html


<!-- 参考信息 -->