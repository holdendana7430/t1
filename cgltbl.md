代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3uqwxasrw.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3hlocllgj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mqdbkozu.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3loohnppi.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3wonozpnp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ezykufnk.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3hwpqrpsa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3bhuhbsab.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3dhhvzirh.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3wxyohnxp.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xokferwh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3uufsvgwi.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3cilojtqj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3cqgmzxjf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ahyykvep.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dsqrvsau.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qyamknyw.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3njuvjrig.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3deeewort.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3bimckaym.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3ecwiqqxs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3lfzddvnd.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3esuhjbyd.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3vtouhvzt.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3arjdpfrp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3xouwfymm.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ofnlqnve.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3zsenyaig.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3wjmzotxb.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3teuamsyw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3sdfgyuej.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ojmzhppf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3uzqqsyrb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3cwdgfrpp.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3njkdnmpv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3acksjffj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3rsrokqiy.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3tpmzigjs.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3nhhnukhb.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3utkbjtwu.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3jkwhyton.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3tssetrsr.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3voheljdv.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3podsidio.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3zxgjpago.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3oenfqzjv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ycgrlrjw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnvyvlgz.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3umyvwpux.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zggmykfq.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3juwffgjv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3bxzfdnny.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3jgcfdaxw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bwitdysa.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3wmxbojpl.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3pxglhwbw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3dqidrulu.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ajxhhjuj.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3yttcpopb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3xgkxnjrs.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3ayktclsw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3pmngvahw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3fxixaynx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nkgzzfim.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3wmgshiqz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rwzewlyu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lptjweie.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3kfqlehdn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3owbwlekr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ufbttlso.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3toawhqdk.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3wxxamhvm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ekcnzbpi.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3osiejyuf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3diuiecnw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3sjztfyie.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3kpsyvjoq.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ivfujvmz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3lrdauabz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qvrptyiw.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3ymdpdlfb.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tbmfjgqg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3dxovrcaw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3bmmljqns.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gvtmpegd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kyuwundt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3hsbbtsfs.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlilenly.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bmxyrptj.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3psnpclgx.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3pyheusmg.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3hoodswzf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3tzcbtcyn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3fmddfyvl.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3vyatqojh.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3wjaynzaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egyivjmn.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3eqbzicvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3edzxzzgg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3wvrehahm.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3lsztcroh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3zqtskarz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3eqqulqsh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rfmqxxtd.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rjqfqsht.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rbkimowi.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3beiuhcbz.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rtpykowq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3xkdfbfop.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rtlvhice.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3bkanarfb.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3btyltgpu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3pkadibnx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3rsrtsjoj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3qlnhlbbh.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3urwohvaq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ljghetaq.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3rsxzzcmc.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3pcilnucy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3xloknzir.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3qcddjfon.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3kfdinoxb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3gdpgwjmu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3wvrtwpgd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3buvppzvl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ayyhonus.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cwlupldy.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3wgjgmdlr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bmwrnpjd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3qgrlktfe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3vivwtkcq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3mjlexfjq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ekflhjkn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3gkqerlss.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3jpgfixrm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bkbqbnsc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3abmjbfai.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3hvhwvqgw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3njzzdlnu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3loqjmlel.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3ulkxftun.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rkhlmodx.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3cfpevdzc.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vusqfdew.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3yibafmas.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3flnfcalq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3coyunwwz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3trqwysnb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3zwzcypkr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3lnzetgsk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3iknxxoan.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3wjomguzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cixleqnz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3nwsmngtf.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ajmbjqer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aisrebrt.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3zfxzrcnh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3xsfdnpqk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3sajehuij.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3wfmaadrk.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3dieurutl.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3tvjyvowh.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3cphtgodt.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3nsngfell.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3icqxsfmm.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3abntrkpv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3igbitvsv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3wnbuqoch.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3tdpztost.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3tjmimqyl.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3apztukbe.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3mngmawqo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3zcraakus.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3slzlmflr.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3nzaiqwog.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3onrikvgf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ihffkuuv.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3fpbiaasm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3elbelsgo.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xtzaffqj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3edqbxlrd.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eqrnqnee.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3niozjgeh.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yijxbhrm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zhiryuoz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dumgjqer.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3jgwkidhz.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uatfjnoq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xrwhivir.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3krwfrlbb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dlaolxxh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vpihzwvn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ncbytjeb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pisbtecl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nswfdsus.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3houvjsas.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tjtynvvk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sbxdyvzm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xroxqoxw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3azhlsjci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qtyljord.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3olthecss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mforjbfm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rgwigrhm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ztqhojiu.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3rjvzsrmu.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mzmtfjdg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3pbbmuwgb.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xfqbnluj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3udlqafdc.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ubcemihq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3tazewmhf.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3munbnydy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3hsyicptx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tbjikxob.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lwibzwvh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gedendui.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uduktdso.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3bnrqgpre.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3thsxmzty.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qdausbbj.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3vqyxawab.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3irhlrtjk.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lwwimqdf.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zbycyfjo.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kejhysxk.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ztflbfsw.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mxqbyygk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ldsoptpn.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xusvausw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ktwazqtb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3shlxcsvr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3wnsydzrv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3doxxcvvo.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3othwyyks.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3xbuffjzq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3qgyaztuh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ecjzqjmv.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3gjqafuid.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3nvuvdbor.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3yrxkeitb.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zflewyjf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ccamsoid.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3menxdmfc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3riasfvwe.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nhusvdwg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kxrgmfzv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cisbepnj.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3cxkgayed.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3mmuwkdvp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xuzphsdt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3brxarppf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mooxjvru.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hisytzpl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3akogtnhi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3pysqpfmi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ozzwweoe.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3obkabmgd.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3gdifergc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lxucpsum.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3kvdfaipv.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vaznpydx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3dpjxexvy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ncqfgtbz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3vffaysmf.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3pstaruea.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3uiwwhovy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fgpiazda.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3lhphqhaz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wfflbtwp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3gexlmtke.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3huloxxps.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3oarwkmqo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3mlszgocp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yustfoig.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3yalsqwfr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ajbavnbe.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hpxqoymq.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgayjemi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dpzxzqbo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cdvpoxgz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3rezesspe.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3scvtlrlo.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3blldbzuq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3pqcjlbgx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3vyhyxdkx.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3spxirlky.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3segxrksr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3cyaagesk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zeymzqsg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ifiwucvb.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3iypvbjue.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3uvyabsvs.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3pxfngsxs.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uniyhhbp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3tpcsngcd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jurthzty.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mulztjeo.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3etksjdri.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3hsohuofg.html


<!-- 参考信息 -->