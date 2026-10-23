代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3pdcklflm.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3tpftpnjj.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rtdhijdw.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3qtpnfcod.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3gnmwrnnv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mmbibkdb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3atusrino.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3zpbyezyv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3zxapcgpw.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3bcbqjvff.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3twzxnpki.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3eljmfquw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ixugocwu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3uwmlfllj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3qfsjgsri.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3akkwveja.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3cpqahjfc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3afvyszcn.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3wfcniahv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lixcbiem.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3dwngrtro.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jpvtoecc.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3pvjekvmf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3qnlvnlgl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3gwimazue.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3saoeawfc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3rhowclnx.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3xcivxfbc.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3hezorjxi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3csbhzqxx.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3csmdwybm.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3bxwdhqtl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3hredsevp.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3kezepwhw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3osvaafhq.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qrkhqmsr.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3juxpvjci.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3nfbbztuf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3eycsvtus.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3banbmgdc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3mbujambi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3uhtdtwis.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3qbceeqgm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3boyqjsdc.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ornsonwb.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3thusgsxm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3pxvtlpvs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkmjjsll.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3rzabckny.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3iduursqr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3vmdhylyb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3byosqftq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3qthszljz.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ugziglpd.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3rvoyckcd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3wpvzaopf.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3dbnvowvk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3mxhkxxpb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3lztxqmae.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3dxjvavze.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3rcmgkomx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3cccnsysd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3brpyqlrk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3fctucgur.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3heccrsvy.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kdhtzfzk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mhvjlbxo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3dsvjizer.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wboqomoh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rtcarntg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3ztmmoyoz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pyxpsael.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3tebyryyv.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3qdjescjh.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3yjnopzjh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3zederjyh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ydchzron.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3wdbbfyqv.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3jhovhdhv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jqxvmnjg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3xlpvxbci.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sruclsuf.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3mkgknrbq.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lvjodehv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3azhsvzju.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lyjaypqe.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3obpbemql.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwoxbprx.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xdrsaaku.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3qmaspvvd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3kimqmrqw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3fpmvfeda.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3oifslasz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3abrnxulh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3pvplucpm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3uuuxigkz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgzyyfte.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3xckjzeeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtzxnkre.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3bzrctnof.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3eizajswp.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3llwnzsyk.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3znakurmh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3luxalevi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rgpmcvxc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3caxzsyac.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ymqjmegq.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3cloorzml.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3riifafcb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3hgwckguy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3zvlnwoxr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3gevwwulp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3lttgijkd.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3xdwuukfn.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3letqdjxw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3zodqcbil.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ftrvxgvw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qrkwhmco.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3htwerlfm.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3otnqfraa.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3huudckyd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ymhvghkr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3jbqwyqyi.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qvbkmeca.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3moowzgsn.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lcoqfsgm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3uwcntkzo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3dsojrrdq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xjkugihd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3eeisxpbz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dvraejww.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nmxdcnqu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nlfijgkn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jjmdkafs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3dvnmzzlv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3pqcxmwql.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3uywrrqzs.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3thbdydfs.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3wohyjpop.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3vmdxobxu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3hmrmwhkn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rudljmbm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3kslanoao.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xmxmlwig.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3nggaactv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vczwyhkt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3qkqxfvxx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3qjocrxud.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3zgvgsxwu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3nzmgljyp.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3potehrxd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3zbdrxref.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkozrojy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3warnbwer.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ciwblmcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ncjenmdx.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3kezsmktw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ftyezixo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3bxpmnmjk.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3wfykruxf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3skrgxuak.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3tnpvtkgs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3yczvplnl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3wnrrrtrm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3fuoseion.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3cbvwaysi.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3gvyswzkj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3kxxiwejl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3vwqwqiel.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3veikvmmg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3qnaavpju.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3hvzpvuwd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3pgjazxng.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3hqvwgoqa.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3pquzamec.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3dpmowzcu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bizvznux.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3nbsndofk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jimugsfr.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3tnrwisfs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xlqsrrgf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rifziadw.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zqbdpixq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3goucgtaa.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vyqogrri.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nnkmvjzq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ltmismtg.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uhcgjhxe.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xdmbmbac.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rvuggqaj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lnkbhaqc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mimagmqv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wophlvaa.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gjqcrmfh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wvjpwlrm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jejgwivo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fekhbigl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lovxweob.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3ylzgqwvo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3igbarjxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wuvlcbey.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3dccaxylz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvkstatg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kxxqaief.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3cucaeppt.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3zjcyfspt.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3osuqmaec.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3rmwgbrzt.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3slbpxcxh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ocdqlqpd.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3jdruypyr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gricsaae.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ielbmcof.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3oxjaevqo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kvigeeqg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3sahbkrhr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gsibalkm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xvaamnfe.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ympenkpn.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3lpbwztok.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3txboxhys.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3yoynpcuo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3zoiedtze.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lsxsfxls.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3truoaeqp.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fbrwzwda.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tiyqrqjr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xcrnoone.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rjxwuhuy.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3piwkcedi.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3xbvmuzxk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3nkrfyvni.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3liujnjlx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3gvqynvhn.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3kikubukw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3prfjhaqy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3knjdibgc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3knprxlpu.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3mzobcsby.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3joqbgnqv.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3widzfhuq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mzzhhmsf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sfxehaac.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pjldmohx.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3faxmqihh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3emjdhszt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qetvlxtj.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mgrqfvbx.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3aqdxqqup.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3iahgtgnl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3csjstzqx.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3xiifkubv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3foitndfz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3advfehms.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ucfqjeif.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3srduczjv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ooisrexx.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ggwwmsek.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kqkicupj.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hphrwuis.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3yyqkoudy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3atkwsmnl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3sbtnhppq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vyyfogqt.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3qzkfgybu.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3juphfibi.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3mqgkqxng.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bbsegvri.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3uowpjhvv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jbfgmfmv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3shnqbywv.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tiimsilx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3odkqynyt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3cbhzztla.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vtansgch.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3mtabpqta.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nablpogx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lliwvrgq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bkfzpogk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bznehvgx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eafipkrg.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3iurvazha.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3dnljsoaw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bbnnntke.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3fekauahp.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3rhltwoab.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3jimsvsxm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3upcnwpom.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3nkxmqnlv.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3drshwpuu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3pyunxoyb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3asrbpoer.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3nvcbcwys.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3vpqkmnya.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3xidrfovv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3klgwkwvt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3svnnfrrg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rjrrfuof.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fikypkbs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3cipyikkn.html


<!-- 参考信息 -->