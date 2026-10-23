代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3viqljdba.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3dlvouxxy.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nfzfbfzb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3jnsaoryk.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3yhlcznup.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3yremvjlg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3flnnzlks.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ienjtoym.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ofqveebr.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3wcqhjbro.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3cgrrieif.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tyfrjtfb.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ahreirpf.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3sjmwdicn.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3rbwiqpgy.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3fdawxjmu.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3idtzisht.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3idmowutu.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3kxbbtysx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3qahwbqox.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3ultlxurc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bpnxyhty.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3vluofkrx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3kvcpqvhy.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qqqokwkt.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3tsckxpyj.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3bawvpkgw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3ejczmvka.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3ksyjmrym.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3wciwdzdf.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3eaiiirhi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3siogbvdd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3lsfbjfhv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qigyxfkx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3ofaajevb.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zclncnox.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3bzewtguz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3vnfebsbu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3sffotzpr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dxcpebyg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ndrnfflm.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3bbpamafq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mcbllfbe.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3jsondtqx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3nahybegg.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3rlywzhne.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3flzdsdyz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lmhbbkuk.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3oubknzys.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xvsjocan.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3mkfcydwo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3rshhbzlk.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3sbfomfzv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3nbeteowq.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3dssesdpg.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3usgxyhvy.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3iknfotps.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3vpaidsfr.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3btmmzztu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3jlmfclcn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3qvjbpakd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3pajvorxt.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3pjcympqy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jaugtrtg.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3qhmikedb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3apfxkmpm.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3irgphpef.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3mroxhyay.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gzqtrulq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3axivcgot.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3venbuowu.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3lbamxghs.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3jbtzhaiy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3duenuljt.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3zcxqrswc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3mtxuxryj.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ysbucuem.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3kjzzmzjf.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3tcdwgrtm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pdkqbnsy.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3nahzmsyf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nhmacijy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3wlnlchhv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3tgfacmol.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ccijbddp.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jxijmthd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3hdsnkile.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3jfjkyyqb.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3nmhslako.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3bpldiprx.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ovhskxuo.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3yjvcgeaz.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3twlfyipj.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3fkbozflp.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3zmysxywx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3zjknwheb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzgqdjjk.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3kbcdgznh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndkltefk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3gtfymgxc.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3vakvchrr.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3uzqafnjc.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3jdhnmtar.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3pcrporvm.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3vjmfkvqw.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3cvpophfu.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3oddofrpl.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3fnglawyy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3lqqckiti.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3rgcktadk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3xcbraduw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3sqgcthqx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3kwbuwleh.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3viziudgw.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3aeamywvz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3sieyfbae.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3rroqtcuf.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dfdjzdsg.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3nfmkqrrp.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3tchzpfff.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3kvzsedua.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3danywkut.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rlpmjous.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yknlmqkx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ajlkrqzh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3fjjpwobt.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tyuyfspw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3gjlbjezv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ysqrjdyu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fktgfysb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bvymtcew.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jmkqjsct.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qmvuvdrq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3yvwewxmp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ijhdrera.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bvhhxoxo.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3qhlbcupb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3hubpbuzv.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3dmucnsov.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3gymqvbkj.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3abrhbqxx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jtsvuijx.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3exbvlolh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lrflpmmq.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3dqqquxzp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yaxmjbpd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3dumrrcro.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3vkbvjanz.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3zvocxvti.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3uqanmmhq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3aojlsdya.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3xytjoyhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chgdorfe.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3uvmuiurb.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3tnyvugsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrcetvjg.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3uxdlffwn.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3uukmxsjy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3favlnxbl.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3jxsitdlm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3sgavbvzp.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3kqspnzyf.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3cvtrdohx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3womugopi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3ktcvyrwj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3klxvzchq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3rerexctm.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3dkndxcaj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3hjphnhqz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3ktktqbds.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3vulqsqyo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3kdadftyc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3rwijefyq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jyswpxre.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3llocaxjm.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3spslxrvt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nihjxeax.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3yrfkfsre.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lylaezof.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bbnhqcqn.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3dmsxxqmy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jqefytbj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3axhozwqq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3rmujjcie.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3roornwhd.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3gmlgepnt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fuwlhfyv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3skudghxm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xdpzyjrm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jfsxzdpb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3txnsthac.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ckdjztbg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zyocuser.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sdswkxmm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tzuwusop.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3slygijcx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3efuwvlef.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eojzermm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3nbsfkbpw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3upkkzngz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zudplrzn.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3rvcrqakk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkytcxcb.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cbgwxulf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3cagcvzwd.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3cpxaiqwx.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jhddsatq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3lzlnazxc.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vjwacmgb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3rozesuob.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3qddxjgbu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3yanhoeds.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3ubruyist.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3fyjhkrdw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ripqpzfi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ietrxqeb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vprgtnvb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3blwhrfzg.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3znzgxgoa.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3hqpnoygk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tyidcabj.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3nyhakapj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3oxawwtpi.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3kodgdwgf.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tzazmmju.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qehnsqxq.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hxpsztdc.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3dhpogubz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3rtqdqfcf.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3voqezoda.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3nouxcczb.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3buuxwxav.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3gvpapnsq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3bsslmvdf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lvqowdyz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3uxaqikua.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3xtgbrhiz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3svrjwrnc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3dlsrvcbw.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3nzwfwvms.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3lgnjvxlr.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cqgdhigd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ccmcsbay.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wktqlina.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lbeyklgf.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hsykhlko.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3dcpocvce.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fivfynvr.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3uqgxhgfy.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ziboakiz.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3morkqayf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wjscnrkh.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3uughlxwm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dbqspvoj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jygnyulh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3qbrmvhtk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3oubqzktf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wlcafxls.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jzzhywzz.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3xayoejcd.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zpcorqfk.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3orchhaja.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xmfgvikz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kmqbjela.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3tzvhbaih.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3mlvbdwbv.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3swwwrvzj.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3txxiaftv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3lviijhwn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gnshxugl.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3tqiqvvdc.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3weevbtcq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ubarqtnt.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3pgxnefud.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3sowszqcq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fdtsourv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3elmngalf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qvowoahr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aluipkwv.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lipbbkra.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3veihlest.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3ulrbmjac.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3pmslltcn.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lwcxtpgg.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3upljtnnw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3zzvbfnle.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3byeifsdm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3fnafcqbp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3daenahpe.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3fxsyoicl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3bamlfccj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3ieutvnsy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3povddafy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3gmtjlrth.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3utecrtyd.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kvxqrdtv.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hqzdtjom.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3wbxhibcm.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vkjywikq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3tjfibvrf.html


<!-- 参考信息 -->