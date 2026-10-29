代发 wailian999

[U81] JS：初始化项目
来源：http://baike.zdbjq.cn/Article/details/gdsxjqbcz.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gkwgezeyw.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gzdjhdewt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/ghtayudus.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gkbqcbwzo.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gwvajvpfm.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gjvobsmum.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gbtdvxwmc.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/ghsyvqnyr.sHtML

a?.b?.c
来源：http://www.blog.zdbjq.cn/Article/details/gvasjdnch.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gqhwlvhvs.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gixdfzjku.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gdxygigyd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gckiwdgdm.sHtML

[U88] JS：对象展开合并
来源：http://3g.hesvh.cn/Article/details/gjjqkihzo.sHtML

{ ...a, ...b }
来源：http://www.m.share.hesvh.cn/Article/details/gobnlujdr.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gvxxdwrzl.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gltwpdhkg.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gvnutqtxo.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gsiyotezb.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/goujaplgp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gsehneahs.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/grgmsefcl.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gzydbudeu.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gsshvpuai.sHtML

`共 ${n} 条`
来源：http://read.share.zdbjq.cn/Article/details/gvntdggzx.sHtML

[U94] JS：箭头函数
来源：http://3g.hesvh.cn/Article/details/guiliagym.sHtML

const double = x => x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gbpawwcml.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gwfulgjsw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gdlorfkgu.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/gizzfdmjd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gchepscsw.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gwwqogguv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gkdurkcoj.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gtszxwtnz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.m.share.fehbvm.com/Article/details/gpigyfanm.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/gjiolkucj.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.hesvh.cn/Article/details/gsipwfzsi.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gcfnfqfmz.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gfxycpxro.sHtML

[U101] JS：classList 操作
来源：http://baike.hesvh.cn/Article/details/gyoioxspb.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gbukidakq.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gwdleekdy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gzloltrxj.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gkjhnzabh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.fehbvm.com/Article/details/gedrndwyy.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gllpckedn.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/grmrfrsje.sHtML

[U105] JS：节流
来源：http://3g.hesvh.cn/Article/details/gwmjcrwmh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gjnofiqrw.sHtML

[U106] JS：日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gubwrbdkz.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gpxcwlrrt.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gbwhtfxji.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gwqcmpwbo.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gpzsypstt.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.hesvh.cn/Article/details/gyausuerg.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gmuqkpjhd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gtjyzvhol.sHtML

[U110] JS：数组分块
来源：http://blog.fehbvm.com/Article/details/gcrgjlhns.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/glgunygdv.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/gueltsdtz.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gevyjjmsl.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gpusafpcl.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gejfyjikl.sHtML

[U113] JS：正则替换全部
来源：http://blog.fehbvm.com/Article/details/gutxllhxy.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdgrqouby.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gbagxqzzn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/giaxgvmwl.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gkiefvtoo.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gtkzhyjja.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gphwdymtl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.fehbvm.com/Article/details/guuazmzqp.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/gasacmfja.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/gsidsssaa.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gcdfrmvkh.sHtML

npm i -D vite;  npx vite
来源：http://3g.hesvh.cn/Article/details/ghfvrxyok.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/gfipwxjpw.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gvlimpryt.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/ghzfeqlzq.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.hesvh.cn/Article/details/gzmbtntea.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdliruetc.sHtML

统计汇总
来源：http://read.share.hesvh.cn/Article/details/gcxsezjbw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geqvzniuw.sHtML

按语言统计（条）：
来源：http://www.blog.fehbvm.com/Article/details/gbwaimnfg.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/gyxxtrjsd.sHtML

PHP ............ 252
来源：http://baike.zdbjq.cn/Article/details/gxdfdlkji.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gdhghzctb.sHtML

TypeScript ..... 212
来源：http://www.m.share.hesvh.cn/Article/details/gyoqctkji.sHtML

Java ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gmqvmlyxj.sHtML

Go ............. 212
来源：http://www.blog.fehbvm.com/Article/details/gwekacdon.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gfctmsgso.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/guegvilww.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gdmmcdchv.sHtML

C++ ............ 30
来源：http://3g.zdbjq.cn/Article/details/gsibmlgca.sHtML

SQL ............ 90
来源：http://www.share.zdbjq.cn/Article/details/gzutjliyr.sHtML

Bash ........... 80
来源：http://www.m.share.zdbjq.cn/Article/details/goozkyiap.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gvolcdtow.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gouqutlgg.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/gytppazwu.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gkneggdqq.sHtML

Scala .......... 10
来源：http://www.m.share.hesvh.cn/Article/details/gucakqbtz.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gqvaaipkz.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gcaryamim.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gycqokncc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gisobeham.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gywhtzzkw.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gdthvawyc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gbbwiwhia.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/guuispmug.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gymyjgcnf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gpjfdtlwe.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/glyrqcfgf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/grpnwwvgr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/glnwpotuv.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gprlsegtr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/ggkjiubzy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gadjfxgbg.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gbzfvspiw.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://m.share.zdbjq.cn/Article/details/gwguoilvs.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gwdnjnjmq.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gbiuclokz.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gmthbcrxz.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gqtazoodu.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gfpspkgqf.sHtML

U 高频实用片段                         120
来源：http://read.share.fehbvm.com/Article/details/gcxatrfiu.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gujpsakbu.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gcomiyrtb.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gfamnqtus.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gukpqbuxo.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/ghutnjrto.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gspijrnsc.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.zdbjq.cn/Article/details/gbchixdcy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gzzgzvkmz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gqcltyhho.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.zdbjq.cn/Article/details/glhxritvt.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gpgdapofj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grtjrlzcu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gdsjnummj.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/gbsrnpsab.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmvavtejw.sHtML

【收录内容】
来源：http://www.m.share.hesvh.cn/Article/details/gnxwhgorp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.hesvh.cn/Article/details/gstybdeeb.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/gqfmqqqmh.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gpjkhwuvk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.fehbvm.com/Article/details/grkbcxfml.sHtML

【使用说明】
来源：http://wap.fehbvm.com/Article/details/goskukksm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gzckoelaj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/grxzfnxlj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.blog.hesvh.cn/Article/details/ghoqtjgyp.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gzhhupcud.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gacxabexd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/ghbvxwjha.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gywmzismh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.hesvh.cn/Article/details/gvqlfpwac.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gdaqlumfx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.share.hesvh.cn/Article/details/gpyxnzvwn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gjilkbjon.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gnndqpwiu.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/gnmixfvqp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.zdbjq.cn/Article/details/gatfubdxz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gfkvlpurc.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/getvchrxr.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/giuktsgku.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjypdmqjz.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/ggihipufw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gunailvph.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gzrimnxas.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/gelumccal.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gyyzxgbyx.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gbrbjervb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gmfgbjwmg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gejhqhydu.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/glabtgcds.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gbaknlmfk.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/grlogdyfp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gopggqrlx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gwepdfbzs.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.zdbjq.cn/Article/details/gupxoaqfp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gnblscduk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gvnuwmstd.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbbjlcski.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gvsbmrzlt.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gtbkvcczw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/ghhpsdwlk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtfmjwmwh.sHtML

A. 基础语法与类型
来源：http://www.share.fehbvm.com/Article/details/gkqhmuwrg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpivvpesp.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/gtowhqzvs.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gxeyghgjw.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/gtklovdpa.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gbdtoahuq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gyldilqpg.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gjffunsjp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gajxiqwmq.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.zdbjq.cn/Article/details/gyrfkxbdk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/grbwwrdpu.sHtML

[A02] 变量声明与赋值
来源：http://read.share.zdbjq.cn/Article/details/gbuephbdp.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gmarbnjva.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gamrdupaf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.hesvh.cn/Article/details/geqngsakr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gdetivefl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gwatuefpf.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/gllksorpv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gmccjjtzq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gghgyvjem.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/gqcyxprbi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gcgdvghct.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gtfhftcvo.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/giaeggvxh.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gukyruoen.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gsnbpbepc.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gbmyjvanz.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gmcrifrxt.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gzffdrprx.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gnwqnpoec.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://3g.hesvh.cn/Article/details/ghidnhrnc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/gcsthqhry.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.share.zdbjq.cn/Article/details/gappmzxqk.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gwacuzgqa.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/gfbgumdre.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gjtqsfeci.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gnmpemizp.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gaglfxqpx.sHtML

[A05] 整数除法与取模
来源：http://read.share.hesvh.cn/Article/details/giuknxdke.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.fehbvm.com/Article/details/gccnhtsvi.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gefwuysms.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gahlcodfe.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.fehbvm.com/Article/details/gwjfokiog.sHtML

Java: 7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gumtupdyk.sHtML

Go:   7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gunanvwtn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gjzlipaxi.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gwwilgybf.sHtML

[A06] 字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gzjlnizof.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/gobrjznnb.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gwtbpufoz.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/ghhepvbjl.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.hesvh.cn/Article/details/gkyyldobe.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/gygzfrhry.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gtbhjgxxf.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.fehbvm.com/Article/details/grwnvapuj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.zdbjq.cn/Article/details/gmusynrci.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gcmcghrtb.sHtML

Py:   str(42)
来源：http://3g.zdbjq.cn/Article/details/gckrhuyda.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/glykjewpl.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/ggdbhwtrn.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/gqpcjsvxk.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fehbvm.com/Article/details/gmemodykr.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.zdbjq.cn/Article/details/gqqsiehag.sHtML

Ruby: 42.to_s
来源：http://wap.zdbjq.cn/Article/details/grsfneysv.sHtML

C#:   42.ToString()
来源：http://baike.zdbjq.cn/Article/details/gdftdrmzd.sHtML

[A08] 取整与四舍五入
来源：http://baike.fehbvm.com/Article/details/glbchhlwm.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gifnuomwq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/gqsjtlkms.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/geymmsnav.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.fehbvm.com/Article/details/gytlghabg.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/grlutdtio.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gisaxreah.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.zdbjq.cn/Article/details/gknmrpkok.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gacgnnhrp.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gncolsonr.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gyvpygoge.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gkgbmcdql.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gedgvcajo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjhohngwy.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gaknkubxj.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.hesvh.cn/Article/details/gpzjcaphw.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.zdbjq.cn/Article/details/ggazcbyse.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/ggsxpwnse.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/gavthzhhv.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.hesvh.cn/Article/details/gaatznyxv.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.hesvh.cn/Article/details/goxhstlzv.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/ggpgntyrk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gdhbumvkv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://baike.zdbjq.cn/Article/details/gjcypallv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.share.zdbjq.cn/Article/details/gekauljdz.sHtML

Ruby: rand(1..100)
来源：http://www.share.fehbvm.com/Article/details/grwxngdnd.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gxzmfvgqj.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/gpvdnxqnn.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gqjxqztpm.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/ghtixxyga.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gwqczuusg.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gcmacntqf.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gyfxeylfz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.fehbvm.com/Article/details/gfqgrwpvl.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/ggdbhyfck.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gcpibpvjm.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fehbvm.com/Article/details/gmlunwlgr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://baike.zdbjq.cn/Article/details/gdankbcba.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.hesvh.cn/Article/details/gapbdlezc.sHtML

JS:   `Hello, ${name}!`
来源：http://read.share.zdbjq.cn/Article/details/glbqyubua.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.hesvh.cn/Article/details/gxcrfkksz.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.hesvh.cn/Article/details/goimtgwmq.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://blog.zdbjq.cn/Article/details/gkxynsntr.sHtML

Ruby: "Hello, #{name}!"
来源：http://blog.zdbjq.cn/Article/details/gxkpplkvx.sHtML

C#:   $"Hello, {name}!"
来源：http://blog.zdbjq.cn/Article/details/gfuegzwhr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://m.share.zdbjq.cn/Article/details/gcjfshaka.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gbelzucjh.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.hesvh.cn/Article/details/ghkojvafx.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gqxxedlpk.sHtML

TS:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gjbsxplzm.sHtML


<!-- 参考信息 -->