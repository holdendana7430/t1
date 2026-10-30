代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gzgvytgxo.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.fehbvm.com/Article/details/gxenhblkn.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gjwonrxmt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.blog.hesvh.cn/Article/details/gmbxfsgux.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gsoaowcsk.sHtML

composer require psr/container
来源：http://m.share.zdbjq.cn/Article/details/gaskumubn.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gryqnvtgf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/guwsbfzrd.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gidyfqkov.sHtML

composer require twig/twig
来源：http://www.blog.hesvh.cn/Article/details/gycurnveq.sHtML

[U78] PHP：单元测试
来源：http://3g.fehbvm.com/Article/details/gxjqvtznh.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/gbfiwviyi.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gfwzmelec.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.hesvh.cn/Article/details/gglhtjmdk.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gaesoufuj.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gtwgyqdfv.sHtML

[U81] JS：初始化项目
来源：http://www.blog.hesvh.cn/Article/details/gzgewsdbc.sHtML

npm init -y;  npm i express
来源：http://mobile.hesvh.cn/Article/details/gowfgndcz.sHtML

[U82] JS：package.json 脚本
来源：http://3g.zdbjq.cn/Article/details/grwzkwkes.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gafhjondb.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gsjvmormt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/guksmeiyc.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gneovnhcd.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gxixzrohs.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/galciovgr.sHtML

a?.b?.c
来源：http://wap.hesvh.cn/Article/details/glboxlnin.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gbcygswrn.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gcxiisddj.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/geffnuytu.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gnmwxijcp.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gvmvohirb.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/gbwcrlqnd.sHtML

[U89] JS：数组去重
来源：http://read.share.zdbjq.cn/Article/details/giuunbwkd.sHtML

[...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gqsfwyvgr.sHtML

[U90] JS：数字数组排序
来源：http://baike.fehbvm.com/Article/details/gxbjwcitf.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gnlvriifz.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gvrqrfcra.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gzbamfpay.sHtML

[U92] JS：深拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gvgqswaar.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gdfndxvvd.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gbwtigkne.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gdtepwoqq.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/goekgujie.sHtML

const double = x => x * 2;
来源：http://blog.hesvh.cn/Article/details/gjyzszxbq.sHtML

[U95] JS：Promise 包装
来源：http://mobile.zdbjq.cn/Article/details/gjvuoodcb.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.hesvh.cn/Article/details/gixvermkv.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/gmkhkprmf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gxijmerlg.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gvszgngts.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/guyrhsgcq.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.hesvh.cn/Article/details/gsrehxsgo.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/gvklgexna.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gpdfkxgnj.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gwjglpdrr.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/guxwkmles.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gickerdwc.sHtML

[U101] JS：classList 操作
来源：http://mobile.fehbvm.com/Article/details/gzzporxht.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gurqehgnb.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/ggdflagxu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.zdbjq.cn/Article/details/giermbxkp.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gsqgptmnk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.fehbvm.com/Article/details/gcanoanhm.sHtML

[U104] JS：防抖
来源：http://mobile.hesvh.cn/Article/details/glftrtbqm.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/glfroycpb.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gmeqtukcd.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gxmnoauqb.sHtML

[U106] JS：日期格式化
来源：http://3g.zdbjq.cn/Article/details/gjnzgewda.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gxoljsfrl.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gvjfdkgaq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/ghrlzkqlo.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gnrscosjs.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.hesvh.cn/Article/details/gqzuagjob.sHtML

[U109] JS：数组分组
来源：http://www.share.fehbvm.com/Article/details/gtpnoxhgz.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/grzridkuu.sHtML

[U110] JS：数组分块
来源：http://mobile.fehbvm.com/Article/details/ghgosxxcn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://blog.zdbjq.cn/Article/details/gyvjrrodp.sHtML

[U111] JS：对象转 Map
来源：http://blog.fehbvm.com/Article/details/grdtfflgl.sHtML

new Map(Object.entries(obj))
来源：http://blog.zdbjq.cn/Article/details/gpfiqfsog.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gywbhbgca.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gmzljteog.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.zdbjq.cn/Article/details/gimanuhkm.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gxbayvfzy.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/gbwngmpax.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gaedmynue.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/geqbnlmrz.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gcmbjjkzg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://3g.hesvh.cn/Article/details/gcfdtiywj.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/grcyykynq.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/grcszsdwa.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gwmlsmodv.sHtML

[U118] JS：开发服务器
来源：http://blog.hesvh.cn/Article/details/gzszbagcp.sHtML

npm i -D vite;  npx vite
来源：http://www.share.hesvh.cn/Article/details/giafvrifc.sHtML

[U119] JS：生产构建
来源：http://www.blog.fehbvm.com/Article/details/gugmdvpii.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gnvtsginq.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/grmezpozl.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/gqmatiqry.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxcivmlcl.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gsldigace.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gugavcdxt.sHtML

按语言统计（条）：
来源：http://blog.fehbvm.com/Article/details/gkawxzpjs.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gycszanxp.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gdssjuzlk.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/glkozpwsk.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gpgijygiy.sHtML

Java ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/gdwrwhizc.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gbsjgpwbt.sHtML

Ruby ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/grcqfxbte.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gvpfkhqbb.sHtML

C .............. 30
来源：http://www.share.hesvh.cn/Article/details/grufuiugu.sHtML

C++ ............ 30
来源：http://www.share.zdbjq.cn/Article/details/gbfjuvefn.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/goyermulz.sHtML

Bash ........... 80
来源：http://www.share.zdbjq.cn/Article/details/gobbdfzqh.sHtML

Kotlin ......... 15
来源：http://mobile.zdbjq.cn/Article/details/ggwhqexgj.sHtML

Swift .......... 15
来源：http://wap.fehbvm.com/Article/details/gnprtkfnv.sHtML

Lua ............ 10
来源：http://www.share.fehbvm.com/Article/details/gefohjgyk.sHtML

Perl ........... 10
来源：http://baike.zdbjq.cn/Article/details/gllrauinl.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gtmqdkgnu.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/giypnrutm.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gqkbgrovx.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/gmrvyeepp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fehbvm.com/Article/details/gqxwlfikz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gjsrxfmcb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gaazfhbxi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/glcjydvab.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.hesvh.cn/Article/details/gepqbfffp.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gugrzxtrl.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.zdbjq.cn/Article/details/gfykwsrfh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gyhbowbae.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gobtiehlk.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.zdbjq.cn/Article/details/gsmtqtkoc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gfjkytxtk.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/guchntvoh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/greqlqcdy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gmthjwrdc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.fehbvm.com/Article/details/grphgpvlx.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.zdbjq.cn/Article/details/gmgnqtsud.sHtML

Q SQL 专题                              90
来源：http://blog.zdbjq.cn/Article/details/gxwxlysel.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gsfqtbdpw.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gxohslnpz.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/ggjpvcytc.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/geszvaaey.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gqjbauvyu.sHtML

合计                                  2106 条
来源：http://blog.zdbjq.cn/Article/details/gzjwyufjm.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gwmhyguib.sHtML

使用提醒
来源：http://www.share.fehbvm.com/Article/details/glgcghxak.sHtML

--------------------------------------------------------------------------------
来源：http://baike.fehbvm.com/Article/details/gnxnqgmzc.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gnihmcexg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.hesvh.cn/Article/details/gkmrsgcve.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://mobile.hesvh.cn/Article/details/gdkajjbrp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/guusflqem.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gydqgsvel.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gcmrgqpgc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grptqkuaj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gbvtppili.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gkentbpey.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gixmuihfu.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gisdxvftf.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gvqsdztnh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.fehbvm.com/Article/details/gnwlzmxiy.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/geiknionx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gcwqesjtz.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/guislvuqz.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.hesvh.cn/Article/details/gwftwjffi.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gzgkdyobs.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.zdbjq.cn/Article/details/gqurahbxj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.zdbjq.cn/Article/details/gdzpyzyxx.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.hesvh.cn/Article/details/ghwcgdhcx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gfxepotpz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gikivgwlr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.hesvh.cn/Article/details/guffsdsvb.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.zdbjq.cn/Article/details/gustpcnjy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.hesvh.cn/Article/details/gbvsfgsie.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.zdbjq.cn/Article/details/gwgxkjpon.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/ggogssdlm.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gsvhfxuyf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.hesvh.cn/Article/details/gdiacnjgm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gpewfbuax.sHtML

目  录
来源：http://blog.hesvh.cn/Article/details/gsdncmlrg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gkwnebown.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/groqjrzqr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/glvurkdtm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gkwvyljhy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/gerezyfsv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gxkjftekj.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/glotrnmhp.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gynokmvqc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gzjxtclrz.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gzkwjvoxt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gyewqlrbp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gqorkuedp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gddhqzecy.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gyasstpbl.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwaaddjav.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/ggvtcxtqf.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/guwptyghe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.hesvh.cn/Article/details/gtzcskkpj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gxvegszpp.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gnpdstcop.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gafilpnkr.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gimtcwhtn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcdinjfel.sHtML

A. 基础语法与类型
来源：http://wap.hesvh.cn/Article/details/gbtzopewh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbdddjkgb.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gzuwzjshl.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gkqiuyyfg.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/girevhhsa.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gcsfxmxzs.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gxeodajdg.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/gbkmztubi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/glbhnreue.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.hesvh.cn/Article/details/grpsocbfj.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/gfcolefii.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gprgfzuvo.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gbvsscnsc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/goifocgtb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://3g.zdbjq.cn/Article/details/gagvqphfz.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gdcfafcgg.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gquagosbw.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/gvaafdwnm.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.hesvh.cn/Article/details/gseisqtbe.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/ghsjnimpl.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gukkhxpxs.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fehbvm.com/Article/details/gtmvdxldh.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/glrmyjkox.sHtML

JS:   const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gsdsjycdt.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gzbwutvou.sHtML

Java: static final double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gzvlvljyt.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/glaqpjice.sHtML

Ruby: PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gpusugioh.sHtML

C#:   const double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gkagwwpxp.sHtML

[A04] 判断变量类型
来源：http://www.share.hesvh.cn/Article/details/gjuwzumyc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.hesvh.cn/Article/details/ggpzorbrr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://baike.zdbjq.cn/Article/details/gwvwaetmy.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gmrjlxoai.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.fehbvm.com/Article/details/grxinbexv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.zdbjq.cn/Article/details/ggehgmttx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gpqtomynf.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/gbuzmrqjl.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/guvbuufvg.sHtML

[A05] 整数除法与取模
来源：http://www.blog.fehbvm.com/Article/details/gznamgmlz.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gnfxafghr.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gaitcykyz.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gticgxyva.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/ghylrmodd.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gugtuzomb.sHtML

Go:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gjpfekkwp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gdmkpalyb.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gujbmdafo.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/guqltbcpl.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/gzycmajec.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gataqpvbs.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gqbarxuna.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.zdbjq.cn/Article/details/gnoikzdvi.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/ggbzkczwo.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.zdbjq.cn/Article/details/gwwgdablv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.hesvh.cn/Article/details/gddhyzmmw.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gldezehwb.sHtML

[A07] 数字转字符串
来源：http://www.share.hesvh.cn/Article/details/gfywrbjzi.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/gotndvsdg.sHtML

PHP:  (string) 42; strval(42)
来源：http://mobile.zdbjq.cn/Article/details/getlgdnld.sHtML

JS:   String(42); (42).toString()
来源：http://wap.zdbjq.cn/Article/details/gwgnsqkzu.sHtML

TS:   String(42)
来源：http://blog.fehbvm.com/Article/details/goefwybnl.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.share.zdbjq.cn/Article/details/gjpyzcmkf.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.hesvh.cn/Article/details/gtirerdgf.sHtML

Ruby: 42.to_s
来源：http://www.m.share.hesvh.cn/Article/details/ghrrgmrjn.sHtML

C#:   42.ToString()
来源：http://mobile.fehbvm.com/Article/details/gdpiwfdqq.sHtML

[A08] 取整与四舍五入
来源：http://blog.hesvh.cn/Article/details/getvixzcn.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/genjysesj.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.fehbvm.com/Article/details/gqkbbxlri.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gccqobasx.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.hesvh.cn/Article/details/gkzbpbjlt.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gzlejbnsv.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gnjygdosi.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/gvjsjauhn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://mobile.fehbvm.com/Article/details/gayprhauo.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gjxuakkoe.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.hesvh.cn/Article/details/gxqfkeyjs.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.fehbvm.com/Article/details/glbcpozkq.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gkkmregsu.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/godtywthd.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gqexjhedg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.zdbjq.cn/Article/details/gwvshvmln.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.zdbjq.cn/Article/details/gfcooaffa.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gduykgxba.sHtML

[A10] 生成随机数
来源：http://baike.fehbvm.com/Article/details/gtgmhodgx.sHtML

Py:   import random; random.randint(1, 100)
来源：http://blog.hesvh.cn/Article/details/gcwgwgpfg.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.zdbjq.cn/Article/details/gertxdzhx.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gloogtiae.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.zdbjq.cn/Article/details/gattdmdts.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.fehbvm.com/Article/details/grtwxwbtz.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fehbvm.com/Article/details/gcibbdapw.sHtML

Ruby: rand(1..100)
来源：http://3g.zdbjq.cn/Article/details/grixfytpv.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gkmtdsvhe.sHtML

[A11] 条件表达式（三元）
来源：http://baike.zdbjq.cn/Article/details/gtzlribxr.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fehbvm.com/Article/details/guyxlhrxc.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/grfzrifba.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gqxwbfhld.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gekjgybbc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/glpbyhnah.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://mobile.fehbvm.com/Article/details/gubyxfejr.sHtML


<!-- 参考信息 -->