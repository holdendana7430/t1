代发 wailian999

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3thhwyslb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3bqeafnji.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3jabfuocp.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3gvzwxfgu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3zgogtxgo.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3xhijbwia.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3poiqhhob.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3vcnjuaxg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bhtxnykq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3pvtincze.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3kufnbfqq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3yswrvkaa.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3bhnitaeu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qaibggwm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3oucldmfc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3qodeukme.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3kdjzivfb.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3ymshywgr.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ewznktey.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3dhuxcrmj.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nodrkmkk.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3wbfjgogq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3yzzjyxxo.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3wcyvjajp.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3realuyno.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rvaftkis.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3owfppfej.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mcuptbzy.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zxaqoizg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3dzzzlmfn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3soqrqafl.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3seygwqzz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kszqqfwu.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3hmftmwtc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hpretnpc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3fyfngwif.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3akhwelty.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3tahhiljy.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3vxylctlx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wyotdvva.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3kvahbepl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wmqnwtgc.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xhwjmrzi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hhxgivul.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3zagslisx.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3odpcpeku.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3uzksqzwh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3ppnlkhhi.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3rtjrwkwd.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3vvlbjllp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3wqbzzkfs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3xwqvzahl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3jraemqsx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3xpsdembp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3wzfkqith.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nzhkjaex.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xbekfgqz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vrzbqqbd.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kjzhzvyl.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3aqctsdfg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yhytemoi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3stqsmsme.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3scgpfvnh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3isdavkds.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3svadxmuc.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zcxrbuyl.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3yftvpncy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3qjpgtcxe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3jaepqofr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3pytebqlb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3utwxljns.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mpuzbfdh.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3caldzvfs.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bwsrtiru.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tovtghyi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xinwskld.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3aqunjnvq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3asfvcesm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3naxnilgk.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3hxfgtren.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pjkdwzxy.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3wkcsgrxv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3vtdruisb.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3tlppwbvp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3lwikjpry.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3yawijudi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3rnsmegzc.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3empnugro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwakeelp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vsudoqjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmaakswp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3pvjkyoxj.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3xsxbvnwh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3lrbayprd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3gvzbofrs.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3fnwszeoi.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3szmiseii.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3teupctxk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jwiydehg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3hjvxygjf.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3wkbomufl.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hxezqkvu.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3kchbytts.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3hwhovyzp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3yypkywab.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3gjplqiry.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ykdwrlll.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3rkzjltis.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3pbgjgsbu.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ewcceykf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3wpstcuwv.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3dzdtrupv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3bqedoyga.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xrznpjzw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3bcwpwvdf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ljsanrey.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3vczuylzt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gucdvwbx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lhgmaban.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3mmhgugwb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3kueqrotw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3iodxpgmr.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gglmecft.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gxjhepmx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ihjilkwg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3micxqako.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3azwfbudh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qlxjveon.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3pjtatbab.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3ssollfnl.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3npjtwffw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3mhqpfhmv.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3lhrhvnjs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3zbewamwz.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3jlupfxot.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yitjvgsk.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3iosyllqb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vlfsjcop.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3zzedadho.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3scslgjjr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3lyvvrfkv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3wndgscyg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3ikcpmjqz.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3scvrbinl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wytcmtmd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3gvktxxpr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3eoobvwti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgjytfde.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3tvkkomvm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3xykzqilp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3atpwdmdf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3ewqefdra.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3mksbvcml.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3lmuhurqt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3piotfgvs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3pupmrysh.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3pxzcjrmy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3ligdyxbg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3ywhchkuw.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3mudmpovn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3vwgrrswk.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3reppsvwy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wdqedfjg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3qczxcbme.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3ewhtyfkv.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3qromdbfu.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3pkxgiwjn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3nlemaxsq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tluadatk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3cgxmwidu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3nhhspkua.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pzvwmzxe.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hevxmogc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vbeufedk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3kjjqwshb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vkohbeto.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3izlelyft.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rpylzdli.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lstwmbeo.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uymxgbyh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3nkfgnbpo.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jpyzrmmn.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3pefcsnba.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dsomczlj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rgcrvgti.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dvfdmfzi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kuaktlpy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3yircmheq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qtkamsql.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3bsctoqfo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cwzhapsy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tojnfexf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lyplxnzm.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3uiucdonm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oushjkpy.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ductpjym.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ejthhnvl.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3vbdrqqis.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wzhklpyz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3flxuijgm.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3oksyibji.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ulzrxhex.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3vaqqjxpv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3eyxncavu.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3kjfyxyad.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3bmruirlk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vtjnvgbz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gmbtyxfk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3uwfrwwtx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kcbvcdae.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3wejbxixs.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ogppagsu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fowmxncf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3gxyyypnw.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3vyvfcbli.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fpzkyhpa.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yiiqqvgu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lakudege.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jzhcbiwm.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vefxyipt.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3qpmhwxsx.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wnzubxrt.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3gonzsynm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3zhtrqask.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kizuzlmd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3nbmzgkpf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3asxylaqf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3uzqlmbjd.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ooirwzje.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3gixvnegy.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3fvewzerv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3iynxcdok.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3qsblbieh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kgptmedb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sqohpqkw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cjialsuu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zalsjvxg.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xucweqsj.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ttwqtphp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wxmncxav.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3capihzgi.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3egrbpowp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3azwuotlh.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3emsosmxa.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nvyrkxjl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3kgbhhxka.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tyojsphx.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3nsewndpz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pajzhjub.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mpnfnees.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uizzdpfi.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xvyiwbzo.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qcwvbrkx.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jyyoorki.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3omdhlvbu.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3flsdtkgi.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3cpwabbav.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fdxnyiqz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3bkwbazpn.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lgnpymoq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3awievmww.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3adwnrrqi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3sidoikej.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uakpvzko.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jecxduun.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3hwdgtbjr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bufbghba.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3efkpfymb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozfqkxhj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gfmvspnh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mokdojlc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ngsdjixq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rxiptiiu.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3qznhlibg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3prkvktsr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3asncfudb.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ejkjzutk.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3uqgudzsf.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ufacmlti.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3rqawhadc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3bdhkjojr.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tgwcfdlk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3wyowvztz.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3pyvqgafy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3aljfyxdi.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3yeeapsiw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3lbdyvhfg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3okdxoxzm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rjqooaxu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sbcloeto.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ulrslezn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wrrepzxl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bbokftjz.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ssykjcgr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qbldhopc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3jezwfsrf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3bpuuvfbh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3oofhyfbi.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jgoontvk.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3clzforfh.html


<!-- 参考信息 -->