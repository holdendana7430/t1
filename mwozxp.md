代发 wailian999

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ayygjwde.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vvgrmpoz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3eopgpasf.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3sfcvizfm.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3tlabzuqc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3qrfyqslh.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3sdqsbhfp.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3dztgrpqb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3byfeorwi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3adkvyfdi.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3dvjtzelp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3anaqifrz.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3cfxchxpr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3mllfnywd.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xlegjjpv.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3lmmeutkq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ltpruipi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3drkqcucm.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3wfgnptvy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3zvzebgjj.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3ynmhxkir.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3iusggjxk.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ivtwgbnb.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3pkodqyfp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3cswxqzao.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wvdhetni.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3duogbnqy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3lujayeec.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3tmokyaso.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zorcnbfw.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3loybwjuu.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3httznmlr.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ifixjsgx.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3fltqhgih.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ympbcolt.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3aztugsqa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3oyrhidzr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bsvdhnny.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ujfkawcv.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kcmqzttu.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wrsemmqo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3cxnhrevm.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3knmfodso.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ufsvmfsf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3zuacumvj.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wofbiipm.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xnjmopts.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3ozzxixpy.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3eekguejw.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3bcyodmky.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3savcpczj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivgkzcxb.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3azcolleb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fedafnvw.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sxmwgvvd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3etjrzleg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3phefrpmb.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3mviujbqr.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3mbszqkii.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3lajrrnpv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3tazxanml.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3cqwocckx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3dcmmmyaz.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3ahbmwmgc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3fbsbqvyf.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3xybgatek.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3koccqetj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3qtkeaznk.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3sabcckuv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3vnuggqrr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xeymqrrw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3svyqxrwh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3adiueymo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3warcwlmo.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3toipyuag.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3pmrbrnvj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3dbcfesay.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3mtvkvwne.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3aggrrmsf.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3yvtnacqo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3mcobbgqp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fksbnwra.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3fxubfzhx.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fzwjjmcd.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3aqibmfvg.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kifilkdm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3tvazlosr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nabzseom.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nurkqdfj.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bfljijoy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3ctejkfbi.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3srqmwunr.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rwsdbyqn.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3whatjjlc.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3slfxwmkm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3pusemuul.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3ugdvxhcq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3krqjepjy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3dzfwzyke.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ghlldaxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thnugvcq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3zkmuylcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvofmxfn.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3ynmdxdad.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3oxqicqdn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3heumejsl.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3pcstvohk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3mejwybud.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3agxipxnt.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3jlzlaigy.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3noctcrou.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3czlztdqz.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3vhunqcgp.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3yorslnmz.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3dytpeesf.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3qkbezprm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3uemqtgbj.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ncgtcpta.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3jlneqmte.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3gggjlyvt.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3ymqlotgs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mzqepwcq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3rsrihyar.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3zxuhjccq.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3wacdwvph.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dlnvyudf.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3dpasfuro.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3uygzacdg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3mkottyhh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3daendsep.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cfrjfzai.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3uhczwugu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jeadkdjf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3lgrsewdd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3faygdxvg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qxosoghy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3dhgobnwr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3boqtwoae.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3sybqijko.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3izhiddaq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3pbzpnwod.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3eipjwjqd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3zemcbpjd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3qyxvvafh.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3quoviqap.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mqzcrrah.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3rsbofqoy.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3achxcprg.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3dzcnwjxr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3npdvfmdt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3wbsfbfdq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3gofnwxpg.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3leoywabc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3uopgjvhd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3tbrhqppm.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3bcucylmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pkoclcab.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3nklxhhoo.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3ckasmdgj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lucwyhyf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3jhqiibar.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3rfbgssds.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3xaxyolrh.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3makjhnhf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3qaiqypaf.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3wspbyqei.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3sjqxubwb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3lfmallrk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3xoyjguig.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3pypeyxks.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3liyzqneh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3sgzkpbwm.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3uhdzucxy.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3cupdhpku.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3xwualcyz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3moreqmrj.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3zoqhsuhn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3ylhcyghy.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3pwtublrd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3vjccprwt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dulhzwyi.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ldicvnol.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ecoyjedc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xkxsapsc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3fynoonjn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tjstzshs.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3ygsnsqxk.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3grcmdapj.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mjdadmic.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kxpywfhw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3wcpkjutj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bofnywvi.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ijwmvmzl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hvcgfrdb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3gnmfjbbd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zmyfjqcw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cedtbufa.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3uutcfcma.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3plqdarar.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3ouvnmagl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3aluvxkmg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3naqinzoy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nhyrxqev.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3dhhyojcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mriaqkjh.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3qkikgesx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duqokrzb.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3wmafviui.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ydpvglwj.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3inwszheo.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3rcwgvxnt.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3caosiyea.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3xngrskiw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3efoxrmlq.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3klhzoxmc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3grjpzuxc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3uobalgri.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3wrolsuob.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3pesiwhuz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rzbcmivt.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3hwwssmxu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3krhxtxwa.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3nywmveqz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3xyigjgbk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3trdwbeag.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3iifahrqo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3datxzcus.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dovzzltj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zfgirvki.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wdgudvpd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uritfoik.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ljpxihbj.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3bbqqjknu.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yyksrfju.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3mvsbaboj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3xywdqpum.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3zwwpxvco.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lpordhdt.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3uwtkchcb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3nfmqhorm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3fkxzpvnu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3rugnmvye.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3wcnvfksy.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3kcbhopto.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3acghnotr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uamyrdfk.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3upctyywu.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jsfajbpt.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hgbxuxex.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3libbpmmx.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rawvpjjd.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vyxnqrdk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3clmiaqme.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ohyrhwfh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zorsltvm.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ltqkgqpq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qiglnons.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ekdifazh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ouxtgkul.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3uifslczr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3uypuibwr.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3anloojpd.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fqzccoda.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3tvcjavea.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yxrxtqhb.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3grjtqceo.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3kenqlrht.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3vmvcjbgy.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ebwrtile.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3swaegczr.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3cxjufzal.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nsjuzedv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3szzvammf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3stzlhjmd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3dbyxkkzl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ivymcwpw.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nlnxjiep.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3twtpkayo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3cqgxhles.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jheiyemm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wtvnlmqz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vgnbhrgg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ocdgikua.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktowwrcv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zfanugqh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3ltewjyop.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3uepwgncd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqexsmdo.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3krafulfx.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3lbztgkty.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3nfjywmsi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3liegctqg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zjtkehef.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qtibqhrw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3dquflppk.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3jjwdazcl.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3iargsgpl.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3otospuzo.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3pacywfkx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3oeikoswt.html


<!-- 参考信息 -->