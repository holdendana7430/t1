代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gitdnppuk.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gfrpnnzcq.sHtML

[U74] PHP：读取环境变量
来源：http://wap.zdbjq.cn/Article/details/ggvhxgdsc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/garlsvasi.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/ggsysetii.sHtML

composer require psr/container
来源：http://www.m.share.hesvh.cn/Article/details/gatjoahev.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.fehbvm.com/Article/details/gvidkjrpn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gonrclvxo.sHtML

[U77] PHP：模板渲染
来源：http://read.share.hesvh.cn/Article/details/glbcxkpcq.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/grbsdincq.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gmwivtjdb.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.fehbvm.com/Article/details/gyvfmhmms.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/gvqpdmdgr.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gogkwyfgz.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.zdbjq.cn/Article/details/gzbmpkyie.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/grjqsfzsl.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gzjeuwhor.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gitattrye.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gkrrnfqud.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gqbjhklss.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/grohyfntv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.fehbvm.com/Article/details/grgnwrkoi.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.fehbvm.com/Article/details/ghrreggte.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.hesvh.cn/Article/details/gjysofzrn.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gtpveavpq.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gducxzywt.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gmiiaxehv.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/gzllysenb.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gobbfegjm.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gulitcydg.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gzfiqtuit.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gqandbnqj.sHtML

[U89] JS：数组去重
来源：http://3g.hesvh.cn/Article/details/gplxsahpp.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ggbsozkjv.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gemsqocuw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gmoupjpxj.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gpgkdndox.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/ggipnycpf.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/grtnykgrm.sHtML

structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/ghjmqrrwu.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gftoajowr.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/ggafdvuev.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fehbvm.com/Article/details/guunkvzbo.sHtML

const double = x => x * 2;
来源：http://www.m.share.zdbjq.cn/Article/details/gcdtzvqub.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gkimxczjb.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gxhmhmfkj.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gzcbcrfnk.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gmztoktay.sHtML

[U97] JS：并发请求
来源：http://www.blog.fehbvm.com/Article/details/guqrfklbx.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gphletbsw.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gzvasnawx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gfwpkleqh.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/ghsnpvtey.sHtML

el.addEventListener("click", e => {})
来源：http://blog.zdbjq.cn/Article/details/glyjbxvqd.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/giinsfpkj.sHtML

document.querySelector(".item")
来源：http://m.share.zdbjq.cn/Article/details/ggndsbkds.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gghuzlmzb.sHtML

el.classList.toggle("active")
来源：http://3g.fehbvm.com/Article/details/gyfdlrwow.sHtML

[U102] JS：本地存储
来源：http://www.blog.fehbvm.com/Article/details/gaxhuwklt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.fehbvm.com/Article/details/ggyfriubz.sHtML

[U103] JS：定时器
来源：http://wap.fehbvm.com/Article/details/gdswefncc.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/glyrnwxsh.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gbhbxjjau.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/gjegzkioh.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gsuseuxvg.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.hesvh.cn/Article/details/gfxvaddqf.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/gvbupoaye.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.hesvh.cn/Article/details/gknrefjww.sHtML

[U107] JS：数字千分位
来源：http://m.share.hesvh.cn/Article/details/gufvfmovy.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gbrlxghac.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/grmhfzpjk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gobeuunnr.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gujuzfhuo.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gpgzglybt.sHtML

[U110] JS：数组分块
来源：http://www.m.share.hesvh.cn/Article/details/gigedikio.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gdmaodpjk.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/ggkusvfpp.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gfquhslvy.sHtML

[U112] JS：字符串补位
来源：http://m.share.hesvh.cn/Article/details/gpkiguyys.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/guypzowta.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/gbwmjaojx.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gpkinqwro.sHtML

[U114] JS：JSON 深比较
来源：http://wap.fehbvm.com/Article/details/gfwykkwyf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gvgnzorbt.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gtpilzdsu.sHtML

crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gfbntclzi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.fehbvm.com/Article/details/gqpjlmfsd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gnrfyvxjd.sHtML

[U117] JS：单元测试
来源：http://3g.hesvh.cn/Article/details/grwaodrpa.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gyutiwkra.sHtML

[U118] JS：开发服务器
来源：http://mobile.zdbjq.cn/Article/details/gnntjlbuw.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gazfdarqp.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/gnuzotkqw.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gspxdusal.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/geeywunff.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/gblnxkrzz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbppyycpz.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/gnzixzovi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwlhkgzpm.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gguwnyykw.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/gvavqxzyd.sHtML

PHP ............ 252
来源：http://wap.fehbvm.com/Article/details/gqvzpaqlq.sHtML

JavaScript ..... 252
来源：http://blog.zdbjq.cn/Article/details/gbgzmpmaj.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/gchidwgce.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/glyrsoegf.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gwkonyskj.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/guvpvnsrw.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gyxoecxgn.sHtML

C .............. 30
来源：http://baike.fehbvm.com/Article/details/gnoqrkhvx.sHtML

C++ ............ 30
来源：http://m.share.hesvh.cn/Article/details/grnfexrux.sHtML

SQL ............ 90
来源：http://blog.zdbjq.cn/Article/details/gkywfrmyl.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gqmepwtwj.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/grvusaiwc.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gczijcpxt.sHtML

Lua ............ 10
来源：http://baike.fehbvm.com/Article/details/gdshaghwc.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gxnllarwu.sHtML

Scala .......... 10
来源：http://baike.hesvh.cn/Article/details/gnfkfzlwl.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gxhtknhvb.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gqcfrqqxk.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/ggvnwiydh.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gtpaxemem.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gxerdmjyf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/guwectptr.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.fehbvm.com/Article/details/gjibzgbtb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.hesvh.cn/Article/details/gqtjwcosl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/gvjptnodu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gnyhqlriz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/giedskqpk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/goerujljd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/guacrokar.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gmsvfvuld.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gvtlegbyi.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gkgzatgmi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gjrvvhzom.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/ggcddpqrb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/ghsettevn.sHtML

Q SQL 专题                              90
来源：http://www.m.share.hesvh.cn/Article/details/gvmkmnvwr.sHtML

R Bash 专题                             80
来源：http://m.share.hesvh.cn/Article/details/gqejgvtkx.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gkqikzbpm.sHtML

T 其他语言补充                          60
来源：http://read.share.hesvh.cn/Article/details/gvnvrhlja.sHtML

U 高频实用片段                         120
来源：http://www.share.zdbjq.cn/Article/details/gumvoeumk.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gfgvlinmv.sHtML

合计                                  2106 条
来源：http://wap.fehbvm.com/Article/details/gwzkghcvr.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gdluxstmy.sHtML

使用提醒
来源：http://mobile.zdbjq.cn/Article/details/gizklaxgz.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/goocgoumx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/ggxwaoscd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.hesvh.cn/Article/details/gvdddtkpw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.hesvh.cn/Article/details/gcphplekl.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.fehbvm.com/Article/details/ghnhyrtkz.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/gtxxnuqng.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gfjwfkdrh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwavdndlu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gsebnihlm.sHtML

Common Programming Examples Cheat Book
来源：http://read.share.fehbvm.com/Article/details/gppseoiaw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxkpisckg.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gvuajzird.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gnhohcwbo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gsvffaofv.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gshjviptn.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.fehbvm.com/Article/details/gphcwjuxm.sHtML

【使用说明】
来源：http://mobile.hesvh.cn/Article/details/gihpokrdd.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.fehbvm.com/Article/details/gfdaokmeh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gnkpvpycg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/glxurpthf.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.hesvh.cn/Article/details/gffleppwq.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gtfwowxtk.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gmiyzxela.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.zdbjq.cn/Article/details/gibgdhbbh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://baike.fehbvm.com/Article/details/gazsstnhj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.zdbjq.cn/Article/details/gjaciiosy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/gslugtyro.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.zdbjq.cn/Article/details/gwijooasw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gxboiqljp.sHtML

【文件统计】
来源：http://m.share.fehbvm.com/Article/details/gowmojmvu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gflvfccel.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gvwbwqjit.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gsqnnttmx.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/gzrtbcokg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.fehbvm.com/Article/details/gtadooyyn.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/giptvtkbr.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gmbgppzgr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/grdbfcyth.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/giljnitrw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gujwyrtqs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gqxeonotj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gyvjsofuf.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gdeaaphpk.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/galxzwnge.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gtxuqbsmo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gjjzdffqe.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gtfgeilor.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gbclhwfvg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.fehbvm.com/Article/details/gxvsrrvqd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/guzsgcckg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gvdxmmcgy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gwltlmmha.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.hesvh.cn/Article/details/gemhuxsiy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gpslrlxua.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gsdyhfwyu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwcrbhpxi.sHtML

A. 基础语法与类型
来源：http://blog.hesvh.cn/Article/details/gitjmirqz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtwxcxdcl.sHtML

[A01] Hello World
来源：http://baike.zdbjq.cn/Article/details/gtpttjzvo.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gaxfytxxa.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.fehbvm.com/Article/details/gdnnlqrzl.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gqebidbkp.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://3g.zdbjq.cn/Article/details/glruaplvl.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gpdkvuvrl.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gccwxxhtl.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gjsadvydm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gikeyhkxw.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/ghdnhyglr.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.hesvh.cn/Article/details/gwkmcmjjy.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gosrvmbst.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gdszrcbed.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gbywivana.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://blog.fehbvm.com/Article/details/gxsolhaks.sHtML

Go:   name := "Alex"; age := 20
来源：http://blog.fehbvm.com/Article/details/gtretcbuj.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.zdbjq.cn/Article/details/gauuzqyhr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/govhbfijb.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gcqgwqhlt.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.fehbvm.com/Article/details/genuutieb.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gmfkvtnqx.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gxehmmsrl.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/ghkjibfxc.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gmtchalgu.sHtML

Go:   const PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/geqojopli.sHtML

Ruby: PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gxtwaldfs.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gfyzfjjqh.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gvmfypzwy.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.zdbjq.cn/Article/details/gskntipjl.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.zdbjq.cn/Article/details/gukiozjag.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/ghmfxvfkv.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/glkjtrxtz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.hesvh.cn/Article/details/gxzoyfcjl.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.fehbvm.com/Article/details/gfezfmutj.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gvsixjnex.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gsydufngq.sHtML

[A05] 整数除法与取模
来源：http://m.share.hesvh.cn/Article/details/gmdstjgel.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gsgesunus.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gscnyvpwu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gvxnpfzus.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gbvmqugvi.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/ghvrswhlb.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gmywokzrc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/griipruva.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gnefxydre.sHtML

[A06] 字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gknxnojdo.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gtxpdulgc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.zdbjq.cn/Article/details/gzcpsrznb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gkdstrdvk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.fehbvm.com/Article/details/gveaznnaj.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.fehbvm.com/Article/details/gpwypoaic.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gsiqutoqt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.fehbvm.com/Article/details/ggpeuzlws.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/gmedbehjh.sHtML

[A07] 数字转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gyhcgecxe.sHtML

Py:   str(42)
来源：http://read.share.hesvh.cn/Article/details/gpvhotfmd.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.zdbjq.cn/Article/details/gpovovuel.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gbkaownyy.sHtML

TS:   String(42)
来源：http://m.share.zdbjq.cn/Article/details/gjlfjwlvi.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/giigjlxot.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.zdbjq.cn/Article/details/ggbbpwmbw.sHtML

Ruby: 42.to_s
来源：http://m.share.fehbvm.com/Article/details/gaoblklsu.sHtML

C#:   42.ToString()
来源：http://m.share.fehbvm.com/Article/details/gygyvolrw.sHtML

[A08] 取整与四舍五入
来源：http://blog.zdbjq.cn/Article/details/glnqjocdl.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/glsicnmsy.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.fehbvm.com/Article/details/gludxgzic.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/grjluljee.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fehbvm.com/Article/details/gnqkaifqt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gzvkbmrmt.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gafkatyus.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.zdbjq.cn/Article/details/gceyewozi.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/grcmxrpkj.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gxiaxmswn.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.zdbjq.cn/Article/details/ghonoafea.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gnqpnmasv.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/ghxytusej.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gpyqbyeli.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gllmotxka.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wap.zdbjq.cn/Article/details/geownfekk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.zdbjq.cn/Article/details/gmbkqqjkl.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/grjqtfkgh.sHtML

[A10] 生成随机数
来源：http://3g.hesvh.cn/Article/details/gkwbdcygg.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/guohrsgkz.sHtML

PHP:  random_int(1, 100);
来源：http://www.m.share.zdbjq.cn/Article/details/gwkptlzev.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://mobile.hesvh.cn/Article/details/gvpgmhojw.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.share.hesvh.cn/Article/details/gpweggluv.sHtML

Java: new Random().nextInt(100) + 1
来源：http://3g.zdbjq.cn/Article/details/gayrcaiij.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fehbvm.com/Article/details/gwaivozfi.sHtML

Ruby: rand(1..100)
来源：http://www.share.zdbjq.cn/Article/details/gpurzxkls.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.hesvh.cn/Article/details/gntxtefxx.sHtML

[A11] 条件表达式（三元）
来源：http://blog.zdbjq.cn/Article/details/gtrhiehtf.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gwgvkimks.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/ghxaivfgp.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gwhmbppca.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gyjfxxuza.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gjgnicggo.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fehbvm.com/Article/details/gmtpbmhni.sHtML


<!-- 参考信息 -->