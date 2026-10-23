代发 wailian999

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3imgzjivn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3jmsmzequ.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3pkskwhrn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3jzzwydoe.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3tpuqshzf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3hnshwdte.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vxqrbfld.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3iazmgpww.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3vaclefkv.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3iqrthpkh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3bcjiyokx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ivvynalo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3bwowccqq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3levsleqv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3awswavvn.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3rrpqxqco.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ktctjrnw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3fjtpfeim.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ndmacsvb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3byfwmwyw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3knvqjlmo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3cqyperzu.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3hsrjnavb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3idmznbrg.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3miesaxei.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3uqscnqgy.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xdrhnfvt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3npxoctnq.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3pdbiafxu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3jwrdehwh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3plespmwe.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3jhovqwyp.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3qthzxgvu.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3inncsekt.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3jajtewtx.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3towgsthh.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3mtwbjtwf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3upfxecnj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3muftwqou.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gcyozwsh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dpyhwdgt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ahobidrs.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rbtxiwjv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rmmellbv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rfaziqrr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qsiqrbwd.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pcqjuqal.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vqjtbqoa.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3fqtqgxtb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jonnhndj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3fdmxrmrm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3plejlkll.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3zqeyapfp.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3iesctjgl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3vwmrmknn.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3gornhrkx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fozqmsaq.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3rhygrlol.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3lpfzmkix.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3udugkeqw.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ikwatmbh.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3ukmsruro.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ruolglom.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3gnjvxqxd.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3bfzwyefi.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3vkdhvvqf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3hakkjhiy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bdkaphyy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xjyssbbc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3fvicnaps.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3tjjsbgjr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3hmlacoxr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tprxbvae.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jugyrazp.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3iszcxggw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3bpahigzp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3vhcrnzzw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ncigrbxg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3qvvsiykf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3rkvtvdwo.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vlazodhj.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vixxwuoz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3srvcbahs.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3glccqjru.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3sztqsgsz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hyfxckuk.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3idgqlihj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jfzuwvdq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3kzotqdoc.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3fuvakssk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3jflasazo.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yovjqswu.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3dfrykpgu.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3gyezfnfb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3pnxekbxd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3kqifurgb.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3elfppxhk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3okbiquos.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3zdfdvzry.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3kdcxzqxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgndebcc.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3akkozjes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjjhhvbo.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3drevstse.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3zcapcoqa.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3djensosh.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3reuikctk.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3gmsrcpex.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3oaqvjavc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3mnhxgisx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3piucrxxj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3oziwqqtq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3sepokzre.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ymrexmzd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3befktkck.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3jzznqwzo.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3igexilvu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3cehbbstk.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3xjsrutdr.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3pzbikfek.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vucjggfc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dytyyski.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3jnfmuyxu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3eszbsvei.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xmdcvlmc.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3osdkbdnb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3dhncgpkk.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gkvwodbk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3vmjnezww.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wrnksggi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3hfctdrdw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3obpmmzik.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fgddwytv.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3gfjtcdzc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ouiocycf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uydhmeas.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hfqzxtpn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3yduyhbeg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3aqenxhhb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rlvdlqcs.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3wuktqqkx.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3uhkfnkfm.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jkphtoxk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3xbujymen.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3zjluvejn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zjbtoino.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3uhbgexhe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3iuwjabup.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3wlqpeifp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3eqedpsic.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3wntltvhn.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3mkjvttmg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ezpizidu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3pqpxaxum.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3kkwinzal.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3kxphvvyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crbwrxui.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3rnfkqcaf.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3extlwrhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpnglqjj.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3wixfrbwo.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3bqchtlvj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3xgyfcome.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3wnvqcumt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3ywdduxxp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3bdxvcolr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3msnqwkrr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3piepxpxb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3yhybocbv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3dzuxkfdx.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3rlqbwqjg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3hztndnhp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3cacnlnbc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3knlslext.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3pyaennxl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3ayccgwej.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3rluryrhc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3euhqjurt.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3mfzilkur.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3kpvuhafr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3erxtisws.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3feukfild.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3gqgjtfri.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3wuvbaruz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3earujuyo.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3aeffihde.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xdkinsbf.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ilkbelnw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vazrhriy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3duelhohf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eyjkuoki.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3elsmzjtf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bgtjxgdr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tnwhsbtw.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3exqkrajz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kxkgupkw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ltppjpkm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ocpjorpd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3durivohc.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3olpfeljq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vnpsrtbm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3dvjbquhj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nqzxzxub.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3vkeenekk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owsumfza.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3mxerbzpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swoxphxr.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3txjfdlyi.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ccoinyud.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3njyemdol.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3eyzjclkn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3dhispsuk.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3byohrdhn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3embcugry.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3wirgndll.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3suzpquik.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3guvwkqts.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ozibcsbz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hqkuptsw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kiabjrws.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3zsqgvpdk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xpiiymgn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3duiathms.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3wjqyqdft.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mgvyrqgd.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3dlnlubty.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3wvoguxfb.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pnndczad.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mhyvymak.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wwftytil.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fcyayytd.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3geicthft.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3voxoodkn.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3eqsteadm.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3klmpguxg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3abvxnngh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvqoalio.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3fontxizo.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3muxezchg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3flubizwh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3lfxihdgb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3idhftpqu.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3naglwzma.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3rahfyxqd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3lkjhhbvy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fkmxwpvj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pufxnhkg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pvohxvyy.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zmbtzkvi.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nraszadg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nswhuasl.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qxsmgjqz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3tkptcbkv.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3atnqeltc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3dhoyrvro.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3cqeyykto.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3htccpfid.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3urlzzxsq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wdtkszjf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3bhmajqov.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3tmvpqlnz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3kdkdainl.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3cqrzqwhe.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3helonsxc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3ydctbyid.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3gzrzeurj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3gkpjwefu.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3zzuzsqxa.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3esiuncsk.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3wxrgpyvn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3pkjovlle.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fmrwuxpo.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3uwpngsmg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3urugivhy.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ayvnzygw.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3wrgcirqd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mdzzlafw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3wnflxaja.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3cbhdhugv.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3egfsmixs.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3twielhrn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3norcpjnb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rgtaiiag.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3phewitij.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jgkimtrt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3zzenpwtu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3wwkuivpz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3krxdbkmt.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kokjlqwi.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3psdlgquk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3mcjwyihf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ashccbai.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3wecxqdjw.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3nuohnsfp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3wmzxklwm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3luonmido.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ncofwiyt.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3bxekuryp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uroccqac.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ifpctbak.html


<!-- 参考信息 -->