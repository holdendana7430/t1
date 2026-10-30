代发 wailian999

[U77] PHP：模板渲染
来源：http://wap.zdbjq.cn/Article/details/gmodccblx.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gqpdapahx.sHtML

[U78] PHP：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gplcadoko.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/ghotabidg.sHtML

[U79] PHP：静态分析
来源：http://mobile.zdbjq.cn/Article/details/gxgzouffs.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.hesvh.cn/Article/details/ghmhcjaoh.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.hesvh.cn/Article/details/guudrhtko.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.fehbvm.com/Article/details/gknpcyhvf.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gwjntuqnc.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gioktxynd.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/geekmmnme.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gbfxzizgo.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.zdbjq.cn/Article/details/gylzzaewu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gxrfpdarm.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/giwxdaggr.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.zdbjq.cn/Article/details/gcfurczoe.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gvbcahhqt.sHtML

a?.b?.c
来源：http://3g.hesvh.cn/Article/details/gsvujllik.sHtML

[U86] JS：空值合并
来源：http://wap.fehbvm.com/Article/details/gwxqjbxil.sHtML

a ?? b
来源：http://blog.hesvh.cn/Article/details/gmkvtpxee.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/gvhwrjrxj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/ggpsfisjn.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/grieeabks.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gyyflfylq.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/ghkxxutuk.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gbuatnmeb.sHtML

[U90] JS：数字数组排序
来源：http://mobile.fehbvm.com/Article/details/gnvrmoaor.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gyuvsfdxr.sHtML

[U91] JS：对象键值遍历
来源：http://www.m.share.hesvh.cn/Article/details/glpzdjavn.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gbtqmjyay.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/goteiotmx.sHtML

structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gsbkkpxoy.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gxxdbokkx.sHtML

`共 ${n} 条`
来源：http://www.blog.hesvh.cn/Article/details/ggviyyuvc.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gekgmxhwb.sHtML

const double = x => x * 2;
来源：http://m.share.fehbvm.com/Article/details/gexcbgguf.sHtML

[U95] JS：Promise 包装
来源：http://baike.zdbjq.cn/Article/details/gbvurpzvk.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.hesvh.cn/Article/details/grgsembbq.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/gqnygbiiq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gthfvjxfv.sHtML

[U97] JS：并发请求
来源：http://mobile.fehbvm.com/Article/details/ggdyozdrr.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gotgpychd.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gborpjult.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/gjyqwguxy.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gugdqetuf.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gnzvupjvg.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gqpweltra.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gqeccwrpg.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gmraorwdm.sHtML

el.classList.toggle("active")
来源：http://www.m.share.fehbvm.com/Article/details/gjiqpbdot.sHtML

[U102] JS：本地存储
来源：http://www.blog.zdbjq.cn/Article/details/grnvbjnso.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.hesvh.cn/Article/details/gdaxzeoyj.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/gmwxpnjjh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/ggwvmrwnm.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gqhcfkjms.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/ggljdkwxf.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gxercchwv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.fehbvm.com/Article/details/glocdifnk.sHtML

[U106] JS：日期格式化
来源：http://mobile.hesvh.cn/Article/details/ggbloetny.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/grhkantfa.sHtML

[U107] JS：数字千分位
来源：http://m.share.fehbvm.com/Article/details/gmkyohjjc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/ghzkzekft.sHtML

[U108] JS：随机整数
来源：http://www.blog.zdbjq.cn/Article/details/gbgepayfm.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gweajjdod.sHtML

[U109] JS：数组分组
来源：http://baike.hesvh.cn/Article/details/gcvlikfig.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gunyjvmaa.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gihwlbjnz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.fehbvm.com/Article/details/gwgaquzwz.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gluqyvipi.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gibhyoeek.sHtML

[U112] JS：字符串补位
来源：http://baike.hesvh.cn/Article/details/glrjfyyic.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/grnhtwjbn.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gxyfgasfj.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gcidfohni.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gnntdfwag.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gepdrqruh.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.zdbjq.cn/Article/details/gnzoaibav.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/gnioqscgn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/grvtsxeoz.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkqlpzkyu.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gbjtfluhv.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.fehbvm.com/Article/details/giumpmcyu.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gxyrayuai.sHtML

npm i -D vite;  npx vite
来源：http://m.share.hesvh.cn/Article/details/ghhmujbns.sHtML

[U119] JS：生产构建
来源：http://blog.zdbjq.cn/Article/details/gszcxrwwg.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gdavfojun.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gtobnlmhm.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.fehbvm.com/Article/details/gpmuhjdsi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtormragt.sHtML

统计汇总
来源：http://blog.fehbvm.com/Article/details/gpwvsoyjy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geokwvrjz.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/ggjkhxvfl.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gvoevrlsy.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/ghgasbtkh.sHtML

JavaScript ..... 252
来源：http://www.m.share.fehbvm.com/Article/details/goqndzqlf.sHtML

TypeScript ..... 212
来源：http://read.share.fehbvm.com/Article/details/gozxequue.sHtML

Java ........... 212
来源：http://read.share.hesvh.cn/Article/details/gokxlqozv.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gcvrvtfij.sHtML

Ruby ........... 212
来源：http://www.share.hesvh.cn/Article/details/gtunlrthg.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gyqrijptg.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gjvkmnmnn.sHtML

C++ ............ 30
来源：http://www.share.fehbvm.com/Article/details/gxdvwnkcb.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gnzkfuaea.sHtML

Bash ........... 80
来源：http://www.m.share.hesvh.cn/Article/details/goykkvooe.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gazqipvem.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gdlikpmqk.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gpuuxxdgz.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/giukbatcw.sHtML

Scala .......... 10
来源：http://wap.zdbjq.cn/Article/details/gtchzdbxk.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gfjqiihkb.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gmsutdyrp.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/ggtfulbch.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gqdzasosa.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/guzmmmybt.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gfibylafj.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.hesvh.cn/Article/details/gtgzwlmoe.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.zdbjq.cn/Article/details/gcofrnsby.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gqjtsrint.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/guoldkqti.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gjuevxvzo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/ghixjwaem.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gconjhjhc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/ghjskqygg.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gifytkpgs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gprweutds.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gujwqzvqr.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/gkcsdlmzm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gdabtpzwg.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gozepvrjb.sHtML

R Bash 专题                             80
来源：http://blog.zdbjq.cn/Article/details/ghbobertx.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gryehrtxk.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gwsxbxgep.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gbsnjxlbp.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/ghnonknji.sHtML

合计                                  2106 条
来源：http://blog.fehbvm.com/Article/details/ggtidfjts.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/guzxlaozt.sHtML

使用提醒
来源：http://m.share.zdbjq.cn/Article/details/gfmigazmg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gbbqepout.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gpwcxttwi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.hesvh.cn/Article/details/gnkqztvmm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/gmajkhgqi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/guwdeyoov.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gopevwklj.sHtML

—— 文件结束 ——
来源：http://read.share.zdbjq.cn/Article/details/gyccdvbgr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvfdhypln.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/glwumeryt.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gqbcoaecm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxhlicbol.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gomgiuygm.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gqcpptssc.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.zdbjq.cn/Article/details/gyhtwefdk.sHtML

SQL · Bash · C · C++
来源：http://3g.hesvh.cn/Article/details/gsfqvanqo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gbidwyvlp.sHtML

【使用说明】
来源：http://3g.hesvh.cn/Article/details/gemswfrfv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/glwgbdlwv.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/glhkwsvck.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/gggdvegfs.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gesssptbu.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://mobile.zdbjq.cn/Article/details/gtnebppfz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.zdbjq.cn/Article/details/gntvkfahw.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/ggncxhmbb.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/ggyqhkcob.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gtmakcumj.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.fehbvm.com/Article/details/gtnnajahd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gidkcrhzm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gdclyinve.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gsdaypwnx.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gbegvfthv.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gkdzcoxuc.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gfovqytxu.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/gnoncelbt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gyrdmxnud.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gagnmubzg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/ghdxxxhtd.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gukocivxr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/gthjllzpo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gaurjndco.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gabrbjwcc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gtkuexmhk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/guvzuirde.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/grptlbfmz.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/glnvrvjdl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gtbmfnlxt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gqlpzdvjb.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gzymmwhey.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.zdbjq.cn/Article/details/gymsdqjho.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gbbymecwb.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.hesvh.cn/Article/details/gdcfnhgjl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/givvlxirv.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gurlckxgs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gdqremebe.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gulthnjia.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gphlbsqdg.sHtML

A. 基础语法与类型
来源：http://www.share.hesvh.cn/Article/details/gwftyyoea.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfoqzzhnf.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gcplvaynl.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.hesvh.cn/Article/details/gbbczaemd.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gnqikvxqq.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gywndbjui.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/glybrckti.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/gkuklkgad.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/guoeivxtn.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gwtrxjtxx.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/goouftzqx.sHtML

[A02] 变量声明与赋值
来源：http://read.share.zdbjq.cn/Article/details/grsuacodo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.fehbvm.com/Article/details/gybzsttzq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.hesvh.cn/Article/details/gfsqmjjtn.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/grkdjcugv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gokrmlnne.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gyrfxnmsk.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/gaxkucodq.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/grbrngexd.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gsgrhgbxq.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/gnixehcvb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.zdbjq.cn/Article/details/gvnfyxvxz.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gihtkycux.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gvfrohjfl.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gxojzqidg.sHtML

Java: static final double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gapdpejbl.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/grawwafer.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gdgutbsyq.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gvzoodjlr.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gktykwqwe.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/gpwccxhyo.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gorjvjtxh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gafifvjjg.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/ghjfnlaun.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gihfvrcqa.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/gjjbufnbb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgbmtegm.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.hesvh.cn/Article/details/ghhxuqfrz.sHtML

[A05] 整数除法与取模
来源：http://www.share.hesvh.cn/Article/details/gnjkndzui.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.hesvh.cn/Article/details/gpzckrisd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gpqclfkcz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gqkjgoenn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gkuxmhrzv.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/ggosofagl.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gnsyscuwl.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gunlydtay.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gbirgzibk.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/guuihhyrr.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/gtdwjotcu.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://wap.zdbjq.cn/Article/details/gqcjhslrm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.share.hesvh.cn/Article/details/gbozalavv.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gyowxwnkq.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://read.share.zdbjq.cn/Article/details/ggtffkhbo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.hesvh.cn/Article/details/gqxzyrqai.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/grpvyqnwe.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.zdbjq.cn/Article/details/grxlnvgum.sHtML

[A07] 数字转字符串
来源：http://3g.zdbjq.cn/Article/details/ghqoboddj.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gjubesycu.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.fehbvm.com/Article/details/gkyhzcnut.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/geovbwmar.sHtML

TS:   String(42)
来源：http://www.m.share.fehbvm.com/Article/details/gffjeigdp.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.m.share.fehbvm.com/Article/details/gimkcsrtm.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fehbvm.com/Article/details/ghfewixgx.sHtML

Ruby: 42.to_s
来源：http://www.share.zdbjq.cn/Article/details/gclyduqgo.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/giduqdlhn.sHtML

[A08] 取整与四舍五入
来源：http://www.blog.zdbjq.cn/Article/details/gapycmhhd.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gkipuhhgx.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fehbvm.com/Article/details/gadmxkeex.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gydxshyrs.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mobile.zdbjq.cn/Article/details/gourtmkhf.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/grmncizvu.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gimgdiiks.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://mobile.hesvh.cn/Article/details/gvhufxiqq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gpqumcfvw.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.fehbvm.com/Article/details/gysywsmbq.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gtomszqld.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggiacnwrz.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/ghhufahyr.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqmdtzlj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gxzkvwjau.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.hesvh.cn/Article/details/glsabnyqt.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://baike.zdbjq.cn/Article/details/gwpbfarcp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gadcypnov.sHtML

[A10] 生成随机数
来源：http://blog.fehbvm.com/Article/details/geckbkgas.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.zdbjq.cn/Article/details/gfltfbiek.sHtML

PHP:  random_int(1, 100);
来源：http://www.blog.zdbjq.cn/Article/details/gvuydtfgb.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.zdbjq.cn/Article/details/gmuuipnvk.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.zdbjq.cn/Article/details/gwectvvig.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.fehbvm.com/Article/details/gwiavyrnr.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/gvewuuhhy.sHtML

Ruby: rand(1..100)
来源：http://blog.hesvh.cn/Article/details/gwbeercmi.sHtML

C#:   new Random().Next(1, 101)
来源：http://blog.hesvh.cn/Article/details/giluztdsj.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.zdbjq.cn/Article/details/gldwexdyy.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://3g.zdbjq.cn/Article/details/gecnaenzb.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/gwflkbzpw.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gkrodbbsc.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/grgruhfie.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gijvaftwg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://blog.zdbjq.cn/Article/details/gqqudkjnv.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://3g.zdbjq.cn/Article/details/gkzvfkvku.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gczbiytov.sHtML

[A12] 字符串插值 / 格式化
来源：http://mobile.fehbvm.com/Article/details/ggayyzpjn.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://read.share.zdbjq.cn/Article/details/ghhfxtuvm.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://read.share.zdbjq.cn/Article/details/ggfjrowuu.sHtML

JS:   `Hello, ${name}!`
来源：http://mobile.hesvh.cn/Article/details/gldtuqmov.sHtML

TS:   `Hello, ${name}!`
来源：http://wap.fehbvm.com/Article/details/gyounsfea.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.hesvh.cn/Article/details/gsrxwlmqr.sHtML


<!-- 参考信息 -->