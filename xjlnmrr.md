代发 wailian999

[U75] PHP：依赖注入
来源：http://blog.hesvh.cn/Article/details/ggavkudiz.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gakcmnblg.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gzkpvmhdr.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gxfdwncdq.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gkukteebg.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gpqyghfqs.sHtML

[U78] PHP：单元测试
来源：http://3g.hesvh.cn/Article/details/geipngbmh.sHtML

composer require --dev phpunit/phpunit
来源：http://www.m.share.zdbjq.cn/Article/details/gxvwuxznl.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/govzzwxrr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.zdbjq.cn/Article/details/gtuxuudoj.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/gqhqmnrqy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/gmlslnmbj.sHtML

[U81] JS：初始化项目
来源：http://wap.hesvh.cn/Article/details/gtyvoaevn.sHtML

npm init -y;  npm i express
来源：http://blog.zdbjq.cn/Article/details/gboaqgqwa.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gdeyicdpc.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.zdbjq.cn/Article/details/gfbqqqumz.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.fehbvm.com/Article/details/gpnugikxy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gfpzsvmar.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.hesvh.cn/Article/details/giinjcnjb.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/gnbnyzstl.sHtML

[U85] JS：可选链
来源：http://read.share.zdbjq.cn/Article/details/ghbyygcfj.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gsxenuhpo.sHtML

[U86] JS：空值合并
来源：http://3g.zdbjq.cn/Article/details/gydfmdjlj.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gxtskzeum.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gsiqwhson.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gexogqcko.sHtML

[U88] JS：对象展开合并
来源：http://m.share.hesvh.cn/Article/details/gddmngnzf.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gavdylhnz.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gpnbssgtk.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gflyqdgsn.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/gtzarfnaw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gmxuxiior.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gldnrzcff.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gyikhpzmo.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gzmmqxsps.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gvasgkahq.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gjrflnehl.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gextzrfvf.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gsgfmbfun.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gujylvlnd.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gpwvylplb.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gramzdndz.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gbfigabfg.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gwvrzoztz.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/ghmkejlwq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gmknvzhpk.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.zdbjq.cn/Article/details/galkauigc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gltasplim.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/gncgxgsfs.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gduloskra.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gclvlmjii.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/geeqtqrmg.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gplwkczua.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gmvroqdeq.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gmpaybqaq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.fehbvm.com/Article/details/gookcfdgz.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/gvbrfwspu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.fehbvm.com/Article/details/gcvbwwsfz.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/gfxjzaqnh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gxtzfofyf.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gehxdfrwi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/getbgummu.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gnnualtir.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.zdbjq.cn/Article/details/gzlqeqief.sHtML

[U107] JS：数字千分位
来源：http://www.share.fehbvm.com/Article/details/gqnqfhnvd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.hesvh.cn/Article/details/gixxnachk.sHtML

[U108] JS：随机整数
来源：http://wap.hesvh.cn/Article/details/gydfxggik.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.fehbvm.com/Article/details/grubozslx.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/grztvqesg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gwdcqgbph.sHtML

[U110] JS：数组分块
来源：http://3g.hesvh.cn/Article/details/gzzrswctw.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gaaclsbhl.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gicvkrduz.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gesnwzkwx.sHtML

[U112] JS：字符串补位
来源：http://read.share.hesvh.cn/Article/details/gfpkymxbs.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/ggsetqjab.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gbybbomfw.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gynttcotu.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gukuzseqi.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gkokbapww.sHtML

[U115] JS：生成 UUID
来源：http://blog.hesvh.cn/Article/details/gwavgerwp.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gobbzqpqk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gjfcyabrh.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbtzljjtm.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gebbvdpyd.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gwyeyqcvi.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/gdeznxiax.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gyarzcebk.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/gewhnyudp.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gqmzgdtou.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/gxwycdcbe.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gkffkclvm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjexuuxux.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gjhzqfidz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gautholhy.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gcdrnkbhm.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gcxpipuak.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gwnxclxbm.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gtbwksjjd.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gaqvkmlun.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gzuoyfccf.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gkbwfzibx.sHtML

Ruby ........... 212
来源：http://blog.hesvh.cn/Article/details/gthvkawiz.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/giaqelabk.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gvpsleyws.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gtpqldjih.sHtML

SQL ............ 90
来源：http://mobile.hesvh.cn/Article/details/gglltbjtg.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/glqbtnoqo.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gfrnekdjt.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/ghenxbght.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gkvrywjlb.sHtML

Perl ........... 10
来源：http://3g.zdbjq.cn/Article/details/gzclbtnip.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gwewivwea.sHtML

------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gaddmjmsz.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/glfqggxus.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gtihjxjhs.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/ghyyistbs.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gicvepxoh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/goqnndmlo.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/grczoixsn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gozaikrpa.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gbtuzjyrs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gcqpozlpg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gnylvasnw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gdjiumddf.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gfwqeshzv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gazocldcz.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/ghodctjky.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gludkapso.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gahawvuro.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gmrbdfrib.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gwlqafpum.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/gjnvxylqg.sHtML

R Bash 专题                             80
来源：http://www.blog.zdbjq.cn/Article/details/gcmcxzwer.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gtcdranfx.sHtML

T 其他语言补充                          60
来源：http://www.m.share.fehbvm.com/Article/details/gzbiwpiku.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gjecloooj.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gfawlmapu.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gkzxfrjpx.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/ggikqfcnp.sHtML

使用提醒
来源：http://blog.fehbvm.com/Article/details/gsykjirlw.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gseahemvq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.zdbjq.cn/Article/details/gcneoqeyx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gtzcabsdv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.fehbvm.com/Article/details/gvqtmtqcu.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/grtxjbdag.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gfwmvjowh.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/grewyqeyp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzkbxdflo.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gleyrbayq.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gydazcdjm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gstkmnnxt.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/gwliscwyv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/gudnldhoc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gejjhnoiv.sHtML

SQL · Bash · C · C++
来源：http://mobile.zdbjq.cn/Article/details/gqnozpces.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.fehbvm.com/Article/details/ggthakcir.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/glfinchym.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/ghbcbszxc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.hesvh.cn/Article/details/grwlbeozy.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/grmdiqkqk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.hesvh.cn/Article/details/gwabygbnq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gzgkowdak.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.zdbjq.cn/Article/details/gjsrolvat.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.zdbjq.cn/Article/details/gibkgybrz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gbgzxzqrg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/gceiowdvz.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/grltlquwt.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.fehbvm.com/Article/details/guvrhmgqi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/gtzqpkrft.sHtML

【文件统计】
来源：http://www.share.zdbjq.cn/Article/details/gdzagtrvd.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/ghgotjgnu.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/ggmumrvlu.sHtML

目  录
来源：http://www.blog.fehbvm.com/Article/details/gfdkxhedv.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gfmgkxpka.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gmpaszelt.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gynkefmlq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gpfxdfopv.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gukwgjelf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gcfbhtykg.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gwtrtguho.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gfkiwffei.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqokdjlyx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/grtvdywrn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gytxeefjc.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gukzvhcvw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/guumjesag.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gerhhiidl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gblqdujim.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.hesvh.cn/Article/details/gfweljkkn.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gwuolpxys.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.fehbvm.com/Article/details/gxrwzvojv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/genkikktb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://blog.hesvh.cn/Article/details/gubuyahas.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gzsjxeama.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.fehbvm.com/Article/details/gxyercear.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gszxsqsfv.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/gowwrslio.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwqjhnvgj.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/ghcowjfqu.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gyvrrkibm.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gwcreyebj.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gvqjiqpsa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.fehbvm.com/Article/details/glgobxtsh.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gpttikpuk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.m.share.fehbvm.com/Article/details/gdhjqoeut.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/gxuhmvqot.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gtldrjxon.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/gpfimugbi.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gxvcvcnum.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gswjdoves.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gbuzjcgga.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/gzfbwhaip.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/glqevksqi.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/guhgbrxgz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gmwleqcky.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gaknusvqj.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/gcadtkfkr.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/gaflgxnmj.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/giwrwbqop.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/grkvrswca.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gotwsqepk.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gfxhfmzjg.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gcrcecqmb.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gojalpmzx.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gwjnnnjom.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gnmxycqlf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gdtvfjglm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gjcenxerk.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gokdfwmnl.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gghjuzlyn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/ggxodbvgb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/gwhihivgg.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.fehbvm.com/Article/details/gayijqnca.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gxeaujfvl.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gorrymijm.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.fehbvm.com/Article/details/gdiysdfej.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gsgpvnbum.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gqixbfkuv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/grnkxgmug.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/goasatmtl.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gshblcirp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gvumlqzmp.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gpuritoqm.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/gvjoxjmkh.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gcelfccvq.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gpzsrpppf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gmfqywdqv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gzwdleudx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/gckonsewv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.hesvh.cn/Article/details/gcjbiagan.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.hesvh.cn/Article/details/gvfxmuzrh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/gffrcqntw.sHtML

[A07] 数字转字符串
来源：http://baike.zdbjq.cn/Article/details/ggdnspegx.sHtML

Py:   str(42)
来源：http://wap.hesvh.cn/Article/details/godknaweo.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.fehbvm.com/Article/details/gragbterp.sHtML

JS:   String(42); (42).toString()
来源：http://3g.zdbjq.cn/Article/details/gqmzmpbps.sHtML

TS:   String(42)
来源：http://3g.hesvh.cn/Article/details/gvfgkbvbj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gpajifdfw.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.hesvh.cn/Article/details/gkfvekvhc.sHtML

Ruby: 42.to_s
来源：http://blog.fehbvm.com/Article/details/gzjfsyfkq.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gchtpjryg.sHtML

[A08] 取整与四舍五入
来源：http://blog.zdbjq.cn/Article/details/gzllimowq.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gwbqyrcjk.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wap.zdbjq.cn/Article/details/gdpmrbaov.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gofqctcer.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.fehbvm.com/Article/details/gfngtheqx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gylsubsii.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gplnetqrl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://wap.zdbjq.cn/Article/details/gqnbfygfi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gtvgqmtjf.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gnyhoilej.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gwxsicltv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/ghbucomcu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gzwarljmi.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gbmirbkbo.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gqknkxrmj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.hesvh.cn/Article/details/gmxdeuqng.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.hesvh.cn/Article/details/ghlodznyh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gkdcmiwdb.sHtML

[A10] 生成随机数
来源：http://blog.zdbjq.cn/Article/details/gkgqyhbcx.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/gbciiqudz.sHtML

PHP:  random_int(1, 100);
来源：http://3g.hesvh.cn/Article/details/gudrljbpi.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gnhzzpbzy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/giyxhjjvk.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.hesvh.cn/Article/details/gbnjpnsri.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.fehbvm.com/Article/details/geeopvmgh.sHtML

Ruby: rand(1..100)
来源：http://3g.hesvh.cn/Article/details/gprvzgufq.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.hesvh.cn/Article/details/gfybfsflb.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/gfuhphavx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.hesvh.cn/Article/details/gixgcnuen.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gicqrdmzv.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gkzlckfbp.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/geprwlqhv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/grrebloip.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.share.hesvh.cn/Article/details/gbndprimi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gbxdbfvyw.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gmicccppc.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.fehbvm.com/Article/details/gikxbmjqk.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.hesvh.cn/Article/details/gklpgfoxe.sHtML


<!-- 参考信息 -->