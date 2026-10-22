代发 wailian999

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2klayqrmc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2gucdikjx.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2holxmesj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2qfolfpri.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2vmkrlsnq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2faqhodfu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2jjdxwcgg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2kynbutsj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2pnjultkb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2cmkjbhdn.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2ptculino.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2jzszuelr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yeffcvzs.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2zoqhfmtt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gvbvwgpo.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ytethkmj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2xmoamkia.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dmjrbuqg.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2jcmjrrrk.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2oytzawtn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hhzvettt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2bfmixlgr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lagpbuba.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tjprbxwv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2edpzinay.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2xyektvmx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rowkpjmb.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2gwbsuvmf.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ytdmphke.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ypknrjvm.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ehtxorop.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2urganlje.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2qvekhhgw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qbvgzmqx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bjnsiudv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ebwuuree.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2xpkodigz.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2bhhqtwbb.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2idkvvrcu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2dysmcnft.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ddimzwxc.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2aggtflyw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2dnldbgex.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2jalwaimt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2kutpzppc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2iczabejv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2hpfbszto.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2phwikxnp.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2upbmvzpa.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tttpeoll.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cjjzqdfm.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2jtcqjaqe.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yibjamsd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kitxsllk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2kvygybmy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2vamweerl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2lyhdiclv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jrpvrysz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2ltgpvpmw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2kcqrxujf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2gowzpzai.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2agctwxgq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2lsnoelnz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bqujgoyx.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2imekwyne.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tikznkrv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2umolfjfx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zrwaotrj.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nepgltba.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xyfnvour.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2neismats.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2azqlinzh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vmujhxom.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2bgmjhfnd.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2nifuwhfb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ubtohimn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2nghlrlqy.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2domflizx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2kqwfcsxx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2fabfkoxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxkahfig.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2wnxqnkhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgpabhjl.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2ahbeqznp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rhdmkwdm.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2jetvdbtp.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2wjjteyom.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2hvfgdvpf.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2dppbqzyy.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2bipqjjpy.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mhwwsans.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2eiectesp.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ezbpjqqr.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2afutxbrt.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2qdscbqpe.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2qkdldyog.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2pcdpbljb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2wbigywds.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ddsybzau.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qjfenchf.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2xcgsxkdi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qkcxbfbz.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2stbvjsqb.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2taqjhhjl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2whzvdvlh.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2gpxsdfha.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2jklyneyj.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2kznyegxk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2warntbmm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2gaqdivlp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xoygooth.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2bbpcvfot.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mvmsohfz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gjvglypd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ikpkvskp.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2szjbnuyw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xikcgbui.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2yursrvcb.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2vdkaohyw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2snwwooaa.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2jaehjvyd.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2tojmlgna.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2yqjvwbdi.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2hfuenzat.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ngfeeytw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kuovmyad.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2vdcmeeia.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zcohnktz.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2abhpcrtz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yzfkumzw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ijsbeplj.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ebmkwvas.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2abscrera.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2msnbxdlg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2prwtlpff.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2itaqywjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fsfoyzbg.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2wvgimnrl.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2uzznunbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynczfgxi.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ymwdypdr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2rlfeuvmt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2nyipcqcg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2cwhqvoes.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2gopgwojd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2reyioyad.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2rtytkdse.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2rvslciar.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2dxutqyku.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2efupnaog.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2mxvvyuqd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2khdzumnv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ucpupxpn.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2zwxhcged.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2jqhbxuhp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2smrcgsin.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2okqkxzkn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2aiyzolps.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2ngivgxwk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2wfydjcox.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zhoxqcnr.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2xvemjmrq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hwvqkznf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2szdwofsx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2netavlbq.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mmasmchk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2gdhyoade.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2qvxfjdre.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xhnofatz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2phdvcegg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2yshgcfew.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hjtwvclw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jluampsp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vccnhqkf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dejxspdt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fzvmdfuj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2goxktpdd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dmhgnnzi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ghlzreoo.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wnwxhmmf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cilixjfk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2quimcctj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2uxfrndii.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vlanajms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igbxqdcq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2bxaurcvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxzalzfz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wkumoksg.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2udblyucn.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2nzuapmlq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qqmjaxgc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2zkpnawki.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2uzztesgt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2tlaproxj.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2zwdoyuhm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ujptuvrv.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2tawodepk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2vvwejoda.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2eewwjyhn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2elyhxkqs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hfljbuzi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2awxtrkns.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ecmncand.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2vfesuqvo.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xbkfdhxh.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ytezxnya.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2wvkbwwdl.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zpkobdeu.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fapfardo.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pxsjgynk.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fushjtfs.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2xefrjgti.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2fjoybclb.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2rtitllok.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2vnomynhc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2higiqqpw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2lnrwgaon.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2hnshqwyg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2hydykkkn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2blrkrbrx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2pvnahbyy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2jcdxzcho.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2eismzxoy.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2hqiaitui.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2gibwmofb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gfdkcado.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2iovrkwvr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jflrwuqf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lwyslzug.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jmvkugsf.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qlzyfmna.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2puuyoiex.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2fecbddwi.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lklbnvfp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ftawpupf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2hqkuldvk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ojifuizd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2emmtarna.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fzwelmrh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2hfeuczwu.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rtkokdct.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ihhsitpf.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tgymysla.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ftazhdrn.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nuuuxaij.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wtilrvzt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2npzznglo.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vpixhjhg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2puboeisu.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2bmtemyfi.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2wqkyagae.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2bdlsbtyi.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2wotrkbmh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2czgagdpp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2rwzivpbh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bpnefuem.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zmbyqxyi.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2llmaiqqw.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rlrhfulx.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2tmuinrzr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2stfnmunx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wokobbwp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uxbipsxi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2niiitjoh.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xpejgwtf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2zukryzjw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2pbaymqfk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ylnclhjs.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2ioqtekgz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2udnauyqf.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2odxljjba.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2xslkrxke.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vplogifg.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2auajlmig.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2wlsxmihl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2yequhqeh.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2wteqrkcn.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ifilhxew.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2fbxqxrcs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xqkgjqku.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jsqrjhks.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2hnxitdib.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2svpeeklf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ewcfcxwx.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vzuculcw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vctaljfe.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xofifclj.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2mecmyjsp.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2gkirohqz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2nuqsmkib.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2oxrnkvpe.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ysyiskew.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ikcdeejz.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2phvqnqae.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2xknlymtp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qehnfskv.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2saashmva.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fzzapxkw.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tiwdbxpk.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kafqsdpr.html


<!-- 参考信息 -->