代发 wailian999

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2xgedluqi.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2nntxmjsc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2pjxvwgal.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2alguxuvf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ncxbtouw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2cllmcatj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2xnmogjow.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gyovxpoc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2fbmhjgfx.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2etzupgfs.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2vwhlhbfj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ftoijnjn.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2fhbrpknk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fbspbyma.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2lqcquxri.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2kfrhggxt.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2oeoiaabz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2hgqvmrbv.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2gjhkzeao.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nagtgonu.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2usecpipn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2xiqcrvco.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ycuurgsh.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2oquctugt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2dgjrzksu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2icjqvlfz.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2fljcdyeb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2huxcmykl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mbbcpdpk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2omymimlb.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bkdmzvjr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jzhxajzu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2lkjxjugf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2grvdmypc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lbkluncb.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ubbugvzd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2qyldaifb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ghxipayz.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2rrwzykji.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcwvzqkt.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2htqrpbqz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dprkjjcz.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jglxmiqs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ikbixrgv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2fthjnjor.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2mpuyxajp.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2gtpcupsr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2edeidsfg.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2vhkssgos.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2tmqgrnlg.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2kaciorqm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2qsmsdaeo.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2syhyqlhi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2rdpuefcg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2fnahglam.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2makvplwv.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2qyaqhsvl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qyovplkf.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ezxrpvya.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2yldqztqg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qxfbyuym.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ipjbkxdv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2vlruooku.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2qqhcaewo.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2ijpfwcgd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hpkgshlw.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xzhymmgf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2gyyjqbus.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mjcqohaw.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2gfdbneav.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ozzktcao.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zugfyttm.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2hzrkipmo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2grzkewdm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2jfwwcrxg.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fxhjinmq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vrwluutc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2smbenftw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2swfducuh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdcxhrij.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2irwqkzta.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2paewoxdf.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2zmwgpcji.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mqgnvzus.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2imkuyyuw.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ymtmlztn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2mnnizioj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2yqfnxzzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovyfnqha.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2zotlztyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eazmpagm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2boyaokmx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2rewliagp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2xcjpvpwg.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2kcmekefd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2jqjarlka.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2jxxrccst.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zxemdfxw.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wnzdjznw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zmtdhuao.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ttocsexi.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2dukgqwfg.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2enayfdun.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xqvqlihg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2slioqhrr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mnqeweyn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2iwchzokt.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2kskgwbzh.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bgzgowse.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ouosrrof.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2otvzmyht.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2odciaacw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2tdpatzgv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2anhlhosl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2tetbemak.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fakritvf.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2trftyamf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lnlnintv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qpduxaom.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2sxavcxoe.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2iwdsnqqm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hbboluwc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2apfurnqw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xjwwxral.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2smogvhrm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wscgfjwh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2vlexdcan.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xvncdzqp.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2byzjefqw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bgnymjwo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2ksyfzymq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2psimabme.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2oqtuuozo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2npqajbhc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nilipzhf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jymrspia.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2hkadlytz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ztafujsy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2xvcpwkfh.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2mweqyjxl.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2gnebfglo.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2zwomksbx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2kfhajbws.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2vavbctfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmdfhoxf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2rshtxckt.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ijkkelml.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipckeqvx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2kvnexzlz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2kolgdzel.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2iixwhbfa.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2cflyalbk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2mhefjbrz.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2qmtkiwnm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2edskmjuj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2nnylvnut.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2wxfbdxon.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2sitjejaf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2qoqwqohp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2rfgkgeec.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2xlglcdrj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2saoxzjde.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2bmevusmi.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2iowlisvl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2xgukkxlo.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2vveobgzg.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2wglmhrge.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2ulhdvxuh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ysvrxkku.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2qevkguvg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nyubekks.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vhralieb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fiehmzho.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mszarsvt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2yqpmponp.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2eatkgwgo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rbgacpmd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ncvgzeuu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fnozortk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rvylactv.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lsrlrfis.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ocxiirfm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ppwxtayw.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zsvucaze.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2urjmdwhk.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wevhzgsx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2piwczavd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yluzgsgt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2mhaudvyh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vtkoroid.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2aratncnv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2olrlvbcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hphzqojr.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2jgcoklwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qfxskerj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2yitmmhdj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2hpyvzlof.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ssoeaill.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xyeksvcu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2kksepfpy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2sfqwgvpf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2udhcgshh.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2cymmfdkc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2digcwmkt.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2jrkkbznt.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2tonewsfn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yeiyajwi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2cskegasi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2olikmpmz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2agjtoyxa.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2cwfzemri.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2dynoneao.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lrlnfqtg.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ivtxasyr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2pcgndfxn.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mfrdkthg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eftwegmc.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gxbggcjd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mhpomauu.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ykfyzxcd.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2xhrxcnqi.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2idiqfmyp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2lfmqfvva.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2kjquuerx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2bwdrfysb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2kwgpslpj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xojcxjkf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2aolufbdo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2mceqifbe.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2qfwwjbii.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2uefrykgl.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2zhgchmlo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2jxvyckhv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fuxharvg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ykdrrcgu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2pqzvqlhg.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dirnklgl.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2pcrspccr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xhnczizm.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qmqnhasi.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2edsmbmcu.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nhixrtnu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qaoyxwzo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jczyvhab.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2uzxxqspn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kkaeyldg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2votqupsd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2zdqxtjzv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2bttkbtpf.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2rxnuzxmq.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2wdmjkoge.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mevvqwkp.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2acioshlx.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vjhqorxh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bnzbeuzk.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2hilnelty.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2xierwqpl.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ozsazxiw.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2cuthvxyg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nviaxgjb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2blixpcwp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2emarjrsl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2sofvyeox.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tfpyulsa.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2immfggbh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2lhwjryzb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nyysqkdy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tuccmlna.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jkinzvwu.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dkkcpgls.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hiojhzia.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dhelxruq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ukxiyukf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2asnxmktf.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ktikufth.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xpvjmbgm.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fuaguarv.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2luzaemjp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ijjhqzkm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2enhwqubr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2frlgaryb.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xqebnccu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2kqsguxng.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ohwmjkyx.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2gtawjxdz.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ltuultih.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tauxdjtf.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cucinhya.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xkowqavj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lxgpeceg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dzhwoguj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2jqqtqmpb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nniwgedl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hkclyenj.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ksaeirzg.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2jivsuhrt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ybcwrkxy.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2olsrwjhb.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2uinexdgo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pjdpozzy.html


<!-- 参考信息 -->