代发 wailian999

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjnvphcp.sHtML

composer require twig/twig
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojbevjyf.sHtML

[U78] PHP：单元测试
来源：http://m.share.fanxiaobao.xyz/Article/details/gksrmwzvm.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnxfsaso.sHtML

[U79] PHP：静态分析
来源：http://wap.fanxiaobao.xyz/Article/details/gzkdxwytm.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdektqzsh.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.fanxiaobao.xyz/Article/details/goqbhzslb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fanxiaobao.xyz/Article/details/gohuztcqs.sHtML

[U81] JS：初始化项目
来源：http://read.share.fanxiaobao.xyz/Article/details/ghumshhuu.sHtML

npm init -y;  npm i express
来源：http://blog.fanxiaobao.xyz/Article/details/ggjmyzbxk.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzhfgizk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.fanxiaobao.xyz/Article/details/gfskpjsur.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiuyohbi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gugxcpxdr.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fanxiaobao.xyz/Article/details/guddbppqd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fanxiaobao.xyz/Article/details/glxouqldt.sHtML

[U85] JS：可选链
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkgyszvv.sHtML

a?.b?.c
来源：http://blog.fanxiaobao.xyz/Article/details/gaosnexny.sHtML

[U86] JS：空值合并
来源：http://wap.fanxiaobao.xyz/Article/details/giagxrtbf.sHtML

a ?? b
来源：http://m.share.fanxiaobao.xyz/Article/details/gnskszsjo.sHtML

[U87] JS：解构默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gyxztytfl.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvozgnec.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gujrrovor.sHtML

{ ...a, ...b }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyarasdx.sHtML

[U89] JS：数组去重
来源：http://blog.fanxiaobao.xyz/Article/details/gpfevyoph.sHtML

[...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrltxakg.sHtML

[U90] JS：数字数组排序
来源：http://blog.fanxiaobao.xyz/Article/details/gakyxmbaf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/greufcxqu.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeesyyyp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepaufsxm.sHtML

[U92] JS：深拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gginmcmfx.sHtML

structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gmuncfkie.sHtML

[U93] JS：模板字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsmngqum.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gpogxktvr.sHtML

[U94] JS：箭头函数
来源：http://baike.fanxiaobao.xyz/Article/details/gesxuvkzy.sHtML

const double = x => x * 2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbknvbrpr.sHtML

[U95] JS：Promise 包装
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqqmlder.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijbmcaal.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fanxiaobao.xyz/Article/details/givysgmvb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbzafeqo.sHtML

[U97] JS：并发请求
来源：http://wap.fanxiaobao.xyz/Article/details/gduvhzryg.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gugmhbclv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gskiqbslr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gxwfalppk.sHtML

[U99] JS：事件监听
来源：http://blog.fanxiaobao.xyz/Article/details/gkizvkpks.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipkyapng.sHtML

[U100] JS：DOM 查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzpjnhht.sHtML

document.querySelector(".item")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhbjkvtr.sHtML

[U101] JS：classList 操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gzunitjzl.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geplshklc.sHtML

[U102] JS：本地存储
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxzisfjo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.fanxiaobao.xyz/Article/details/gexnuyojc.sHtML

[U103] JS：定时器
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxglyuzu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjqerjwr.sHtML

[U104] JS：防抖
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbesgrsy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fanxiaobao.xyz/Article/details/gqqkpcnkq.sHtML

[U105] JS：节流
来源：http://wap.fanxiaobao.xyz/Article/details/gqncwgyap.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhtcvnev.sHtML

[U106] JS：日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gynowadno.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeeiklru.sHtML

[U107] JS：数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gmcnbugyg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvtqbdke.sHtML

[U108] JS：随机整数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbfdavtr.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fanxiaobao.xyz/Article/details/ghvfwdqop.sHtML

[U109] JS：数组分组
来源：http://3g.fanxiaobao.xyz/Article/details/gisulqadj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gtbcookvl.sHtML

[U110] JS：数组分块
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzgnwzyp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fanxiaobao.xyz/Article/details/gxixzryht.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgtqcphy.sHtML

new Map(Object.entries(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gxrbmlcrj.sHtML

[U112] JS：字符串补位
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkgjvqjx.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gbbtqvsly.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gjyjwnmch.sHtML

s.replaceAll("a", "b")
来源：http://wap.fanxiaobao.xyz/Article/details/gnbppvwqq.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fanxiaobao.xyz/Article/details/gunfxtmsr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrrsuwly.sHtML

[U115] JS：生成 UUID
来源：http://read.share.fanxiaobao.xyz/Article/details/gczykgils.sHtML

crypto.randomUUID()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcsmkcyx.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gyvwsncii.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gazbuwczh.sHtML

[U117] JS：单元测试
来源：http://baike.fanxiaobao.xyz/Article/details/gcxpejwrj.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fanxiaobao.xyz/Article/details/gyacpdbnd.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwbtamns.sHtML

npm i -D vite;  npx vite
来源：http://3g.fanxiaobao.xyz/Article/details/goihowqnf.sHtML

[U119] JS：生产构建
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmcpkiqi.sHtML

npx vite build
来源：http://blog.fanxiaobao.xyz/Article/details/gwdqwhsig.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplvohbnh.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpobbreu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiinifkv.sHtML

统计汇总
来源：http://blog.fanxiaobao.xyz/Article/details/gggehzyuf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfldtwynx.sHtML

按语言统计（条）：
来源：http://blog.fanxiaobao.xyz/Article/details/gcnrlrnrg.sHtML

Python ......... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/goyymdzcz.sHtML

PHP ............ 252
来源：http://www.share.fanxiaobao.xyz/Article/details/glymynjha.sHtML

JavaScript ..... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gywjuzdxv.sHtML

TypeScript ..... 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxyulvnv.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaoqtyqd.sHtML

Go ............. 212
来源：http://blog.fanxiaobao.xyz/Article/details/gvqpwkubc.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/guwgfxuss.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gohgjczir.sHtML

C .............. 30
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwntjxva.sHtML

C++ ............ 30
来源：http://baike.fanxiaobao.xyz/Article/details/gaxeiydeu.sHtML

SQL ............ 90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidoxgxsl.sHtML

Bash ........... 80
来源：http://www.share.fanxiaobao.xyz/Article/details/gqasaqpuq.sHtML

Kotlin ......... 15
来源：http://blog.fanxiaobao.xyz/Article/details/grpwbyghh.sHtML

Swift .......... 15
来源：http://3g.fanxiaobao.xyz/Article/details/gzwuassnr.sHtML

Lua ............ 10
来源：http://baike.fanxiaobao.xyz/Article/details/gbgarwyix.sHtML

Perl ........... 10
来源：http://blog.fanxiaobao.xyz/Article/details/gszkhpiqw.sHtML

Scala .......... 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gscgrvjte.sHtML

------------------------------------
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfkzbwqi.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxozsnog.sHtML

按章节统计：
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhhllgsw.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/gwryixydb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwxausml.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fanxiaobao.xyz/Article/details/gvvmxrhfk.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzemaksz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzgpxkue.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkylhmel.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcvkjzld.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.fanxiaobao.xyz/Article/details/gnsnunhvn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gennocnur.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gweyjpmze.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwamfnmy.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gtkkbpwny.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdnnzznd.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmwgxhgc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fanxiaobao.xyz/Article/details/gokccqchs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrugqpjo.sHtML

Q SQL 专题                              90
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glulzsxro.sHtML

R Bash 专题                             80
来源：http://3g.fanxiaobao.xyz/Article/details/gtlgxsrqi.sHtML

S C / C++ 专题                          60
来源：http://www.share.fanxiaobao.xyz/Article/details/gosjctojx.sHtML

T 其他语言补充                          60
来源：http://wap.fanxiaobao.xyz/Article/details/ggjadausq.sHtML

U 高频实用片段                         120
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjlymcvs.sHtML

------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gbwjxzrlt.sHtML

合计                                  2106 条
来源：http://baike.fanxiaobao.xyz/Article/details/gjhnklotf.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gpwtqpmdy.sHtML

使用提醒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakjudvsh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisppumev.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscgecbpi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fanxiaobao.xyz/Article/details/gesdnmycq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fanxiaobao.xyz/Article/details/goffokwor.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiojikdo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsupepgc.sHtML

—— 文件结束 ——
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdletazyr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvipmrjjx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fanxiaobao.xyz/Article/details/gfxlxourh.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fanxiaobao.xyz/Article/details/gxsyuxzhk.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjtpdvnv.sHtML

【收录内容】
来源：http://blog.fanxiaobao.xyz/Article/details/gxqvdifss.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fanxiaobao.xyz/Article/details/gypdjgsyz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fanxiaobao.xyz/Article/details/gcqhgdlcj.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gwinpbsnu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.fanxiaobao.xyz/Article/details/gydahvloa.sHtML

【使用说明】
来源：http://3g.fanxiaobao.xyz/Article/details/gwkcsljrb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fanxiaobao.xyz/Article/details/gktyxofla.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/glaoiwoqx.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlpjvzhc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.fanxiaobao.xyz/Article/details/gkquqzeej.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gunltblzj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikkjxizm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fanxiaobao.xyz/Article/details/guxxmlinn.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fanxiaobao.xyz/Article/details/gklpeuqfu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.fanxiaobao.xyz/Article/details/ggftgtvac.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdwrsakx.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fanxiaobao.xyz/Article/details/gppukuvrr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fanxiaobao.xyz/Article/details/gsnvhopib.sHtML

【文件统计】
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpixrssin.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfwoubww.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoufdeyx.sHtML

目  录
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoijynno.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/ggipxolpc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/geesyohoj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwluernyf.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gabligtui.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fanxiaobao.xyz/Article/details/golodfycs.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gqcxijkny.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxucgkqei.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/grdqbxucd.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gzxlcqtsx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/grwrbhnkh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gwsljlwwj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gatzqwjqu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gpzwxwxne.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnqboshl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gxhtuivgm.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grtzsedgs.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gyscsctoe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfecrdyea.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftqkzadl.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifjdhnqn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjetiwsn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gbputtglh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guozyoswn.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/gfkovviqa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevwaosiz.sHtML

[A01] Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/ggyplgkkm.sHtML

Py:   print("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdhqiood.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gckvzhwuj.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjoudsfo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgojspkr.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giivfdmka.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fanxiaobao.xyz/Article/details/gqjeggehq.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaawtogq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.fanxiaobao.xyz/Article/details/gydoxlsuz.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnvxifim.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fanxiaobao.xyz/Article/details/gdeosxqhk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gevglentw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghrbyrarp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggomsvdrl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaudnpbp.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fanxiaobao.xyz/Article/details/gotnjcpol.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoufkxhv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gxorjcojq.sHtML

[A03] 常量定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcfyrkaw.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fanxiaobao.xyz/Article/details/gpckzpejn.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzjanlyg.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gbdiebiws.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gxtdewszx.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gmgmgjrve.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoylrhex.sHtML

Ruby: PI = 3.14159
来源：http://3g.fanxiaobao.xyz/Article/details/gbloaamks.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/ghirfnzuj.sHtML

[A04] 判断变量类型
来源：http://blog.fanxiaobao.xyz/Article/details/gpnfmmzbp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fanxiaobao.xyz/Article/details/gnzyhquim.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtieudwho.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkphovsz.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzlycthk.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhuzxkmx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduinmdqq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjcwfapi.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlscfege.sHtML

[A05] 整数除法与取模
来源：http://3g.fanxiaobao.xyz/Article/details/gjjyobuet.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://wap.fanxiaobao.xyz/Article/details/gtezaruxo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxqyebmny.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/gkrztivkz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiozcbkk.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gfyhmknla.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/govcwwkqd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtnzemnj.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/getugvlky.sHtML

[A06] 字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/glgvqzgzs.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycfyqoov.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.fanxiaobao.xyz/Article/details/gltqoaesz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyguvpbzd.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbnhcczx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.fanxiaobao.xyz/Article/details/gnfguyymq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/glkeoputo.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.fanxiaobao.xyz/Article/details/gnckoodba.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggewcasjj.sHtML

[A07] 数字转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gfsyccunv.sHtML

Py:   str(42)
来源：http://baike.fanxiaobao.xyz/Article/details/gbhxjbwmu.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fanxiaobao.xyz/Article/details/gekizxcwz.sHtML

JS:   String(42); (42).toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrpvulof.sHtML

TS:   String(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkkbbpbj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxadyuuro.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fanxiaobao.xyz/Article/details/ghzzygmxd.sHtML

Ruby: 42.to_s
来源：http://mobile.fanxiaobao.xyz/Article/details/gedmtngez.sHtML

C#:   42.ToString()
来源：http://blog.fanxiaobao.xyz/Article/details/gvnwapmsr.sHtML

[A08] 取整与四舍五入
来源：http://3g.fanxiaobao.xyz/Article/details/gosebjkqz.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpfygvms.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjhchgkj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/guvbvcyuy.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fanxiaobao.xyz/Article/details/gfghrbhtp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikdayujo.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmjeadnc.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbvjakde.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gcecwolwq.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbamcfmn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gkffeiuwh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfuplgxj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gljuamekt.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gsujarpbn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gxoltbqvx.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.fanxiaobao.xyz/Article/details/gfmlusmyy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fanxiaobao.xyz/Article/details/gawyaqhox.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzctjtlmb.sHtML

[A10] 生成随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gjkvosaiq.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggebrfwzp.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fanxiaobao.xyz/Article/details/gsphbjpmb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gldsfcwwx.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqhyyvdr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fanxiaobao.xyz/Article/details/glhvdkqmc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsomivdo.sHtML

Ruby: rand(1..100)
来源：http://read.share.fanxiaobao.xyz/Article/details/ganufdibs.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fanxiaobao.xyz/Article/details/gdetcpngv.sHtML

[A11] 条件表达式（三元）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffobmwmi.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybtxsvus.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gtelltygx.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fanxiaobao.xyz/Article/details/gnbuzxhfi.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gnqnvxdoe.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyupffnv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.fanxiaobao.xyz/Article/details/gkcpgthqw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvproevzd.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkstcmtno.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gwwapblgp.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiyeaufj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvesdrkva.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwlnrgoy.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.fanxiaobao.xyz/Article/details/gbzsxnnjw.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://blog.fanxiaobao.xyz/Article/details/ggeombzid.sHtML


<!-- 参考信息 -->