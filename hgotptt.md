代发 wailian999

[U75] PHP：依赖注入
来源：http://read.share.fanxiaobao.xyz/Article/details/gojubxoxg.sHtML

composer require psr/container
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtqivckz.sHtML

[U76] PHP：简单路由
来源：http://baike.fanxiaobao.xyz/Article/details/gnirwaywb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.fanxiaobao.xyz/Article/details/genvfnwtk.sHtML

[U77] PHP：模板渲染
来源：http://www.share.fanxiaobao.xyz/Article/details/gfistufro.sHtML

composer require twig/twig
来源：http://m.share.fanxiaobao.xyz/Article/details/gngporupo.sHtML

[U78] PHP：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/glcozitxt.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fanxiaobao.xyz/Article/details/gcxrxmmwl.sHtML

[U79] PHP：静态分析
来源：http://baike.fanxiaobao.xyz/Article/details/gohzvsctp.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fanxiaobao.xyz/Article/details/ghwzabqtj.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fanxiaobao.xyz/Article/details/gxlwfdmte.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fanxiaobao.xyz/Article/details/gffgmwenv.sHtML

[U81] JS：初始化项目
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwnrgqix.sHtML

npm init -y;  npm i express
来源：http://wap.fanxiaobao.xyz/Article/details/gauhcmdgs.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpwsubcm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxwrgmwx.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnqyezgz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/getfvcaaq.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fanxiaobao.xyz/Article/details/gmghfxoij.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqccnxas.sHtML

[U85] JS：可选链
来源：http://blog.fanxiaobao.xyz/Article/details/gthkvpelt.sHtML

a?.b?.c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqwqojwr.sHtML

[U86] JS：空值合并
来源：http://3g.fanxiaobao.xyz/Article/details/gwfcpljvc.sHtML

a ?? b
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzcrbfry.sHtML

[U87] JS：解构默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gngkbpzmt.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fanxiaobao.xyz/Article/details/gicxvjqff.sHtML

[U88] JS：对象展开合并
来源：http://wap.fanxiaobao.xyz/Article/details/gajipwcds.sHtML

{ ...a, ...b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpzmscoe.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/gzddgwsfh.sHtML

[...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/guurvkium.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgbjcgxy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.fanxiaobao.xyz/Article/details/grhtkzljx.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywcgxzdq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiqhrhqd.sHtML

[U92] JS：深拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiovnxma.sHtML

structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gwrvhkkie.sHtML

[U93] JS：模板字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gsimajbwf.sHtML

`共 ${n} 条`
来源：http://read.share.fanxiaobao.xyz/Article/details/gtflmvuxp.sHtML

[U94] JS：箭头函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gaonzrspi.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsofsviei.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzfflqqf.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/grzexllnv.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.fanxiaobao.xyz/Article/details/guccxkuxv.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fanxiaobao.xyz/Article/details/gnehejdur.sHtML

[U97] JS：并发请求
来源：http://mobile.fanxiaobao.xyz/Article/details/gbppinlbe.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrgedsye.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gjbqkycks.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbixstmiu.sHtML

[U99] JS：事件监听
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiqpnvbk.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gnllqozgu.sHtML

[U100] JS：DOM 查询
来源：http://blog.fanxiaobao.xyz/Article/details/gzturqlwe.sHtML

document.querySelector(".item")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwnodtvk.sHtML

[U101] JS：classList 操作
来源：http://wap.fanxiaobao.xyz/Article/details/goplyyucd.sHtML

el.classList.toggle("active")
来源：http://3g.fanxiaobao.xyz/Article/details/grnhnyzln.sHtML

[U102] JS：本地存储
来源：http://3g.fanxiaobao.xyz/Article/details/ghxqxcusr.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fanxiaobao.xyz/Article/details/gzxtagalv.sHtML

[U103] JS：定时器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxprgmcwk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkacjkfd.sHtML

[U104] JS：防抖
来源：http://www.blog.fanxiaobao.xyz/Article/details/golwjbxvf.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fanxiaobao.xyz/Article/details/gdnzesevv.sHtML

[U105] JS：节流
来源：http://read.share.fanxiaobao.xyz/Article/details/galvdphdq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fanxiaobao.xyz/Article/details/gvegxnogd.sHtML

[U106] JS：日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhbopxlu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnykqfps.sHtML

[U107] JS：数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/ggmiotzib.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gzkxnjppz.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqpgtxlu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjukwhwn.sHtML

[U109] JS：数组分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnxenrcz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gkgethjid.sHtML

[U110] JS：数组分块
来源：http://baike.fanxiaobao.xyz/Article/details/gbgdzzkag.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fanxiaobao.xyz/Article/details/gsllurkfe.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/grqiyfzyk.sHtML

new Map(Object.entries(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/gknryyrnr.sHtML

[U112] JS：字符串补位
来源：http://baike.fanxiaobao.xyz/Article/details/gaspmzzzl.sHtML

"7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/gzbpwohvq.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasqlvwwd.sHtML

s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gvvsoukla.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gdchraicn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgizftzv.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmrgctzh.sHtML

crypto.randomUUID()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmkdlahp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.fanxiaobao.xyz/Article/details/gdjyckzqk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbbehlyh.sHtML

[U117] JS：单元测试
来源：http://mobile.fanxiaobao.xyz/Article/details/gaulwzksq.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.fanxiaobao.xyz/Article/details/grkdjhqbb.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gzmzqnucg.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrdlhcbo.sHtML

[U119] JS：生产构建
来源：http://blog.fanxiaobao.xyz/Article/details/gyyibufrk.sHtML

npx vite build
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkywmjqe.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdartdzo.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdjhuxlm.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganjekunh.sHtML

统计汇总
来源：http://m.share.fanxiaobao.xyz/Article/details/gkymkievj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqphkagxd.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gejwcdwab.sHtML

Python ......... 252
来源：http://blog.fanxiaobao.xyz/Article/details/gpbsaiblw.sHtML

PHP ............ 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloulfhyk.sHtML

JavaScript ..... 252
来源：http://www.share.fanxiaobao.xyz/Article/details/grztqjiku.sHtML

TypeScript ..... 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpqpfhij.sHtML

Java ........... 212
来源：http://3g.fanxiaobao.xyz/Article/details/gmkppseoy.sHtML

Go ............. 212
来源：http://read.share.fanxiaobao.xyz/Article/details/gadjeektk.sHtML

Ruby ........... 212
来源：http://baike.fanxiaobao.xyz/Article/details/gapjanklu.sHtML

C# ............. 212
来源：http://wap.fanxiaobao.xyz/Article/details/gkjseqlkp.sHtML

C .............. 30
来源：http://baike.fanxiaobao.xyz/Article/details/gictjqazf.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdnmoujf.sHtML

SQL ............ 90
来源：http://wap.fanxiaobao.xyz/Article/details/gcbywntao.sHtML

Bash ........... 80
来源：http://read.share.fanxiaobao.xyz/Article/details/glzwgtjul.sHtML

Kotlin ......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gjgrtlovf.sHtML

Swift .......... 15
来源：http://wap.fanxiaobao.xyz/Article/details/gjtswnrgt.sHtML

Lua ............ 10
来源：http://3g.fanxiaobao.xyz/Article/details/gsxrmentj.sHtML

Perl ........... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzhccmdc.sHtML

Scala .......... 10
来源：http://wap.fanxiaobao.xyz/Article/details/gdghnjyfg.sHtML

------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/ghephapxy.sHtML

合计 ........... 2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvxgmydi.sHtML

按章节统计：
来源：http://3g.fanxiaobao.xyz/Article/details/grzikrqki.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.fanxiaobao.xyz/Article/details/gmrkykgat.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fanxiaobao.xyz/Article/details/gmavfkpva.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhtirgwm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fanxiaobao.xyz/Article/details/gbmbvoenh.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggobcrdnh.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfsdxeve.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.fanxiaobao.xyz/Article/details/gtvbbgmvm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwyjgyhn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxjyjtax.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fanxiaobao.xyz/Article/details/gfjkdmzmo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrrfuuxw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.fanxiaobao.xyz/Article/details/gzudbgnwv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnouxpcr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/goclhfihw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fanxiaobao.xyz/Article/details/ghxwrahzs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbfppfcb.sHtML

Q SQL 专题                              90
来源：http://blog.fanxiaobao.xyz/Article/details/gdfanlfqa.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqvthkpu.sHtML

S C / C++ 专题                          60
来源：http://wap.fanxiaobao.xyz/Article/details/gubyxmrkt.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaivajqp.sHtML

U 高频实用片段                         120
来源：http://wap.fanxiaobao.xyz/Article/details/gkjigtxng.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbuplgph.sHtML

合计                                  2106 条
来源：http://blog.fanxiaobao.xyz/Article/details/gdoihjsoj.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gjzotfpca.sHtML

使用提醒
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcgmdypr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrwfsxoy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlgfgdmv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwzxtvph.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fanxiaobao.xyz/Article/details/gsdzdnduu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fanxiaobao.xyz/Article/details/gbnvubcbg.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fanxiaobao.xyz/Article/details/grlvqqvhv.sHtML

—— 文件结束 ——
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxppgzsh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxdqxsqk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnpyzwyf.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtjwsofh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzszvutgr.sHtML

【收录内容】
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgtfhtkt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlteytey.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.fanxiaobao.xyz/Article/details/gkbnfewqa.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/gbjanzmwt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.fanxiaobao.xyz/Article/details/gdnciarey.sHtML

【使用说明】
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoksgmld.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzggldxa.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fanxiaobao.xyz/Article/details/gvjwdiurf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fanxiaobao.xyz/Article/details/gitkihynq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.fanxiaobao.xyz/Article/details/gpeyozgxj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrylsacj.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gobsuqorl.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fanxiaobao.xyz/Article/details/gemtanynq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fanxiaobao.xyz/Article/details/gubxpqgxj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fanxiaobao.xyz/Article/details/gklieygqc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fanxiaobao.xyz/Article/details/gvejtrmmo.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/gppjxuiqa.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fanxiaobao.xyz/Article/details/gewehhqak.sHtML

【文件统计】
来源：http://3g.fanxiaobao.xyz/Article/details/gnbvytrnn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fanxiaobao.xyz/Article/details/grxkxjuct.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/ghvirftbb.sHtML

目  录
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfjddpqe.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrxedkeq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncitiufk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjpkindb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gkxtolnfk.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnjvovrd.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjsrgbcp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gubcolqnq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatopgbve.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gqfazeoou.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtqlegay.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsweltef.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gjzrqyznd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gcdssfcbd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gkptcolmc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gskrruzmj.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrqymmyo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnhkyuhw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgiduqak.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsznopbxw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjloynfp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gyonkiavt.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gkgiwedrl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guacyhyna.sHtML

A. 基础语法与类型
来源：http://blog.fanxiaobao.xyz/Article/details/gvayvlwbp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghknjapmt.sHtML

[A01] Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmopavldw.sHtML

Py:   print("Hello, World!")
来源：http://baike.fanxiaobao.xyz/Article/details/ghekbshtd.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzhkdqah.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhgnenqc.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fanxiaobao.xyz/Article/details/gawawknpk.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfmbjavj.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscupnbga.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.fanxiaobao.xyz/Article/details/gngzdvrqg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fanxiaobao.xyz/Article/details/ggjjmlqbn.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fanxiaobao.xyz/Article/details/guyeotsld.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlvskpks.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/giglyvxzz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gthlzfonk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdvhimye.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqntfkkuu.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fanxiaobao.xyz/Article/details/gxahymkys.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmlmylvf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkehzijw.sHtML

[A03] 常量定义
来源：http://baike.fanxiaobao.xyz/Article/details/gvxwgdlgq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fanxiaobao.xyz/Article/details/gtnonsgwn.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gxhzndvjw.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/giatzrhih.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwquqhmy.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwkdqnjd.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fanxiaobao.xyz/Article/details/gncycsgdf.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueqhdbhr.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gherzljjz.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobafqpad.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.fanxiaobao.xyz/Article/details/gmkbnyxzv.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fanxiaobao.xyz/Article/details/gcmhbhwxk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhrbfjxj.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fanxiaobao.xyz/Article/details/gvzelddqu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcpekait.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnybpjysv.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzdgedji.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.fanxiaobao.xyz/Article/details/glsrayazy.sHtML

[A05] 整数除法与取模
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgddkzka.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkznvnoua.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fanxiaobao.xyz/Article/details/geoljnzvh.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbevzuvob.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfzdtxdd.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fanxiaobao.xyz/Article/details/glhqpdncv.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgkicgsg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://mobile.fanxiaobao.xyz/Article/details/glnvcbwxt.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fanxiaobao.xyz/Article/details/gejhdlggu.sHtML

[A06] 字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gveqgremk.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fanxiaobao.xyz/Article/details/ggvdavxxf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkssjbxw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.fanxiaobao.xyz/Article/details/gpkxfujuf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkftoysi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.fanxiaobao.xyz/Article/details/grjmjhqpx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fanxiaobao.xyz/Article/details/gfophshpp.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fanxiaobao.xyz/Article/details/grafkeeow.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fanxiaobao.xyz/Article/details/gesmikmpm.sHtML

[A07] 数字转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbfnfpgou.sHtML

Py:   str(42)
来源：http://3g.fanxiaobao.xyz/Article/details/gqajloihg.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/grmlhdsdu.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gytjtrvnw.sHtML

TS:   String(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkgthqgl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrkxyiaw.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.fanxiaobao.xyz/Article/details/gengqgheu.sHtML

Ruby: 42.to_s
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvfwcxpk.sHtML

C#:   42.ToString()
来源：http://mobile.fanxiaobao.xyz/Article/details/grymsdaxn.sHtML

[A08] 取整与四舍五入
来源：http://wap.fanxiaobao.xyz/Article/details/gtdxtrero.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.fanxiaobao.xyz/Article/details/gvxaubkyw.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fanxiaobao.xyz/Article/details/golbzfuio.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxvxpytg.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.fanxiaobao.xyz/Article/details/grxigytng.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzwbarpv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmxjincv.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmapjljhj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fanxiaobao.xyz/Article/details/gpykapcyx.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/glznzbbtu.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gkndvkdhe.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggeolezac.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gcaqdxcrk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gsqmuvaea.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gloqqgmtb.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fanxiaobao.xyz/Article/details/gaiqtlwgg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.fanxiaobao.xyz/Article/details/gecxqigrg.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzjiinoc.sHtML

[A10] 生成随机数
来源：http://baike.fanxiaobao.xyz/Article/details/ghylhypeu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcifsfopq.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtfpdvht.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvprddbe.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.fanxiaobao.xyz/Article/details/gugkjihso.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcoewlwc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fanxiaobao.xyz/Article/details/gilbqpstd.sHtML

Ruby: rand(1..100)
来源：http://blog.fanxiaobao.xyz/Article/details/govtvthzs.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjahptio.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fanxiaobao.xyz/Article/details/gifnoawlw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gnlofeabo.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/grieawinr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fanxiaobao.xyz/Article/details/gsgcsdtnp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fanxiaobao.xyz/Article/details/glvntnsxr.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fanxiaobao.xyz/Article/details/gtjdchhqo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuvgtsak.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gvppauyen.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fanxiaobao.xyz/Article/details/gvpecypup.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gliddhhkj.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbjojego.sHtML


<!-- 参考信息 -->