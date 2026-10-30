代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gcphxfllc.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gcsznhpzk.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gjfvkzzgi.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.zdbjq.cn/Article/details/gsiuwklnu.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gcdxpydph.sHtML

composer require psr/container
来源：http://3g.hesvh.cn/Article/details/glpsatusr.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/gudqfueff.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.hesvh.cn/Article/details/guegidttt.sHtML

[U77] PHP：模板渲染
来源：http://read.share.fehbvm.com/Article/details/gizpqqbuy.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gawchdnwj.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gophjjyxy.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/gpuetvckn.sHtML

[U79] PHP：静态分析
来源：http://3g.fehbvm.com/Article/details/goklvkkyo.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gsdrwplxc.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gcpgzviok.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.zdbjq.cn/Article/details/gatuutyap.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gkpdemfox.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/grqhnkhgz.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gyyafpzod.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gxzylsuql.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.zdbjq.cn/Article/details/gwobesqul.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gpihjexho.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/getmpapju.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://blog.zdbjq.cn/Article/details/gexnzeosj.sHtML

[U85] JS：可选链
来源：http://3g.zdbjq.cn/Article/details/gblaoshas.sHtML

a?.b?.c
来源：http://m.share.hesvh.cn/Article/details/gkbzntuwk.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gsgtpqgmr.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gjerixhme.sHtML

[U87] JS：解构默认值
来源：http://read.share.hesvh.cn/Article/details/gnztemkgx.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/grzbrogvr.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gkqvirots.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gpiwowjqu.sHtML

[U89] JS：数组去重
来源：http://read.share.hesvh.cn/Article/details/gcciurtii.sHtML

[...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gviwnbgpj.sHtML

[U90] JS：数字数组排序
来源：http://baike.hesvh.cn/Article/details/gbywscdbu.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gqfkltrda.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/grispzpkr.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.fehbvm.com/Article/details/gebtjfcpr.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gojqkignk.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gfygiwhrw.sHtML

[U93] JS：模板字符串
来源：http://mobile.fehbvm.com/Article/details/gjtkbrxra.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gwhghzrue.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gtxkmrvvz.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gpauxwaek.sHtML

[U95] JS：Promise 包装
来源：http://m.share.fehbvm.com/Article/details/gbdbwgfyn.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.fehbvm.com/Article/details/gnqqveduy.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.hesvh.cn/Article/details/gwfmtujdm.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gkqseyfbt.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/gfajbccbv.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gmfgwgwac.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gezugdxpc.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.zdbjq.cn/Article/details/geskytxzr.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gafevqilv.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gfbmwokek.sHtML

[U100] JS：DOM 查询
来源：http://mobile.hesvh.cn/Article/details/gjpkkwdtk.sHtML

document.querySelector(".item")
来源：http://mobile.zdbjq.cn/Article/details/gmybravea.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gobaaevfi.sHtML

el.classList.toggle("active")
来源：http://www.share.hesvh.cn/Article/details/gkftqljxr.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gpqzujbda.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gjzsbcbqj.sHtML

[U103] JS：定时器
来源：http://www.share.fehbvm.com/Article/details/gvwtkowkz.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.fehbvm.com/Article/details/gnnxhytzg.sHtML

[U104] JS：防抖
来源：http://baike.zdbjq.cn/Article/details/gtnumrehp.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/ggssbkcsn.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gdfuhigud.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.zdbjq.cn/Article/details/gsdlmbubn.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/ggnefdcgi.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gwazkwfge.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gwmxjeqsz.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gualdsiom.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gjtvtybjk.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gcgpofkgi.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gqfhbiuio.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/guujjqlef.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gmxkuxyyq.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.hesvh.cn/Article/details/gtqbefnft.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gqqoavdxm.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gfoycbkrq.sHtML

[U112] JS：字符串补位
来源：http://www.share.zdbjq.cn/Article/details/gjscpokgo.sHtML

"7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gmspjrbyp.sHtML

[U113] JS：正则替换全部
来源：http://read.share.hesvh.cn/Article/details/gfccrgfuf.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gfjsjybes.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gfqfbxjmo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gvnwdvgrt.sHtML

[U115] JS：生成 UUID
来源：http://mobile.fehbvm.com/Article/details/gmkenexsr.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/ghninjvfw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gvysswmnt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbilpleku.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gnaobsgua.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.zdbjq.cn/Article/details/ghrjqwliz.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gkhmvefbz.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/gxzgqhztk.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/glocbgiwd.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/gigvhzayr.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://m.share.fehbvm.com/Article/details/ghovrapok.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gxlcgvcid.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcugpdpwv.sHtML

统计汇总
来源：http://mobile.zdbjq.cn/Article/details/gxfqarral.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtqlljoqv.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/giqptovni.sHtML

Python ......... 252
来源：http://www.blog.hesvh.cn/Article/details/gibukufhf.sHtML

PHP ............ 252
来源：http://blog.hesvh.cn/Article/details/gjubtxdou.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gzbhrtkwg.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gmpklypim.sHtML

Java ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gnpvfvsnn.sHtML

Go ............. 212
来源：http://www.m.share.hesvh.cn/Article/details/gujggzxly.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gnmendxfz.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gwnhehalf.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/gsdygklka.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gewjqlrwd.sHtML

SQL ............ 90
来源：http://baike.fehbvm.com/Article/details/gpyblhwdi.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gwbbsioaj.sHtML

Kotlin ......... 15
来源：http://blog.fehbvm.com/Article/details/gxovjonjh.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/glfirycdj.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gthvbogum.sHtML

Perl ........... 10
来源：http://www.share.zdbjq.cn/Article/details/gnidtiyhk.sHtML

Scala .......... 10
来源：http://mobile.zdbjq.cn/Article/details/gleaxawil.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gasgxwqxo.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gibxvrjso.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gxnqtzode.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gfbioyymr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gzobnkptc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gslskvqfw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.zdbjq.cn/Article/details/gumvamcka.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gdlgkdeqs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gxijtwgkt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/grtvovkta.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gohweacdv.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gnypkolca.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fehbvm.com/Article/details/gwofovdei.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gfyaizvjw.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/geeycwxpg.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/glxeatkfy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gwvdqzwgc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/grwaseqaj.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gltljgooz.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gdajltvst.sHtML

R Bash 专题                             80
来源：http://read.share.hesvh.cn/Article/details/gmlgoskml.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gxqnzobbk.sHtML

T 其他语言补充                          60
来源：http://wap.zdbjq.cn/Article/details/gidclfvpo.sHtML

U 高频实用片段                         120
来源：http://www.m.share.hesvh.cn/Article/details/gtouwadfh.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gbayejlrv.sHtML

合计                                  2106 条
来源：http://www.blog.hesvh.cn/Article/details/gufuuvtth.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gqbrrmmsy.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gjrvcruna.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gwitiwjhh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gxjndrgqe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/gjhvwnvym.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/ghswxcljx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://blog.zdbjq.cn/Article/details/gxwimvvyc.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/glmtzeerh.sHtML

—— 文件结束 ——
来源：http://3g.fehbvm.com/Article/details/gfiqkjbvq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/genlqamal.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.hesvh.cn/Article/details/gmnrwndvt.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.fehbvm.com/Article/details/grlepnxhv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghhfbeyir.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gdbshsypi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/gjceacmye.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.zdbjq.cn/Article/details/gvqbagtnp.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gyangrwel.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.m.share.hesvh.cn/Article/details/gkrlwmkbl.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gfhqsqaex.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gdcakfifa.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.fehbvm.com/Article/details/gdgatjnns.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.hesvh.cn/Article/details/goxfsckxd.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/glbyicbyx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/gmedfbfhd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/goecfzzzr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.fehbvm.com/Article/details/gxsrfwhot.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gnzdirisj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://wap.zdbjq.cn/Article/details/gixaevrsv.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.fehbvm.com/Article/details/gpbbrgfmd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gqrbuoawe.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gmkujlplv.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gbnihtqfu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gottuyjot.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gqdhmfzql.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/glcoutrzb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gregjudmi.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gjzywqebw.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gmwozuswt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gxiqoeons.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/grodxuhbi.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/ghtksoguh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gkqgyfqot.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/goqmaaixk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://read.share.zdbjq.cn/Article/details/gechnumfs.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gupofdkrb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.hesvh.cn/Article/details/gihhaegus.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gpzohfdpw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggovxusaw.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/ggwpdffwn.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.zdbjq.cn/Article/details/gpzgsreoo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gywuhgqog.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gggiuchoe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://mobile.hesvh.cn/Article/details/gerrkpxwc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/grrlnzgpz.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.zdbjq.cn/Article/details/gdggumuaw.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gmtgsxxpz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.zdbjq.cn/Article/details/ganmhkabq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvqlcikkv.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/ggeuyzvyq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxfaqwdrn.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/giilanbyk.sHtML

Py:   print("Hello, World!")
来源：http://m.share.hesvh.cn/Article/details/gshcioikq.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gqcejbvce.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gvfoyecih.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gcqjapcdr.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/ghvepqxhe.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gvvignypf.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.fehbvm.com/Article/details/ggrvzovan.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gwjjqygvo.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/gfajlmvwh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/gnvzorxcg.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gcgsuxmru.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.fehbvm.com/Article/details/gsmjsqpmc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gshwfzhgr.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gkfhsceck.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/gtejnbtjw.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.fehbvm.com/Article/details/glnrfrrsa.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/giwarwiih.sHtML

[A03] 常量定义
来源：http://blog.hesvh.cn/Article/details/guhuuswpy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gntjtbzij.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gzbyakyxo.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gslhqwglo.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gbbodevgl.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gnesqvpzi.sHtML

Go:   const PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gykimmmnx.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gtehylrkg.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gsyfvvehf.sHtML

[A04] 判断变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gniewmleh.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gvvrkhviy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/geqdmfcqp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gfhlpsert.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gvmirjnjc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.hesvh.cn/Article/details/gbmlmlrss.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.hesvh.cn/Article/details/ggwzrkral.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.blog.zdbjq.cn/Article/details/glicoqyer.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.zdbjq.cn/Article/details/glrncmnvc.sHtML

[A05] 整数除法与取模
来源：http://3g.hesvh.cn/Article/details/gikqvjsqk.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.fehbvm.com/Article/details/gpvncpwof.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gqfzrgmma.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/glvaxucdn.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/grgmbfqra.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gatcysjmk.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gwlvdmdev.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/ghfxzrubn.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/ghhnuzqnz.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/ggwjtztiu.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/grxpnkqqy.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://blog.hesvh.cn/Article/details/gviaerwqf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gfopzjwrs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gnyjhcwwx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gedpeorcx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.share.fehbvm.com/Article/details/gacfpuqbu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/gpaqavxtf.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.zdbjq.cn/Article/details/ghnyjndsy.sHtML

[A07] 数字转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gimzzmyne.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/grcmmhrba.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.zdbjq.cn/Article/details/geojxwdqn.sHtML

JS:   String(42); (42).toString()
来源：http://www.blog.zdbjq.cn/Article/details/gxnjtqlmx.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/gjtacuely.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gamliluuo.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/gwdxgphhg.sHtML

Ruby: 42.to_s
来源：http://m.share.fehbvm.com/Article/details/gdsonzdeh.sHtML

C#:   42.ToString()
来源：http://www.m.share.hesvh.cn/Article/details/gjbvslsyp.sHtML

[A08] 取整与四舍五入
来源：http://www.share.zdbjq.cn/Article/details/gnkejgdnf.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/grjblysfs.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.m.share.hesvh.cn/Article/details/gopjzjwsr.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/glngfmlpf.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fehbvm.com/Article/details/gwgvcvche.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/gppotnvyb.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gsngocvvq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gvtdcbyzl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gzmjgxgtr.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gntzxrwsy.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/godgtrqjd.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gpfihtnfr.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gatwdhwgk.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/greynsern.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrykjvww.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.hesvh.cn/Article/details/gfslvqpgm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.fehbvm.com/Article/details/gluyojqkq.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gbsdgxjul.sHtML

[A10] 生成随机数
来源：http://wap.hesvh.cn/Article/details/gfjgjakeu.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.blog.fehbvm.com/Article/details/geggiumni.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.zdbjq.cn/Article/details/gheshkaww.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.hesvh.cn/Article/details/gwfknatxf.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.zdbjq.cn/Article/details/govbvzkmh.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.fehbvm.com/Article/details/ghfyjhtqc.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.fehbvm.com/Article/details/gjxjjverk.sHtML

Ruby: rand(1..100)
来源：http://mobile.fehbvm.com/Article/details/gecyorpxk.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gpzepntzc.sHtML

[A11] 条件表达式（三元）
来源：http://wap.fehbvm.com/Article/details/gdjjmfkpt.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://read.share.zdbjq.cn/Article/details/gtzeiohas.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/grfqsizww.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gfvpxqyrn.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gjafgskkv.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/gacrdgmge.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/gjhdlxtja.sHtML


<!-- 参考信息 -->