代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2tybvioyt.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2wcajdmmz.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2bxuawnpc.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2vinwjsux.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uzxupcvw.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fjhxpbrd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2luygwcbq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2wfvlmfsz.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2nwjdaikm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2ierfygot.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2obfkvdlv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2klrhgitu.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2anfvazka.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2digthnjc.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2hngnesen.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2qdgvvefo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2poweswlb.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ebdnmsyv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2cwmyetom.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2hcxjdnvv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2wfktlinf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2yfkwjcrc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2vcsaeyuz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2fhcetfdr.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2qrtpsxmo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2scrgrcsw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2fjgbuaca.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2gpfmviqq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2obzgzcsb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gsuetlhg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ncplvvbg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2wktzmbai.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2eddtsflm.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2obocsemx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2mahlhshr.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2hjnfbmws.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mjrinseh.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2bxzwvngv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2gphdapjy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2swwsyzyt.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2eguexnvt.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ydhwdput.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2bcsvyoum.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wgjklvzr.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2dbvbwbpj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2qpefsvmj.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vntkekfd.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2atvxjsxc.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ootgnfdj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2fbwxmskl.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xcjtljxf.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mqqhjafc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2nntnvcnv.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kdqslgev.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2mdesvbcj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2blcpioce.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2tvgbujmy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wtqtdwvc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dkmpnptl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2hpbckmcl.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ynwncpas.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2kpugrobc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2corylmys.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2osnxrexb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2dmvejwam.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2xsjmnwxk.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2dmykigzd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2nxwngftu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ofiygrrk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2wqrgtcxq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mpqzgexj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2etybzlly.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mryeegxs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gxucuiui.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mhbxxxet.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2velainwu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2knjnaodz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hwssennu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2fdbheyss.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2twnrhyup.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2egxryxmz.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2kcjjvfit.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2tnoxfcct.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2mdmkliqp.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2seicrgth.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2mhcxpiuw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2gjfgzntf.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qgtegxke.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2xdfrcpxf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mrfjluen.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2wppeqxev.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uohhdxlh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2wckxznrf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2gxwetnmi.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2aqdzujgz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gessacwo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lqdtvrsz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2hguxqjys.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ekzpvuzz.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2rekuyrln.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ujlddzjl.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ahgbslnx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2jzksipyt.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2icbhqkpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zuznmoad.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2dtdzoxjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyufocyd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2fthyhtsk.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2vliohezp.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2cotbeofd.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2donlbfvl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2xrfeltit.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kzeqqvlx.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2febhhwgw.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wwtarqef.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wfvrmaxv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2mzcjvhuo.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2sqgvfyig.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2pyikausn.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2qqoejdts.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ahzxcgbn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2ujuomfgn.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ummifcqu.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2swkaiqkn.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2orjrdsdh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2giadaosi.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ubgdhapg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2yhxxuwzz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2opaqjgxi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wiaywfgu.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2uhwvkeih.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2fmkzaalq.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2wkijvefr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ncnhnokj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2cpeiapga.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2uqukuvuu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uljghdsh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hzpsayrx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kzwyzsrw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tvlgvuaw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ozgacxby.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hblslvpi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2lvwoddis.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gfuudaem.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2dfpbvwag.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2zjpyexkr.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2rtwolzeq.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lmajknby.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2rfsaanmz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2mmshxtid.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ryydchzb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2olcyfyuh.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2qpdvkzwp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rvwdsgsp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2jveyodjw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2yyokhjft.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2slkuzzle.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2zcgsxmrf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2qmcyihcb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2idoaaiuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gevdsayn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2elsebrdf.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2rpkxbxrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgrviosf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ztioopkg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2nxefpsvv.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2gjukoejd.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2zxsznauo.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2mqwmedar.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2jnwooowi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2msliqvfw.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2tieuknoq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2xafxfhtq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2rcngspyc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2jubdbvkv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2clvaauln.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2loyqrtsx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2kpjhekij.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2tdszvipf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2myhmeqrz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2rsaqabbd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2zhvksgno.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2kemcevto.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2xjxnxqvl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fkboqoai.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2xzvtxpua.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ooditlwp.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2quibdgop.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2xywpcpaj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jkcnfqnx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2bwvxgcbe.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ydhvrdbm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2dfaaorfu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lztsvuae.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uzihprml.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qvdhovsx.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2ssmgkwbs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2knuipewx.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ahhmwsmn.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jtmcyusm.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2rksxbgeh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2jdopojig.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tkamncix.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ivusumco.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2oektabrc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2frqmtxpn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2spnsdysy.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wclvnfuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2waymjqyk.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2njgduluv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuqpbfeb.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uzvxcxsm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2oskgpoio.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2wgatftdq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rigycoif.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2uujiczrk.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hkygdwek.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2yzywuzif.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2nopzdwbi.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lgzcedjo.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2sjxgnjxz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2drsysoae.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2klciosmx.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fnxuoruu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2bmcbgldc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pjncwnnh.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2pkktwvxm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2vzzqjsyp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pwaajsxg.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2wdmmvfmd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2jzzcddjs.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ckjkgbux.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zkwqdtza.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ppilehto.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dkvajzby.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2nsdlzyyh.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2yyuksapi.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tjjxefnm.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2scpzvvwh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ftjtoqtj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2katoedyp.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pavkjdes.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nakgxkyg.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2yptxoupv.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2kbicqqgk.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2qwtpneyp.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2ztzrvxfj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2tjouzqrc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2yxywyspm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qqrmxtmy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gqiopyij.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bxmlhxjw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nbwkkykr.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2eunyeyvd.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dulsyktp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bebgoxue.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2npokbryo.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pilvuruw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2umcxgvxu.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2anjwafqr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ipgybngd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2vyivyejl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2jduozkjc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2jhenxuzi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gojclohz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2uohorvjc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2dtedkbzi.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2bakduaur.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2btdioqfc.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2srdiocyg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2iupedest.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ikzqeubk.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2wlmoapdh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dzeoeawv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2gpxlyder.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2kofknabt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2dihsuvih.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2jdrfdqpl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2xgrtgtjq.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2oogewsrh.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xspplltr.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2qgkdsdnh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qjurdgcw.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2yimbxjzv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kdfbeeja.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vqwqbjqc.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2irlmaedy.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2twavbomy.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gtpipefp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2kitzitox.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2euaxyzrn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zuvklesm.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2fkkulqnj.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2weiufplz.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2udevqcql.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2diwdqgwb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kkumuwvt.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rrcznwey.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2xbgpscae.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2skfphjsl.html


<!-- 参考信息 -->