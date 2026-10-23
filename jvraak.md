代发 wailian999

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3mzoqxrnn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3eskgljlq.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3zytjlajt.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3bdxuuokw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3pfwbuftn.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3utqnstgh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3frefdjit.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3jqjbobqy.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3tpptakbw.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3ratqkesh.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3eayyofzo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ewntlszr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3qkuzeasl.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3jgcuppkz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3sdsharnu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3bhyizqzz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3daskioxt.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3daszoixn.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3tjusskhv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3rumkgdof.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3sgrwmsfb.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3dhvrdgts.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3sletckdm.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3bdqwbyyt.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3rnzhumdw.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3usydrkbj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3xhxiqryi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3qzcowgas.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3yeuonlcx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gtzytmyd.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3gogtzxav.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3syialfbu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zpyxveuw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ifxesnaf.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3orsbzxxr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sgwhokus.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qjfyybuk.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3mwfjgdoi.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3pzgvvlgi.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3abshabtn.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3udacnirj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3rxoennyn.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3xyitbkje.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bfhonius.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3qgxqmoxc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yfbrzhjj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xirvykxm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3hoeeydwz.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3xeraviaj.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3larpnmai.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3endelcto.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3uapefhbr.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3whgshwdr.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3lcdxhiie.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3yddgvauu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3vnafulym.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qqudoszw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3llxysbhl.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3brhjvdye.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ljvtqoie.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ojdahlgr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fmuchpil.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jraradpe.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3jlkhhdzm.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qtgknmjp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ggezztqc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3gmbymhml.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3iieidaul.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3yauvvnfo.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zvgloiui.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3jnbejuow.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3lyukqvya.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ufrricox.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3nyasjyii.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3aygvfyqq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3membjdvg.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jhaebewx.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ckpcmfdt.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3dwsoitsr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pgbzgjoo.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3eemyozeo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3ozmwcqdr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3uxkwerji.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdjhmwhk.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ikqgnsqt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zezupbyd.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3ewlygcvz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3qayvazve.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3wlcppcpd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3jsapjbdj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3plsrjbsm.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3jjrtptab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrqtiyvn.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ijaethyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smxmrbwm.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3xezyhffk.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rtpwkgys.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3aboffpqa.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3thftcnhe.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3enbdsmjb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3dpyjkbvz.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ugwnzkuk.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3axjuxgxo.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3cqwrtziu.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3hacfslaf.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ozvyffdb.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3pewwdvim.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wftlnafq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3skchwvam.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3kowzggcl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3rhqgihvt.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gauqlqxl.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3exkzkkma.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uiyfumvt.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3hmvxvove.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3zwkcllvg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bmnojbgf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3msycjvku.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3deiakeko.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3djewudue.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3muiskhhh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3coernmbd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3bavelmly.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ggqvcnkw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sbuncifs.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xgisljas.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rrrollez.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vqfdfrrp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3prausmeh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3xcqcoafu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3pbplckdo.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uphslsjv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3vsnotpbp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ydkplndh.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3vwyqvmaf.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3iatgqzcn.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ryrzoygd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lrwevqfy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3zvzeerxe.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3odtnmxwl.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3sswnfpde.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ywibrics.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3rnrlpelk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3bgjntwgj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3yctolywv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3usmtduqa.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3wumkuigu.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3sxeqftgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3akpofyim.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3wcwzipfb.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3rzbemkpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3audvnglr.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3pipbhepg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3mlhscmjo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3qwvqdvrt.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3wgiprdeg.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3pcrxfrtp.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3dbsdiqxz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ufxbsesh.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3hpirbexu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3sxmrrwta.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3cdgbxdds.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3fkasyoaj.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3biknfjzm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3xbmeflqp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3vvljgohf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3aeaqekgm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3kcexjqzh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3iylxtdsb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3eotskjsb.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3iphspndk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3sbkgxrkr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nagialwc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3jtohmsyx.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ptrkyaey.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3uvecxscp.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nxzpkidl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qfjplxig.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ohrcpuuv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3zhadjtba.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zltmnswt.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3tjlidrhf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3inttezga.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3khcyfxpa.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vqkcdkwe.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3szpapknt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3shrcggpt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cxlzqxhw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3tbgmrvnn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wluwzarw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zbujsbwv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3evtqyaxo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3hyfwwpay.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3qyugvovd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3nekrmoox.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3lpabluju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfyjwzsx.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ofoypjwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3caoavdab.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zrzfhwjk.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3uqcsjshm.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3yirttfwu.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xgwrytug.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ipyjtejg.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qewkpxqh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rblvbgtf.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3hzkjolrq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dfngxzzb.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3cokovlis.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3uvqufzlb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lptmaepe.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3twvzfgxc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tcddqzkv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bzoabskc.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3avisjiis.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ebutxled.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jievmrox.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3rlorewvh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3cttjffck.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3amcowrha.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tjwwblqs.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ayqasqqx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lnvclsgm.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3fbukzsqu.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3fwzcnvbi.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3taqxpumy.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3tsdduvlo.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3mxbvitne.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3xolypjsa.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3rbqmekqj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3vbxzvped.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3pontuoec.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ixshbfln.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ycdvetlk.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ojfccwdl.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3bbfsykvw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3yptelgrq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fjxhuknh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3svnevwfi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3kqrsujse.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jtpohdad.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bidvoiff.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ikuejccx.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3msmajfpu.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rpgcifjy.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3uhhdkmrl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3oevrairv.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3yuajncvs.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3mtsthwkd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nouddtbq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3noosnoxr.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3txhuzequ.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3lbppuyyz.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hncnleno.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3pusssjor.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ldwfpxzo.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3egzthcug.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3gpzuhlbq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3itpmriuj.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3oqbdcxkj.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3bcvjrkqq.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3fgrlwulm.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3avvjtdvp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rdvnoyay.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3vuiyoddq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jbhondyg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3xzeeooxm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nglgqnmb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3twrquwsr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3oybihcde.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dztudsri.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3awyysblk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tdnjrtxh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3urbrwoqh.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kfnbqtxz.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zdonevfg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dupfdyjf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3pplurdrk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3mdrxuswi.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bqtbpaun.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3olkphvpn.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3bgktobqi.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3ykudrzmu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3iqdavovu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bsvnsijd.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zshopjeb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3jfgcjoon.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3pwpgfjxv.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3vmgjykqp.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3bywbpaxx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3feobotgb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3uqctxghw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gwuoexmw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mqoixlrw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3livahhaa.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3xskseyer.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3klrjjzfy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3stetuoin.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3theudkyb.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3unbulemg.html


<!-- 参考信息 -->