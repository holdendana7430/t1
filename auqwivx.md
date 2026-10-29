代发 wailian999

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gpejoamxv.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gerqwbndy.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/geejmdhft.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/gxrehamld.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.fehbvm.com/Article/details/gxktwpbao.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gyshvxmrk.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/ghbmjpqmf.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.hesvh.cn/Article/details/ghftrptel.sHtML

[U79] PHP：静态分析
来源：http://wap.hesvh.cn/Article/details/gqxpttojc.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gzmdgagvn.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.hesvh.cn/Article/details/gserjgafl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.zdbjq.cn/Article/details/gkzyhonef.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gxpjcenyz.sHtML

npm init -y;  npm i express
来源：http://read.share.zdbjq.cn/Article/details/gvlsinnbr.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gphkcdxmf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://baike.hesvh.cn/Article/details/glkkkjnyc.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.zdbjq.cn/Article/details/ghomxnlvx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gygazwifs.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.hesvh.cn/Article/details/giyogshrj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gvuhxylng.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gmblfuaax.sHtML

a?.b?.c
来源：http://m.share.zdbjq.cn/Article/details/gdqupgrff.sHtML

[U86] JS：空值合并
来源：http://blog.fehbvm.com/Article/details/gifzkhffq.sHtML

a ?? b
来源：http://www.share.hesvh.cn/Article/details/gajftxkfa.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gbfbywiqj.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.zdbjq.cn/Article/details/gtfhjdtbl.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gcbecbpxs.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gddugwzbi.sHtML

[U89] JS：数组去重
来源：http://m.share.hesvh.cn/Article/details/gthcbynbb.sHtML

[...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gapztdimo.sHtML

[U90] JS：数字数组排序
来源：http://3g.hesvh.cn/Article/details/gucbiiwbb.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gkndtotwn.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.hesvh.cn/Article/details/galkrmeku.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.zdbjq.cn/Article/details/gikecxoub.sHtML

[U92] JS：深拷贝
来源：http://blog.zdbjq.cn/Article/details/gmmwaafmw.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gnfkualjd.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/geazakngy.sHtML

`共 ${n} 条`
来源：http://m.share.hesvh.cn/Article/details/gpevukone.sHtML

[U94] JS：箭头函数
来源：http://blog.zdbjq.cn/Article/details/gfhuicagj.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gezyxtykw.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/gulttxhpl.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/ggfgljhpt.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.fehbvm.com/Article/details/ggaxxwllf.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvglfkxha.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gfombqcej.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/giijjkoei.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.zdbjq.cn/Article/details/ggzdwjlpa.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gxgyyfwlq.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gtoirbxkf.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gnjscbecx.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/goobtbdiq.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gaipzqwtl.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gwqnnnrtc.sHtML

el.classList.toggle("active")
来源：http://www.m.share.zdbjq.cn/Article/details/gjiqiwyff.sHtML

[U102] JS：本地存储
来源：http://mobile.fehbvm.com/Article/details/goxhjkwnz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gfgqfnfzg.sHtML

[U103] JS：定时器
来源：http://mobile.zdbjq.cn/Article/details/glaoqotnu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gxrkvxrdc.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/giankepjk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gsrgfwqzf.sHtML

[U105] JS：节流
来源：http://www.blog.hesvh.cn/Article/details/gypcwogke.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fehbvm.com/Article/details/gozvrrgtj.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gxkirvank.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gumacvbbr.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gplyytsth.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://3g.hesvh.cn/Article/details/gmjbbjtvl.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gmpsnuuep.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/ghjnqsgrx.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/grnnocbce.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gmjocbbew.sHtML

[U110] JS：数组分块
来源：http://m.share.fehbvm.com/Article/details/gvocgeqfe.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gjpjtyftl.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.hesvh.cn/Article/details/gnakudpja.sHtML

new Map(Object.entries(obj))
来源：http://wap.zdbjq.cn/Article/details/gztbrostx.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gzxedkeyn.sHtML

"7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gcawjneec.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gmupuaqxo.sHtML

s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/guwyvevks.sHtML

[U114] JS：JSON 深比较
来源：http://blog.hesvh.cn/Article/details/gilnvcpvo.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gumgmpgun.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/glhyeqbxg.sHtML

crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/geiqpbjrb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gutudnrfy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfuuabexx.sHtML

[U117] JS：单元测试
来源：http://read.share.fehbvm.com/Article/details/gloytztbr.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.hesvh.cn/Article/details/gltkfpynw.sHtML

[U118] JS：开发服务器
来源：http://www.share.zdbjq.cn/Article/details/gierpesoq.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/ghupfzugf.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/glddxcbhr.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/giwunlnta.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gfzogwuga.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gpqoagylw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfnyzxtye.sHtML

统计汇总
来源：http://mobile.fehbvm.com/Article/details/gnttpvxhn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gljdswfuo.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gjiscafjm.sHtML

Python ......... 252
来源：http://3g.hesvh.cn/Article/details/ghashjcmd.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gkbuyiupc.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/glhsdzlwn.sHtML

TypeScript ..... 212
来源：http://mobile.fehbvm.com/Article/details/gvbumwwgz.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gjxkmzakp.sHtML

Go ............. 212
来源：http://wap.zdbjq.cn/Article/details/gzgmnawec.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gafeehspy.sHtML

C# ............. 212
来源：http://read.share.hesvh.cn/Article/details/gobxjmvjj.sHtML

C .............. 30
来源：http://www.m.share.zdbjq.cn/Article/details/gglpuvvtx.sHtML

C++ ............ 30
来源：http://blog.hesvh.cn/Article/details/gmmexaqfb.sHtML

SQL ............ 90
来源：http://mobile.fehbvm.com/Article/details/gjbmrhmer.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gfhbvlwlf.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gzvcdzvad.sHtML

Swift .......... 15
来源：http://m.share.hesvh.cn/Article/details/gnpnifkdy.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/glhyffpcq.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/gizpaylxp.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gajbvxdtp.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gpdvcnhfe.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/ghvvochqp.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gkdxvhcmu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.fehbvm.com/Article/details/gtuufehnp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/gxjesohtc.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gzgqoqrne.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gwtkigbfw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gtoauwkiz.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/glzwjobmw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.fehbvm.com/Article/details/giaiwhild.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gorsxjrtk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gfalfnsop.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gbgihzodt.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/grnibviko.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/ggekvdpwe.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.fehbvm.com/Article/details/gwhkxezss.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gwdcxxewz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gfxfdelgv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gjfjlbjok.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/grsqgzlss.sHtML

R Bash 专题                             80
来源：http://read.share.zdbjq.cn/Article/details/gujodjwkn.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gizryglzz.sHtML

T 其他语言补充                          60
来源：http://m.share.zdbjq.cn/Article/details/gfqlmvspw.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gamjxfnee.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/gvvgxufzu.sHtML

合计                                  2106 条
来源：http://m.share.hesvh.cn/Article/details/glzjlpgds.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gmhwdiqjv.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gwibhpahq.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gundrsabs.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://3g.zdbjq.cn/Article/details/gqqimothp.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.hesvh.cn/Article/details/grlnjsxoi.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gnvgndvwi.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.zdbjq.cn/Article/details/gplnuinmx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gkuyxjltk.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/gdgzohakt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goaqygvcl.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.hesvh.cn/Article/details/gqmyscqyu.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.fehbvm.com/Article/details/gxfaexlfz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtntrbppc.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/glwwpgogv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.zdbjq.cn/Article/details/gikdiqyzt.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/geituxnfs.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gcpqcejyx.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.hesvh.cn/Article/details/gdijecmwj.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gjkvjwqht.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gtwdvztkc.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gwvfvrnxe.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.share.fehbvm.com/Article/details/gfesqioiy.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gtqsmduqk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gkrcyplpa.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.zdbjq.cn/Article/details/gkojjzfgc.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gdqcegkil.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/gheqkrpbg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.zdbjq.cn/Article/details/glmxfaupl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.zdbjq.cn/Article/details/gecemxgms.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.hesvh.cn/Article/details/gvooihbzu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/gaknowiis.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/gifoqgddm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.fehbvm.com/Article/details/gnddqewse.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/guyiipine.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gmezocjgd.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gbxoshpic.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/gegulycng.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gmlgwcqea.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzxyvsapc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.zdbjq.cn/Article/details/ggjixwbyk.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.hesvh.cn/Article/details/gzejpaupx.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/gkwindhzc.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/gguvmwusp.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/glflqbnst.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gzvhomnig.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gjvwtguyl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://baike.fehbvm.com/Article/details/gfbiuubze.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gfmciugyd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gkxdrfsml.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gmqaarchf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://3g.zdbjq.cn/Article/details/gpresprkm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gxhrvdzut.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.hesvh.cn/Article/details/griidqvtz.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://wap.hesvh.cn/Article/details/gtxyxkejk.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/ghibqxrjj.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.zdbjq.cn/Article/details/gdrcoywqc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/ghrpmvbjx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaflxaqpo.sHtML

A. 基础语法与类型
来源：http://mobile.hesvh.cn/Article/details/gnbjeyrhj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcarclqvi.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gfhpqzfnb.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gjhjvioss.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gsfqaxtje.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/glbxbaoxk.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://baike.hesvh.cn/Article/details/gkppdhzvc.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.hesvh.cn/Article/details/grmxlmqiz.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.hesvh.cn/Article/details/gjyziaiab.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.fehbvm.com/Article/details/gcqgrfcae.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/grxltnahk.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.fehbvm.com/Article/details/gmubabzpb.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.zdbjq.cn/Article/details/gstocflzo.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.fehbvm.com/Article/details/ghporgosc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gugxrlkrf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/gkabqgyns.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gtqnsxukd.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.hesvh.cn/Article/details/gkbmsjbmd.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.fehbvm.com/Article/details/gqykyubvt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gxodjwbwj.sHtML

[A03] 常量定义
来源：http://wap.zdbjq.cn/Article/details/gsojijgzu.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://baike.zdbjq.cn/Article/details/gwvylxknj.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gprpioefj.sHtML

JS:   const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gvncbxxpt.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gvbrulliz.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gxoockdou.sHtML

Go:   const PI = 3.14159
来源：http://baike.zdbjq.cn/Article/details/gsuphbkud.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gzsjvwlhc.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gktnnmrdl.sHtML

[A04] 判断变量类型
来源：http://www.share.fehbvm.com/Article/details/gktibamwa.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/ghbewkbiy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gibyyhqzo.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gosxszgez.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gvpxvmygc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.zdbjq.cn/Article/details/gvsprarey.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.share.zdbjq.cn/Article/details/goupqqtbz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.m.share.fehbvm.com/Article/details/gsjxlrkyu.sHtML

C#:   x.GetType().Name; x is int
来源：http://blog.fehbvm.com/Article/details/gbhusjnsf.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gylcacxgs.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://blog.zdbjq.cn/Article/details/gukartbdb.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gtfggsbyw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gcmxeegye.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gmdxndzue.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.hesvh.cn/Article/details/gjdbxgpkj.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gtifikdkn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/ghqgfkplw.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/ghmslczkl.sHtML

[A06] 字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gdeqvydti.sHtML

Py:   int("42"); float("3.14")
来源：http://m.share.hesvh.cn/Article/details/gyjwjzmnx.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.fehbvm.com/Article/details/gtzfxpwbp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/gaxgecwko.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://baike.zdbjq.cn/Article/details/gpmixejdx.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.blog.zdbjq.cn/Article/details/gcjcfpsgr.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gtmklehsl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.zdbjq.cn/Article/details/gqzhsbghg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.fehbvm.com/Article/details/gqsldbxgm.sHtML

[A07] 数字转字符串
来源：http://www.blog.hesvh.cn/Article/details/ghclqqxzc.sHtML

Py:   str(42)
来源：http://baike.fehbvm.com/Article/details/gsrrzgqka.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/gskqusqtd.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fehbvm.com/Article/details/gxgkmevef.sHtML

TS:   String(42)
来源：http://wap.zdbjq.cn/Article/details/gblbqqbeb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.fehbvm.com/Article/details/gcuulhdtb.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.fehbvm.com/Article/details/gvcebuvgb.sHtML

Ruby: 42.to_s
来源：http://m.share.zdbjq.cn/Article/details/ggiyjdqyj.sHtML

C#:   42.ToString()
来源：http://wap.hesvh.cn/Article/details/grmqklwuc.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/geqqstjsu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gkgsbyjfd.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://mobile.hesvh.cn/Article/details/glvjzgeze.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gpduuktre.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.fehbvm.com/Article/details/gneshgisa.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gajkutlny.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/ghsxmfkxs.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.fehbvm.com/Article/details/gqwvrjkrl.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gumokxrux.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gqnjmkyxw.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gagsstgvh.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://wap.fehbvm.com/Article/details/gaqnvnshg.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.zdbjq.cn/Article/details/grgeavcfv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://baike.fehbvm.com/Article/details/ggvcksdmu.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://3g.hesvh.cn/Article/details/guhoaehul.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/gydltmxqm.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://read.share.zdbjq.cn/Article/details/ghxjmhtvx.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsmpyiwoz.sHtML

[A10] 生成随机数
来源：http://3g.fehbvm.com/Article/details/gdlengppd.sHtML

Py:   import random; random.randint(1, 100)
来源：http://baike.fehbvm.com/Article/details/gbulmtiah.sHtML

PHP:  random_int(1, 100);
来源：http://mobile.fehbvm.com/Article/details/gvkuleubp.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/grfvtbxdf.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://baike.zdbjq.cn/Article/details/gssntasdm.sHtML

Java: new Random().nextInt(100) + 1
来源：http://read.share.hesvh.cn/Article/details/gpqmfocfu.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.blog.hesvh.cn/Article/details/gkqeadksi.sHtML

Ruby: rand(1..100)
来源：http://blog.zdbjq.cn/Article/details/ghdhwanyz.sHtML

C#:   new Random().Next(1, 101)
来源：http://mobile.hesvh.cn/Article/details/ggucncxav.sHtML

[A11] 条件表达式（三元）
来源：http://3g.fehbvm.com/Article/details/gyymvsvyw.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.hesvh.cn/Article/details/gnzxwvogf.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://wap.hesvh.cn/Article/details/gpzpwxqsg.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gjvznbhkb.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gxwzuaqzn.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gibviljei.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://read.share.zdbjq.cn/Article/details/gbfhztrzw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gguyfzzha.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gbosriqgb.sHtML

[A12] 字符串插值 / 格式化
来源：http://m.share.fehbvm.com/Article/details/gabfeemkr.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.hesvh.cn/Article/details/gtccltmci.sHtML


<!-- 参考信息 -->