代发 wailian999

[U71] PHP：抛出异常
来源：http://mobile.hesvh.cn/Article/details/gvavbfwzn.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.zdbjq.cn/Article/details/gbitmqtvm.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gxistubwj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.fehbvm.com/Article/details/gpkwhhbny.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.zdbjq.cn/Article/details/gszftjgbn.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gcmltrikg.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gnfuzcmfa.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gvcaybele.sHtML

[U75] PHP：依赖注入
来源：http://wap.fehbvm.com/Article/details/grjwbatut.sHtML

composer require psr/container
来源：http://blog.zdbjq.cn/Article/details/gqqnhpjkg.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gutfntebh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/gjdavknvp.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gtwvsaivn.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/grjklbvvu.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gyodciwhp.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.hesvh.cn/Article/details/gxkdotsmr.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gqprveecr.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gtxfjjuox.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.fehbvm.com/Article/details/gxwepzrjy.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gfkurodcb.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/grlzbzqgm.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gfkobinqx.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/guqaalzyv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://blog.hesvh.cn/Article/details/gnvvkkuar.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.hesvh.cn/Article/details/gphogprmb.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gfjlefbhp.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.zdbjq.cn/Article/details/gafkobdsn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gzcerwvvi.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gbryhewet.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gknzamsxk.sHtML

[U86] JS：空值合并
来源：http://m.share.zdbjq.cn/Article/details/gxcukhjci.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/grwfcycnv.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gubuwjsai.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.m.share.zdbjq.cn/Article/details/gqjvbkudg.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.hesvh.cn/Article/details/gdhackxrd.sHtML

{ ...a, ...b }
来源：http://read.share.hesvh.cn/Article/details/gwflvmjlv.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gwzqivhfz.sHtML

[...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/grunbunga.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/guphxzest.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gpauxbcaw.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkpeypdpd.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gncoehocv.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gxfpxhshi.sHtML

structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gmbjlplua.sHtML

[U93] JS：模板字符串
来源：http://3g.zdbjq.cn/Article/details/gqsyhasea.sHtML

`共 ${n} 条`
来源：http://wap.fehbvm.com/Article/details/gbbdsrsdb.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gnjpnydku.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/gdkkboauf.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/ggyjvvdht.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gmonbfzej.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.hesvh.cn/Article/details/godtsjtfp.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gvlqqfxjb.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gfzgesofq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gqxgzcqfj.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/gswaqivze.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gqjzcehqm.sHtML

[U99] JS：事件监听
来源：http://mobile.fehbvm.com/Article/details/gwwgdmfdf.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gjvtvdabs.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gjlixqykv.sHtML

document.querySelector(".item")
来源：http://read.share.hesvh.cn/Article/details/gqhtyvkwp.sHtML

[U101] JS：classList 操作
来源：http://3g.hesvh.cn/Article/details/gcmmncima.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gcgporxif.sHtML

[U102] JS：本地存储
来源：http://www.m.share.fehbvm.com/Article/details/gzxrcjjvu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.zdbjq.cn/Article/details/gograhfqc.sHtML

[U103] JS：定时器
来源：http://mobile.hesvh.cn/Article/details/ghldebbjb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.zdbjq.cn/Article/details/gsslnovwx.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/gvypgghfu.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/glvqqpyza.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gqcqhazix.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gdtriilxp.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gqnhxynpo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gfvikynor.sHtML

[U107] JS：数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gizgnzndp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gppkqoeub.sHtML

[U108] JS：随机整数
来源：http://www.blog.fehbvm.com/Article/details/gpoqyxgyu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://mobile.zdbjq.cn/Article/details/girhgrorn.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gelumbbre.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gopzxolqb.sHtML

[U110] JS：数组分块
来源：http://baike.hesvh.cn/Article/details/gjovdtvue.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.fehbvm.com/Article/details/givmmpkoi.sHtML

[U111] JS：对象转 Map
来源：http://3g.zdbjq.cn/Article/details/gbvrhyjzg.sHtML

new Map(Object.entries(obj))
来源：http://mobile.zdbjq.cn/Article/details/gvohcjsou.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gfriqdsyl.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gmyxyllin.sHtML

[U113] JS：正则替换全部
来源：http://blog.hesvh.cn/Article/details/gyeryxnjs.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gshkioxzh.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gimqtyula.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gsgvboayo.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/glwyasbfp.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/gpsojvegk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gccrzaxzs.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwnkxpehx.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gfjsmlxnd.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/gizxrbwem.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/goddzsiwi.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gwxzwzxrk.sHtML

[U119] JS：生产构建
来源：http://wap.hesvh.cn/Article/details/gxygiwrrp.sHtML

npx vite build
来源：http://www.blog.fehbvm.com/Article/details/grxcgkvav.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://mobile.zdbjq.cn/Article/details/gcbqwneoy.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.fehbvm.com/Article/details/gnowfgcsp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnsmrrfnb.sHtML

统计汇总
来源：http://blog.hesvh.cn/Article/details/gowmkmvrh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glaizfgwm.sHtML

按语言统计（条）：
来源：http://blog.hesvh.cn/Article/details/gyvuqnogh.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gnagyvtdm.sHtML

PHP ............ 252
来源：http://m.share.fehbvm.com/Article/details/gncjzefic.sHtML

JavaScript ..... 252
来源：http://read.share.zdbjq.cn/Article/details/gyhmjdspj.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gylrsjdcx.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/ghddrdtfl.sHtML

Go ............. 212
来源：http://www.share.hesvh.cn/Article/details/gnczwygln.sHtML

Ruby ........... 212
来源：http://blog.zdbjq.cn/Article/details/gxvwzlsrc.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/glldodyod.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gazccoyfl.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gpwnkarsg.sHtML

SQL ............ 90
来源：http://www.m.share.hesvh.cn/Article/details/gkgrevdst.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gpgmunurn.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gaqbjslov.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gunallnra.sHtML

Lua ............ 10
来源：http://read.share.hesvh.cn/Article/details/gsvhlbxjy.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gbtngsagl.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gmcowhqnc.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gvfbkalcg.sHtML

合计 ........... 2106 条
来源：http://www.share.fehbvm.com/Article/details/gufsbotye.sHtML

按章节统计：
来源：http://3g.zdbjq.cn/Article/details/gzldqxhte.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gyzzdsxzg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gkehzchaz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/glthtnhdd.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gijawoglj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gteyxseif.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gcjpkqgha.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gkiqgjtyi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/goqghhcqr.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gyylotyja.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gffkdsgii.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gbftlrtto.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gwzfwitzz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gzsbduiyx.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.hesvh.cn/Article/details/gxyigcgfq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.zdbjq.cn/Article/details/gbbvuuwzm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gqsegzngq.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/guiarzuzz.sHtML

R Bash 专题                             80
来源：http://3g.fehbvm.com/Article/details/gxsycdglg.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gprrccqgf.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gkqinydjo.sHtML

U 高频实用片段                         120
来源：http://www.blog.zdbjq.cn/Article/details/gqnchqtjp.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gpbbzazft.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/gvqfymdha.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gzceiaqyx.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/gliqrqshr.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gvekmeurj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.fehbvm.com/Article/details/grvenmyjq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gaqqbcyry.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.fehbvm.com/Article/details/glisdtdbk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/giyohwyxq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.zdbjq.cn/Article/details/gorbejhzp.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/giylvwtpz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmpchpias.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/gkakjuibb.sHtML

Common Programming Examples Cheat Book
来源：http://m.share.hesvh.cn/Article/details/gdvnogntm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gujazkczo.sHtML

【收录内容】
来源：http://blog.fehbvm.com/Article/details/gwblkgcdj.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.hesvh.cn/Article/details/gtwieorgi.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/gixcsffva.sHtML

SQL · Bash · C · C++
来源：http://baike.hesvh.cn/Article/details/gvtbvqwel.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://mobile.hesvh.cn/Article/details/gvtfgvjhh.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/ggjtfydpu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.hesvh.cn/Article/details/ggyoehipn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.hesvh.cn/Article/details/gzjsfozbr.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gwqegjlce.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.blog.zdbjq.cn/Article/details/gztgvgmck.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/gwqrwmzue.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/ghpqvwcnj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.m.share.fehbvm.com/Article/details/ghdtmjege.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/grktvzdzq.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/gvwpqwcoy.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gdhsgtnly.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gyouhpchv.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/grlhzneyr.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gbnnlbrfe.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/glgjjqjtl.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gnhpakhkm.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gmlblqokb.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gfbeiptux.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/gllacemhy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gwpdydvrd.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.hesvh.cn/Article/details/gaxefcbxe.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gisyupbar.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.fehbvm.com/Article/details/godtnfwvs.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gbugkacfb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gwrckjroz.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gxfozpolx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gjcnuwzgn.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gowsrrwcm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gvkeaswys.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gvypagklh.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gaysxtjxu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gdjtxnhby.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.hesvh.cn/Article/details/gxqnzoyjm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/galkcmbjo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gsemsuffm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gjnqnjutf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://read.share.zdbjq.cn/Article/details/gcdpnpvqy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/ggfxjfkup.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.hesvh.cn/Article/details/gaucsxszn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gamtrtpij.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/gjkgvgfmn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggpjiabih.sHtML

[A01] Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gcljwiwwz.sHtML

Py:   print("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/ghqnfdlhe.sHtML

PHP:  echo "Hello, World!";
来源：http://www.blog.hesvh.cn/Article/details/gevtvylwi.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gvtdskxnh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.hesvh.cn/Article/details/ggxrroenz.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gejapahvd.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.hesvh.cn/Article/details/gdhzvkzsy.sHtML

Ruby: puts "Hello, World!"
来源：http://3g.hesvh.cn/Article/details/guntvaetw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/gspexnewl.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/gyjroloqm.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/guksaoocj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/gkpqijjfh.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://blog.zdbjq.cn/Article/details/gpsvzvdtd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gzcguloqp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gcmqyvvgy.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.hesvh.cn/Article/details/ginoyzkik.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gnbpnbtgo.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gesachznb.sHtML

[A03] 常量定义
来源：http://read.share.fehbvm.com/Article/details/grsavdqfc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gxynmcasc.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gwzearyrs.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gpakhvuwy.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gfucmtpgp.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gbfhdkyvm.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gjgivkflw.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.zdbjq.cn/Article/details/gqmxskzfa.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gozfuxsva.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/ggoonaqqg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.zdbjq.cn/Article/details/gxahkyepa.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gyhxwwuqh.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gadisbxuo.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/ggwkuryjt.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gpsvpnand.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.zdbjq.cn/Article/details/gqsumxqcx.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/ggrjlckmt.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.zdbjq.cn/Article/details/gozsvhbzq.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/gmutscnmw.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gdtkguszn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/gvnmpfkcg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gdqupvqpb.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gndfabbdy.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gtnxkwfjg.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/govwmwdlw.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gjnkuopjh.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gpdqoqsgs.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gdzuhgwuv.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.hesvh.cn/Article/details/gdchmbqqx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.fehbvm.com/Article/details/goikrvhhq.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://wap.hesvh.cn/Article/details/gplyljrkx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.fehbvm.com/Article/details/gjahscvnu.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://m.share.fehbvm.com/Article/details/grthqszzj.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gwxvopfqm.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://baike.hesvh.cn/Article/details/gjqwtncrh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.share.fehbvm.com/Article/details/gydxadmjm.sHtML

[A07] 数字转字符串
来源：http://blog.fehbvm.com/Article/details/gucftwhmz.sHtML

Py:   str(42)
来源：http://baike.zdbjq.cn/Article/details/grqcellvi.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.fehbvm.com/Article/details/gnmhogtpa.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fehbvm.com/Article/details/gaowfuzeb.sHtML

TS:   String(42)
来源：http://blog.hesvh.cn/Article/details/guwrbhivj.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/goqwplyap.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gxzwnzlbr.sHtML

Ruby: 42.to_s
来源：http://www.m.share.fehbvm.com/Article/details/gqyuilcxq.sHtML

C#:   42.ToString()
来源：http://www.share.hesvh.cn/Article/details/grnkteykj.sHtML

[A08] 取整与四舍五入
来源：http://3g.hesvh.cn/Article/details/giljcewwk.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gezqlqusz.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.hesvh.cn/Article/details/griaddjin.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gfiobxvsm.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.fehbvm.com/Article/details/gucapabfh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/ggjpbqzej.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gdakldvzw.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.fehbvm.com/Article/details/glholnhoj.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gfixhlpgs.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/grogfvxbe.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gsapmxtar.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gvedsmmmp.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://3g.hesvh.cn/Article/details/gakjvqgtn.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://3g.fehbvm.com/Article/details/gvoanswhs.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/gazfhhzbz.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.blog.fehbvm.com/Article/details/ggpdlnywb.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://m.share.fehbvm.com/Article/details/gjgnvwjbp.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gssopwlix.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/gnammiewh.sHtML

Py:   import random; random.randint(1, 100)
来源：http://mobile.fehbvm.com/Article/details/gazqyeeqk.sHtML

PHP:  random_int(1, 100);
来源：http://wap.fehbvm.com/Article/details/gfsmfpsqs.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.hesvh.cn/Article/details/gxaujtqqi.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/ggddqnovb.sHtML

Java: new Random().nextInt(100) + 1
来源：http://mobile.hesvh.cn/Article/details/gqgqvxyag.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.zdbjq.cn/Article/details/gdizesrxt.sHtML

Ruby: rand(1..100)
来源：http://blog.fehbvm.com/Article/details/gsklmnsrq.sHtML

C#:   new Random().Next(1, 101)
来源：http://baike.fehbvm.com/Article/details/gfzyykftf.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.fehbvm.com/Article/details/gfduobuau.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.m.share.fehbvm.com/Article/details/goggeotfp.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gstykpphs.sHtML


<!-- 参考信息 -->