代发 wailian999

[U79] PHP：静态分析
来源：http://www.share.fehbvm.com/Article/details/gymvrfreb.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gmsqbieue.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gcznuyfcy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gfndrarck.sHtML

[U81] JS：初始化项目
来源：http://blog.zdbjq.cn/Article/details/gqfhuwwqu.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/glbwsxtqa.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gqhkitcpv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gswxosmpm.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/ghvmfhfzi.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/grouyajbn.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gseofhoku.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.fehbvm.com/Article/details/gfofvnnwj.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gzrlhwgoq.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/gtsiegxjw.sHtML

[U86] JS：空值合并
来源：http://www.share.hesvh.cn/Article/details/gmzufjrgq.sHtML

a ?? b
来源：http://www.m.share.zdbjq.cn/Article/details/gcxdivgac.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gryhqtcjg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/ghiympjms.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gcpmlplrl.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gdylrqejx.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/giicotctd.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gjureczto.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gnkinookc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gpssvpyvn.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.hesvh.cn/Article/details/gcrqhdzgp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/giuegcyrk.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/ghdfmesdd.sHtML

structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gmskboiic.sHtML

[U93] JS：模板字符串
来源：http://www.share.fehbvm.com/Article/details/gntzvsrki.sHtML

`共 ${n} 条`
来源：http://www.share.zdbjq.cn/Article/details/ghlvrhbpp.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/guncnxtho.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/grwuycwdf.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gctfzfxvw.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/goewfwzbd.sHtML

[U96] JS：async/await 与异常
来源：http://wap.fehbvm.com/Article/details/ggldzizbw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gezwhgshx.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/grhcchmsn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gqvrfmeww.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/glievujcd.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.hesvh.cn/Article/details/gejfwsjiw.sHtML

[U99] JS：事件监听
来源：http://baike.hesvh.cn/Article/details/guywjhkip.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fehbvm.com/Article/details/ghrxnhtnn.sHtML

[U100] JS：DOM 查询
来源：http://mobile.zdbjq.cn/Article/details/ghqieodoj.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gamdkllcl.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gxlnisyza.sHtML

el.classList.toggle("active")
来源：http://www.blog.hesvh.cn/Article/details/ghzeilgza.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gjfbweejv.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwcaxkj.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gudgdrysf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gfwjegkwx.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/geyotsxzu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gmdyhdcbt.sHtML

[U105] JS：节流
来源：http://read.share.fehbvm.com/Article/details/gqnncoxlv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gwoxkiepr.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gxkvctnae.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gmkmqggaa.sHtML

[U107] JS：数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gahnkjiha.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gujvlohab.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gueudtyaj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gqhjdoybz.sHtML

[U109] JS：数组分组
来源：http://m.share.hesvh.cn/Article/details/gluzdctyi.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gsmfypseu.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gcdzkcsqz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/glvaumyxl.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/grecwvbbn.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gccypwsoa.sHtML

[U112] JS：字符串补位
来源：http://www.blog.zdbjq.cn/Article/details/gskgxmbsx.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gvrdbouwy.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gcpwfyrvo.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/ggqhfwzdg.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/giidvcakm.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/ghpakbdrd.sHtML

[U115] JS：生成 UUID
来源：http://read.share.hesvh.cn/Article/details/grnbggoxb.sHtML

crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gophdolce.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.hesvh.cn/Article/details/gbchfmnbx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdpdketci.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gpjgscdxq.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/gkxvkuogd.sHtML

[U118] JS：开发服务器
来源：http://wap.zdbjq.cn/Article/details/ggmdumusu.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.zdbjq.cn/Article/details/gzekkbehz.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gjkuebuab.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/guoqbbogp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gukwpjtyo.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gqpizcrzf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gndsropkw.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/ghbciohus.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtudsdexb.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gnanzijcb.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gdqyepbed.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gwsnaolov.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gvwtfzgsx.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/ghjmyzqih.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/ghpjshnbb.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gneywslza.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gyuylbanx.sHtML

C# ............. 212
来源：http://www.blog.fehbvm.com/Article/details/glkpeschw.sHtML

C .............. 30
来源：http://www.share.zdbjq.cn/Article/details/gxfcfsaxf.sHtML

C++ ............ 30
来源：http://mobile.fehbvm.com/Article/details/gevvlqjni.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/ginvhncyt.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gdcylexui.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gkmjtfswg.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gcxfazoqy.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gwdmekzoe.sHtML

Perl ........... 10
来源：http://www.m.share.fehbvm.com/Article/details/gxdrvujwp.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gyxisnxty.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gufnhgjko.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gsnsrncvu.sHtML

按章节统计：
来源：http://m.share.fehbvm.com/Article/details/gaiwyhazg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/glamaaoki.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/govrhcrop.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gxmbhyocp.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/ghzvfipfr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gtbmdnppm.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.hesvh.cn/Article/details/glmbumjqq.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gukpznfei.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/grzrdlocj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gyvwenlcl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/grkbzczvk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gcyalvybw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/grufgafmi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gahpwyxgm.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/ggndpmmqf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.fehbvm.com/Article/details/gxaehatnq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gucvbfooh.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gwzpmoezw.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gzwtmihup.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/geqmnblrh.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gnotptlph.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/ggvadmfnd.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gpnmbnvac.sHtML

合计                                  2106 条
来源：http://m.share.zdbjq.cn/Article/details/gggsujwzh.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gsvtpmqcj.sHtML

使用提醒
来源：http://www.blog.zdbjq.cn/Article/details/gzhwdqxzd.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gnebwzdrm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gcmlvyasx.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/gwikdkmab.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/goflxwvon.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/grpkyqkxo.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.fehbvm.com/Article/details/gcrlrvhll.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gykdsimzl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzewprynu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gnegyqxvo.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gxjhnbjmy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gejeltxxv.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gkdkqbjta.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.hesvh.cn/Article/details/gqoayasqr.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gikjjnixs.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/glbgqetfa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gegvzuswu.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/gigvhpbsd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.hesvh.cn/Article/details/gvgokhktd.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gzmbyneqp.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/gbdqdodfu.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.hesvh.cn/Article/details/gkdroldwu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.zdbjq.cn/Article/details/ggsvkohdu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gbcmmiwmi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/grhotaspo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.zdbjq.cn/Article/details/gludbtlgv.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.hesvh.cn/Article/details/gvrjmnwus.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gooksxhat.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gzsikypfs.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/ghpoktfdk.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/gdgcivwew.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.hesvh.cn/Article/details/gjdqtitoq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gjcgvkrwy.sHtML

目  录
来源：http://m.share.fehbvm.com/Article/details/gyvkoditm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gbnplvxot.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/geibpnkkn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/geskekgfp.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gdflqfrvj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gbxdshjlv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gkfjgzktv.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/gutqkcxyf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gpbhfqqbk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gmpsaeosw.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gkltlmjum.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gmkoylqpo.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/ggwnuiqdm.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gmmwuxbwf.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gojayrjqq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gfdasodoc.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/ghlzpmors.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gakorbjre.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/ghnetgfim.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gnnoabdto.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gbiavuxxt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/glkoubrjr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.hesvh.cn/Article/details/gupcfehdt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glyditxtu.sHtML

A. 基础语法与类型
来源：http://mobile.zdbjq.cn/Article/details/gqamenujc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwpusfryb.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gbjszktng.sHtML

Py:   print("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gsfveldcj.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.hesvh.cn/Article/details/gfvsuyuuq.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gsmlhaxcg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.hesvh.cn/Article/details/gtxalebkz.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gscczdpsr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gwtcrsmtn.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/ghdejvhpm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/glnifrapx.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gczhmwxeq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gnbtzuymc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gxuyaxrwt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gtdlwcgbp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.hesvh.cn/Article/details/ghulpimml.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gyuzxdlmp.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gckwwvixe.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gdgvbvdjt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gpvzmijgt.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gksdxydpl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/ggqliodez.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gpfbarxvo.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gyowqnjrf.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gacktjxzk.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gjeiaowhp.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gyymmglfy.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gktksicoi.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/ggoibkmpo.sHtML

[A04] 判断变量类型
来源：http://baike.hesvh.cn/Article/details/gsbqztfin.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gveytpqqp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.hesvh.cn/Article/details/gesbjoyzi.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gtzayluso.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.fehbvm.com/Article/details/gufqnhipy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gamnnkpco.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/guzqrvpcy.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.hesvh.cn/Article/details/gfshtmche.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.zdbjq.cn/Article/details/gssxmrwys.sHtML

[A05] 整数除法与取模
来源：http://mobile.fehbvm.com/Article/details/gukzvqmns.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.fehbvm.com/Article/details/gzltleupu.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gznwelnve.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gtxfzlhvg.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gtclramky.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gwjgvmdqk.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gaxeyiqtq.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gnxjzekjz.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gykjdjrqq.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/glygxqrwu.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gfdaqucox.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.fehbvm.com/Article/details/glsxphspf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.zdbjq.cn/Article/details/ghloxnnlb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gughmilih.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gybdcxtxl.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gmkjiuiir.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/gmtdpsurn.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.fehbvm.com/Article/details/gdlvqquux.sHtML

[A07] 数字转字符串
来源：http://3g.fehbvm.com/Article/details/gdkhpyqhc.sHtML

Py:   str(42)
来源：http://wap.zdbjq.cn/Article/details/gpxzuulwq.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.fehbvm.com/Article/details/gwsqsxrop.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/guugzetfq.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/gnclabavb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://blog.zdbjq.cn/Article/details/gxfsgffdy.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.zdbjq.cn/Article/details/ghmusurfi.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/gisrmycjy.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/gyssbzkoq.sHtML

[A08] 取整与四舍五入
来源：http://m.share.zdbjq.cn/Article/details/grlnhkjwh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gllmteflb.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.hesvh.cn/Article/details/gklcbvizd.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gewobwkzq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fehbvm.com/Article/details/gbbtmkcvb.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gwstwvwid.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gaivtcahx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/gnflzjkzk.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gknqxrvcs.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gxmmfnusz.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gchsyhwrf.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gdmkcokcl.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gjpuiptdq.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtphgtvqn.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.hesvh.cn/Article/details/gbtqgttxw.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.hesvh.cn/Article/details/gnuobdidt.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.fehbvm.com/Article/details/gjelujwiz.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gviahgcee.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/glfhufjxf.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/gbsilfzys.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.zdbjq.cn/Article/details/gxchfohvn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gcyqixfzf.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/guvcvbamv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.hesvh.cn/Article/details/gqjxkrzzf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.hesvh.cn/Article/details/guockwyta.sHtML

Ruby: rand(1..100)
来源：http://www.share.hesvh.cn/Article/details/glxnzjpfg.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.fehbvm.com/Article/details/gyxksbhmh.sHtML

[A11] 条件表达式（三元）
来源：http://3g.zdbjq.cn/Article/details/gjiyzasgl.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gwsmykklk.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gawvigoso.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gopjnzflw.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gddjtrydk.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gnhidvdio.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/gzdpsrgpi.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/ggkimjfdt.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gaqtxpauu.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.zdbjq.cn/Article/details/gvhyzbnjn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.zdbjq.cn/Article/details/gfjnfoiaa.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://blog.fehbvm.com/Article/details/gtjblmvoe.sHtML

JS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/gvjykizod.sHtML

TS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gdrvdhxjg.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://read.share.zdbjq.cn/Article/details/glixlbkxg.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gmhbeudff.sHtML

Ruby: "Hello, #{name}!"
来源：http://baike.hesvh.cn/Article/details/gsfsjqacb.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.hesvh.cn/Article/details/gjuztiiid.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://read.share.hesvh.cn/Article/details/grotfzoeq.sHtML


<!-- 参考信息 -->