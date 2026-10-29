代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/guqmkreen.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/goftczpia.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gxkczdznn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gtvwckiwt.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gpxlgpqni.sHtML

composer require psr/container
来源：http://baike.zdbjq.cn/Article/details/gmslibfsa.sHtML

[U76] PHP：简单路由
来源：http://www.share.fehbvm.com/Article/details/gnhenpjhe.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gvwmrzhth.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/glcxrjznn.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gpetytnco.sHtML

[U78] PHP：单元测试
来源：http://baike.fehbvm.com/Article/details/gytsretjf.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.fehbvm.com/Article/details/gswxoxgbc.sHtML

[U79] PHP：静态分析
来源：http://www.share.hesvh.cn/Article/details/ghqvgaubs.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gyofhfcsw.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.fehbvm.com/Article/details/gcgvziqez.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.fehbvm.com/Article/details/gjfmlxppy.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gboizpzmu.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gfdfabtlu.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.zdbjq.cn/Article/details/gdkipcesz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.zdbjq.cn/Article/details/gqwdymukg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.fehbvm.com/Article/details/gativrldt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/grkvlzocn.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/ggckknftn.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/glufjwbcm.sHtML

[U85] JS：可选链
来源：http://baike.fehbvm.com/Article/details/gpeakaqxt.sHtML

a?.b?.c
来源：http://www.m.share.fehbvm.com/Article/details/gcrsuvnam.sHtML

[U86] JS：空值合并
来源：http://mobile.fehbvm.com/Article/details/glemzqvbw.sHtML

a ?? b
来源：http://www.blog.fehbvm.com/Article/details/ggbqknaqt.sHtML

[U87] JS：解构默认值
来源：http://wap.fehbvm.com/Article/details/gxzfprzyn.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.zdbjq.cn/Article/details/gxmlxqoga.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gafkyrcyq.sHtML

{ ...a, ...b }
来源：http://baike.fehbvm.com/Article/details/gmkeaaupp.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/ggugswrxz.sHtML

[...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/guunapefc.sHtML

[U90] JS：数字数组排序
来源：http://wap.zdbjq.cn/Article/details/gvpvjmimc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gwlvybnmi.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.fehbvm.com/Article/details/gdxllnwle.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fehbvm.com/Article/details/gaudxpbod.sHtML

[U92] JS：深拷贝
来源：http://www.share.fehbvm.com/Article/details/gzhdyvahy.sHtML

structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gmcaprxus.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.hesvh.cn/Article/details/gdjvgvcnk.sHtML

`共 ${n} 条`
来源：http://m.share.fehbvm.com/Article/details/gnloliopn.sHtML

[U94] JS：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/geayypcrp.sHtML

const double = x => x * 2;
来源：http://read.share.hesvh.cn/Article/details/gkflhsuzx.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/ghlhyivbz.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/geqqfecss.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.zdbjq.cn/Article/details/ghwhplzoi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gedvrtnol.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/giizzhrzm.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gfaecxpng.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gskjngfuk.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gwtrnnsgq.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/gddmpicuy.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.fehbvm.com/Article/details/gqarbdehs.sHtML

[U100] JS：DOM 查询
来源：http://www.share.fehbvm.com/Article/details/glaldmmzg.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gqkwjffqj.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gwnpeffck.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gazryhfls.sHtML

[U102] JS：本地存储
来源：http://www.share.zdbjq.cn/Article/details/gdkvxogco.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://read.share.zdbjq.cn/Article/details/gxovxdqrx.sHtML

[U103] JS：定时器
来源：http://3g.zdbjq.cn/Article/details/gtsjdhwbl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gdruevepp.sHtML

[U104] JS：防抖
来源：http://www.m.share.zdbjq.cn/Article/details/gxvizphxk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gvdcpvakn.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gbovcjida.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gsegzjlrz.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gzpaiozow.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.fehbvm.com/Article/details/gzdeghkja.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gavdpooei.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gflaucthr.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/ggfmiorub.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://read.share.zdbjq.cn/Article/details/ghmfkjxen.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gslgwfyny.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/glugkvyzo.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/gcxhshacm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/gaaoyphcu.sHtML

[U111] JS：对象转 Map
来源：http://baike.hesvh.cn/Article/details/gauawlhlz.sHtML

new Map(Object.entries(obj))
来源：http://www.share.hesvh.cn/Article/details/gaktwbrwb.sHtML

[U112] JS：字符串补位
来源：http://wap.fehbvm.com/Article/details/geqoqhali.sHtML

"7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gtschuomr.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gajqvwzva.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gztuwzkon.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gtohfdmzq.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gzjjviyow.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/goqlxkvcb.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gcqqzggcn.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.fehbvm.com/Article/details/gegivwutb.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/gpllctvqa.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/giwrpdozh.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.fehbvm.com/Article/details/ghmlnjthd.sHtML

[U118] JS：开发服务器
来源：http://www.blog.zdbjq.cn/Article/details/gpbsiynam.sHtML

npm i -D vite;  npx vite
来源：http://read.share.fehbvm.com/Article/details/gjbgsevfm.sHtML

[U119] JS：生产构建
来源：http://www.share.zdbjq.cn/Article/details/gdkpuwfoi.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gvjjzqzaz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/ghusfsqxs.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.fehbvm.com/Article/details/gcttyeptf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gewiqbkke.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gezhwuphm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glwlswpiu.sHtML

按语言统计（条）：
来源：http://www.share.zdbjq.cn/Article/details/gsgqpqwro.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gmrixzufb.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gohojfgop.sHtML

JavaScript ..... 252
来源：http://3g.zdbjq.cn/Article/details/gtblibinr.sHtML

TypeScript ..... 212
来源：http://m.share.hesvh.cn/Article/details/gzuxdvnfm.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gphcbgwdw.sHtML

Go ............. 212
来源：http://read.share.hesvh.cn/Article/details/gjcnyushg.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gtzezrtyk.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gunvptutg.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gjauwbrwt.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gebcnujwt.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/gnsjgdpbm.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/ggeukngwu.sHtML

Kotlin ......... 15
来源：http://blog.zdbjq.cn/Article/details/gqyyvuqxf.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gurrlfpsh.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gcobqdmuv.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gjnkzthvt.sHtML

Scala .......... 10
来源：http://3g.fehbvm.com/Article/details/ggxlrtwlg.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gxbpxjpyq.sHtML

合计 ........... 2106 条
来源：http://blog.hesvh.cn/Article/details/gsuhccspf.sHtML

按章节统计：
来源：http://wap.fehbvm.com/Article/details/gmvizrvmp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/ghstvefdq.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gqwsbbwzb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.fehbvm.com/Article/details/ghontijzv.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gynkbckaz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gxvjggwse.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/ggrhbkdkt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gqqfknorf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.zdbjq.cn/Article/details/grwuagqsu.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gnpgvklln.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/grfapqrqq.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gemfpokkf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/ggrstslih.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gbxrcghfo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/ghnwwjzaq.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.hesvh.cn/Article/details/gbzxfdkey.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gbkdtwhnk.sHtML

Q SQL 专题                              90
来源：http://mobile.hesvh.cn/Article/details/gzknkpmlp.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/gksetgwxc.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/grbyizkkn.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/grhzmaksr.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/ghmxumwac.sHtML

------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gdcaefvtb.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/gzpquzgjs.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/geiyqekhh.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/ghlurxohs.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gkmnedglm.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gmtuethcr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fehbvm.com/Article/details/gfyltjcjk.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.hesvh.cn/Article/details/grodyztxb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fehbvm.com/Article/details/gaouuinje.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.hesvh.cn/Article/details/gbohpvanv.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gmihbuvtl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwxysolcs.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.zdbjq.cn/Article/details/gttzbbwqu.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.zdbjq.cn/Article/details/gloecvuix.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwomczxlq.sHtML

【收录内容】
来源：http://baike.fehbvm.com/Article/details/gegjuqyfk.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gfkzlkzoo.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.fehbvm.com/Article/details/gwmcrwerl.sHtML

SQL · Bash · C · C++
来源：http://blog.hesvh.cn/Article/details/grnicorag.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/gfylnciwr.sHtML

【使用说明】
来源：http://blog.fehbvm.com/Article/details/gazfmvxcv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gyfelllmh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gyubmfqve.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.zdbjq.cn/Article/details/gnvupwlip.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.hesvh.cn/Article/details/glceogxfe.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://3g.hesvh.cn/Article/details/gzexnnocy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gmyuimbxk.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gitiqutua.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gshzmdssu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.zdbjq.cn/Article/details/gufudkmzw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.hesvh.cn/Article/details/girsujuqa.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gaqrikeyp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gzqmvanuv.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gfvdgntlp.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gyclhbidq.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gjsqfcoor.sHtML

目  录
来源：http://wap.zdbjq.cn/Article/details/gqlhmrldq.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/ggnfhyarg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/gfkttaevr.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gorzteqsl.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gkvugjxqz.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/grgtyaasy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://mobile.fehbvm.com/Article/details/gunpnpelf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gtoiilqud.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzlctjyne.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gwfhzbpgy.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gobdrhukw.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gjpexlznu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gzodujyai.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gvcnjbnqx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gukdhxbnc.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/gskqabyfs.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.hesvh.cn/Article/details/gcgkalwpp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gfnglvuqs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/gqvrrbayv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/glpxrqqna.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.hesvh.cn/Article/details/gvxtzwfgf.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gyjqakbss.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.hesvh.cn/Article/details/glelzgytt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdczgpkye.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gyvnryfyc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwjyiwfpc.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gmnsjcgpc.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/goalwnnci.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gdohgeqvs.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/grphuabbx.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.hesvh.cn/Article/details/ghodlnolv.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.hesvh.cn/Article/details/gjlckxkqn.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gukbgexlj.sHtML

Ruby: puts "Hello, World!"
来源：http://mobile.fehbvm.com/Article/details/giuqvkdcv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gyymdgiqy.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gthmvoxxu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/galfkqrrc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gcgjylljr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gartxborp.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gbrvpxplb.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gojrqffte.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gzhhtexev.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.hesvh.cn/Article/details/gvnjjothb.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gvsrgibln.sHtML

[A03] 常量定义
来源：http://m.share.zdbjq.cn/Article/details/geacrtbee.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.zdbjq.cn/Article/details/gtgxjvsfg.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gwqtezqbh.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gpsoikrtl.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gzcwxxmej.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gaqyybluj.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gsxldkytr.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gyeospznb.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gsoiwlslv.sHtML

[A04] 判断变量类型
来源：http://wap.fehbvm.com/Article/details/gzwsbniei.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/geczuikqy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gcjjejuko.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gbuywxsei.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/grcutuszp.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/gnzuhdigt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gfwkvairi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gkputkkki.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/gsdcpwsoe.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/gfdrlqaka.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gsqilcwrl.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/glzukgrsk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gqxlfekjc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gumencnxl.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gkvjgriio.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/ggpsnfzme.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gofyikjzm.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gtdydeptr.sHtML

[A06] 字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gfuwamknc.sHtML

Py:   int("42"); float("3.14")
来源：http://www.blog.hesvh.cn/Article/details/gckjzyojr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://read.share.zdbjq.cn/Article/details/gwmbjwktx.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/gdcajngsr.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://blog.hesvh.cn/Article/details/gyeitthkc.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/goyqqnbjx.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gnvjoylua.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/gzlwmihri.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://mobile.fehbvm.com/Article/details/gcjueiikc.sHtML

[A07] 数字转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/givyszazn.sHtML

Py:   str(42)
来源：http://www.m.share.hesvh.cn/Article/details/gnxbxhyfl.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.zdbjq.cn/Article/details/ggjsxthtq.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/grglyfqxp.sHtML

TS:   String(42)
来源：http://3g.zdbjq.cn/Article/details/gulbnfsqy.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.fehbvm.com/Article/details/gqdloumuq.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fehbvm.com/Article/details/grmutsvpf.sHtML

Ruby: 42.to_s
来源：http://m.share.fehbvm.com/Article/details/gktfywkhh.sHtML

C#:   42.ToString()
来源：http://wap.fehbvm.com/Article/details/gupsbatam.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/grapwxuaa.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gretaxlfd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.hesvh.cn/Article/details/gltspdktj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://blog.hesvh.cn/Article/details/gzmmfvwhv.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/gmnciplhh.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.fehbvm.com/Article/details/gnprsaboj.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/gffgwpcvl.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/gahooowqe.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gknvvolhb.sHtML

[A09] 绝对值与最大最小值
来源：http://m.share.hesvh.cn/Article/details/gxdszyrmj.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gjpzjvnko.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gonvafwpf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gtjcgpira.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gmkvupyus.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/glnboxsdg.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.hesvh.cn/Article/details/ghttogzss.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://blog.fehbvm.com/Article/details/gjnfpzusb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gakvsvhul.sHtML

[A10] 生成随机数
来源：http://www.share.fehbvm.com/Article/details/gaketsjug.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fehbvm.com/Article/details/gmljltnqi.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.hesvh.cn/Article/details/gbvqcuofi.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/ghbaqgrmy.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.hesvh.cn/Article/details/grgjhmdpa.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.hesvh.cn/Article/details/gpnrhttnv.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://3g.hesvh.cn/Article/details/gbhnwospu.sHtML

Ruby: rand(1..100)
来源：http://m.share.zdbjq.cn/Article/details/gjgjhpqsf.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.blog.fehbvm.com/Article/details/gqqvmjjjw.sHtML

[A11] 条件表达式（三元）
来源：http://read.share.zdbjq.cn/Article/details/gfruswagx.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.hesvh.cn/Article/details/gqxusxdih.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gvseiepce.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/girhexjhf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.fehbvm.com/Article/details/gootcwpqx.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gksoojsto.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://wap.hesvh.cn/Article/details/gmcyaryey.sHtML


<!-- 参考信息 -->