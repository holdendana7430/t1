代发 wailian999

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/gqcihszoj.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gddvfzabr.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gwmoyprad.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gbulnzeez.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/ggtcsqavr.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gqqfmpmwu.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/glnofywqy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gxwvnklni.sHtML

[U81] JS：初始化项目
来源：http://m.share.hesvh.cn/Article/details/gixotbrgg.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gznkxwloe.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gtzptzsoz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.zdbjq.cn/Article/details/gktoswnab.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/glpxqdbiz.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gfptferas.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gtkllfkne.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gzfbxxtqd.sHtML

[U85] JS：可选链
来源：http://www.blog.fehbvm.com/Article/details/gsbqomqto.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gfwnzebgp.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gwtrcawar.sHtML

a ?? b
来源：http://read.share.fehbvm.com/Article/details/gcvcywqps.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gcidztabh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gqoyghoin.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/ghcxpudvn.sHtML

{ ...a, ...b }
来源：http://www.blog.hesvh.cn/Article/details/gfokwwlji.sHtML

[U89] JS：数组去重
来源：http://www.share.hesvh.cn/Article/details/gjugmeqbd.sHtML

[...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/ginvimzpn.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gjmomiloz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gwmunwrfy.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gigsmigit.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.zdbjq.cn/Article/details/gfrcbncaa.sHtML

[U92] JS：深拷贝
来源：http://read.share.fehbvm.com/Article/details/gdtybatzk.sHtML

structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/groogvpnc.sHtML

[U93] JS：模板字符串
来源：http://3g.fehbvm.com/Article/details/gxnrnbsad.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gouduxnpu.sHtML

[U94] JS：箭头函数
来源：http://mobile.zdbjq.cn/Article/details/gsqgxzvgx.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/ghazdomti.sHtML

[U95] JS：Promise 包装
来源：http://m.share.hesvh.cn/Article/details/gqkprwmgu.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gvwklojhz.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.hesvh.cn/Article/details/gdolozjzt.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gfjdrroil.sHtML

[U97] JS：并发请求
来源：http://www.m.share.zdbjq.cn/Article/details/gfojmnsjy.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gqdjvpnqk.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gscimwjrl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.zdbjq.cn/Article/details/grctdzoig.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gdklnbgwr.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gybabdmsa.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.hesvh.cn/Article/details/gekdzafjc.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/gpfzfpnor.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gxkbgzrgd.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gmmlnswap.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gqwcalvmf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.hesvh.cn/Article/details/gnzeacxkz.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gdanszrza.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/grzyecogu.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gybpvgvit.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/gxynexjsh.sHtML

[U105] JS：节流
来源：http://mobile.hesvh.cn/Article/details/gjughwjim.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gqysqmuay.sHtML

[U106] JS：日期格式化
来源：http://baike.fehbvm.com/Article/details/gamtuyyon.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gmwifbcdv.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/ghyyxtobw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gjwhjdjmv.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gmybstxvz.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.fehbvm.com/Article/details/gxgsmknts.sHtML

[U109] JS：数组分组
来源：http://m.share.fehbvm.com/Article/details/gibugzhuc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/grsmxyren.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/geyyjfdux.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://m.share.zdbjq.cn/Article/details/gniyqfvqn.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gvrfapmoy.sHtML

new Map(Object.entries(obj))
来源：http://3g.fehbvm.com/Article/details/gteomjeoe.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/gwyddvtwn.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gztdwtryi.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gidlnatvn.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gqtevqtrc.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.zdbjq.cn/Article/details/guqllbtrq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/ghyzsbzzg.sHtML

[U115] JS：生成 UUID
来源：http://blog.fehbvm.com/Article/details/grftszkiv.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gewwprppg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://blog.hesvh.cn/Article/details/gfjwoakoj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.fehbvm.com/Article/details/gdzlvnpmg.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/ggsatwcvp.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/girnpwlos.sHtML

[U118] JS：开发服务器
来源：http://baike.fehbvm.com/Article/details/gqbvgvhdm.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gnkelocya.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gzrcgbuad.sHtML

npx vite build
来源：http://3g.fehbvm.com/Article/details/gpraohqne.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gyexzoxnx.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gvpherbho.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gawwttjvv.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gkuheaull.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gecpdfdvb.sHtML

按语言统计（条）：
来源：http://blog.zdbjq.cn/Article/details/gwcunkddy.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gsqcpihjr.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gozvvvveo.sHtML

JavaScript ..... 252
来源：http://read.share.fehbvm.com/Article/details/gqjbelytt.sHtML

TypeScript ..... 212
来源：http://wap.fehbvm.com/Article/details/gopaigvlr.sHtML

Java ........... 212
来源：http://mobile.fehbvm.com/Article/details/gibrekifc.sHtML

Go ............. 212
来源：http://www.blog.hesvh.cn/Article/details/gdvyiavqk.sHtML

Ruby ........... 212
来源：http://3g.hesvh.cn/Article/details/gyjdvxmhr.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gxmqbrizh.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/ghsublebs.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gqvizgqql.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/gjdafdlzw.sHtML

Bash ........... 80
来源：http://mobile.fehbvm.com/Article/details/gixyzpnkm.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gaebnjxki.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gswpdjyrb.sHtML

Lua ............ 10
来源：http://m.share.fehbvm.com/Article/details/gobzrnefc.sHtML

Perl ........... 10
来源：http://read.share.hesvh.cn/Article/details/gbdfyckno.sHtML

Scala .......... 10
来源：http://www.share.hesvh.cn/Article/details/giaworgic.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gfkbkydbg.sHtML

合计 ........... 2106 条
来源：http://baike.fehbvm.com/Article/details/gieteugyl.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gowwaxfvn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.zdbjq.cn/Article/details/gfpvhixdb.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/ghhyjcwpf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gcvgyxcvx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gpyuvpxea.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/groqmjlup.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gjbokdabz.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/griykwbfv.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gipsfznrt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gpgfhghqp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.fehbvm.com/Article/details/gpyytjjjr.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gnokvgtfv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gmxubgxaf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gnrmbbhii.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.fehbvm.com/Article/details/gsampwzvp.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/gdkdltluz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/goofydedv.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gwxlbjack.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gborqqsnc.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.fehbvm.com/Article/details/golsqrvpv.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gcmaxkkvc.sHtML

U 高频实用片段                         120
来源：http://www.share.fehbvm.com/Article/details/gexznjqct.sHtML

------------------------------------
来源：http://wap.fehbvm.com/Article/details/gvbymgzun.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/giisjhbcs.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gecvtdofy.sHtML

使用提醒
来源：http://www.share.hesvh.cn/Article/details/gmcvmclhq.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gkynmhoqq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/gjbzoivfz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gsgkduicc.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gyosqnvel.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gcisuzptf.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.zdbjq.cn/Article/details/gonnnzgwu.sHtML

—— 文件结束 ——
来源：http://baike.zdbjq.cn/Article/details/glaqbkhsv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gntojosvm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.m.share.zdbjq.cn/Article/details/gcoxhifeo.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.zdbjq.cn/Article/details/gyfbwjtqz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnjivbhcl.sHtML

【收录内容】
来源：http://3g.fehbvm.com/Article/details/gmcmvvues.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gdfpuznxv.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gngkyvcti.sHtML

SQL · Bash · C · C++
来源：http://www.share.fehbvm.com/Article/details/gsffhemyg.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gvqgvvqoa.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gjtpieipl.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gsqzxpyob.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gcvdjhvcg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gtxmxptdn.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/grlkqfktk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gxbfmwysi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gmeldricm.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/gryquvhky.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/gzguzrtnu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/gbairdxgq.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.zdbjq.cn/Article/details/gjpnhnbnj.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://baike.zdbjq.cn/Article/details/gqlosifyw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/geotsrsaw.sHtML

【文件统计】
来源：http://blog.zdbjq.cn/Article/details/gopodghuq.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.fehbvm.com/Article/details/gqbvxzjml.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gzkmoyjtd.sHtML

目  录
来源：http://www.share.fehbvm.com/Article/details/gcnjybbzc.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gjsfzjcga.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.fehbvm.com/Article/details/gewclntcd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/gulnarrbq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnqmctzbq.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbgdjvhdx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fehbvm.com/Article/details/gimcdbmnu.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gvhgcegsq.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gzzdebljv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gojduejxe.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gxmzlpbjk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gkrdsxgxt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbqszmlsl.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gvnjybnsc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gwadpzltu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gfkapjxbq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.hesvh.cn/Article/details/gjjwbcmrb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/galdoqhby.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.zdbjq.cn/Article/details/ghzcpzeoy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gmpllxvqf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.zdbjq.cn/Article/details/gpqswvcdq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gtjpjrrjy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gtkiophkz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxmxlicqu.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/girfeytjj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggtwzktfz.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gcrtkyhcw.sHtML

Py:   print("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gfzwjhupk.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.zdbjq.cn/Article/details/gpgmhifyj.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gujwlndpg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.zdbjq.cn/Article/details/gidkqrlxn.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gnnxnhdfk.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/gpuhwymmq.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/gnexgmoah.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gjpwutmvq.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/govcuovvq.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.hesvh.cn/Article/details/goegievwq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gwhrvuhgq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gtieytrjq.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gyyxijjak.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gpatezqgz.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.fehbvm.com/Article/details/gksafvtyo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gwyydtoqf.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gcfzccdeg.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/gcayrkdje.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.zdbjq.cn/Article/details/gmeijghch.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gjagqmwsg.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gakaxizfy.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gtfidqnhq.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gfvuajmzl.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gmksqjfzi.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gmlmvvdqg.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/grteohjfb.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gxsdtottt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.fehbvm.com/Article/details/gqocfunse.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.blog.hesvh.cn/Article/details/gmhdxdecz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gpuxixjsd.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.share.fehbvm.com/Article/details/gdygahdvv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gbkzxylal.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gccpckbyu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://3g.fehbvm.com/Article/details/gvyngjeai.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/goldlkmcq.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gmgnpycxo.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/ghowcfiyv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gutatekxj.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gbjwuuolx.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/grltfqfxo.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/givmiqhln.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gurbxpdig.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gufjrpudv.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gtjybnjdz.sHtML

[A06] 字符串转数字
来源：http://mobile.hesvh.cn/Article/details/govbmfoty.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gcbfblosw.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.hesvh.cn/Article/details/gjowtlhzf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gxheznyeb.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.zdbjq.cn/Article/details/gazyroyec.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://wap.zdbjq.cn/Article/details/gokpenbqy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gqtnyjiiq.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.fehbvm.com/Article/details/gxmekvdxd.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.hesvh.cn/Article/details/giphgwxcp.sHtML

[A07] 数字转字符串
来源：http://baike.fehbvm.com/Article/details/gvmhcedlq.sHtML

Py:   str(42)
来源：http://mobile.hesvh.cn/Article/details/gqjrbqlyy.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/gnganbplm.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/gxkvhsueh.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/gsethvkkm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gmocqnrym.sHtML

Go:   strconv.Itoa(42)
来源：http://www.share.hesvh.cn/Article/details/gsbezmyup.sHtML

Ruby: 42.to_s
来源：http://m.share.fehbvm.com/Article/details/gedhfhswa.sHtML

C#:   42.ToString()
来源：http://read.share.fehbvm.com/Article/details/grnotsadk.sHtML

[A08] 取整与四舍五入
来源：http://www.share.hesvh.cn/Article/details/gsylzrvun.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/glewzfxqq.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.hesvh.cn/Article/details/gfvcpmjjx.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/glslxelqm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.hesvh.cn/Article/details/gofdkuvpp.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gfkbtglgb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gisrmndmf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.zdbjq.cn/Article/details/gkpsgplwl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gybiwfpga.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.zdbjq.cn/Article/details/griakiaad.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gzgfgielm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gsqtabhbp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gdwgohalf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/guqxjzzgx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gftrddrer.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://blog.hesvh.cn/Article/details/geeohwajy.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://3g.fehbvm.com/Article/details/gbhihchqk.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gvbdoilyt.sHtML

[A10] 生成随机数
来源：http://read.share.fehbvm.com/Article/details/gzevwbtwk.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.zdbjq.cn/Article/details/gjwymdirs.sHtML

PHP:  random_int(1, 100);
来源：http://3g.zdbjq.cn/Article/details/ghyexsfpq.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gmbqwsnty.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.fehbvm.com/Article/details/gufqruhnl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://blog.zdbjq.cn/Article/details/gddmufqtf.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://read.share.zdbjq.cn/Article/details/gllfnipiu.sHtML

Ruby: rand(1..100)
来源：http://www.share.zdbjq.cn/Article/details/ghozpevno.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.zdbjq.cn/Article/details/gqktkxqmt.sHtML

[A11] 条件表达式（三元）
来源：http://baike.zdbjq.cn/Article/details/gtmvckiki.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.fehbvm.com/Article/details/gaeznwyxx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/geoqjoqqg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/glztnlsbh.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/ggbxmwtnb.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/grbeavlix.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.hesvh.cn/Article/details/gjvtthzks.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.m.share.zdbjq.cn/Article/details/ghndqxglq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gcucnzuhq.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.fehbvm.com/Article/details/gkgvmyzwt.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://mobile.hesvh.cn/Article/details/gkdrcevao.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.hesvh.cn/Article/details/ggspstrco.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.zdbjq.cn/Article/details/glvxiehwq.sHtML

TS:   `Hello, ${name}!`
来源：http://3g.fehbvm.com/Article/details/grqpmyfyv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.hesvh.cn/Article/details/gyjrrqsot.sHtML


<!-- 参考信息 -->