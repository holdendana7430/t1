代发 wailian999

[U79] PHP：静态分析
来源：http://m.share.zdbjq.cn/Article/details/gvrnoytny.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.fehbvm.com/Article/details/grqakkzmr.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gskiailxi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.hesvh.cn/Article/details/goxxnyicy.sHtML

[U81] JS：初始化项目
来源：http://3g.fehbvm.com/Article/details/gbscdhngj.sHtML

npm init -y;  npm i express
来源：http://mobile.zdbjq.cn/Article/details/ggredgjmy.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gqrpglgjk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.fehbvm.com/Article/details/gwwkvqoxd.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gpgxhnzff.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/ghbgflktr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.m.share.hesvh.cn/Article/details/gbfojplmx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gtmkvqlgw.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/gpylbkqqg.sHtML

a?.b?.c
来源：http://mobile.fehbvm.com/Article/details/gqcyytbwz.sHtML

[U86] JS：空值合并
来源：http://www.blog.fehbvm.com/Article/details/ghptlcwir.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gspvqrftn.sHtML

[U87] JS：解构默认值
来源：http://blog.fehbvm.com/Article/details/geivjtkua.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gwitkzvwx.sHtML

[U88] JS：对象展开合并
来源：http://mobile.fehbvm.com/Article/details/gyzgquynv.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gdxuxnneg.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gxufnghky.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gmtqlxoyx.sHtML

[U90] JS：数字数组排序
来源：http://read.share.zdbjq.cn/Article/details/gesbleqvy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gicujxejm.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gmzzjiblk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.hesvh.cn/Article/details/gmhvzniom.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/gxtpifqsa.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gfsomjcvc.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpofuewwc.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/geddtvpyf.sHtML

[U94] JS：箭头函数
来源：http://wap.zdbjq.cn/Article/details/gzuyiuytw.sHtML

const double = x => x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gwkqsfvaa.sHtML

[U95] JS：Promise 包装
来源：http://wap.fehbvm.com/Article/details/gmnqokanx.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/ganmhaxov.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/ghuiiazul.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/ghhmlvzsx.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gfaulbivl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gswpbrhtz.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gonuwutof.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gajmnvkxi.sHtML

[U99] JS：事件监听
来源：http://www.share.fehbvm.com/Article/details/gwxzuwvpr.sHtML

el.addEventListener("click", e => {})
来源：http://blog.fehbvm.com/Article/details/gdmrwcyzk.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/gnuweyibo.sHtML

document.querySelector(".item")
来源：http://m.share.fehbvm.com/Article/details/gmnyhbrql.sHtML

[U101] JS：classList 操作
来源：http://www.blog.zdbjq.cn/Article/details/gvskxaqgb.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gmtggnztv.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/grwxvnnqq.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gkozhywsc.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gxyqzkrep.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.hesvh.cn/Article/details/gpwqgrjyh.sHtML

[U104] JS：防抖
来源：http://www.share.hesvh.cn/Article/details/ggyopekld.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gjauhjsuj.sHtML

[U105] JS：节流
来源：http://m.share.fehbvm.com/Article/details/gtphaonxx.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/garjoeuhc.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gfgpsdhyn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.zdbjq.cn/Article/details/gcoatxznl.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gxpjehzlm.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gqiudnybk.sHtML

[U108] JS：随机整数
来源：http://www.share.fehbvm.com/Article/details/gtibjqzrv.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/ghgrmacfp.sHtML

[U109] JS：数组分组
来源：http://mobile.hesvh.cn/Article/details/gnljqqpap.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gxjcrengi.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gomlnwcix.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gdbfywuhj.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/ghewzwvwc.sHtML

new Map(Object.entries(obj))
来源：http://baike.fehbvm.com/Article/details/goxqpgcek.sHtML

[U112] JS：字符串补位
来源：http://3g.hesvh.cn/Article/details/gdrxpyfqv.sHtML

"7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ghdqqxskw.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gvjxllgxl.sHtML

s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gadzkzkux.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gzpltierf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/gpqfzuywj.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gnnnghqbi.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gtuntghwa.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.hesvh.cn/Article/details/gfrgxmfqo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.hesvh.cn/Article/details/gkmtspzgv.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gaakftjxu.sHtML

npm i -D vitest;  npx vitest
来源：http://3g.fehbvm.com/Article/details/gpyfgnhxq.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.zdbjq.cn/Article/details/gkxetvhkw.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gfdvdteri.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gzdkxquft.sHtML

npx vite build
来源：http://blog.hesvh.cn/Article/details/gvwxmvrcs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.hesvh.cn/Article/details/geyfgvmmv.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.zdbjq.cn/Article/details/gduarlysq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzwfrdwxs.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/ggoccomja.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gizlqhhmz.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/ggfniocla.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/gniaimvgm.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gpcuencaj.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/govwmjprs.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gnunvxzgm.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/grjqoxkan.sHtML

Go ............. 212
来源：http://mobile.fehbvm.com/Article/details/gjcgdtywz.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gieuveaqx.sHtML

C# ............. 212
来源：http://3g.fehbvm.com/Article/details/gymwezkal.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gdrdoeuff.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gstczjxvq.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gminwqszu.sHtML

Bash ........... 80
来源：http://www.share.fehbvm.com/Article/details/gpmfowcdv.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gofazvosu.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/glwpnqsoa.sHtML

Lua ............ 10
来源：http://baike.zdbjq.cn/Article/details/gupegsnwh.sHtML

Perl ........... 10
来源：http://blog.fehbvm.com/Article/details/gbyslmkux.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/ghxufukmn.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/ghztyeezt.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gupxfjkyp.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/grlbhluce.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gzgbnxkih.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gthteqpxw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/ghoadjarz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.fehbvm.com/Article/details/gthijsqex.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.zdbjq.cn/Article/details/gudpprpwq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.hesvh.cn/Article/details/gtvwlpped.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/grrerczit.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gyazwluwf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gwnndjlsz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gdfwppkvq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gmqosbqpc.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gywcxjozz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gdsaeyhzx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gmicfzhsw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.fehbvm.com/Article/details/gxfxfakhk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gncihwpzw.sHtML

Q SQL 专题                              90
来源：http://www.share.zdbjq.cn/Article/details/gfmoojcim.sHtML

R Bash 专题                             80
来源：http://www.share.fehbvm.com/Article/details/gtqfbigfi.sHtML

S C / C++ 专题                          60
来源：http://www.blog.fehbvm.com/Article/details/gvqwfqzau.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gjeiktdph.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gckbwipmk.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gbtmzuhpo.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gmpycymai.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gcumyslgm.sHtML

使用提醒
来源：http://wap.fehbvm.com/Article/details/gtuahoxlf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gldibwuwg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gaprtlbue.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gymjnonuy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gslhskcqj.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gxnowixfe.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gjgjludtq.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gbikpgkui.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gexxahvxe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gglsqvagt.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gevquxoce.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdbsnqpne.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/giafuimfu.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gndfolhuy.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gfxaddiqi.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/glypmwonv.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/goltujhfo.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gekjvhbfe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/gzosyusth.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.hesvh.cn/Article/details/gdkmyfaik.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gmriqmntp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gilnyvbrz.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.hesvh.cn/Article/details/gmqbzyssq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gpyoaitul.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gkpehwgqz.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gfzawfkfl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.fehbvm.com/Article/details/ggdwdiknt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.fehbvm.com/Article/details/gtpnflouj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.hesvh.cn/Article/details/gnvhendop.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/gkhzptpqc.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gvyiwzgkk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gglcvhelx.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gbkzmongb.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gevatwalf.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gupjrhapb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gtuorouma.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/giwuxbciw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gdhprsezi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gwcdhvnlb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/ggepbeohf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gsthymmte.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gmqvfatbi.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gtqdlmqzd.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gdorqoymw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/galvedjpv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gatobirxr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/giteamojx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/grqbqpsbn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.hesvh.cn/Article/details/grpaigrgk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gwmchkglg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gnsveihxi.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/glznwvkpb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/gxzckproa.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gjrvaxzrn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gbchljeks.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gjcnchcic.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmueowgpk.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gqnlyvphx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsamgseuc.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/guyszamxs.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gyzfbinxn.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/gpilzhlzv.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gxtpyaigt.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.share.fehbvm.com/Article/details/gkvqypgfi.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gaqixnxon.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/ghachxmus.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/gsbqyvoig.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gsqcspdrs.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gnqydqceh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.zdbjq.cn/Article/details/golskidan.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gjiufpvhs.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gbiuadyep.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gddmlreef.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gsdzwrakc.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/gisrqksea.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.fehbvm.com/Article/details/geuqejzni.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gourdotpc.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/gbknatwod.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gcnsondun.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gokdijktx.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/guszlrpme.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gfhxcivug.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gvahpuwxi.sHtML

Go:   const PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gdbnfjdey.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gazbngntj.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gnxnfsazu.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/gyztkxdmb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.fehbvm.com/Article/details/gqakcaiew.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gxmtmhkea.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gjthrulwy.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gkhwknxlz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gsmxdesuk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/girgstrrt.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gfftkskzj.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/gsorsvmbh.sHtML

[A05] 整数除法与取模
来源：http://wap.zdbjq.cn/Article/details/gmvndhvtx.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gjwevnads.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gkwkjqztp.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/ggfatoemf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gdbxlayee.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gxbwircrm.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/goexqpokf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/ghhnttcie.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/ghxottunm.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/gasfdpavm.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/gedbskucu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.hesvh.cn/Article/details/gxlrgpvhz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gfczeeyym.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gfgylbbnx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/gxenisilb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.zdbjq.cn/Article/details/ghtlbepiz.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gmbarvmid.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gblasqpuc.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gpnhohmit.sHtML

Py:   str(42)
来源：http://m.share.zdbjq.cn/Article/details/gacyahjid.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/gnewpoljv.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/goxwfcsia.sHtML

TS:   String(42)
来源：http://wap.hesvh.cn/Article/details/gkqeypkfx.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.zdbjq.cn/Article/details/grfepmrix.sHtML

Go:   strconv.Itoa(42)
来源：http://m.share.zdbjq.cn/Article/details/guxgtiryu.sHtML

Ruby: 42.to_s
来源：http://blog.zdbjq.cn/Article/details/gxvtotdpo.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/gbdqngvbt.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.hesvh.cn/Article/details/gufvjebsc.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gxqcualgs.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/gtbmwzyfu.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gihtvlnbx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/gpfpzwbgz.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.fehbvm.com/Article/details/gmhpksppx.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gqvdlnvwy.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.zdbjq.cn/Article/details/gfhgdjlaz.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.hesvh.cn/Article/details/gmvhulbka.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.hesvh.cn/Article/details/gnupqjrnq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/glppbkjrj.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gjvbdwyxo.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gmlrccbbr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gqvdluxce.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gkaaplbuh.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://read.share.hesvh.cn/Article/details/gzjchmpfn.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gpdhjnent.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gpifnuhuv.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/gisaydvwu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.zdbjq.cn/Article/details/ghryypgba.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gklknvnoy.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/geeamyqfv.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.fehbvm.com/Article/details/gwxcqllzr.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gdgykrmyd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/grrqtnemi.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/gpzkbsxmg.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.fehbvm.com/Article/details/gnxgezzbe.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/gqdgdpyfq.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fehbvm.com/Article/details/gosmwymcp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gnqdmcrcq.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/ggbniffdd.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gqmfcvren.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gnzrkgyxm.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.zdbjq.cn/Article/details/gxieojnia.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.zdbjq.cn/Article/details/guoyvvvwh.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gscluijrr.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/gthssqvdw.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.share.zdbjq.cn/Article/details/gpgulowho.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.zdbjq.cn/Article/details/gtexemhen.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/ggwwjkmnd.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.hesvh.cn/Article/details/gvrmxpvfl.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gpokusqpl.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.hesvh.cn/Article/details/grpevaorp.sHtML

Ruby: "Hello, #{name}!"
来源：http://m.share.hesvh.cn/Article/details/gbrqshgtr.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.hesvh.cn/Article/details/grnoqhrkp.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://3g.fehbvm.com/Article/details/gskwopcst.sHtML


<!-- 参考信息 -->