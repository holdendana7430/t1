代发 wailian999

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/gbublghma.sHtML

composer require psr/container
来源：http://www.blog.zdbjq.cn/Article/details/gxulbcxeg.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gipzkzbog.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://m.share.zdbjq.cn/Article/details/gysgrsicx.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gikejujvg.sHtML

composer require twig/twig
来源：http://mobile.fehbvm.com/Article/details/gptnohazu.sHtML

[U78] PHP：单元测试
来源：http://mobile.fehbvm.com/Article/details/gbelogmko.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/goslialgq.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/grglwxghb.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.zdbjq.cn/Article/details/gxctdiehq.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gtwntsvbl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gszxgsmgc.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gkjqirleh.sHtML

npm init -y;  npm i express
来源：http://m.share.fehbvm.com/Article/details/gpzygqypn.sHtML

[U82] JS：package.json 脚本
来源：http://baike.zdbjq.cn/Article/details/gqfwshvdi.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.hesvh.cn/Article/details/gppalirqm.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gatfygecc.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gnpwicfxx.sHtML

[U84] JS：CommonJS 写法
来源：http://blog.zdbjq.cn/Article/details/gmlcgcauw.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gorazkmyo.sHtML

[U85] JS：可选链
来源：http://blog.hesvh.cn/Article/details/gazaonlnb.sHtML

a?.b?.c
来源：http://wap.fehbvm.com/Article/details/ghlqnylsd.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gcwwlrrjz.sHtML

a ?? b
来源：http://3g.zdbjq.cn/Article/details/gjrcvildd.sHtML

[U87] JS：解构默认值
来源：http://www.blog.zdbjq.cn/Article/details/gldullbwo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.hesvh.cn/Article/details/glwvexome.sHtML

[U88] JS：对象展开合并
来源：http://www.blog.hesvh.cn/Article/details/gvrsushvf.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gynncxrjx.sHtML

[U89] JS：数组去重
来源：http://www.blog.zdbjq.cn/Article/details/ggtccgkmh.sHtML

[...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gqtgngmdw.sHtML

[U90] JS：数字数组排序
来源：http://m.share.zdbjq.cn/Article/details/gpqugtjcr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gjfnlwkne.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fehbvm.com/Article/details/govnkdrkl.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gmqruygjd.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gsuagzvtf.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gfjmyxlrs.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkpbjlgdj.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/gzcecniwe.sHtML

[U94] JS：箭头函数
来源：http://www.share.hesvh.cn/Article/details/gufgairtg.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gzluertqs.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gbftnfkex.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gplqcrabs.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gpncvfpdt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gqcuncpfp.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/goxjamynu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gwbgijzkg.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gmzenkgtw.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.zdbjq.cn/Article/details/gawocabni.sHtML

[U99] JS：事件监听
来源：http://wap.hesvh.cn/Article/details/gqmlitrpd.sHtML

el.addEventListener("click", e => {})
来源：http://wap.hesvh.cn/Article/details/gajfwykaw.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gmitvqrce.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/ggqdhqchd.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/guurviffq.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gzeauqnmc.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/gkpuhizcy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/grjenibgv.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/ghropzbqk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.fehbvm.com/Article/details/gcuylssst.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gqjowhdgc.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.fehbvm.com/Article/details/gutyxxbzi.sHtML

[U105] JS：节流
来源：http://blog.hesvh.cn/Article/details/glyniugit.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.fehbvm.com/Article/details/gltmygpaz.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/ghrmieygc.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.fehbvm.com/Article/details/gsevhgicu.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gvwngjmjg.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gpnonussb.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gmcfxainh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gupafkbpn.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gyhnzzapd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gwvqsmsgo.sHtML

[U110] JS：数组分块
来源：http://read.share.zdbjq.cn/Article/details/gjepkoejz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.share.hesvh.cn/Article/details/gsyvmzwvo.sHtML

[U111] JS：对象转 Map
来源：http://m.share.hesvh.cn/Article/details/ghzjiwesz.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/ggfzkudle.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gewxemddk.sHtML

"7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gmuvoyfou.sHtML

[U113] JS：正则替换全部
来源：http://3g.hesvh.cn/Article/details/gancaonff.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gqrxhcumw.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gmmbhyvto.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.zdbjq.cn/Article/details/gtyjjqifg.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/ghactcwui.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gjpipciac.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gxsmdwtdf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gfdfgtiil.sHtML

[U117] JS：单元测试
来源：http://read.share.hesvh.cn/Article/details/gjrdduwhs.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.fehbvm.com/Article/details/gdjmkcecq.sHtML

[U118] JS：开发服务器
来源：http://read.share.hesvh.cn/Article/details/ggforvgim.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/gtbsfsvgd.sHtML

[U119] JS：生产构建
来源：http://www.blog.zdbjq.cn/Article/details/gpauomfku.sHtML

npx vite build
来源：http://www.m.share.fehbvm.com/Article/details/gpxgfbjjk.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/gputighhm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/gycavzrvj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goxlvqspl.sHtML

统计汇总
来源：http://blog.zdbjq.cn/Article/details/giuzbodwa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjmmwdpiq.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gokzylhls.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/ggfvzmmct.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/guxscgkiw.sHtML

JavaScript ..... 252
来源：http://read.share.hesvh.cn/Article/details/gzlxlgowo.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gvxgablis.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gmutlhoip.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gueketncd.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gszfjfioh.sHtML

C# ............. 212
来源：http://blog.zdbjq.cn/Article/details/ghbwqurwd.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gqnihhimu.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/glqvnsbkj.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gzvouzymb.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gqcfyurrs.sHtML

Kotlin ......... 15
来源：http://www.m.share.fehbvm.com/Article/details/grehvycfn.sHtML

Swift .......... 15
来源：http://baike.zdbjq.cn/Article/details/glflrivcx.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/gdowivdcp.sHtML

Perl ........... 10
来源：http://www.blog.hesvh.cn/Article/details/gcogotnuf.sHtML

Scala .......... 10
来源：http://www.m.share.fehbvm.com/Article/details/geeeyvpdj.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gjsdpadvc.sHtML

合计 ........... 2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gqtyxnznw.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gycgstopz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/ghownorsu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/goegckmze.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gmbijtces.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/gtbxduvif.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.zdbjq.cn/Article/details/gbffabqfb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/gzgbdkmhf.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gveeafcxj.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.zdbjq.cn/Article/details/gbueeaqlc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gyzbyzfrc.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/glamdpnth.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gqxxogxzm.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gtfifolln.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gbnvxgbee.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/grubdxsbq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gpvmsrncq.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/goegogawp.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/ghoevtinq.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gtopovrxd.sHtML

S C / C++ 专题                          60
来源：http://blog.fehbvm.com/Article/details/gehemjrjc.sHtML

T 其他语言补充                          60
来源：http://www.blog.hesvh.cn/Article/details/gbjkaknfu.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gsxwdoerp.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/ghrmnnabs.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gsnzleliy.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/grarwjhuh.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gzjttcpfh.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gonlqupmg.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gflebeuix.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/grcthkkrn.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gtxxlftoc.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.hesvh.cn/Article/details/gbguuoiyd.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.hesvh.cn/Article/details/gzacolovh.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gxelqmccj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geoxzmyob.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/grhzzixzc.sHtML

Common Programming Examples Cheat Book
来源：http://3g.hesvh.cn/Article/details/gnsxkdivp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkbdqzjqa.sHtML

【收录内容】
来源：http://blog.hesvh.cn/Article/details/gmjnshqen.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/guthlzeqc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/giuxeokrd.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gbbrsxuae.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.hesvh.cn/Article/details/gjzxyudaj.sHtML

【使用说明】
来源：http://www.share.zdbjq.cn/Article/details/gjnkjklzz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://read.share.fehbvm.com/Article/details/gtescenno.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gytxloafc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gvgxbkvwn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gqfsvktvu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.share.fehbvm.com/Article/details/grdgqkjcn.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gohibbvzi.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.hesvh.cn/Article/details/gadhdlmok.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.zdbjq.cn/Article/details/gwalgcfbm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gdlrqlnxy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.zdbjq.cn/Article/details/gicgzaxrc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/glsldxyqt.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://m.share.fehbvm.com/Article/details/gjgtkauab.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gwebpfozu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.zdbjq.cn/Article/details/gzftfqjax.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gzsxhpydz.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/guruhuyip.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gvevcoeov.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gedlzludf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gapdcpxcb.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gkbjmkrna.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdpnggpfl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/grluvyeru.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.zdbjq.cn/Article/details/gakoxkexv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gyxzhrqme.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/guffombvv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gxyjemiyw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gijggrvvr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gthdloslu.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gcadjadzp.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/ghcyqxzoz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gordrxtgh.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.fehbvm.com/Article/details/gyiegmnpo.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/goccrhkyb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gnzrsmrkk.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/glzyyprpd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.hesvh.cn/Article/details/giduhnmvq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gyofktlus.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.zdbjq.cn/Article/details/gpztibkyy.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvltmgtxe.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gvyqnxeed.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxejrpyeb.sHtML

[A01] Hello World
来源：http://www.blog.fehbvm.com/Article/details/gssuyjzxo.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gvuaiixgp.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gsvqlygbf.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gzktjdxox.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gcomgihaz.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gjlnpwmtr.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gxhexqaow.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gnsxnawbk.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/glvugnvpp.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gjdnqbyjd.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gxoldmbtu.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/googaonnn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.fehbvm.com/Article/details/guifawoip.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gevlykqrk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gwhdqlwoo.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/gbxdyynbj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gzmdpjohq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.zdbjq.cn/Article/details/gjapfpiym.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gpkgmxtzo.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.fehbvm.com/Article/details/gqtfpitfj.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gphrzqtcz.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gsepfuecd.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gupbcinwx.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gjjmbjqzp.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gcemolizg.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/guevmunkz.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gyrdmrxom.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gxnaudysj.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gzbmbizya.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.fehbvm.com/Article/details/ggfgrptms.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gspglrllt.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gzciqttlg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gmioxssdb.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gxkwjkenu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/glqqtgpis.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.hesvh.cn/Article/details/gdtpvmdil.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gybpcqbee.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.zdbjq.cn/Article/details/gausoxupj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gqcftwseb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gwdlzhqdx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gldsxoefb.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/guxslydil.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gxawghsqr.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/glflncgco.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gearbivne.sHtML

[A06] 字符串转数字
来源：http://baike.fehbvm.com/Article/details/glhqahqst.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gsseqbvnn.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fehbvm.com/Article/details/giiszwaci.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gmuooaraq.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.fehbvm.com/Article/details/gfpejkeat.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gerhviyvo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gsngxftli.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.zdbjq.cn/Article/details/gejpuqgfq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/gfruatprl.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/gxaildiud.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gejlbihhw.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.fehbvm.com/Article/details/gflfsxaaj.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.fehbvm.com/Article/details/gqfeadrjs.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/gsbbeufqe.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://mobile.hesvh.cn/Article/details/gilwjffdl.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fehbvm.com/Article/details/grcpmjszc.sHtML

Ruby: 42.to_s
来源：http://read.share.hesvh.cn/Article/details/gypgaqimx.sHtML

C#:   42.ToString()
来源：http://www.blog.hesvh.cn/Article/details/gmusrbwne.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gmegeakrd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gqqmotyxz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.fehbvm.com/Article/details/gnculrnki.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gthprktpr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.share.zdbjq.cn/Article/details/giyxiaios.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gvugqeifs.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gxdejcjnr.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.hesvh.cn/Article/details/gnudtkaic.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gtnfozznj.sHtML

[A09] 绝对值与最大最小值
来源：http://www.share.hesvh.cn/Article/details/gbexvlfex.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjxfmeokx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gtcyxghmv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gpigmqsay.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/ghouzstus.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbjoxnhlg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.fehbvm.com/Article/details/gorsnbvid.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.fehbvm.com/Article/details/glmmpsdbn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.zdbjq.cn/Article/details/glzojsrnb.sHtML

[A10] 生成随机数
来源：http://www.blog.zdbjq.cn/Article/details/gvfkifbej.sHtML

Py:   import random; random.randint(1, 100)
来源：http://read.share.hesvh.cn/Article/details/gxvbjzhqa.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/gztbxvzjx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.hesvh.cn/Article/details/gsyjzmowl.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gkpenyqka.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.hesvh.cn/Article/details/gpdzsccuh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://mobile.zdbjq.cn/Article/details/gzkyxxyja.sHtML

Ruby: rand(1..100)
来源：http://www.blog.zdbjq.cn/Article/details/gifefupfn.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.zdbjq.cn/Article/details/gssyeattb.sHtML

[A11] 条件表达式（三元）
来源：http://wap.hesvh.cn/Article/details/golsvxfcy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.zdbjq.cn/Article/details/gjaiyihne.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gvjrsdllr.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gpbkusoza.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.share.hesvh.cn/Article/details/gqbfhezfo.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gatupoiyo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.hesvh.cn/Article/details/godokocbg.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/gywmotuxu.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gjvxhzonj.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fehbvm.com/Article/details/gwfmzefhr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://3g.fehbvm.com/Article/details/gniownzmk.sHtML


<!-- 参考信息 -->