代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2bnvxdcwc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2mmmprvrg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2upccqful.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2vomzvxot.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2qturgwzf.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2cdgcribf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2agcjbiew.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2bukfnilh.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2mfryggmu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2jrahzgno.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2onzhaszn.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2vnrjeiwp.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2qrlrvrcf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2edxdpixh.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2fyhlgwrz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2dgrcdopm.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2knjmotnd.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2jijreggv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2fpwobhhq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2wwiuiane.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2zdeduezg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lupgklgd.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2nqbpxktc.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2rktnqttu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2twuugxcn.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2eppgvkax.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2uiiyqrtt.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ahndlovw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xymgwsqh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2bizomyae.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2rehrvrrl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2tciebefy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2blmwhczd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2szdrzelj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2pmplrmcf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xpsqgsso.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kzaziays.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2xxoxwsxz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2jsrskhtx.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qpkxdgvk.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jmjsuyym.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2fbkyuooj.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2fousohip.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2mczdemxd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2hyfmyjan.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2undjyamv.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2mnxubxub.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwcbwoly.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2qfcnymmh.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ihboextd.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kyhguprg.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2wyfhuxip.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wvuerbey.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2syhylotr.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2madbftju.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2bdxpbxfy.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2cffctnli.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2qqplwsjv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2xwitdrti.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2utdkbwzj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2cwhmuxqp.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2tvkfljqj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ptazmpcj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2sqqizmvs.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2kzryvyld.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2rufbwcjy.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ojodfrqh.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2mycwaqbe.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rsvgsulr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rcqwaqom.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nidvtefa.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2nhblxcqz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2shznsmwu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zpttzdsb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2bclqvvjg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2wksaimrw.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2inatblnw.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xvzmmkph.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2cxffcdzq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rtdxrhbz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2hvqgvxum.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xqupavoj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2stcnznwe.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2irqxaqly.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2islnptbz.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2olhxvqes.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2urwapqhx.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2wcmxujvw.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2obhblxhu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2rjuziesn.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2lnxeksxp.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2qdgjufaa.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2hqotxrmj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2isuflwvs.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2nxzjtrhj.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wqoxsafj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubixwzsz.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2emvcjmnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eovvzgnf.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2huhzqere.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2njskzljf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2gurdfuws.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2ckapdvot.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2cepywcey.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qqzxsays.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nayhficp.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zprcxmia.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2byjpnwxc.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2yaayesnf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2fezgijai.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2dccwsgvu.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2irpckpry.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jllphfkj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2kjxfshwh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2kxhowqzo.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2fysbjxzo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2mzncbcbv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hprvfqyr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2oqsrjtpg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2mzqtlpyf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2iszmqhrg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nesqcrpn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2rlyxnfiy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2apfbjlnq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2qeeotmrt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2sphkvenj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2bnvrfydl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2qxhpxseb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2evvrwtoj.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dgaawhwl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2paknparn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2inqubbdr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ngfumccg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2zqfxmtwi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2juywjmhg.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2iputymxd.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2suqagfra.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2dlcibgjw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ctfgeycb.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2olgbunsq.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2uyudoiac.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2auqpaplf.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2phyxkksa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2oojbomko.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2oepwsbsj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2idimeern.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2xgmwquyw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2dpggtrwg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2nugcqdxt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2vdoczmfu.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ddvojebd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2zsgfqpes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrvemnvl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2xgftpxqp.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2iqhnpurv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tvbokkyx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2xfvpxvle.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2gkiswikg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ilaxcwlu.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2oeofkbfh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2xnfvwoqa.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2tcwhxbcg.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ufeqalfc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2trcvmair.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2zdvicxwb.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2hyukvxpr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2toykkjoc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ejbadzfw.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2lppsefzm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2jqgzvebn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2hmgeqgcg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2ejacbtca.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2mqjxykcn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2ilnwuwme.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2kdsovzcg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2tfldvilo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nybcxbui.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2xlnvkxff.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2itgviaak.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2pqtjuipn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xksnyhzw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hvgasabi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2udqentqt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2squdftzf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yullxtxa.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ykxgldiv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2lkyiytav.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iblchkla.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nqbwexil.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wvnvkswg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dgmvhyxp.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2zzcfyooo.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2detxwnrb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2swmyjmol.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bznnakre.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2rukooobx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2pirafgvn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bkgherss.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2nbjgexdp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2symzkbhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hnesgvgp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2yaawgkii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twduuunr.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2jsqrcnvy.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2hvomogrg.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2cdzatqya.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2larsunmu.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2rgwimxpl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wbhbjwgy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2kbskptjp.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2olfvtfoi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2nuikxcgn.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2lvdzhqek.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2mntfdlbk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zsoeskeq.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cvoprvgo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2tbhykmsr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ogcvqbrq.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2jzhcggqm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2amyvcvmp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pbzsbsel.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2xkfhjpif.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2nbyhuoni.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eqkmelao.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2obiqzbhi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lrnfqtqu.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sxyicybq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qukjwpms.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2demjmyxp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ewasjxpr.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ebounahs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvfrvab.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2stafxpkm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2clpyxbwz.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xgvrkwdk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2obvqybwv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2duyestmb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2rxdfvgdn.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2pfjkwkiq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ljtpntww.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2brkcikku.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qrmzetwl.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2yxmilvgg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nogcrlcx.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hfwswgvn.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lwqewmyv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2retuytyf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2napjxsqy.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kbjrbkxw.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2wfpnycsv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2rdpzgfqi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2mzsmaeew.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2zpphbyaq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2vcjorceq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fnbdfnla.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2rhzrgdtc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ikxqmwkq.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hciheiab.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tsrxmqlz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ulnddnii.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2uomwgyvh.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2nnymempi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ijhdgsgc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2dxgkjedk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2lgziijoe.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ldmvhunp.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2tuhqldpf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pmhgyqly.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2mrljqfdu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qxjxpmro.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2havjbxyx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2olddtdmv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2rwrksazf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2qhgbxhlu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cudkziqc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gpjypebd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hhdmyfex.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfessqtw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bpvmcncu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rnqqkyvr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2agldrtoa.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2difeymee.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2mjhipmwh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yghotmfr.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2razbywnn.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2eyrkmawl.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2nmgumahq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zokdptjp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2csizgxff.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2jwfrgzfk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2gsqlrdrn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ksdatcbw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2cermvpcj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2speuhpoq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ovcgkbas.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rxzxsofb.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vauktbor.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jhrvfrqa.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2sdfgorda.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2gdcsqjmb.html


<!-- 参考信息 -->