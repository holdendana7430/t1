代发 wailian999

[U83] JS：ES Module 导入导出
来源：http://baike.zdbjq.cn/Article/details/ggahngjfv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.hesvh.cn/Article/details/gxtwhtocd.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/giiewoufg.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gfrklmstc.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gjubotcpj.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gqakkbvlq.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gcdfzfjcm.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gnxpmgpht.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gevaqhhvj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gbsyokezy.sHtML

[U88] JS：对象展开合并
来源：http://3g.zdbjq.cn/Article/details/gjazjqtyd.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gpclslwdb.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/ghakyrwpx.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/groruyxsi.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/ggephbkmf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gpehyrdeg.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/gibpypyfr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gxbboxnkk.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gdgaatuvn.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gafgpzuqi.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/grdqxlvyq.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gcqkayyzf.sHtML

[U94] JS：箭头函数
来源：http://www.blog.hesvh.cn/Article/details/ghwkuzfto.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gdkjahhps.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gjhbxzxua.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.fehbvm.com/Article/details/gafupayxc.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gbvofvzvu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gsciwajbu.sHtML

[U97] JS：并发请求
来源：http://mobile.hesvh.cn/Article/details/glwffopwx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/geaynxmaq.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gaytonbmz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gueffyzkn.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gktzagvkh.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gcztedpsp.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.fehbvm.com/Article/details/gmwejeuau.sHtML

document.querySelector(".item")
来源：http://www.share.fehbvm.com/Article/details/gqbgmrfou.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gtmzgkqow.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gipoodkkg.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gnxwcfqtn.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.zdbjq.cn/Article/details/ggychjgbx.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/ggnointvj.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gavxffcal.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/ghyqppfuj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gmvibvfhw.sHtML

[U105] JS：节流
来源：http://mobile.zdbjq.cn/Article/details/gjdnpwldi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gicophxts.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gyksqnozj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gdftocaau.sHtML

[U107] JS：数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gmplkmdjx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/grpvfldry.sHtML

[U108] JS：随机整数
来源：http://read.share.hesvh.cn/Article/details/gvehsxjds.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gqapvakjh.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gpxuyyogj.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gigwolcbr.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gkaxbourl.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gafnutskc.sHtML

[U111] JS：对象转 Map
来源：http://wap.hesvh.cn/Article/details/gkbzouint.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gfmkvxlct.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gowpbmtpn.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gghnpizlq.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gyyqnwtre.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gzcisrocj.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gbrnkcpgj.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/giqwpqfpl.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gepyhmhac.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gyssximha.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gdgvwacyp.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxyuxygkq.sHtML

[U117] JS：单元测试
来源：http://www.share.fehbvm.com/Article/details/gouooywbv.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.hesvh.cn/Article/details/geojuvihd.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/ghgsfdesx.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/glhjolhvg.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gbwdtguwt.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gpougmozw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/ghlwoerzs.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/giqyhjgxf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbamxmsgz.sHtML

统计汇总
来源：http://baike.hesvh.cn/Article/details/gbzmunhyk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/girqcerrj.sHtML

按语言统计（条）：
来源：http://www.m.share.fehbvm.com/Article/details/gzsavzxdx.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/ggmvuxfst.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/gzclithfs.sHtML

JavaScript ..... 252
来源：http://m.share.fehbvm.com/Article/details/gjbunhdka.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/ghoqlkslo.sHtML

Java ........... 212
来源：http://wap.zdbjq.cn/Article/details/gtktkfkxx.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/guwrtjebd.sHtML

Ruby ........... 212
来源：http://wap.zdbjq.cn/Article/details/gfaogkpsg.sHtML

C# ............. 212
来源：http://m.share.fehbvm.com/Article/details/gxjtqrcbq.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gkowsviti.sHtML

C++ ............ 30
来源：http://www.blog.fehbvm.com/Article/details/gzbfiidry.sHtML

SQL ............ 90
来源：http://www.blog.zdbjq.cn/Article/details/gofzwyimu.sHtML

Bash ........... 80
来源：http://mobile.hesvh.cn/Article/details/gdkalflcb.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gpzlesaon.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/gmdkdnajk.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gyzqtyeyi.sHtML

Perl ........... 10
来源：http://blog.hesvh.cn/Article/details/gsavwtuke.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gkyeiryzu.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gxfhbfmes.sHtML

合计 ........... 2106 条
来源：http://read.share.zdbjq.cn/Article/details/gdwknezyy.sHtML

按章节统计：
来源：http://wap.hesvh.cn/Article/details/gslctaxds.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/giwjxmamj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gxdskwjfb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gyqsevmpm.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gvqmhskzg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.zdbjq.cn/Article/details/gorjrjvsg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gechnsdnz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gysfvxgoa.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.zdbjq.cn/Article/details/gfwptklrs.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gixhdjagr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gvzalcbfy.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/ggdowgcsq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gdlehnzww.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gtkbwcwbv.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gkmyvstsa.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gulvjokkc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/govevwuvm.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gdggezchq.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/gmirbiqgy.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gutsbqrrt.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/ggfguuinc.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/gvgoacydd.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gnzpojshd.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gbsjbsoyp.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gmdfbpvhv.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gmlzybdhd.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwysdswxp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gdnkhxdjx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gaedyqbhh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gelejgagx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gjfbupeut.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gplovwzfi.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/glyfxffvh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqhqvwdyq.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/goujwptcd.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gqrjwtgpy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwlxocsnr.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gtccagnyv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gajjepkxx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/grbambsye.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/gbcfoupff.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gpskibduv.sHtML

【使用说明】
来源：http://m.share.hesvh.cn/Article/details/ggyxcsseg.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gsohngeng.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/goucpdnax.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gapwttcpt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/guvvwqxfb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.fehbvm.com/Article/details/gvxraujyl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gphmgprew.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gbtmzewce.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.hesvh.cn/Article/details/gflcpsjem.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.hesvh.cn/Article/details/gknxuywpq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/gvkvfahoi.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/glgzvxrko.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/ggznnclem.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gfcnuerqp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/gsekilvet.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gnigufzjl.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gxlgrndyk.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gzzkaywjn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/glnufauvk.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/ghxwpndkq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/glzhmzhgr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/godiryyyp.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/ghigoeync.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gabjblkpl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.zdbjq.cn/Article/details/gviuoheml.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gquvsuwnb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gderltnoj.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gxrvwhdjd.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/ggsulbqso.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gcjeqovyo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gxjgvymju.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/gedcxqbtd.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/glmewapyw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gjvpkzzvs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.hesvh.cn/Article/details/gvwbqyrfw.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gjyydfjec.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gtoatfunj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gpmxppcyy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/ghwwnpvqo.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsbehubpa.sHtML

A. 基础语法与类型
来源：http://www.share.zdbjq.cn/Article/details/gcpuzzttc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnbiuxowj.sHtML

[A01] Hello World
来源：http://m.share.fehbvm.com/Article/details/gqeygyohv.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gkqykmtpz.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.hesvh.cn/Article/details/gfkopveya.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gktwqjujm.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/guoqwteod.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gyccbmtrk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.zdbjq.cn/Article/details/gjxjjqgeq.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gwjvgupdv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/glgtuhlew.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/grvomnglt.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.fehbvm.com/Article/details/gyeubaagp.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gbeffbixw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gogkvuduu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.hesvh.cn/Article/details/gnrvoqcav.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/gegqolhbc.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gvxvwloew.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gyzvarzol.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gbtwebbla.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/gvooxunqv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.zdbjq.cn/Article/details/gvdjtjlmr.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gmuhocbzb.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/geblkqbvf.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/ggzjokhst.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gibteansm.sHtML

Go:   const PI = 3.14159
来源：http://www.share.fehbvm.com/Article/details/gnsjhdvol.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gnxhhplle.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gevpjlfmp.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/gjrtvftdx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/gwsckjsxo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/gbfgqkqah.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/guwvybqdb.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gvtdhgxdq.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/gmgoqjasa.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.hesvh.cn/Article/details/goqkabkke.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.zdbjq.cn/Article/details/goglrkywz.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.blog.fehbvm.com/Article/details/gdgiyvcqc.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gznactfeb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.zdbjq.cn/Article/details/gmxawxxsy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gymonabwm.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/geqnozzqp.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gkumbgawk.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/givavarrf.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gvzbsfjkb.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gcubhjrtw.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gxzznhabw.sHtML

[A06] 字符串转数字
来源：http://www.blog.zdbjq.cn/Article/details/gnabfbssm.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.hesvh.cn/Article/details/ghadexfsb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gqnkixkrv.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.zdbjq.cn/Article/details/gvsjybpwu.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gsnqoqzrl.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gkfakzqfq.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.blog.zdbjq.cn/Article/details/gqzgpgnvx.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/gfgljoags.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gjlwhexnj.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gbvqoxzqf.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxepbqzx.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.share.fehbvm.com/Article/details/gxbrfktea.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.hesvh.cn/Article/details/gbhsrwobl.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/gnkyvjgmf.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gawzqhaaq.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.fehbvm.com/Article/details/gbrbhjyuw.sHtML

Ruby: 42.to_s
来源：http://wap.fehbvm.com/Article/details/grdgxlsrb.sHtML

C#:   42.ToString()
来源：http://read.share.zdbjq.cn/Article/details/gtoclwlhn.sHtML

[A08] 取整与四舍五入
来源：http://baike.zdbjq.cn/Article/details/gqwyphljx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gmsymjaqa.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://baike.zdbjq.cn/Article/details/gnyqhgadg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.hesvh.cn/Article/details/gdflppnak.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.hesvh.cn/Article/details/gxooqnykh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gbvlciqez.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/glmwfmvvm.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/gkxifzcwd.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gxoxpanvi.sHtML

[A09] 绝对值与最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gvlrltoxl.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gyxuzmbts.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.hesvh.cn/Article/details/gihxsyirz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gwqjyqkgw.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/geddaejim.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gjsjftnbv.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.zdbjq.cn/Article/details/gvreyiokw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.hesvh.cn/Article/details/giodrntoh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/guyqnqsbv.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/guvszikbu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.fehbvm.com/Article/details/gwdmtfncr.sHtML

PHP:  random_int(1, 100);
来源：http://blog.fehbvm.com/Article/details/gmjozaxfv.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggcycrlgs.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/gyphmljmh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gioczteth.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.zdbjq.cn/Article/details/grbmkkzcg.sHtML

Ruby: rand(1..100)
来源：http://www.share.fehbvm.com/Article/details/gimrqgncq.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.zdbjq.cn/Article/details/gmsebtnhb.sHtML

[A11] 条件表达式（三元）
来源：http://m.share.zdbjq.cn/Article/details/gdssquhjc.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.zdbjq.cn/Article/details/gpibymfis.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gkeymofnc.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gukddzqpl.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gounobmeg.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gpodnoqfw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.zdbjq.cn/Article/details/gzchuefnc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gbhzldrzo.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gcddtsksj.sHtML

[A12] 字符串插值 / 格式化
来源：http://baike.hesvh.cn/Article/details/gcoriuquc.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.hesvh.cn/Article/details/gzjvzawdo.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.fehbvm.com/Article/details/gdbweqggr.sHtML

JS:   `Hello, ${name}!`
来源：http://m.share.fehbvm.com/Article/details/gnruwxxqm.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gggyqibcj.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/griuwlgfk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.hesvh.cn/Article/details/gfnhkieen.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.fehbvm.com/Article/details/gjbveibok.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/gkbcsfukg.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.fehbvm.com/Article/details/gwqyasvgc.sHtML

Py:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gjnvmiodi.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/geuvsxtit.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gcwjlarkt.sHtML

TS:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gwsbrroha.sHtML

Java: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gjevgjygu.sHtML

Go:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gqixjlayt.sHtML

Ruby: "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gmyyyuewr.sHtML

C#:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gmgzywjig.sHtML


<!-- 参考信息 -->