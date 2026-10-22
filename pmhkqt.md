代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2pjhbkjqv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2mxqshvhq.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2vgmuyszk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ehucwhzl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ooxhdukp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2jvldnhfs.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ofcufwfu.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2wgtchaak.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2gomkbglo.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2kcyapjbk.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ibjlpxoe.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2grzyqemb.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2hcimiobw.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2comylolp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2juuicjol.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2oyqzueav.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2zlimqavq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2mhtmcixe.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2xhhdnthw.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2xdewfcmu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2bkeeopyc.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2qvafgxgj.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ktwfwxar.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2bssjbnvn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2dfrkgvlb.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2jetxarfr.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2zazjcipx.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2djrdqakp.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2trkjsfwc.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mziwuyad.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2scniqwcr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2tpighxvu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2lhyggjag.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2endedogj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2mrodrppf.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2zeatadho.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2zglfegpq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2jkvhmfkv.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2emujtaky.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2vzrixqgb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ctfqosgm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sypuqjoi.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2eibtyqsz.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mhvgkeec.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wppwoezf.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2jhtuudrr.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bpuzbhad.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2klgevdfz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wwwtzfaa.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2cyqdfkbc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rnlrybvp.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2rhqjczku.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2iupcsmzz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2diqpehkd.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2lfllajug.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pimcfaud.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ymxfqxii.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2heyskqrx.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kistbnvt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xpzizpzd.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ifncvyig.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2elsqsujt.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2tzhmxvqm.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2pmkmlxmf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ssudsolp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2amfhguxd.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2jwfuucru.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2vfpphgkt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2ndrnfhfx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gnjhoglg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2jgrmrouf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dalnzjii.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2jiltixwu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2urbyswom.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vzwsfmxd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2zubeqrnb.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ldlvschk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2djnqiksc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2xolutrpl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2bygirnch.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2yxhgufsh.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2dywidnvg.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2feqmodbp.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2eihlqwyh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mfzcqrwc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2siifwyiw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2yecfxtkv.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ajsgvphl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2tjotatip.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pgthtcdj.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2fvrfyzzr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2riwlgptg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2tjjinatt.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2sfuzoznz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2oewosrjr.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2laeozeod.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2iailncih.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2bvnixbjw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2rltrmrwz.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2selazxrf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2jplklvxw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2dmjojezb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2suyygsri.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2trvdfnws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pomwmklm.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qfekpvfd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rttuavhi.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2vedbjujx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2rkyjrbkr.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2bswcvxej.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xluozuid.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2fgbpyjbk.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2kjbywwvp.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2aairgmzy.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ffzjrqbv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2tfawvvzg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ujghfjqm.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2kbmuzqer.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2mmdetszk.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2anjcyptk.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vmodyfaq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ynmunxew.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2nvabxloz.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2kgnndjch.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2lojqwznn.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xwojhvdu.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2cibhpfkw.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2jbojbeia.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rixzxofr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2omdwqgnh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2wxxmosxe.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2oyyosjju.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2jglvittz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2liznnzoc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kohqmoeo.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gknigujv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kigrgwpe.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2bdxahtlz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2clkyxvhk.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2iwxnptql.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lsmmovrn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2tkihihsy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2cqvkbxwr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qxvysstf.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2hneknord.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2njiloohj.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2rjvqylke.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2qbtekfvl.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2uzzugyci.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tffrfshy.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2xgbtnpsc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aicagggt.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2pcqaxhww.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ntnekzmh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2lilaisqz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2nvyptxrf.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2hujucimc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2sawrioib.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2cxxfizck.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2vhuvlbhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwqmdovl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2xmcrqlmz.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2mkotvvkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tiaquqid.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2rvencygq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2poxhqdrn.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2owhueufu.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2nigcyrgu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2jqzzlxud.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2rjneeypw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2hhwmdvus.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2celahuns.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2fbpiwnlt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2uwheaacj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2pumpcvec.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2yvfqmkgy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2bcgghspp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2enogbhgc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2xwdigyjb.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2pyfrxjkh.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2cshggedf.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2ccdqzxlc.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2cwpigyiz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2pgxzjdap.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kxcldjpa.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2vasywttg.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pxhszikh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hguhckfd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dnxbmoxz.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jkdncidb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2vvzqsqil.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2goxjdjnf.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iebmrlxb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vhpyevvv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qipbzxjj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hfxgtjol.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xcwigfnq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rvmhpreg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gnenjskq.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ctedpsti.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2azcribgd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2srzwilmo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2bgqsykup.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2arkbzuhp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wyenucow.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wzocjsem.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2opedhjje.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cvmbdjjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdqidjhq.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2xsauwdos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljnhtlun.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2waztpgap.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2hgqwyvpg.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2aadozldm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2cazyhgae.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2cmdrjmpy.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jtmitkjf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2uvwsbnuk.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2xkrwwzpk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kzezznrc.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2vfeztcmx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2tafebmvf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2srsjpjdl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2azrcytfx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2zbpvpwiv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cshrfhzc.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2agosgmyb.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2yremcdno.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tachlriy.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2lreieweo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2culfqbcx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hfuywmme.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2sfvmxhhk.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tbpcastf.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gwmmqzwo.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2uyyvtjts.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2vngkmdcm.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gqjezpjh.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2pazuuqdr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ewizhvml.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2wzcpozpb.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nlvsrkeg.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vnvrqevo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2dafkphpb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2cqjornhw.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2fmirjtdk.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2qfswztys.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2vvmzohtb.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2mbftdesk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2afsbeick.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wqbxrzln.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mzriorjy.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2khvjiynd.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jbjbxnkk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uxoatbnz.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2exrjpaqn.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2vblqhjbj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2coezmalw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2pdpudzkf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ijpkbhtl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2iyljvvvm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2upwzaafh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ulpmzwls.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2tuamcpnw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2uqadzldl.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ogbnvbdc.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2utaawryh.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2apidnivs.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ncdejsuh.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cgkahblu.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ylaowhqf.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2gitjmxqr.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2imhgoiaf.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2dvxqimtd.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2jlmyfcvx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2esknikkj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2eujmogur.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pnccvdot.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2mutbwado.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ordkrlrm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ezykxpyo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2lplmjyre.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2sypsfcms.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2valzjxtw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jzpauaoc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2apqmvchz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2auvgobqq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ecuubvpk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cnvbzrvd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2qeojsgey.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2ygixrhvs.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nuutrdhe.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2elzunoto.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2kxkzsggp.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2hcoxpoqi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2nkjabzav.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ffcmklgk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wlbqnoti.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2xqdoojsc.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2rmviqmac.html


<!-- 参考信息 -->