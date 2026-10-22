代发 wailian999

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2qnjzlgrf.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2tkiqwpni.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ovyhmpye.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2jlophnxu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2fshcifts.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2rpbbbvfu.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2psmeqzoj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2imcmjcbg.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2veucrcba.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2aupjecwh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ajwaooip.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ypcpcchl.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2pnyuvaah.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lpokbuvm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2aqipgevr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2fotldxao.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2yalgzzjv.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2bbywioxy.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jtswnnym.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2smvtsmem.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2wdrpsivr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2bemcfiip.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2hjzuvrlp.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ayhkflnr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2rszdibae.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2uyrujjvx.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2brjevdub.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yjlvwnfu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2prvsuryh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2reamnmba.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2wsfzxvko.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vweamhib.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2jpnjanxu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2kwigscfr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tcqjpbfk.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2arbvcrqb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2nkmhwzab.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kavsnmmk.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2sxrikpwk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wynimnwf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2vjneoeug.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qspxorgw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2erxjdbpo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2oozcatku.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ezusheaa.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2prihyamu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2omqditmz.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2vnzxgvgf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2whryxexw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2aywmvlri.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2vzniylai.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2lognpimd.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2awtkjnqb.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2eujlumsg.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ofarlqgp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2rsctsigp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2smmspsxy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2qqlrzbvy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ezzoaqku.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2xyscfiie.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uxazljnp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ckkraons.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gagphahv.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2zicpopwj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2gouojqyx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vbgdkjbn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2bwpmjsxd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xcdjojon.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2cfmnupmg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2yzixqwhl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2zezgdivj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uzalczpe.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2dnpdbnvz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2onsbncbh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2rmdshtdz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xkhikdlt.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cwvwkhky.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2amgpqhey.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2qwuypenx.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpvcspbi.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ugrvzqam.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ocahsqnq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2sywjrxks.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2efaemtvr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2dbbkpnix.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2mgeocqpe.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hcxfosvh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2vprdxoda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sicgztjk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2gluxzkwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sloopukz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2drkaiwhx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nlbmcxct.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2welzkaub.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2skyyitei.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ponpjygf.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kpbdmwyl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2sugdljuj.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2etjnkccb.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kihvtzji.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2imouqxsi.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2alrbnhmg.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2waapshop.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ipeciazg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2kgopcjsl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2lmgflxwf.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2wuuwbhzg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2cduqjjzt.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vcnbimum.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2avcbueej.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cfqjtkyi.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2penpucqx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2bittlwxi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wosklrcw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2dpvqnhvy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vkywyppw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2cwpmgjog.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2xpblofuc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2syebhfdo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2twwpbhwo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lkykpfsv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rfolwjuo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lwwykmen.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sytdbrlz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aanhaqou.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2guqijhyx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2keetyiim.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ezcfhbua.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2jibrmscf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2qxcghwrn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2neofdlql.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2oifqoama.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2xmkxuwrf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fhuvcxyr.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2souuckny.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xezxtvzu.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2verhtinn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2izubnyyx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2vtqgbttj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2zbsqpmez.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2echwjxkr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2bsirycvm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2soxquspu.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2mlzmzvgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bvqmmxbu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2crkzrscf.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2xpcgggzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxjummdn.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2fqtbyfno.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2hlrollnc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ukizvxdl.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2xlngocyo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2rcwjtckk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2llftqpby.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2hdouwufw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2ffumfbzs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ciqtgfcs.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2lqmfnftq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2gymxvfej.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ikairyeh.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2msgelqmv.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2hagnhirw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2tmwekavh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ogggkbbm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2msvxfjsx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2njaiwahg.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2zjjhsrdw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2avpshqzp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2omjgkotp.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2qngushsq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aloqyyas.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pplefytj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yowjdasp.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2pcbeyaui.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rvgrxuak.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2blqhnrho.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aclpdkqq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gompquir.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ccubulss.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2edaaajyz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ajwqbdvs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ovwyhbwm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dplmskgb.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fiyfyfcj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2elorihte.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jdaeqifk.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iyilvhvu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cbpposqt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xijcrnoh.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2bnddgjva.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2cbjtkitw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2aryuthuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zapjnwyh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2hcmxytxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffzdellp.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gjxrjfvj.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ctrxlcsg.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2lxahnlds.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2bzdrzksb.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2yfxrdnhv.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2bpexxekn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2icndtthu.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2kolrsoqn.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hjzbduvj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2jetlcgmp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2yipdymwx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mgjpmpdr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uhprsexy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2sglshnrl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pdyhupgf.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2gtsrcwxb.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2cdypmvfm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bsukemgd.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2jdcaqbvh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2lljicasu.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dufjfqdg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mkfjlosp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vnswfqrq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qfxcxozi.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2kdwgfolt.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jrqvfbkl.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2boyypfgl.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2stgufqpq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2pugnlszl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2glgznifu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2aquhzffe.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pkwnyabv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2bsblxqxs.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2ehrundii.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2yhhkuhca.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2geiqwlzi.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ckdvdszn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2hogrpzeu.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zcutpefg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wivwysrv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vumvivrh.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2oddqrsam.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cdehhdlu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qtzbgzsq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tvsvzomb.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xqlotiuu.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2zlfjvkqp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2dsxwerve.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ihzhaezd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2qqebdrdu.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kzxlltdp.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ejflyfju.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ztlkjpwn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ptvicngi.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wpkjpylm.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2afqppuhb.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2lvmanhmn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bybpqjwc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2zxuknvse.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qlffiwoi.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dbyjmrqs.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2juqcbyye.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2cxzxesoa.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2himgaxrp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uhfylypp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2gfrrdioj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rhtchvga.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2iuypbkfm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2axsvekoy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nfxurksh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ssuransq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2omwtccbl.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2strklrrb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ziwslpzq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qsuqadfl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jsxnkzoa.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ligglcsi.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pwuwlwkt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2nrhwlxbx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2dlpbrlai.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ehfyrwqp.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2mjcodtkj.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2dazwvfsb.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2jhazfgsq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2futbqwxq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vzvzijub.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tfkwyxdl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2mmudimaq.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2rbfybytx.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ctzozqrj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2stgivyta.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ircpsmkp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sebuuwmn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ohjbbmud.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ofbdmrwn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dnipyllb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2lfjcwamf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yrvjkqrd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2quleiwsp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hymgujel.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2rskqsztb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2tbikinjr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xfppkmdj.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lmoaudqq.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mkhevkec.html


<!-- 参考信息 -->