代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wsbvpulr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3buraqjkk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3reakwtci.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3bzembgie.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3iuocayje.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3odvvrxxj.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gfwynljn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3clodzdlz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3gdvvbrdh.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3cvfsniyj.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fsyzkgeq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3lniyhkuc.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3rygzdsyl.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3ywrttmwm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3vuqnvmft.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3tvjvpnni.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zkrdzpgt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3qkovasbv.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3vnytpctu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3ioutmdhu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3fncpukcu.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fqiqpfuf.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3qrtqnsmk.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3hmivvwda.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3vsqucczo.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3yvnxrcrb.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3charepvn.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3hhhxzmap.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3zmdydxjn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3mrnkpyjg.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3hltdmsvr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3qngyhmpc.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3pqihomqi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ywftilqs.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3tomcginu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ddahuoeg.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3wwselfpr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3mhcodbsv.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3stnqwquj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xrnhbijl.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3opmzsavi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3rhsvmvpg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3pqnqscmz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3lqafzues.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3gudgkjgr.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3jlffohod.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3jsnodigy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqkjrljm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3kllkhzwm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rlbsmsox.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3joknzxnk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3jaatrqir.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3hyaldwkf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nbfampwh.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3fjwmkekj.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3rymfdtar.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3yuryzwos.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3drhwyvhd.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3fbtreenk.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3qbowqjbu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3lwefxetc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ibnwavva.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3arqtnxst.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mriiljgn.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3tqjeiaad.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xbmqyhfs.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yttzytos.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3rfdsmakb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vysbiboo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mfhfecpi.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3oojadzxd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3pzpqrycc.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3whhyzuaq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ixoyuzgg.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3uabuhiig.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3baywefmi.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ullneuqx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3feryticw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3xqfdboef.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hoplxngy.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3qgbdsype.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vrrevkyf.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3ougocoml.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ligvfzho.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3hhnjppbo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3mufzfugn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nmgrvjyb.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jelefwqk.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3pcvhvbat.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3thpgsshq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xhgwlqaw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3sbunttsz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3vhuxgfgb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3icjxlfit.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3pomfceew.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3jiqrkums.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phzcdfim.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3hesudhzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ianwmtco.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3afhjlbpx.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3vymxgqll.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3voqxvzfo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3senlqweo.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jbqdgbqv.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3mfytvkbd.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3dtaruulc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jzwrcpet.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3juotjlzn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3rbiwusfa.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3xwjudwwn.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3aydziuqt.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3wshlgifn.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ygknapst.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3bnqahtjj.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3lvxrnnwk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3sszhqfhj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3egimxhcn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bxvoykyr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3iqkqrdau.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3wsduaiqw.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3efvoazaz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tczpnigz.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3qdpnfipn.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3bjdaesro.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ryjxwycj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ygbeuefn.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3oeuyabkg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3gshfkzpp.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ipyswoxc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xnypzioh.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vckofyca.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nazmrcqv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uptxfhuk.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3wvnbsbwx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3buezfjim.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3liahsoks.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3tvhvifxf.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3hvwtmxlt.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3bhrzqatt.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3wtgmelai.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3wzudbqth.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3txguxtgg.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3pxuznqpw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mknxwzvs.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3xlcmvzae.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bfzykece.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3cxwbmrcz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3vhbcxtnw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3kjjgnxlt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3vkbpkkwk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3swekynsi.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3tmxfvusp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbnetaiv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3zqjjdwel.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3ryhuolbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atyliyxg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3yztjmrpv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3rebavokf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3mdwimwyj.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3gekbhdfi.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3mlbradso.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3fekuejcs.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3pwctfefs.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ookekgtq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3vzuziyxl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3rlrvzoyg.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3mnkivyyv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3hqtjtjwn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ovrsgkyw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3qniotbwv.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3svdkhyjc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3xtueffgl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3uojzvjbq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3sbcieaoj.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3foqfwcqg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3ejhaxpne.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rndjtoeh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3vgqqhpro.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vsslmakp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3qpdtbwrj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3pgilzizj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qxtoxkgt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xcxzttpw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3isqznufo.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3sbagyuqa.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kxjmmnir.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3uckjjbfl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kkpaucza.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qpgqwqof.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gzuobvkj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ydzprvmt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kakhvxox.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gjagzcxm.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rclopjya.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ghzamyxh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3gmzqtcjz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pcfjryrw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3eogsxind.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3gavvivfp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tgibszvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cetmqwht.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qppjruxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxqkybqf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cibvkcov.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zmhvfbyy.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3anlvtapf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vtnknbun.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3mquoytqj.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zeeblqzc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3mxbgyomi.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3iwfmnwni.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jrpgfkzl.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3fbpksvan.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3zzpvzjci.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3kldungvb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3spvtvnau.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vhruciaj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ngjkmzli.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3kjxvpmdz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ezjxdjie.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3xvcwkgrk.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3pslbdbve.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3afulwchd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pvhortex.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ivgopeys.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ftnpnyqm.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hfkujmqp.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dsxkllsp.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ktypbinc.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uswzggwv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3lnefycbn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ypixkbwk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3hjjbckxk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3vkjqkxhh.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3uttvvqfw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3zoxsstnc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3risxbkbq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3cpcmaivz.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3cbirvcka.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3ueqeyops.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3gzvblvsl.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3umzstzid.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3imjaafjf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bhzvbhkm.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rakfsvhw.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cuohzvwn.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vietxctb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dovbgdbg.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3wtdwshkl.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ztjleidc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3futmdbyf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3zlxsscjm.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xobqnkhh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ffhisjjd.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3nrymizxb.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3vwrpwboe.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hhtutels.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3vhartfsa.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ysggklzr.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3chgbjoor.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3btizaatv.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3aotfdfbs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3svfdpnwp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ciudrfqx.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ghyfennz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3zgqzicex.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3kjgoiyvz.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jyngxjls.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3vihtzwgb.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pcrauvlu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3oyblgrid.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pdicizgm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vmfhtwwb.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3tkxtshvg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mmszserc.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xxapqobr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dofvgdum.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xarcosug.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pjsdlvpq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jheatgbv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3odsnbwvc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3otnmijum.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3rwdghlpb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bnnfjpif.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3jklvlbtc.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3qyujmcif.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3bigmyfqf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3mjofpfoz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vnpvrazm.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3duroewhi.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3pfdoryjj.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3exslmgog.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3enrazeaz.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3hzcjtjxk.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uywotxeu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3xagghbwu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mcrmxcxg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3oxxcahff.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fyjvynsd.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3liwiudhe.html


<!-- 参考信息 -->