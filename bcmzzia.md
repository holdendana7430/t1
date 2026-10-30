代发 wailian999

[U81] JS：初始化项目
来源：http://m.share.zdbjq.cn/Article/details/gmyllsrld.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gdnxommjh.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gxoimflvq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gtwxpsojd.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gjuejvmtf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gddoszjka.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/grhkksvmz.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.hesvh.cn/Article/details/gdpumnjtd.sHtML

[U85] JS：可选链
来源：http://read.share.fehbvm.com/Article/details/gzhwuowhu.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gwwpiqemr.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/glwkbhbro.sHtML

a ?? b
来源：http://www.share.fehbvm.com/Article/details/gbflbxegv.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gxxahdpvu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/glnfyapqh.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gfaadweyw.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gsokkebne.sHtML

[U89] JS：数组去重
来源：http://baike.zdbjq.cn/Article/details/ggaynszom.sHtML

[...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gzejjhovz.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gvcblslqc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/ggszqrxdu.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/ggdnpytth.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://3g.zdbjq.cn/Article/details/ggnlsvrrz.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gfmmjdict.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gfshapoui.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gmguolwwp.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/geiaaehsi.sHtML

[U94] JS：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gmjkbmcdy.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gkzbyswrr.sHtML

[U95] JS：Promise 包装
来源：http://mobile.hesvh.cn/Article/details/gfqtqljnq.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.fehbvm.com/Article/details/gdjoxsxkc.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/gcljfsqlt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gvfwvyfte.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/glyxiwwye.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gqrdkpzsb.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/gcmbpsvlu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.hesvh.cn/Article/details/gynnyrbph.sHtML

[U99] JS：事件监听
来源：http://mobile.hesvh.cn/Article/details/gmffjtjti.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gbxkjrbot.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/gtewjersd.sHtML

document.querySelector(".item")
来源：http://wap.hesvh.cn/Article/details/gozvtqacy.sHtML

[U101] JS：classList 操作
来源：http://wap.fehbvm.com/Article/details/gjytmudwv.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gtlnowiod.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gunbcasvc.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/garlpbtou.sHtML

[U103] JS：定时器
来源：http://blog.fehbvm.com/Article/details/ghnlokeix.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gkraqxmmx.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gclxvcase.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gmnyhkiws.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gyvsnnmrr.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gutoppykf.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gmesyutfj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gduzrxzzh.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gojovdtyg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gxnvsnprj.sHtML

[U108] JS：随机整数
来源：http://www.share.hesvh.cn/Article/details/gqpuwnkvm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.fehbvm.com/Article/details/gbjbjonmq.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gawfdjwxb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gmwihiifb.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/gkhmoxvgq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.zdbjq.cn/Article/details/gwjugsxjw.sHtML

[U111] JS：对象转 Map
来源：http://baike.fehbvm.com/Article/details/gutgsfdlx.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gihssdieg.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.fehbvm.com/Article/details/gaqfxthaw.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gyilpoqsz.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gufpnvyli.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ghilxoffs.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.fehbvm.com/Article/details/gayimbyko.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/glluebcos.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gnzuonnfb.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/ghlhxvfqr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/grakdmvtf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.fehbvm.com/Article/details/gydreoyls.sHtML

[U117] JS：单元测试
来源：http://mobile.fehbvm.com/Article/details/gxxcdmdnx.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/gducqnjtj.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gfifpxgfz.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gmfnawvir.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gsrziqlof.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gtcusmcjh.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gimjtnuub.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gzqordnvv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfwiposcb.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gnuslsgip.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbpkyukcg.sHtML

按语言统计（条）：
来源：http://baike.zdbjq.cn/Article/details/gaxvrxlni.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gynumncjk.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/gdlvbhhmc.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gwssnousi.sHtML

TypeScript ..... 212
来源：http://3g.hesvh.cn/Article/details/gtozvdwvf.sHtML

Java ........... 212
来源：http://3g.hesvh.cn/Article/details/gnilorhsv.sHtML

Go ............. 212
来源：http://blog.fehbvm.com/Article/details/gencdgvvu.sHtML

Ruby ........... 212
来源：http://wap.hesvh.cn/Article/details/grtqtjeab.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/gwgjxqfyq.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gudpxbros.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gtxsavqxw.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gzzibfciq.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/glgbxccxw.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gvkpcbxkh.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gyhqeeqpp.sHtML

Lua ............ 10
来源：http://www.m.share.zdbjq.cn/Article/details/ghihjsnem.sHtML

Perl ........... 10
来源：http://www.blog.zdbjq.cn/Article/details/ghblpenik.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gulhjdevq.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/groavhuzs.sHtML

合计 ........... 2106 条
来源：http://www.share.zdbjq.cn/Article/details/gxfwyyiiv.sHtML

按章节统计：
来源：http://www.share.zdbjq.cn/Article/details/gowmfltsk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gvmgezxwb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/guqytfstt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.hesvh.cn/Article/details/gekdylsyx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gkmrxdmtw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gsckvxkmc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.zdbjq.cn/Article/details/gxlqohomk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gwzsgfalh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/ghizcrmwi.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gcwrgwrsm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/gctkydrpq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gmcboqlxs.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gsgphgwii.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gsbzoixou.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gfpulmwke.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gshyojwqu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/giwbqamfz.sHtML

Q SQL 专题                              90
来源：http://www.blog.fehbvm.com/Article/details/gqxgrhgdw.sHtML

R Bash 专题                             80
来源：http://blog.fehbvm.com/Article/details/ghnqdizsm.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gdovvnfsu.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gmydyraei.sHtML

U 高频实用片段                         120
来源：http://m.share.zdbjq.cn/Article/details/gxwbltpqi.sHtML

------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gwcppnvji.sHtML

合计                                  2106 条
来源：http://baike.fehbvm.com/Article/details/gjqbdifhh.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gnwdcwcpf.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gqntmskct.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gnvewyluy.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gcljglvrf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/gdnxepopo.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gkzmjztni.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gkvftakdb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gzyqyvaid.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gisombstw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqezhjmot.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.hesvh.cn/Article/details/gzxkuliyk.sHtML

Common Programming Examples Cheat Book
来源：http://blog.hesvh.cn/Article/details/gxymbtajm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqgxxzrpe.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gpcqvyepq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/glwkcjgmo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.zdbjq.cn/Article/details/gaosstftp.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gztxogwmi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gltrurmmr.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gmotdbuij.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.zdbjq.cn/Article/details/gzrmrpecv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.zdbjq.cn/Article/details/gywzkmqzn.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gjoxsccrz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gggxhuehj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gyxoeyphd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/givnnzblw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gjzpihdrw.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gfusvcfzd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gsfuqkwbt.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.hesvh.cn/Article/details/gtdxkmupm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.zdbjq.cn/Article/details/gruuhsxfg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/gjvmaktqy.sHtML

【文件统计】
来源：http://wap.zdbjq.cn/Article/details/guohknxlr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gycxbotou.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/grlhcvxce.sHtML

目  录
来源：http://read.share.zdbjq.cn/Article/details/gejawdgiy.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/genfewhvw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gvmthvvai.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gvgcejwin.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gxujdxwff.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gjqiyffjc.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gopnxkwwz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gkintzomh.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/ggkvjdeba.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gvisfqgre.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gsjeddjvk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gdkoscrqi.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gwjkxnrtu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/ghwmuppgo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gyjnuiees.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gpyqgfqlz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gvuqbyoub.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gmkssehuz.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gcglknkwk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gmxyiongq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gwaeqyadi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gbigkzjas.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/graugqsap.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gppzulinb.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/ggqmjaouw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbywinpui.sHtML

[A01] Hello World
来源：http://read.share.hesvh.cn/Article/details/gxmoimdmj.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gkjewfhmk.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gfjshwffd.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gmqmunpvr.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gvivhfdqd.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gxhvceulx.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fehbvm.com/Article/details/gdqnoqpgo.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/glcztevvr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gkpcmeshv.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/gsgvrfymx.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gohyckhnb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gbvmwttyt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gjynkydjo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/goemrygyy.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/ghoattcao.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/gavuqdirp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gufgwzpyi.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gzdtfjeew.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/gxzgrbwzu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/ghozffcrx.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/ghppbgmeq.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/ggvrkzoek.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gtnhgmzim.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gbupnqdvg.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gkjolvtba.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gruyxapva.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gqpucplzg.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gcgbfpzaf.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.zdbjq.cn/Article/details/gvfmjpwcd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/gjtrlpiac.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gaybcfahx.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gndupdqfp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/gvqgoburu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.zdbjq.cn/Article/details/gfowrcdbf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.zdbjq.cn/Article/details/ggqkrdzpp.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.fehbvm.com/Article/details/gyzyhpyah.sHtML

[A05] 整数除法与取模
来源：http://wap.hesvh.cn/Article/details/gimkohmkj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gnrscettt.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gniuhnbxq.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gkoyayypr.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gpmtikbgl.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gipkqafro.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gyqjjhync.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gagfmrvhm.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gusqftfyo.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gxsrbzhui.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.zdbjq.cn/Article/details/gavfvvnqf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/gsavfprtc.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gbbecmtog.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gkjncvmvm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.fehbvm.com/Article/details/grecvzwfz.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gyxczhzgu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.hesvh.cn/Article/details/gfdobifnf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.hesvh.cn/Article/details/gydwpajob.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/gyzkczqck.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/gyankedis.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/gokruuoyw.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.hesvh.cn/Article/details/gtybepvlg.sHtML

TS:   String(42)
来源：http://baike.fehbvm.com/Article/details/grrdicboe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/gkuzobayn.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gstxkycui.sHtML

Ruby: 42.to_s
来源：http://www.blog.zdbjq.cn/Article/details/ghnqnvqra.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gtjbcbsav.sHtML

[A08] 取整与四舍五入
来源：http://baike.zdbjq.cn/Article/details/gvecqxzoo.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gboqonkxg.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fehbvm.com/Article/details/gzlwyodos.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gkookyqxc.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.zdbjq.cn/Article/details/ghkqmzjxd.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gobtsoldt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gmjluihpg.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.fehbvm.com/Article/details/gvhsgedgc.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gmjgfsnci.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.hesvh.cn/Article/details/gxgwyhmgo.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/ghbckcarb.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gvqqoshgj.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gjsrdxvom.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gpbcuyqnk.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/giqwnnfte.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.zdbjq.cn/Article/details/gmmlbzgvv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/gumdsywcj.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gsjcmogsy.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/gzyopmwsh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.zdbjq.cn/Article/details/ggaimngkg.sHtML

PHP:  random_int(1, 100);
来源：http://3g.fehbvm.com/Article/details/gjxebecox.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.hesvh.cn/Article/details/gqoeufcip.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gstxgztfd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/giflbthhn.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/gzqfnvwhs.sHtML

Ruby: rand(1..100)
来源：http://m.share.fehbvm.com/Article/details/gypnlkjjt.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.fehbvm.com/Article/details/ghziwmqlp.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/gwvobuvib.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.blog.fehbvm.com/Article/details/ggvvgpzdh.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gjtxzikga.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gblufdyhj.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/ghxdbqwgt.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gwuhqmugw.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.hesvh.cn/Article/details/ghfctoxlp.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/grmkwpvvq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gmeiqjgco.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/gjconhhbf.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wap.hesvh.cn/Article/details/gktaegnwi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fehbvm.com/Article/details/gwsihubhz.sHtML

JS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/ggvbtnycz.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.hesvh.cn/Article/details/glpqnxdck.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.zdbjq.cn/Article/details/glwdrqtda.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.zdbjq.cn/Article/details/gjgprtmdg.sHtML

Ruby: "Hello, #{name}!"
来源：http://3g.zdbjq.cn/Article/details/glcxjmkji.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gexrhbqbm.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.share.fehbvm.com/Article/details/gnrnddamt.sHtML

Py:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/grfntrdib.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/gdlvbsgxc.sHtML

JS:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gocxqhygl.sHtML

TS:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gymqlhzuf.sHtML


<!-- 参考信息 -->