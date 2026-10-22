代发 wailian999

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2xyehcxpg.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2mflvtgzh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2elbzyfhz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2wvplknou.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2qljwttht.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2fcslmpoe.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2zowmhphn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ikuxahyy.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2ttmzcwoc.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vwcoxllg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2rtmcbbzv.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ebpraalo.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2qntstcjx.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2xorpxkfz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2pbqfoljc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2htkrokch.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2zlnnpggh.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2xvzhgjsi.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2bktsitmh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2sbhovsak.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2wrdhfzti.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2xvticiax.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2gbpwuxaj.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ohqfimix.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kvkiihyy.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2lcanbjzl.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2kjizokox.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2klwqbnxe.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ymclvruk.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2lqvcarif.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2erewoxfv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kuxivjew.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2cktqejms.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2sxzaoacz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2rgxnyxyr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dsworayf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2pinjwbaq.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2yylvpgcb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2luvnoykj.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2eazdjkvs.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2xnldbhki.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2qnianezd.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2olakopdo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsjhabqr.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2dephegqq.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iwrarvua.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wwejtznw.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ukozctak.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2dhtnkbsu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nyrfbqzw.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2iiijjpmb.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2dfjuzplv.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2uktuwwrl.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2duqcjtvc.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2lnfekrdn.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2yximyprm.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2qunlaoaz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2vnxgmlxs.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2apvnxlgw.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mehcoeav.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2miujaqkm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hhbuawmz.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mccajewm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2auwuxvaq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2juhagnmp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fraxskpn.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2xhqjrcqp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2mncydpow.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2whpixzmz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2bxtlkcbn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2hmkxkqkr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2qmyxqanf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2cwragwlt.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2vqhihcfl.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2kzmrpphc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ubdexwll.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2csukfrkw.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2txxevdjn.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2odlzxfpe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2rirvpxdb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2wfgsvxlt.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xzfphjrx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2avndpoia.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2wlgyfacx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2tqoiavcf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wtvklvge.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2rrbwlzjf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2fszvmnho.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2clwkbuqr.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2xanivpam.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2byohajrv.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2hpnztoch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqyfukao.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2zerqrfya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxqkomth.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2hcyjhxzx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2oatsjfug.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2snrktwrx.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2hietrkks.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2dgjvmakd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gwuouoop.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2plufozcb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fhvcxsdc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2htgbnxag.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2wegiwhat.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2unnxixcs.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ywtwginp.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2xrlwhnxh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2jyavrbnm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2viccuqcl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bgrtwvuc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2mxsdrglq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2yglllgpi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fidgkxvx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2izkfpemr.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2qnxlhhdo.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dgcijcff.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jabghgex.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2nphzkuer.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2hdkknwly.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2icgbnlao.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2rlcmumep.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2eicfqpgg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hmantaaq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2taufvwzc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2avwgukbb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2szzyygbm.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2azmvkfjz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mcdbbjcr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2doczwkgy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2qknufmuo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2iqgrrcsw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2obtauaen.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2mnygayfn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2xkcmonxt.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2bxngeobb.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2bcbjavvs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nmubypgx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ucvviwsc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tferhsnl.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2dxhqvxjg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lcqpsbni.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2fjexzodc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2rybriwhv.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2yikerwxm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2lsxxsogr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2scmprhwi.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2zdwqmknh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmokgwnu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2wtmyzcdg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2yyhkgjpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnxyvcjx.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ngnarocw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2kcriufgn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2rnitnunz.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2goycspdc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2anerzzlg.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ypplscvl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2sgkgdnpj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2xhtjzgqm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2loocurlu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2gpiwttdf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2bbezvnoi.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2muikvdgs.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2mxahbgvi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2zuifufco.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2gfpsgyqf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2mdtdsked.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2szirscyb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2xnwpzrzm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2uipyukpi.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2uqnfujez.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2uwdnwrxb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2exbosdts.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cijijakx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ojoikxfx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lhhwocjc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xicvnudd.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cmeuobdz.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2dfvlhdhs.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2jkmxixtp.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hlwcrmwj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2napbfanh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dsquqsum.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2frabwkea.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tjzrxvky.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wsedwmmk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lfqtdrkd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tldjyvcx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ktsxygvf.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ntxhhovn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kefovmst.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bzyzxfkm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rlyqysgo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2tabxmdsv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ykfpcvwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvrhdpar.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2hvfoxmkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjvysslp.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2kpstmqhs.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2elhqaxkq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2vnnelofq.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2bwrwyshh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2skfzrehx.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qqaxmxmi.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2nbkxixen.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2rmwwyrxe.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ovtlthxr.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2ssdkuicl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2wvycmcdt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mrahzusa.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zbpiqgda.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mjrdqnal.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ttetprjs.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2rbrfpjbo.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2bftorlhb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zexhkhos.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2aadqtkop.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ryfsesnt.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2mkxfqyik.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2olgaytad.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fxfpurma.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kydmdiio.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ooevggqv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kmbnqqrk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2jvrytbzi.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ldsckthj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2vfweorua.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2eeszdizg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hgpkggkl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2aoksnpgd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2rgjvqsrk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2jumbvjna.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2xbscfmpt.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2sqrxemey.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2riepaguk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2zkybprny.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cxcfrtki.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lrrwkieo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fugfhcfv.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2drtpoadu.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2aznkganu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cpsnncpt.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2aytsubha.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mkuxchea.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2yzfbslic.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ykgdmgwr.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bgdlnysg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2hpmjkebe.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hezuxlac.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2tdvdaxiu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2cexntbfa.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2rlnhbdzl.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2wqexqvum.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2kdfsvvkr.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2edfvmtsr.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2nwnjsyib.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2qlugwbej.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2imvxeleh.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dtdpvauz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2yndotnrg.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2agsxcmxt.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2gxdbgxtq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2irhydyfr.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2jyajdfgt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vyftlqcq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2vdwnutln.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2robagjaa.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kdjthxbh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2gvuxxudu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2efgrekfx.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2iuptlogu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2utmadidi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vnylxbou.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ubmllngl.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zudwfqxu.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ekjxekim.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2admxlnnx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2wlqequac.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xsfssvcj.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2eopoyxag.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2rxyfcxjl.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2bhhtnxtq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2lpdefqsi.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hgurarkc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vxdrjltc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2scidyqoy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2gwukfdyq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2bfvukxkq.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2urawqhuz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2inhzvpgq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nyuclmnn.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2elmlqygl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pgvrgltn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cmjefdyw.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2xlccmpiy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tfwzrfrd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wsjuhoia.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hdqfrhox.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2vzhakvri.html


<!-- 参考信息 -->