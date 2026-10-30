代发 wailian999

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/giimuuzih.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gqnsehyum.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.fehbvm.com/Article/details/grfjjerqi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.zdbjq.cn/Article/details/gtdkzwtuc.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gcufmjeco.sHtML

npm init -y;  npm i express
来源：http://wap.fehbvm.com/Article/details/gsejzczat.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.hesvh.cn/Article/details/gmthhlejf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gihdputyf.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gxinjmcse.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gfkugzdrk.sHtML

[U84] JS：CommonJS 写法
来源：http://www.share.fehbvm.com/Article/details/gyannaaug.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.zdbjq.cn/Article/details/geeetawut.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/gaehmcplj.sHtML

a?.b?.c
来源：http://wap.zdbjq.cn/Article/details/gvieufrha.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/glzahnafk.sHtML

a ?? b
来源：http://m.share.hesvh.cn/Article/details/gnxthsauk.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gifkdpfir.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/ghticikxv.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gjnpuxguo.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gevnyzbmt.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gkdgfnmqt.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gxqcdqkxt.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gdqwhiinj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gteehmjrp.sHtML

[U91] JS：对象键值遍历
来源：http://3g.hesvh.cn/Article/details/gjxvbxvvv.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.hesvh.cn/Article/details/gtdogaxuy.sHtML

[U92] JS：深拷贝
来源：http://m.share.zdbjq.cn/Article/details/ggaqxugxs.sHtML

structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gkaekdjjl.sHtML

[U93] JS：模板字符串
来源：http://blog.hesvh.cn/Article/details/gcfawzrec.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gwwuzuygb.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gdzyzrzsr.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gbmosdowy.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/grijkbcwl.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/gbshakani.sHtML

[U96] JS：async/await 与异常
来源：http://mobile.zdbjq.cn/Article/details/gasqqjlcq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gxawkkxhb.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gtdpqkbun.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gciqctpya.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/grosdjcxk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gezlcqwug.sHtML

[U99] JS：事件监听
来源：http://m.share.hesvh.cn/Article/details/gdbqmtmki.sHtML

el.addEventListener("click", e => {})
来源：http://blog.hesvh.cn/Article/details/gasdfzmrr.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gswfqmnxu.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gelwnfmly.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/grzvwchkc.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gunfdlbhn.sHtML

[U102] JS：本地存储
来源：http://www.share.hesvh.cn/Article/details/gjbubxarb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gidubmbgk.sHtML

[U103] JS：定时器
来源：http://3g.hesvh.cn/Article/details/gwxboufvh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.hesvh.cn/Article/details/gtymgwsio.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/glykeqloh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gkjoaajse.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gncebpiju.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/goqvzaszo.sHtML

[U106] JS：日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gthbvforn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.fehbvm.com/Article/details/gjrqyfhof.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/genphfzfe.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gpwkyjqio.sHtML

[U108] JS：随机整数
来源：http://m.share.fehbvm.com/Article/details/gogxtazll.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gxozkbaot.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gdnikevft.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gylztanxq.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gwxivokax.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.hesvh.cn/Article/details/gzovgpgsv.sHtML

[U111] JS：对象转 Map
来源：http://mobile.zdbjq.cn/Article/details/gqmwthxwf.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gqwjtgchu.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gkjucfcql.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gzrywwurv.sHtML

[U113] JS：正则替换全部
来源：http://blog.zdbjq.cn/Article/details/gmqwdnfhl.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfazudlon.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gfyiedysl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gqwgyzdbt.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gulpthslp.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gydlfgnhp.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.fehbvm.com/Article/details/gzpyvpall.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.zdbjq.cn/Article/details/grjgssysu.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/graigczmy.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.hesvh.cn/Article/details/glndplcqp.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/giyybzggp.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/glulraynz.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gxbubnatv.sHtML

npx vite build
来源：http://baike.hesvh.cn/Article/details/gubwtculp.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.fehbvm.com/Article/details/gpoqftapq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/gnwfvkgkl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyjnxgmzz.sHtML

统计汇总
来源：http://baike.fehbvm.com/Article/details/gmgpluqyy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/givzisemx.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gkklnoclx.sHtML

Python ......... 252
来源：http://wap.hesvh.cn/Article/details/gcpxyercn.sHtML

PHP ............ 252
来源：http://read.share.zdbjq.cn/Article/details/ghsjtuhfg.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gdugsxvxr.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/giyaprgpa.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gjtvrrmmo.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gyanfiacy.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gcuvqlwjn.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/gibpluftw.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gewdjxppw.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gudqnqqfq.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gdeheyvfl.sHtML

Bash ........... 80
来源：http://www.blog.fehbvm.com/Article/details/gaakyiynp.sHtML

Kotlin ......... 15
来源：http://read.share.hesvh.cn/Article/details/gbysxvztj.sHtML

Swift .......... 15
来源：http://baike.hesvh.cn/Article/details/gfejvzqup.sHtML

Lua ............ 10
来源：http://3g.hesvh.cn/Article/details/gfoayyqvf.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gnuaqcswl.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gywvmwvxk.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gyxdvhgwk.sHtML

合计 ........... 2106 条
来源：http://www.blog.hesvh.cn/Article/details/gmamjsibn.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gbtpgtwbu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.zdbjq.cn/Article/details/gprfprxqt.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/grpxyszdj.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gneyeheio.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/guhdfwsll.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/guqvzyqjn.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/ggnikgeor.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gkqkmxrjf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gpgupihcj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gopwwmjft.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gbsdqxgay.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gulijeirk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gozmazahm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gyndmquwy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gzmdoaqub.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.hesvh.cn/Article/details/glkpghtsg.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gqigxcoik.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gwhoymhhz.sHtML

R Bash 专题                             80
来源：http://wap.fehbvm.com/Article/details/gckvnwesw.sHtML

S C / C++ 专题                          60
来源：http://www.share.fehbvm.com/Article/details/ginijdlng.sHtML

T 其他语言补充                          60
来源：http://www.share.fehbvm.com/Article/details/gjnwzdeog.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gxetwfbqi.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/glaeejuze.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/gfngibkoy.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gpfkzngxn.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/ggcurpngx.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gnrmrpvvu.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gygeuxdoi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gpywlvlye.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gpobwlzsn.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.zdbjq.cn/Article/details/grbgwdpvp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/gsivgnezi.sHtML

—— 文件结束 ——
来源：http://www.share.hesvh.cn/Article/details/gbquhhqni.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsouijmmx.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.hesvh.cn/Article/details/ghmjdzseu.sHtML

Common Programming Examples Cheat Book
来源：http://baike.hesvh.cn/Article/details/gibkyguph.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsandnlor.sHtML

【收录内容】
来源：http://read.share.fehbvm.com/Article/details/gzolwlrdh.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.fehbvm.com/Article/details/gkzxbqkit.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gvbclxgfb.sHtML

SQL · Bash · C · C++
来源：http://read.share.fehbvm.com/Article/details/gwedvjthw.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.zdbjq.cn/Article/details/gnsndzrfy.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gydiosumn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/garjfvzwh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/glhdsulem.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gdmsywtjh.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gkbxrydpu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.fehbvm.com/Article/details/gsoxrgeml.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.hesvh.cn/Article/details/geujxmnxq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/gjanbrfns.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.fehbvm.com/Article/details/gxssgiwez.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gzzuvsdyj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gfijcphgb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gfgpcnply.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.hesvh.cn/Article/details/gthoilppy.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gqfnbsyxc.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/goteuexqe.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gjmtnvcuy.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/gavcozkdm.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gioaywtsx.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gmgdzlzpj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gkvpugvpc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gpyevbzya.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gnnjltfdz.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.hesvh.cn/Article/details/ghzblhtup.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/girejnscl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gkpamrzlg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gzbprrlke.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gyuajpgnr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/glitnghck.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gsnzackpx.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gwymhcumg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqizlknko.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/glhjwswtx.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.fehbvm.com/Article/details/gvwwtnjkg.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ghgemrpnv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/gfxowxlyb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/gmengjoed.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gxbzbvkhn.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gwvcqtenw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.fehbvm.com/Article/details/gxsqckaxq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdwrpjoaa.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/gfvwougxu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvknzlxsm.sHtML

[A01] Hello World
来源：http://www.share.fehbvm.com/Article/details/glbvftotz.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gsbzobesf.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gxjhoimxt.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gyemnutbx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/gqxicawqh.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gkxqbnhev.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/goosctkal.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gatbnnywp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gvfusfwqe.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gejjeaslj.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.hesvh.cn/Article/details/gbohsqqsu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gnekecwsc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gwuzvlmkj.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/grdskocxl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gvfckvcwc.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gxfpkglde.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gnukhorjh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gtimdirpy.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gomzgvtdh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/ghpmqwukt.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gpkecakpr.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gbnjfvhct.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gpxpptjpd.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gkxahscyo.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/guuhvayya.sHtML

Ruby: PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/gqgfhgsbv.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gtjehbvuy.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gslivcbse.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.hesvh.cn/Article/details/gthflabfs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.zdbjq.cn/Article/details/giwvwamev.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gqnaolywb.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gkgwenmkh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.hesvh.cn/Article/details/gqahuqvrk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/gmdfdabgz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.hesvh.cn/Article/details/gpyndyyng.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gswydwsli.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gtgzuxaus.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.zdbjq.cn/Article/details/gyoucwzto.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/giqqyayue.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/goshodnko.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gybsorslf.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gfaqgegab.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gmrpdzjcd.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gpjjyllnc.sHtML

C#:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gkmvsvfic.sHtML

[A06] 字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gubkvfdoz.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/gmqewvexc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.fehbvm.com/Article/details/gkblxskhw.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gwnyfcphr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gmwstvbua.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gponkmgmj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.hesvh.cn/Article/details/gsjvqdcso.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.hesvh.cn/Article/details/ghfwhmikf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://3g.fehbvm.com/Article/details/gjtocoxrk.sHtML

[A07] 数字转字符串
来源：http://www.blog.fehbvm.com/Article/details/gigzttpse.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gpjgyooyu.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/gjeoxurgs.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.hesvh.cn/Article/details/gnmsocrtp.sHtML

TS:   String(42)
来源：http://m.share.fehbvm.com/Article/details/gpcygmkpc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gnfhgkdez.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/gchhtzjhi.sHtML

Ruby: 42.to_s
来源：http://www.blog.fehbvm.com/Article/details/gxnpduixi.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/gvaukpbke.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/glthwnlnr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/glpblihri.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.fehbvm.com/Article/details/gzfcwbmle.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/ggnbmjtxw.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://baike.hesvh.cn/Article/details/gpldgbchk.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gqamnajzl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gndehsnka.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.fehbvm.com/Article/details/gadzhdmvj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gpngxpydp.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gxdfrkthq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/ghqrmdcan.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.zdbjq.cn/Article/details/gcvwtygvm.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gmlficrad.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/ggweuqygz.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gvfyjnkrm.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fehbvm.com/Article/details/grhxeoing.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/ghlmakqhk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzrichtjz.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gjkddqoqi.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.zdbjq.cn/Article/details/gxytanhwi.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.hesvh.cn/Article/details/gbhcihbtc.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gmbngruyg.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gkvwxyqnb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fehbvm.com/Article/details/gcmbgzuxu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/gvsvxjpqa.sHtML

Ruby: rand(1..100)
来源：http://read.share.fehbvm.com/Article/details/gplbmcjjx.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.zdbjq.cn/Article/details/gksttcjyh.sHtML

[A11] 条件表达式（三元）
来源：http://baike.hesvh.cn/Article/details/gkvwjuuyi.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.hesvh.cn/Article/details/garblbnxq.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.fehbvm.com/Article/details/gyxtjnzes.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gobtallti.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gnqpqqoid.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gngieqwyk.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.zdbjq.cn/Article/details/gukwbbtdr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/ghpneweho.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gnbifpfan.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.hesvh.cn/Article/details/gkdtifhwo.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.fehbvm.com/Article/details/gobtpnqhj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wap.fehbvm.com/Article/details/gynthyagp.sHtML

JS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gozydwpwn.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gpstuiunc.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.hesvh.cn/Article/details/gkxwnrzkm.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.fehbvm.com/Article/details/gddumwxfe.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.share.zdbjq.cn/Article/details/gpgehvcxd.sHtML

C#:   $"Hello, {name}!"
来源：http://www.m.share.fehbvm.com/Article/details/gwrnxaiqw.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://blog.fehbvm.com/Article/details/gzdnvdupv.sHtML


<!-- 参考信息 -->