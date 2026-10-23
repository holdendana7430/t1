代发 wailian999

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3zqmqkeud.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3lljtuhva.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3jkrvlmxp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3gakzpiju.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3zsfathbp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3dzfbkerp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3igzgdsbz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3mfwouekn.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ufdmgqin.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3toucdvvt.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3khzzzrdv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3hggjumse.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3wyuaxoxn.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ksidusyw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3zztckngn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3zcauytus.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3nowtdjlw.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cxiijcxb.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3hxhdfuqa.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3duwfoiqs.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3bkqqcgau.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3temygjfq.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3yxcahfry.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3sokgsbbi.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3gfnutyaf.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3moapaebv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3aorhsklb.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3zgoyiegp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3lmluhvph.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3yubnukcs.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3rvjxvoyr.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3namtzmbd.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3htqoebcr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3eokiozcl.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3ainkroda.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tnjlrmfd.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qopcciov.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3kfjtiete.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3eddeeduo.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3dyfzstve.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3xerpvzvy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3lmgaxwsv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3gdzruyba.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjijrnok.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ogovlxgi.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iepxnjkd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3pzhubfmf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3rjresqhc.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3ayfojgtv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3rpuuvydk.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3bmiywlap.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3urmxnfxv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3oortgulp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3khuhtlei.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3brqbrzec.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3zhxbfacd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3dsxrfact.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3umkowuzm.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fviocjmz.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3aobqmnzs.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3etnendty.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vorhwgdp.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3luwwemfx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3ecvvhwol.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kazmxlpd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3batsljke.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3huoymylc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ihvbajyd.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3muozsaoi.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pllnpjcg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3wchxjamp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3fdlopazc.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3eddnayuz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3urhwdlxa.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zdhwpkwf.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tgldtueq.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3umolxrue.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3spijluls.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tpoycpup.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3utdsqkrx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3dwpdhxlt.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3knlwvrev.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3aoimdsiz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkjlvemv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xiutywnr.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3jwxctpda.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3cvpvtmcs.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3geidrjxc.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3labvjxef.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3lxwmfgmh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jjezzsep.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3soxecqnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3neagclhv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3wnvxcyke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlysduza.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3oivlfoao.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3thvoigfh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3cndthwfx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3nicsbaro.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3nxmbfgan.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uadrqogi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ktegogvf.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3qyepvykj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3zmenurpj.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3lcbheplh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3udzyyjnu.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3hmftuloe.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3inxqnnzw.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3dsbuyzlm.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3chibuagq.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3vjzhodos.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3duazoizl.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rouddkxy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3aooutyhb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ufhucfbq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3oxsseizz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3cqwxggzu.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tqlilrus.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fxcxclhh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3onmveqkp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3piwrrqsz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ypkiulub.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ncpyqgqr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tyfwfytw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rzxoocmz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3eovjpduu.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3cacnptpk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hjxqlorr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3spocopek.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3sanrriji.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3smbfilva.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tmleihlp.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3dkluqjfl.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3riwddbnc.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3froqmfbv.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3lmfztxbr.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3fxcyxarf.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3llqghlto.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3qxcujvof.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3krxocgxy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ccujdoss.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3muhilkrp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3sevdvthi.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3tgppiibr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3kceeduhj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3vknzxsaz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3uswymqcu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3dwvioibg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbyflybz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3ybpigqio.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3zlqubxfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3baoqugkj.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3jmwuhqoc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3sasbnzjm.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3uupobpcj.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3qxhkgpec.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3pmilpaiq.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3iufgiofb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3mfqoilfz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3lgmgqiww.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3hsyaolzk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3nqpdarlr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3thulrnas.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3isluavvn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3zlbhvjrz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3txiisphp.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ayfzyjfb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3xqfqhirk.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3hlqgyjnt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3hjknupop.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3otjnujzn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3tpmorcdo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3adkvocbe.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3wtsswyes.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rocqovsr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3lqroaxar.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3mptsumnu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zgnetzrd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3eohjjnsh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3meudxhox.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ymltobsl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3zhqqixuh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mbauagqm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yhbnvrtq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vxjipdqz.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rkokrxek.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vyiltdvk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ebsxyoso.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rwscfyyz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wpeoifdt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yyayiuev.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3gwxqabdl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3acigeeed.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3slfsklyh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fxsafhfm.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3fufvzzzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ingcsegh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3tkrgwspz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ithlilhi.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zctgikpz.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3snshpjtb.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3wkuuolqr.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3pdhtgugn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3eermqyhi.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wuflyivt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3cpgfyjua.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3tmpfiicx.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3evsrvexa.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3mgamwolb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3hiszlwnb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3idrwsocu.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rtglgtgz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cquwthrd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dlnutrjv.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ovpymfla.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3vgkblvfu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gcovnxey.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3oermopsi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3mjwhvril.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hfvdfuxn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ozrhfthl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vcpgzmuq.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tmevzmim.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ynuzkqio.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vobotrjn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tadrvyht.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3odnqtsdh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3sigbzuef.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3vrkflxpg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vxkdhzrk.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3osmdxody.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3mglxjmrj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3dauwfgeb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ixktfqkn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ebmshwep.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3tizgkcuu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3tkznjlji.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hwckvund.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xblflxuw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3oceqlyjk.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3epcswjlx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ctmjbiny.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tltochsk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jcydetmo.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3twtybguh.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qipdwepn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3oauhkomw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3hmkipboq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wvgoaglj.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3sdepubdu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3zlylptpi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3vrhrsxuw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3pmiyfmgm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lntkembk.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3ibfflpmn.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xwhchhbh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ffinqmoz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3stnemlwq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3tvvypdbx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kowvcjdf.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3cuvendhg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3fhpusxtk.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3nubpclfe.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vrehlskb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3lhywwkjb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3zwntdqle.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ygxrqhte.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gjurohxj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vvucxtar.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3bjfiyxmj.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tutkygtb.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jpcrprhd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bywfqoix.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3otrequbl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kbtosygr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3whypxeiv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3irpujsfp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3oxdylozd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3xfhjlpmw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nmjbdfxa.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jssuptew.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3etvwgutq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3nivjwnlc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3tfdwacqs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3aztsfnno.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nufbqpbn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3rsmsvnlg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3ugjqbmib.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3okjyfxmc.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3hosweftv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kndvtnph.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vbguhjxu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cnwmpvhi.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sfnwnktn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cltruqhh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3vbjjhegv.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dlkezqxr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ozoptkoe.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3jlyulacw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3sqahyifm.html


<!-- 参考信息 -->