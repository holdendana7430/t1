代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3jwbsbqqm.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3zkzbnvmn.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3peuzjbsi.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3xzxongge.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3wwvaygof.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mngndqpy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3utuhfrcn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3eazebqic.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3maunayzr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3xnahqabg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3eatzqyqd.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3hzitdlmz.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rgrzwwec.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wnahblxu.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vywalmof.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ptummnde.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ekpttozo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3lqxxrlpi.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3rxzaodyf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3gsajrrkr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3aadzpshg.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3asqvsgny.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3sfhyrwyl.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3niizqgpu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3dmxqobfq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ansmkvot.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3vmjwclxf.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3icezdbvl.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3tvkesivq.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3wjkzcnbp.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3jeasxxdo.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3bnwakwky.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3wegihyxd.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nadtmpgh.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3qjkgjawf.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ytgloaua.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3huvkupcr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3fwbnaruv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3pqzyhoko.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lgnbnfzc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3izliztow.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3lwzehngz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zpislsgs.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zudcxyqm.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3lazdwbyj.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jzunfdzc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ikrrqqqa.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnzrlzqe.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3wbtouftz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3oyifiqns.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dhjamdxf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3gwckhgwd.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3blfgvfdp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3kndxrjxh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3xwxftscp.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3uzfpznns.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3wtrsslwi.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3kovxwydo.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ypqcaxtm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3bqrnvzoi.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3uahsouza.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3dchxqlvl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3idfkbtdo.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wnwiwrut.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3gftcwbkh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3tnvftwqo.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ccroznyv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3sxuanuul.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3emoaiimx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qfamaanr.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3osijewfq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3zjojsgyn.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3jcpoboje.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jlutsxdu.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3piqxhsof.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3enevzkcj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wnijhywj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3liafncqe.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3oqsbzwzb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bfyuhehu.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xhkhisdr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jfbmijez.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3lcywcpsx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3sfiuishh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nfdrqrba.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3osigxsqt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3fvvarghm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3gyfcmwbp.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ipyjhich.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3wwcsirpv.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3jpqykgdp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3dopmkpow.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3vxciijnd.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3ybcjapde.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3orpmvaou.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3wrewkxjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gjenqacf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3rktwkkyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cveqfcdb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ghzwxaxc.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3akilndxd.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3zhbvfavr.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3byquqnhs.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3uricuick.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ttpquscl.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3mfbrnnzl.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hdugqbzi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3epchasqm.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3itaqotqp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3lalgrulw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3kxgbfjwp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3oqsrayff.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3lglratxm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3gbibkrhg.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3wxdmipvn.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3puhhlfkd.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3afitjdfd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bfmakwfx.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zrjdkszc.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3bgsonzhg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3wmunzjkx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3vhxctxpf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gjmiwjoa.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lkysmqzp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3rhmkfxkt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ttzbpyoz.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3smgjksyf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qsqwurnz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3niaxibas.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3zydgncfl.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qjcxsooe.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3grzgszir.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3knwtynfw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ruxwvqps.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3czxnuzmo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uuvtwsvn.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3qdtcoaut.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3mbneugxo.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ozdjwgyu.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3tzlemzue.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3kpmgoztt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3stvksfmn.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3memlgrcf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3icgyampf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3qrblchxa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wlykwuit.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3dmunloxu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3wxzfyugm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3cedfvmpp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3lnczkegq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3uarlysal.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3lvaweavc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msbqsaut.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3uxbgotym.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3rdaofsay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yghxndlk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3zrqqyuef.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3nqpewznj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3ycdekbzg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3nfulxqee.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3depmyngh.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3ibkgiwfp.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3chieybrh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3mmpuflsj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3zqpgnnwg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3kvxbvlrd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3hmuvurli.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3bzgkgacj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3vgtprkuq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3tcxbpbkr.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3lzqknwww.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3wjwoivmg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3ueexqyvs.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3rycmvdcx.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3fovbamkk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3pbxjlxlk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ogmihwwi.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3vnkniitg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3glfxbthw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aebvcjzk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qoiptmiv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3hylabnsr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3esqtrvrj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xtclmwtq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3wtkkymyd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ygrvotfd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wtmwwycv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eoolqhhg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3powginaa.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ompzkipv.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gbdzinog.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jreerrst.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ztsukuwp.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3wrroawwj.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ryjeauzi.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3hbwthsxf.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wbqoxitc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3fdlbfzfo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pzkfwhuc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hjvkqnll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gozqioyr.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ngzxzzpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgmrjuqj.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zidfaouf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ocwxvrkv.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3teyulkuv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nrzhrumz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3isgiqphl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pilrdgmu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3iczcmixe.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3sakdkroe.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3exkkferq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3zuoyfxzg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3ftxfjqzx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gkvseyke.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3pmkvnchm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cpcewgiy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lraaslbw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3lntdyzzk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3skktmdrk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3wqakbmgu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3hnggtvbb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3hgesjbjp.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zfckzusk.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rjjruiwi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vsewzdig.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vzeovzcf.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3xszydmfm.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hhtpzpic.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qozwzino.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3saxhhpbe.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3tgkjhzkw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3putdahsm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ezusyiom.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3jpvuieke.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3emnzocpl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3jdrocilk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3vdccrunb.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3cbzlfaau.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3eoairyyo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3stgzxvlw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pqjydbxm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kwfcyoyl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3biqktnmf.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aqlulqeh.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3alpbscic.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dnyyadct.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3sjjkbaho.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tvriisur.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wirzoyly.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3ihdkaaey.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ezzatlye.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mqajstco.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3tkijdazd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3dtssyqdv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3moqpewfx.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3cpfdftaq.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ecurglee.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vycncuaf.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3sjjhajun.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3abyvamol.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3hprpmniu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3nyirlgch.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fdfeahvb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ctlpzwdq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3pfavlyag.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3yhdixhqf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3reqyqttg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3mlbpokkl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xsepkpvd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3dqyiprov.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxuazsc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3lyjnfibk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3cfjrqmyh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dvftepxd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3caznxfjk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rawiolnz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ofvtsmld.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cokjqhsk.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wyrhrrai.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zofirajc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3yzjiakcy.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3atktbkan.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xtyqxzzx.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ogzlxefw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3qbeishkz.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3aotpcrsl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jztlggdx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3akioavry.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yczadlht.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3tmeergxb.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3drqhhjeq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3vpcocthy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3vpmqxnda.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3tcgesvsc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3oqyosqlg.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qwplawvc.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3redxzjyf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qcqaykoy.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3asprkzkg.html


<!-- 参考信息 -->