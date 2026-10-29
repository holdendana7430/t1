代发 wailian999

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gwyqjszee.sHtML

throw new RuntimeException("失败", 500);
来源：http://3g.hesvh.cn/Article/details/gnrihcmiv.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gpmsoyhni.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.blog.hesvh.cn/Article/details/gxvthbluy.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gxdfomxud.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.hesvh.cn/Article/details/gxcwyztye.sHtML

[U74] PHP：读取环境变量
来源：http://baike.hesvh.cn/Article/details/gijdoscch.sHtML

getenv("APP_ENV") ?: "production"
来源：http://mobile.fehbvm.com/Article/details/gqskimwbu.sHtML

[U75] PHP：依赖注入
来源：http://blog.fehbvm.com/Article/details/gjjdgrwio.sHtML

composer require psr/container
来源：http://read.share.fehbvm.com/Article/details/gqkjwskjb.sHtML

[U76] PHP：简单路由
来源：http://baike.fehbvm.com/Article/details/gwbmlhnwy.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.zdbjq.cn/Article/details/gqbrimfbg.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.fehbvm.com/Article/details/gdyebwome.sHtML

composer require twig/twig
来源：http://blog.zdbjq.cn/Article/details/gvegeiypf.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gqojiymfq.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gmcdlvnhz.sHtML

[U79] PHP：静态分析
来源：http://m.share.fehbvm.com/Article/details/gqktttgim.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gvgjtruqe.sHtML

[U80] PHP：代码规范修复
来源：http://baike.hesvh.cn/Article/details/ggmjpjimi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gglqtbavf.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gglmnyvxb.sHtML

npm init -y;  npm i express
来源：http://baike.zdbjq.cn/Article/details/gxwxxmyku.sHtML

[U82] JS：package.json 脚本
来源：http://blog.fehbvm.com/Article/details/gyjifdrrs.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.hesvh.cn/Article/details/ggcmlhhbj.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gaincgntf.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/galzenopr.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gvohcdrcy.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gmohbqugl.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/grqrheryw.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gnmtitcii.sHtML

[U86] JS：空值合并
来源：http://baike.hesvh.cn/Article/details/giuijbkwr.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gzknttjpg.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gjbdzqycp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.hesvh.cn/Article/details/gkxehiuap.sHtML

[U88] JS：对象展开合并
来源：http://read.share.zdbjq.cn/Article/details/gfandaoxo.sHtML

{ ...a, ...b }
来源：http://baike.hesvh.cn/Article/details/gslulqytp.sHtML

[U89] JS：数组去重
来源：http://blog.zdbjq.cn/Article/details/gbjelefxb.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gpdrykbbo.sHtML

[U90] JS：数字数组排序
来源：http://www.blog.hesvh.cn/Article/details/gcknfkhrn.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gjhbcxewr.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/gfhqujmin.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gjkuumylb.sHtML

[U92] JS：深拷贝
来源：http://www.share.zdbjq.cn/Article/details/givggykvo.sHtML

structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gypghxkuv.sHtML

[U93] JS：模板字符串
来源：http://m.share.zdbjq.cn/Article/details/gngdimrri.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gzijlvjqq.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/grhyqfclm.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gxiigvxcg.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gyxoryvlj.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gvshqnmmj.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gmdtzscfu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gnqdhmunr.sHtML

[U97] JS：并发请求
来源：http://mobile.zdbjq.cn/Article/details/gvmfggwqm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gjmevhrfx.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/gyuodjuld.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.fehbvm.com/Article/details/glkxwkctk.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gokifdvhq.sHtML

el.addEventListener("click", e => {})
来源：http://baike.hesvh.cn/Article/details/gniwquzmm.sHtML

[U100] JS：DOM 查询
来源：http://baike.zdbjq.cn/Article/details/ggsmgacbn.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gsejjepnd.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gmquukbre.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gwjihfxgr.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gmlvusqip.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gseuccyth.sHtML

[U103] JS：定时器
来源：http://www.m.share.zdbjq.cn/Article/details/gzeglpjqy.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gflanpsam.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/grbtkfgka.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gjvtxwsgn.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gepzicjwj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.fehbvm.com/Article/details/gijxmpfdg.sHtML

[U106] JS：日期格式化
来源：http://read.share.fehbvm.com/Article/details/givbpqqbm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.fehbvm.com/Article/details/gdojpdlry.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gnrvaozef.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.hesvh.cn/Article/details/gopfqutpt.sHtML

[U108] JS：随机整数
来源：http://m.share.zdbjq.cn/Article/details/gflhsomaq.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.zdbjq.cn/Article/details/ghjkoryqg.sHtML

[U109] JS：数组分组
来源：http://read.share.hesvh.cn/Article/details/gvjuoexdb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gpurpqnmc.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gijnrwhsp.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/gngghpiqw.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gspgztmeu.sHtML

new Map(Object.entries(obj))
来源：http://read.share.zdbjq.cn/Article/details/ghcctauob.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gpkjhvowx.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gpmhohndi.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gsfqnchdu.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/guaminmcp.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.fehbvm.com/Article/details/gjllonjww.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/gxlkvuwoc.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/ggokivrun.sHtML

crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gdzrctlfi.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gzaxpanht.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.fehbvm.com/Article/details/gwuxnavqt.sHtML

[U117] JS：单元测试
来源：http://baike.zdbjq.cn/Article/details/gsbsippna.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.hesvh.cn/Article/details/gscdfhnbl.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gwpnbxyeo.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gwuaomtpl.sHtML

[U119] JS：生产构建
来源：http://blog.hesvh.cn/Article/details/gipcobpuk.sHtML

npx vite build
来源：http://www.m.share.hesvh.cn/Article/details/gvnmfzohg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.blog.zdbjq.cn/Article/details/gsepysnvy.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gzzysmopn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsgmduyxs.sHtML

统计汇总
来源：http://read.share.fehbvm.com/Article/details/gzcadvjwh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glccerbfc.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gdyodlzdw.sHtML

Python ......... 252
来源：http://blog.zdbjq.cn/Article/details/gxsqtxhwy.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gcygbxjvi.sHtML

JavaScript ..... 252
来源：http://baike.fehbvm.com/Article/details/gofboqfoh.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gpilexfor.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/guaqyqdxi.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gnghqixrr.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gvltplmhq.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gvfrxmgkp.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gikpcuitn.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gsnwrkwao.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/gsmlsaufd.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/gxeqxmhag.sHtML

Kotlin ......... 15
来源：http://baike.hesvh.cn/Article/details/gdezjzhad.sHtML

Swift .......... 15
来源：http://mobile.zdbjq.cn/Article/details/gxdbvxfnf.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/gejrrngtu.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/gupahynmq.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/gfsfaywkw.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/ghwfefjwz.sHtML

合计 ........... 2106 条
来源：http://m.share.zdbjq.cn/Article/details/goxpwfgub.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gesfjqxjr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gtaiprfff.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gumdqzoem.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gbwpktmeb.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.fehbvm.com/Article/details/gtlmdrnol.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gvutgmddx.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gtyynqqgs.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/grczjpvjy.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.hesvh.cn/Article/details/gkimzuplo.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gwtauatgi.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gidsvssff.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gcwxceqah.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gxulgzqgr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gfogprrhl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.fehbvm.com/Article/details/gilpomcth.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.zdbjq.cn/Article/details/gghzmhyeu.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gvzroipid.sHtML

Q SQL 专题                              90
来源：http://baike.zdbjq.cn/Article/details/gahcpylng.sHtML

R Bash 专题                             80
来源：http://www.m.share.zdbjq.cn/Article/details/gxjuxjtgv.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gcqjwiiff.sHtML

T 其他语言补充                          60
来源：http://www.blog.zdbjq.cn/Article/details/gxkxevpsi.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gqeuvdovd.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/glqlqqdfb.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gjwkbokln.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/ggqqwpitj.sHtML

使用提醒
来源：http://blog.hesvh.cn/Article/details/giqhgttgj.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gtkopbjia.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/ghqfdnhzf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.zdbjq.cn/Article/details/glkjgtrax.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.zdbjq.cn/Article/details/glrhkhtfr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.hesvh.cn/Article/details/ghngdphax.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.zdbjq.cn/Article/details/gyknoydmz.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gikvxitra.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/goqvhustj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.zdbjq.cn/Article/details/gcnuqxpfd.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gkbbgvqxe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gabtzmqux.sHtML

【收录内容】
来源：http://mobile.hesvh.cn/Article/details/gzlyatbic.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gbdvqvjir.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.zdbjq.cn/Article/details/gyzacadws.sHtML

SQL · Bash · C · C++
来源：http://blog.fehbvm.com/Article/details/ghwpkqhsy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gplsjfueq.sHtML

【使用说明】
来源：http://baike.zdbjq.cn/Article/details/gegkioape.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/ghwviasnz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.zdbjq.cn/Article/details/gbkcsfhol.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/gwxiohsap.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/gyxjgvjvb.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.zdbjq.cn/Article/details/geitpdwdi.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gkkdpzwuo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.fehbvm.com/Article/details/gwmoyrudq.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gbltrdgeq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.zdbjq.cn/Article/details/glkugradg.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/geyuolcpd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gwfqwndqp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.fehbvm.com/Article/details/gykgliugw.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/gbfwdgdld.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/geuuwepes.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gbegsbfao.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/gpivhxlzh.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gmppassjy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gdbrzbkfb.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gyutfzhey.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glbkvpfvb.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.zdbjq.cn/Article/details/gmtullidk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbzwyrpbi.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gtapjojak.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gwwsybhrz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gqlndzmiu.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gbwjdhfnm.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gpjhmdqlp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gfsmnryda.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gkiursogq.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gobkfmknk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gwzsfeggn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://wap.hesvh.cn/Article/details/gngzyucqx.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gfgodzduw.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.hesvh.cn/Article/details/giqectmip.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/giaiplabi.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gtgpinugs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/grgbafyhm.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/gztglhzes.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsxvkvwqz.sHtML

A. 基础语法与类型
来源：http://www.m.share.hesvh.cn/Article/details/gmofhrsog.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxrsypegy.sHtML

[A01] Hello World
来源：http://baike.fehbvm.com/Article/details/gatvkipwf.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.hesvh.cn/Article/details/gscuhoxru.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/gjnigyscj.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gattaozce.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.fehbvm.com/Article/details/gxvphduck.sHtML

Java: System.out.println("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/geyxdhqcz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/ghhmseuqq.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.fehbvm.com/Article/details/guckawftp.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.fehbvm.com/Article/details/gxamwfwpi.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gsqhsdprf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/gbwuirwfr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/geqjegdix.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gnlmdxfqv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/guzvuucai.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.zdbjq.cn/Article/details/gkvyejetr.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.zdbjq.cn/Article/details/gxgdvjoxp.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.zdbjq.cn/Article/details/gorkwjyig.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://blog.hesvh.cn/Article/details/gazufufow.sHtML

[A03] 常量定义
来源：http://mobile.hesvh.cn/Article/details/gjqfetqcu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gdjxsphgg.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gttfhmkbi.sHtML

JS:   const PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gehogbyst.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/ggscheodb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gpbkriktz.sHtML

Go:   const PI = 3.14159
来源：http://www.share.zdbjq.cn/Article/details/gumlmexfo.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gpmwilkvs.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gqkeqyzdk.sHtML

[A04] 判断变量类型
来源：http://wap.zdbjq.cn/Article/details/gbrlpzhgp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.hesvh.cn/Article/details/gxzynxfli.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.zdbjq.cn/Article/details/gncfbjqdv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://blog.hesvh.cn/Article/details/gvcpyaust.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.hesvh.cn/Article/details/gyqblvusz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.hesvh.cn/Article/details/giivbvjoi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/glavniqvw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.hesvh.cn/Article/details/gdpyiufyl.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/gldiziwao.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/gjxkckcng.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gsicsukin.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/gwxxdghwl.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.hesvh.cn/Article/details/geayzwqao.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gzpqpbtpf.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gxidqtvig.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gwydvvdmg.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gydogytfq.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.hesvh.cn/Article/details/gsytpbawt.sHtML

[A06] 字符串转数字
来源：http://m.share.hesvh.cn/Article/details/gzuwatjtg.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.zdbjq.cn/Article/details/ghbcbyihi.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/gaouhphse.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.zdbjq.cn/Article/details/gqaqnynvk.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gapwcuotn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gwhsjxfhx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://m.share.hesvh.cn/Article/details/gfzixjrvo.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.m.share.zdbjq.cn/Article/details/gcfcatsxg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.hesvh.cn/Article/details/gahzyfsgn.sHtML

[A07] 数字转字符串
来源：http://3g.hesvh.cn/Article/details/ghpmbopvq.sHtML

Py:   str(42)
来源：http://wap.zdbjq.cn/Article/details/gjnybhzfh.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.blog.hesvh.cn/Article/details/gdswiqtyz.sHtML

JS:   String(42); (42).toString()
来源：http://3g.hesvh.cn/Article/details/gdkxjnzwh.sHtML

TS:   String(42)
来源：http://3g.fehbvm.com/Article/details/gduzbfmxh.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.zdbjq.cn/Article/details/gnckjcksb.sHtML

Go:   strconv.Itoa(42)
来源：http://blog.hesvh.cn/Article/details/gkfklkeju.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/ggqwlzkfh.sHtML

C#:   42.ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gffsrjbap.sHtML

[A08] 取整与四舍五入
来源：http://blog.zdbjq.cn/Article/details/gipgzcuet.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gyrxfverr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.hesvh.cn/Article/details/glsaexiup.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gxhtafvck.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.m.share.hesvh.cn/Article/details/gsqrpwkyh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gwugqplxi.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gcffwyghu.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://m.share.fehbvm.com/Article/details/gpdqfqsrd.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gxfzleaul.sHtML

[A09] 绝对值与最大最小值
来源：http://blog.hesvh.cn/Article/details/gvktedxdd.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gxlmdpzsx.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gwbzdrzzg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gnwweouch.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gqmqeybed.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/ghbzmyvbd.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.zdbjq.cn/Article/details/gpwgcjdmb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.m.share.zdbjq.cn/Article/details/gxdurzowh.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gfythesjq.sHtML

[A10] 生成随机数
来源：http://baike.fehbvm.com/Article/details/gspaylmkp.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.hesvh.cn/Article/details/gsunyntsj.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.zdbjq.cn/Article/details/gmqhdviep.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gibzgsviz.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gkmcwpnrd.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fehbvm.com/Article/details/ghzimlqbh.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.fehbvm.com/Article/details/glnchyiop.sHtML

Ruby: rand(1..100)
来源：http://read.share.zdbjq.cn/Article/details/gqkpsudiq.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/gjbxwxpkw.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/gxqxmrtgm.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.hesvh.cn/Article/details/gbxtlxrmx.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gcmzsbgap.sHtML


<!-- 参考信息 -->