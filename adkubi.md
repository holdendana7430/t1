代发 wailian999

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rydakklm.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3oqicddin.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3bzmlotte.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ipevkkgb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3bavczcxf.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3nqcdzlvj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3qrxnsddr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3kcpbrbet.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3mrlsjina.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3oskozsos.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3neakfneb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3wccobhet.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3zprjtxzv.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3wsfelyte.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nyiglxfx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3jcxlvdyt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3jxjkrmot.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3wdrxiode.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3aufhbwoi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3hovbxnir.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3mftjtlor.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3qjxvtbjw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3afxahwtc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3twyufzhi.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3nappbgsx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3borzkzkk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3ihjrrpmi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3deumnirl.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3snbhmugg.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3lqoiybbs.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3mejptpgk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3seehmjel.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3apfbjdib.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3ceejloft.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3bbjepdrh.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3rpalwqpj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3iitaxvmm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xwvxtxwo.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3qcdxlwcx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pljumdkm.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ddpecilv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3suzcvzuc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3gjevpgtn.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3etqmzmpv.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zipaudch.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ortueptx.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3rsccpzky.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3umimozds.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3ucwattmc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3lcuguoxt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3lnfcchrr.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhjsdszf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3rhxvnnqa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3myfnnllf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3baljcmpk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3uhawlpol.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3nduthagp.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3gdvauqpx.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3rlkrjtiv.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3tvmtbouu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3uwfradas.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3jbsamfcb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3quejlqka.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3igoawoit.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3xhspdied.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3jlrupbda.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3nvcmtlei.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3nbgvopjo.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3osrplscl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3nbyadzby.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3iidwnlcw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3jnvqelee.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xkjdlehm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jfdniufk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3nqoyrlmy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3rzwdoqsj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3jtrhreme.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ppjnbjtj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3nihsjyex.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3abqiwstk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3hntkzrln.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3oyqcvzey.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3gvqtypme.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3usxpvcjy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3jpsskkfv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cnfqgtlw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3yexjtzqu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3mifymrza.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zcqdodik.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gtjnayvk.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3tduykxcq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3goslnhee.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3isnmnotv.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zqwkjcnw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3rgczgbxk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3srxbmhpa.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3emymlada.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3hlfybrvf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3afpcjmlp.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3mnahkqpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxrfvevo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3jgvgoujv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vjokgxvw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ukxfzgcn.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3moresqsq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3vfddbxia.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3pogtavtb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3mvvbmvrw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ilocjwjq.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xcsckqaf.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bllnuauu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3oyqjacnw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3bbsdaght.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3hxisakss.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3oqmwkcyz.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3veozqwen.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tmuasodr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3glftvyax.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3lsadrivc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3jzstshsp.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3ftotgoua.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rbbhhskl.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3tzxpmgzt.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3shkxrdno.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ulvkotpg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3hcvyeprm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xutieltf.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lfpjoxjs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3zvgxedan.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3jgikmkun.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dqsdpmxv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3xoihspej.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3mjphjdix.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3rrtjxpgy.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3kusgvwsl.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cedcdizz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3szxxovcf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3bpmysedr.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3stvuokuk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zhrcfpcs.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3wxnqomss.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3oavyprlq.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3oautnkap.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ipecxnky.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3pfayhgmo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wcsqwpnv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3mvixtklf.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hxfhuuxm.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3fmglphzl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dymkibfy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3bwpbbjws.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3xlxoevow.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3nvamnttm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3ywlfcglo.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3olqdysax.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3fmgsahwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oiybhgim.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3hwrvldqv.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3mfjqrady.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmqoipek.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3apyqykso.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3rbqbxlpr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3blchhgxw.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3kqhyaemp.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3zzztovxb.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3ydhjiqdr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3efnlmkpc.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3qsdhjxnm.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3huzdibuz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ohytlhef.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3vdsuwjmo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3aouwpkcl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ctigoceq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3vllwoqfq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3ukkotbkp.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3njykaqzd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3njezjuoz.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3wdfcivwc.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3mpkxljym.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3bcoxxxym.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jbsvesxi.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3agfhnynn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dcgafljw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xxueorjd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3rgqazxto.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fudutdlg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dergknpg.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3fmokmkhw.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qprkvuog.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yxtiqpji.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3mqtixxqq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yubfqebw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eujkbdra.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kzqjqpal.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ezjkhtvy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lmbtvzie.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3axjrunmw.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3agdzoglg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3waghtngg.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3gnhazztl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tsteqqbf.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3coclbtgy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3dwybehcj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3tmpkeyqt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqdljavr.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3diqwhori.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsultnxp.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3nvijybbx.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3iqbtivdj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3oqgekxft.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tzhgzsvc.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3facczbim.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3npdfhtsk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3vgowkody.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3slgjfcuc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3urfauhpe.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3suhmyoma.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3caqwzemq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nzyckusj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nooqmpqb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3eqfddqaj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bglyrdis.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3hjfrzrah.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3gqgzdolm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3irzfmgul.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3kmhlnzjb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3njqdpiox.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cdzbnaga.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3shejlgcx.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3agpyuaqd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bgrmryxq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3sbwnojlh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3pgrfsiwm.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qlerxyyu.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3yfsaikcs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3twshpsdt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3gijrnwry.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3tptoptvn.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ubpifbjn.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3pvtyttbs.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3qfqdrnat.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3xstwflhg.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3bwurruit.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3kwqralxj.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3vlitqfjt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uxgbgbiy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gkvbjcfl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rbtthsku.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rmkdabhn.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wamldnet.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lvteiafn.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ihttxukn.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3flmenxhx.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3srtnjaan.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3fyldnaqm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3bqfppthz.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3sbiosbss.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bhfydzya.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3ehkmottv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3pauxlsqv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3aafusird.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3xnigaqki.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kphpvvxc.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mqmmcotc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3lkojmpcz.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3crmkajca.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ywmelazv.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dnlldubi.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3yqyubslh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3uolskngv.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3aynujmzc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ldysqgsa.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3geftsgpy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sjyuwgwi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3fugxalry.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3aqktkkcw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mebmgoaj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3oewcvahs.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3jswimkri.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tunzsmyu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cpnnvrxx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3trtiksyj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hzsdqaeb.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mkclegky.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3cqtiabat.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ntlovxwe.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3wufziqru.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jdicylei.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kiqakmpo.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3jsepqyry.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3pzglosqu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ulodkvgt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3evdhbirw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3tmmlgjgm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ppconvyc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3mdcclrkm.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3ildvelnw.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3invslhol.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3jhtgcouz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3fjydkzrq.html


<!-- 参考信息 -->