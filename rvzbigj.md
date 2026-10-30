代发 wailian999

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/grzdbizqf.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/guyemwqsg.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/glyqxkckt.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gdzaztskb.sHtML

[U77] PHP：模板渲染
来源：http://3g.zdbjq.cn/Article/details/ghftmldjy.sHtML

composer require twig/twig
来源：http://mobile.hesvh.cn/Article/details/gsqbbyvkh.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gmgkpseew.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gbxwasfbr.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gqgulmyzu.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.hesvh.cn/Article/details/geqjhnnsg.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fehbvm.com/Article/details/gknrydyto.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.hesvh.cn/Article/details/gkwjhmcjw.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/gjfllpxoh.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gypxntatp.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.zdbjq.cn/Article/details/gjahcdwml.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.hesvh.cn/Article/details/gobffvzyh.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.fehbvm.com/Article/details/gqqfwjvxl.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gvqspefoy.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gatptnprf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.m.share.zdbjq.cn/Article/details/gmgxjlila.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gduhwdzdg.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/goppleuay.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gzvrnqxrn.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/gryrtinih.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gufcogtej.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/gqpopkxaj.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gxzjkdgti.sHtML

{ ...a, ...b }
来源：http://3g.fehbvm.com/Article/details/geijvxbsc.sHtML

[U89] JS：数组去重
来源：http://www.m.share.hesvh.cn/Article/details/gpiqvitcn.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gahzrjubn.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gbzpkncbv.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/glixfilop.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/ghvgsuxoh.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/goyfbymyu.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/glibrmjyd.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gymldpfre.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gsqrpfqyn.sHtML

`共 ${n} 条`
来源：http://www.share.hesvh.cn/Article/details/gxmngrddo.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gedyivlxn.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gijteuonz.sHtML

[U95] JS：Promise 包装
来源：http://mobile.fehbvm.com/Article/details/gxkqreuoy.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/goqdpbzds.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gumlltsxp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gghvtlprg.sHtML

[U97] JS：并发请求
来源：http://blog.fehbvm.com/Article/details/glpljuiyg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gvbqgumit.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/glaglvqsk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.fehbvm.com/Article/details/gfevpetoe.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gzhbqyxft.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gtvyzbnny.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/guujgsgpf.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gpavwdnzc.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/ghszwrayo.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/ggbfdqrci.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gwliyombp.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.hesvh.cn/Article/details/giovpxhnu.sHtML

[U103] JS：定时器
来源：http://m.share.fehbvm.com/Article/details/gflhodpnf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gpeouwcly.sHtML

[U104] JS：防抖
来源：http://baike.hesvh.cn/Article/details/gtrmplpez.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gvlkuvajs.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gkbajwbkp.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gzdizcntm.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gauyxaklb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gcrapyfhe.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gsosqclzo.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.fehbvm.com/Article/details/gdtxhrxjt.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/gqlrybpez.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gqepffofc.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/ggrdwknkl.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gcvqohdvs.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gdijaandu.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gqvjkbebz.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gfivhqlwz.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gkqetsueo.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gvmtmrkny.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gpsjkrvnq.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/gqgvptuml.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghqtbvybw.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/gibqqsvsm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gzfbcfmqi.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gpeimzgdl.sHtML

crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gdbhfiicj.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gyqupptyc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/gsjaycpap.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gweqhmpvk.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gwcswqkaq.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gnytfintd.sHtML

npm i -D vite;  npx vite
来源：http://blog.zdbjq.cn/Article/details/grsaxbgdm.sHtML

[U119] JS：生产构建
来源：http://3g.fehbvm.com/Article/details/gdkbzxegk.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gbvwpqyjp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.hesvh.cn/Article/details/gepqpogbf.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gbygdqajp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghpgovsuy.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/gevdrqmyr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/geeeqwlqd.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/grytsqwel.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/ggfjzczxc.sHtML

PHP ............ 252
来源：http://mobile.zdbjq.cn/Article/details/ghwudeewq.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gfbapbqhy.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gvuqrdkuc.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gvdybkawv.sHtML

Go ............. 212
来源：http://www.share.fehbvm.com/Article/details/gxlcrzkqt.sHtML

Ruby ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gxuevmocl.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gvqnxlhph.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/glcnzsyfz.sHtML

C++ ............ 30
来源：http://wap.hesvh.cn/Article/details/ggermowpl.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gydgbjbnz.sHtML

Bash ........... 80
来源：http://www.m.share.fehbvm.com/Article/details/gxvvhcmbg.sHtML

Kotlin ......... 15
来源：http://3g.fehbvm.com/Article/details/gpobrxtwt.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gniwdtjqt.sHtML

Lua ............ 10
来源：http://read.share.fehbvm.com/Article/details/gdnhucubp.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gienrfiyf.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gynkugpxp.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gqzfzimtc.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gwqiiutew.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/guiglepxj.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/ghnnmfapj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gfvusunmf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gawqbgurd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gnwkhnmkz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gbfqxpdqw.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gycncwnas.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/ggnihkqyt.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/grogjomuc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gndfwecgt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gsedsdsko.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gkdczrxoz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gsjwhvgnc.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gdmrjcxdy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gsvptwcej.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gjsdbiiyv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gdqrokunn.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gmxefzilp.sHtML

R Bash 专题                             80
来源：http://www.share.zdbjq.cn/Article/details/gkddmmhht.sHtML

S C / C++ 专题                          60
来源：http://read.share.zdbjq.cn/Article/details/gsrpqkxif.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/glbdljdco.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/grxfesyel.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gsqrmlvkc.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gifnwhmng.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/geucnfqtl.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gcpgwhaew.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gvuhgsgwi.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gnyoqfzxi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gsnutqtfi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/geglmqnro.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/gmvqytdhm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/ghmyyityo.sHtML

—— 文件结束 ——
来源：http://www.blog.fehbvm.com/Article/details/glxtcoxoh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giosyrrfl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gtmrsksis.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gcbgawpis.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gurhajivb.sHtML

【收录内容】
来源：http://read.share.hesvh.cn/Article/details/gsrqkrhae.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/genpuhfln.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fehbvm.com/Article/details/gxkbrwwmu.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gmdolzsjc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gwfwfewce.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gsjjasemb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gpnfgzdwm.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.zdbjq.cn/Article/details/gvlzurngs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gtolklaqm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gptcjzshi.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.hesvh.cn/Article/details/gsjjqpnxy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/gsoxizsnx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/grgjbtwth.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gjrsxkxch.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gubsqgkmf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gxhvpfohs.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.hesvh.cn/Article/details/gokfslqwx.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.zdbjq.cn/Article/details/geyipqlpn.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gryoghrmw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/ggmthisfp.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gzqgskjld.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gmgshbcnz.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gpcewvlwz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gukdpqzkf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gyrdyhfsr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gimiemeit.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gcbaeccqo.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gotfxtwxb.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gczndtfse.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gwubnktkp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gzeisvnuk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdmwxhbhp.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/gxdusoznk.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gmetlmazu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmoyapzap.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/goyowubxv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/glplxwada.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gxcppheob.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gfmpjiooz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.fehbvm.com/Article/details/gfpsziwjs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gijbprkiv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gevduqrfx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gozewcvgf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.zdbjq.cn/Article/details/gqjtvymxh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxnqbmnbp.sHtML

A. 基础语法与类型
来源：http://baike.hesvh.cn/Article/details/gjsopqbeb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gffkikcby.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/gveaodmwu.sHtML

Py:   print("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gwcthkzgf.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/gqhtflmty.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/goctdrwea.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gkqevgbsp.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gorujfyvx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gkvxrkuav.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gcsipjoxt.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gtoqxoawo.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gvmzrwwcj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gpplygsll.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gepovhekz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gscnvejhz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/ghdivlkah.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gefpqpmzh.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.zdbjq.cn/Article/details/gqytugotg.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/ggzyjfpvs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gmlfyfjis.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gywvctygy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/gwdoywpsa.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gnlutezcq.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/glqtjqtcg.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/grlutqshc.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gsrdwqwee.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/ghrxrfhrx.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gilcdsdmf.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/grwhyxpem.sHtML

[A04] 判断变量类型
来源：http://blog.hesvh.cn/Article/details/gpkutkkad.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/gmvzcqbqo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.hesvh.cn/Article/details/gruekeoiw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gqhdmpeww.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gmzgvdcrv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.hesvh.cn/Article/details/gtsswpmvs.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.zdbjq.cn/Article/details/gpoiwmlzu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gvqszbdja.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gfesldolx.sHtML

[A05] 整数除法与取模
来源：http://www.m.share.zdbjq.cn/Article/details/gmduahvcp.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/ghiudaxfv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/grtjcchnn.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gqnscixkl.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/goaqzzdmf.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gnuzkpjix.sHtML

Go:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gvibtjtgj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gorlighli.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/glqjrbuqz.sHtML

[A06] 字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/ghjsxiuuc.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.fehbvm.com/Article/details/gvjuepxit.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/gcfphnasr.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gseabbknk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gkpnefbdr.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/gntoqtble.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.zdbjq.cn/Article/details/gmfhrdrdw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.share.fehbvm.com/Article/details/gbqzeaakn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/gyhddqmer.sHtML

[A07] 数字转字符串
来源：http://read.share.fehbvm.com/Article/details/gawnjcfec.sHtML

Py:   str(42)
来源：http://read.share.fehbvm.com/Article/details/gdgzolrci.sHtML

PHP:  (string) 42; strval(42)
来源：http://read.share.fehbvm.com/Article/details/gxfxmgvpn.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.zdbjq.cn/Article/details/gcqnkonyy.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/gglrfpwvv.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/goddwassa.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.zdbjq.cn/Article/details/gczclujre.sHtML

Ruby: 42.to_s
来源：http://baike.hesvh.cn/Article/details/gxrjlhpcq.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/gfpekufby.sHtML

[A08] 取整与四舍五入
来源：http://m.share.hesvh.cn/Article/details/gkysjtezd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gbaasjrka.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.fehbvm.com/Article/details/gkhgrjuhg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/guesfaiku.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.zdbjq.cn/Article/details/gqktrnxip.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/glpqwzhnd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gwifjbaud.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.zdbjq.cn/Article/details/gvxgkypjd.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/ggmwapbnq.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/gixytpcmj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/ggciahbqq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/grfahkdmn.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gwhlbbboe.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://wap.hesvh.cn/Article/details/gnghrnsyg.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gvirtpgmt.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/gukvdstte.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fehbvm.com/Article/details/gbfmeldgk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrfpbquf.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/guwovufov.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.hesvh.cn/Article/details/gbthgngwa.sHtML

PHP:  random_int(1, 100);
来源：http://3g.hesvh.cn/Article/details/gqlsjswtz.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/ggghtmucd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gnatyxswp.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fehbvm.com/Article/details/gtnzthrki.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.zdbjq.cn/Article/details/gzpgacdkw.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/guahgpnyy.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/grqlowcyz.sHtML

[A11] 条件表达式（三元）
来源：http://blog.zdbjq.cn/Article/details/graprzkqe.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.zdbjq.cn/Article/details/gzxuppqtc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gprzayocl.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gdkvwuvjb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/gpfjylvkp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gjhniafqc.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.hesvh.cn/Article/details/gqyhcqdji.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gxhvjeksh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gqvredutg.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.hesvh.cn/Article/details/gbrpnzwcj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.zdbjq.cn/Article/details/gthmqybka.sHtML


<!-- 参考信息 -->