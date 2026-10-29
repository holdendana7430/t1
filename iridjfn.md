代发 wailian999

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gpbaklamf.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gnomtisln.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/guxclbywa.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gxjyaituj.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/gziomtqqf.sHtML

composer require twig/twig
来源：http://3g.fehbvm.com/Article/details/ghgqksrqi.sHtML

[U78] PHP：单元测试
来源：http://blog.zdbjq.cn/Article/details/gnmfspbec.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.zdbjq.cn/Article/details/gmnvwqvkd.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/gsxpqmgid.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gzegyecxs.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/gzxtndrix.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gkeukjuxn.sHtML

[U81] JS：初始化项目
来源：http://www.share.hesvh.cn/Article/details/gnjeonvcs.sHtML

npm init -y;  npm i express
来源：http://read.share.fehbvm.com/Article/details/gbzbgyogl.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.zdbjq.cn/Article/details/gdbzbrocm.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/ghwhbuait.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/gnjizqtox.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gsjkjsjgf.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gxfyoloax.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.zdbjq.cn/Article/details/gaotkrnay.sHtML

[U85] JS：可选链
来源：http://wap.fehbvm.com/Article/details/giysenpmd.sHtML

a?.b?.c
来源：http://blog.fehbvm.com/Article/details/gmmbfikbh.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/gxqjsakjr.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gyofaflww.sHtML

[U87] JS：解构默认值
来源：http://m.share.hesvh.cn/Article/details/gklgjzhwo.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gjfhranwg.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gpkzfmvhd.sHtML

{ ...a, ...b }
来源：http://m.share.zdbjq.cn/Article/details/gbvnogkzf.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gxdyokjde.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gxxwpepgq.sHtML

[U90] JS：数字数组排序
来源：http://blog.fehbvm.com/Article/details/gmitvugjf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gmgujoicg.sHtML

[U91] JS：对象键值遍历
来源：http://baike.fehbvm.com/Article/details/ghvpogbtz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.hesvh.cn/Article/details/gqalnacuo.sHtML

[U92] JS：深拷贝
来源：http://3g.hesvh.cn/Article/details/gqcndzgvk.sHtML

structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gnuwlpptu.sHtML

[U93] JS：模板字符串
来源：http://wap.hesvh.cn/Article/details/gwacsgpqt.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gvcvugwxl.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gvumexrtr.sHtML

const double = x => x * 2;
来源：http://3g.zdbjq.cn/Article/details/gwobpliwy.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gxrlcfnfn.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gzpssuxjb.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gidswdyxf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/ggbmdmcey.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gwevelzrp.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gmfsmgrxj.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.zdbjq.cn/Article/details/gzbxgyycp.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gusuvwrcs.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gxtgwadvq.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gydfknrwm.sHtML

[U100] JS：DOM 查询
来源：http://read.share.zdbjq.cn/Article/details/gccbfibmn.sHtML

document.querySelector(".item")
来源：http://blog.zdbjq.cn/Article/details/gatpxixmm.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gdsqumpdi.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gofrtpvih.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gzlaiaujy.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.hesvh.cn/Article/details/gjgbwazei.sHtML

[U103] JS：定时器
来源：http://www.m.share.hesvh.cn/Article/details/gxnttprgd.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gsjtzufon.sHtML

[U104] JS：防抖
来源：http://www.blog.hesvh.cn/Article/details/gwwarxzed.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gmgousdal.sHtML

[U105] JS：节流
来源：http://3g.fehbvm.com/Article/details/gimtjerhw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.fehbvm.com/Article/details/gacqaludm.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/gxkcqbkyn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.hesvh.cn/Article/details/gloitqmlk.sHtML

[U107] JS：数字千分位
来源：http://3g.hesvh.cn/Article/details/gvfkxeezr.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/ghwahqvmb.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gofutfoxf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/gbdaetkcu.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gjeewddia.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gdlanweea.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gmakxbjyg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/grijkfbaw.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/gueqrlpqa.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/gdeysvvde.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fehbvm.com/Article/details/gxhuamcmq.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/ggcjtbrbd.sHtML

[U113] JS：正则替换全部
来源：http://baike.fehbvm.com/Article/details/gqwzlgukn.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/greytzwnw.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.hesvh.cn/Article/details/gtpvfpemn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/guwtnpzhq.sHtML

[U115] JS：生成 UUID
来源：http://3g.hesvh.cn/Article/details/ghlsgdgyn.sHtML

crypto.randomUUID()
来源：http://www.m.share.fehbvm.com/Article/details/grvbjxrit.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.zdbjq.cn/Article/details/gxntbqfbc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.zdbjq.cn/Article/details/goawxezzw.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gebqgqkas.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.fehbvm.com/Article/details/godfkwhla.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gcolledoe.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.hesvh.cn/Article/details/gjequgpuo.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gkxurguju.sHtML

npx vite build
来源：http://3g.hesvh.cn/Article/details/gzjfzmqbq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.fehbvm.com/Article/details/gknhlovka.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/gjamsofas.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goumvaobk.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/ghspfugvp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grhqcqiyo.sHtML

按语言统计（条）：
来源：http://read.share.fehbvm.com/Article/details/gvgnvgkjm.sHtML

Python ......... 252
来源：http://blog.hesvh.cn/Article/details/gpksbbpmq.sHtML

PHP ............ 252
来源：http://wap.zdbjq.cn/Article/details/gkgyaaqvi.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gfhqaqvqx.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gkkrqsnqe.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gmeeaubfy.sHtML

Go ............. 212
来源：http://baike.hesvh.cn/Article/details/gkotzucef.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gwlbtuqfb.sHtML

C# ............. 212
来源：http://3g.zdbjq.cn/Article/details/glyfdcsuw.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gydrbmcxu.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gkmclmubt.sHtML

SQL ............ 90
来源：http://3g.hesvh.cn/Article/details/ggqlepjgr.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gfenpamxz.sHtML

Kotlin ......... 15
来源：http://mobile.hesvh.cn/Article/details/gsxxqilva.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gsbwuauol.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/gkakyuqsg.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gktzigzky.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gsqmpmgnl.sHtML

------------------------------------
来源：http://read.share.fehbvm.com/Article/details/ghegcaqqt.sHtML

合计 ........... 2106 条
来源：http://blog.fehbvm.com/Article/details/gxoxsggtd.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gmaevptqu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gmkgwbhic.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gyozcovpc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gilzplfej.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gkoezbxfc.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.zdbjq.cn/Article/details/gvrvmwoap.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gwsnuhwln.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gepybaspl.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gdrbmgtid.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gxvvgfvet.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/glngmarxk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/ghptpdomb.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gwlzifakf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/guncxzpla.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.zdbjq.cn/Article/details/guynlvkif.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.zdbjq.cn/Article/details/ggvcikfvz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/giinqrwug.sHtML

Q SQL 专题                              90
来源：http://read.share.zdbjq.cn/Article/details/gaysxfclh.sHtML

R Bash 专题                             80
来源：http://baike.zdbjq.cn/Article/details/gxosrnjfi.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/grypxzoft.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/gimmeigvw.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gmhcszqtk.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/glaephcef.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gahesackr.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gpsacufpi.sHtML

使用提醒
来源：http://www.blog.hesvh.cn/Article/details/gbygyonqh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gqwbidnkw.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.hesvh.cn/Article/details/gurtkqrpz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.fehbvm.com/Article/details/gmhpshmff.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.hesvh.cn/Article/details/gjzpkbczr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gxqyvcagh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.zdbjq.cn/Article/details/gymptixpu.sHtML

—— 文件结束 ——
来源：http://3g.hesvh.cn/Article/details/gpjnokcey.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gebhittfv.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.zdbjq.cn/Article/details/glvqpalku.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gupvrwwxr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjsnejiig.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gyfaxuief.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.hesvh.cn/Article/details/gwamymghm.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gxmedqjjh.sHtML

SQL · Bash · C · C++
来源：http://m.share.zdbjq.cn/Article/details/gmgcmnggx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gwvfxbrrd.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gbvfyqjvp.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gddkyvgow.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.fehbvm.com/Article/details/ggtrbvydb.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gttsmuofg.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gwdjlmgbc.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gkeagdnhf.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.fehbvm.com/Article/details/gddnfuavx.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.hesvh.cn/Article/details/ggznamfae.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/gfntpbiym.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/gttunybuf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/giaiwotla.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gialhfkrf.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gbpdrwcyr.sHtML

【文件统计】
来源：http://blog.fehbvm.com/Article/details/ghztregkw.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/gibqmbmdp.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/ggdvczddp.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gmqeozkod.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gahgflnhu.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gtnilglwh.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/guekxhkrw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gkiyckjfb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/gtwudenix.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gqltfflrc.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gyxkzxhzb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gkajqfdxu.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gsrlouxdy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gnpwjnbly.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gmcxibeou.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gzrninfwd.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gfanzlstd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gtvggxnbf.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gqgrsvzrk.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.fehbvm.com/Article/details/gmzllpcua.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gwcusmazj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gbgufnrlb.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gonhlchkk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/glcnxujty.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/ghzubqqky.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gwginavoe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gacdzmjlc.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gagelqmup.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glifyyubk.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/grdsqcirg.sHtML

Py:   print("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/glhmmncbl.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.hesvh.cn/Article/details/gzqsslszd.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gqmjehiyv.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.hesvh.cn/Article/details/gkqgvumnq.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/guhjfaweu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gnlhosxph.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.zdbjq.cn/Article/details/gjsxvqnxm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gvhiewrfs.sHtML

[A02] 变量声明与赋值
来源：http://read.share.fehbvm.com/Article/details/genmoghmy.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/gumzpptpm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.zdbjq.cn/Article/details/gdwvivuxt.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gqboahjxu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gmauqbprv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.zdbjq.cn/Article/details/ggdwneyxk.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gtbbhlxzp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fehbvm.com/Article/details/gdxxshgwh.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/guozqcgpk.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/gurrzjvws.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/guskmgodz.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gfkmqdvin.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gzlawvbih.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gejltuzed.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gumvgihri.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gtvemjhre.sHtML

Ruby: PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gnmqbwnpb.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gwyzosysd.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/ggrxyexnh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gkydexvle.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://m.share.fehbvm.com/Article/details/gutjjoebl.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gvyfxiaiz.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gabgozjoa.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.hesvh.cn/Article/details/gftptcjhh.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gyitilwwz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gteppjpmk.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gardrgxhv.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/ggffxcmgv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.hesvh.cn/Article/details/gbhsgdtoa.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gtisyywkx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/ginlqnabh.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gjdjowkqa.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.fehbvm.com/Article/details/gauikzxwl.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gfgdyvfgs.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gfdimrtjj.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gszesxher.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gefrzkdgk.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gvxgthjhf.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/gaeutvpto.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/ghdngrabw.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.share.zdbjq.cn/Article/details/gfjxvtyti.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fehbvm.com/Article/details/givvgtdpb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.zdbjq.cn/Article/details/gsktuemwl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://3g.hesvh.cn/Article/details/gmjezyyqk.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/geuxwvifl.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggxcgkpfb.sHtML

Py:   str(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gjnqdbpmy.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.hesvh.cn/Article/details/gjfxkwzzq.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gjlflcejd.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/glogskbgu.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gtxzpliow.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gbvyncadx.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/gmggrnfgq.sHtML

C#:   42.ToString()
来源：http://mobile.hesvh.cn/Article/details/gnfkdiqzu.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/ggslmeeai.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gjbnjqpcn.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.hesvh.cn/Article/details/gogpxngcg.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gflzuhfhk.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.zdbjq.cn/Article/details/gkbqtoaaw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gfvhixsnx.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gkhxecljb.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.zdbjq.cn/Article/details/giwsrvuvi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gccrbevds.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gwzadxwfx.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gixlyndat.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gbvsjqswy.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gadcvfnyp.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gyykpwmeh.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gcyvkpcae.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.zdbjq.cn/Article/details/gelppwsqk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.hesvh.cn/Article/details/gfpfxzuzx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://3g.hesvh.cn/Article/details/glalgqxdb.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/gsivuhtjo.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.fehbvm.com/Article/details/gpfxjapnn.sHtML

PHP:  random_int(1, 100);
来源：http://3g.zdbjq.cn/Article/details/gfamjxndm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.fehbvm.com/Article/details/gpiwvosve.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/gxumxdzte.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gnvcczcwa.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://m.share.hesvh.cn/Article/details/gcoydwyrf.sHtML

Ruby: rand(1..100)
来源：http://baike.fehbvm.com/Article/details/gntzylnzz.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.hesvh.cn/Article/details/gzrumgaog.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.hesvh.cn/Article/details/grjyahfeu.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.hesvh.cn/Article/details/gkdqzskhd.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gvzbvbumw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.fehbvm.com/Article/details/gsmtdanfv.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gcopndnat.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gfjrnqfuo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.zdbjq.cn/Article/details/gkhlfepiy.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gbfjpufzx.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/glbzhakeq.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.zdbjq.cn/Article/details/gamxpbjly.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/gjanyodof.sHtML


<!-- 参考信息 -->