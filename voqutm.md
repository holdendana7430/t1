代发 wailian999

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3brtuvpvb.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3nzhptsxk.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3jfayoamf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3kdglylxh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3gqqerfzv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3vjtsynav.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3oqjuxmmv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3xgzmylxx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3uvnkpyyh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3rhdwvtao.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3pqwalele.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3bocwslmm.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3jngneddt.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3kzgngqbb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3skwpuatn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3pkhhgnxw.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3jqvrpbwc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3muhcpbog.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3jdysavsn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3huixxido.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3rlkgogqz.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3uampgdgi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3tleoqvwn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3jeiopqrm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3qrpcfwsn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jgogmost.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3ablaigds.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3taqvmalf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3qlbcqmbg.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3frdcjcor.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3jhwgqbak.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3rufvintp.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gvjddgnf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3mcpouwji.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3dpgaclfp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ryraryho.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3gmrumdlb.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ihcoufeu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3sprbffau.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3onjvnlzm.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qlfktpez.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3qpyojysj.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3dmqmqofh.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mpbigokr.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3xvrcrnkr.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3cvnrxnbk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hctgxnzy.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3qmpxyvfq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3urvagaup.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3wpursyvw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3vztnxgsz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3adilhdsf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3dydegtlb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zrxmlfju.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dbcjzgon.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3eydmkzek.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3grexerhy.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3pzyozyrr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3mjclqcvg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3lgxuougc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3kuzmtggg.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3vfhrdfgc.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3fhphfcjd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ttjdxvvw.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3cdmdtuox.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3vtvqastj.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3imslmhte.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3txgnrvks.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3ewhkvnbj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3qhemdsxl.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rqnjszip.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3wwjwrhbk.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mnwwtgyl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lhcwhoej.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3onexuegd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3iijdhsqk.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3qgmqobfe.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kbbouybj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3qojyaoga.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3zaatajdx.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3zsgozjee.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3cgotsbyb.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3trecabhd.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mobiemlx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3pmoqktbo.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ggkiiees.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3yglupfjp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rnbfvkuv.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3jgikqrdb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3phckbjkw.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ktmxftar.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3enkugebo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3aqtlxjlx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3goksqhbg.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3xyfbfbhf.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3kbmidbuw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3mqbzpqln.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3jnblvrtk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3gdnqbwgg.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3migxcctv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qoudadzo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3nyarfiab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkvftjdg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3qqoswwxi.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3iumqrwuv.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3ylmmeimd.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3gulaahlm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3gvlunwnf.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ztbajjwu.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3ptonzduh.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3movknxdr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3kgkmpgkb.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ucaponzb.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3aycpwhwn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3zbudppsl.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3japjnqcs.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3xfyncgqy.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3qqtshikt.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3ralrdbmz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ipelucei.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3lpmxpwle.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tzgosirt.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3uuhcqnpp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3pdzqwvmk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jtlptago.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3leyuvrgv.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ulcwjyox.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3eviavzwk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ctyyfmbs.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3leppnmaf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rqqoulws.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vnriowot.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wrfkbhlc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3qyfepbyt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3clyaqbal.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bgeushud.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ovtctqwo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lcbvzdfp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3sgcvfpkr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wjcyjade.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3ogvgxkan.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3rucbodgn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ztcfkejp.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3nbikiiiw.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3sbcerkfn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ownttdep.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3qoijtaiu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nbgojytc.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3vwohrlft.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3moalxcjl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3qafjqxmp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3xmpnepcg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ylxfwybj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3iznljkgo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3hxzggcts.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3mcaavyyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qmbrshtv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3lvnhghaf.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3dkutabua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jhfwbrjc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3jhdxitrw.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ccfaozsj.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3wvgjahyy.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3jfdfazgu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3adrcynyu.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3gtvjlndr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3tfndwnga.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3pjnpolaw.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3nmqfepyz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3pegjsqsk.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jpgqokuv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ghtdyifz.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3kjzspijf.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3plgrynia.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3brefkoff.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3ylqdzsfv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3dfohonha.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3lfnwrtzo.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3qhgakxdu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3dnftirtr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3agjehzgw.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3faypsbyj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zltacjne.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3bxhbohcf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ggwbdtjc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ogjhyjdr.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3huqusuwk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gnpiwpfd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3dofadcnf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3phvahclo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pkmkazys.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nvhyjnbt.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oqkqveok.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3doukmjdd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3juqeylth.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rxypicax.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3woqgbgdc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3siqkkyel.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3edpqzkif.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3vbmvhcjo.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yxpitizb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aanyuwei.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3twfxlozd.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3hmxcjwag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywnqflfj.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3drqtyoau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtevmoao.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3emsquukt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wsjtmbti.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3jrcfiaeh.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dxrxldbc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3zuvsonvt.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jeoeqtvo.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zskefwyw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3fvsddcly.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3uuyngopy.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3xcjgtimu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3ieyltlkh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3cxggwxeg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3brrafjmx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3bgxkxbhl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rzjokmkb.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ynngrnzz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3shrnnzke.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ciyeusjx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3irhxxrmv.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3szkltgiq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wnlsnzqi.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3srqparij.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hzasyhbg.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3jdwvwxzt.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3qocfqgwn.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dpnodqmq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3mrllixxu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3bpaqmnyf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3evjymmhg.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pgkgarxk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ssvobohr.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3rvcwggky.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3gxiwoojx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3bvuyjorf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3rqbhayio.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3qwdltcfj.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3yddosjpg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3baebmdxy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3jzxvnyus.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bytotwyh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nxwaogzc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lpyaltan.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fppfrkmk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3drcssqtm.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qcaxatlv.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3iwtrcgqy.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ebqszraq.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3vqqhgxei.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3bxkouodz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ryzsxulm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lmkdxfgi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3gvcncoae.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ererscli.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vjagfmjv.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3nocouhnf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3pjbdbotg.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3mukrjvdi.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bumerqun.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uqhjqhjv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3lxtlyrpv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kqbceeum.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3gyzgzkli.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3bjpkfgax.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3scpzpehi.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tolfosiz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdghhcjw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3obihppey.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3fbnhjnsj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hgztckaz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qifpqoqq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3tcworeik.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mnlkoiai.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fgshqukz.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lmudfzpq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dtwsaisg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tldzvsid.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wxhazlrk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ghfsodzl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3rnlbimmk.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3yquefaxk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dslfgzim.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3mkmbvfow.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3xmnpwtox.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3tsnqsott.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3whpfenbr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3yzgvchhj.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qymbqkis.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3vwnhhaut.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3jinxwysu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3hhgpwgos.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3vpfbihgv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3iyqzuojy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3boyittog.html


<!-- 参考信息 -->