代发 wailian999

[U77] PHP：模板渲染
来源：http://blog.fehbvm.com/Article/details/gzqpvybry.sHtML

composer require twig/twig
来源：http://baike.hesvh.cn/Article/details/grallbxjh.sHtML

[U78] PHP：单元测试
来源：http://www.m.share.fehbvm.com/Article/details/gluwtiylw.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.hesvh.cn/Article/details/gubqcztgx.sHtML

[U79] PHP：静态分析
来源：http://wap.fehbvm.com/Article/details/gimpnsbki.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.zdbjq.cn/Article/details/gzvsgwcfb.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.hesvh.cn/Article/details/gbcaimjqa.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/ghmfnqikk.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gckzsepqh.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gjofthnlb.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.fehbvm.com/Article/details/gxipaqvvf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gynmyiesa.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.hesvh.cn/Article/details/gmzrbjphu.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gcdpipplg.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.fehbvm.com/Article/details/gesfamqck.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.hesvh.cn/Article/details/gtkqjmajl.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gmtaaipik.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/glcswgsfw.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/grahkljib.sHtML

a ?? b
来源：http://www.blog.hesvh.cn/Article/details/gjnbdzzvq.sHtML

[U87] JS：解构默认值
来源：http://3g.fehbvm.com/Article/details/gqrygazky.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.hesvh.cn/Article/details/gdjfcxkop.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/glaykchwm.sHtML

{ ...a, ...b }
来源：http://wap.fehbvm.com/Article/details/ghufvmthq.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/glilhgjkx.sHtML

[...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gjwdhxdjs.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/glptcqawk.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gdmsoojxi.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gvndtfumw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/gveltcmip.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/guynledqg.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gmefexwjm.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gxscsjewt.sHtML

`共 ${n} 条`
来源：http://wap.zdbjq.cn/Article/details/geubrzduc.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gnccemots.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gheztrtqn.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/ghasaoair.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/ghunujjfu.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.zdbjq.cn/Article/details/glaaagcnn.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gqbokxgao.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gsbonzjxd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gxhehcmib.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fehbvm.com/Article/details/gqtsqtxyl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/grsfqyzlb.sHtML

[U99] JS：事件监听
来源：http://wap.zdbjq.cn/Article/details/girrmezww.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.fehbvm.com/Article/details/gbrhzucnm.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gnolexvny.sHtML

document.querySelector(".item")
来源：http://mobile.hesvh.cn/Article/details/geyuifjdp.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/gnzwtrwvq.sHtML

el.classList.toggle("active")
来源：http://blog.hesvh.cn/Article/details/gwcaigdgh.sHtML

[U102] JS：本地存储
来源：http://m.share.hesvh.cn/Article/details/gtvcvzgwt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/ghphzgdgw.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/ggmxlkkwk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/gagityxii.sHtML

[U104] JS：防抖
来源：http://www.m.share.fehbvm.com/Article/details/gxcnyebex.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gcdtusqei.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gdjwxstyz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.zdbjq.cn/Article/details/gzhnkzbnr.sHtML

[U106] JS：日期格式化
来源：http://m.share.hesvh.cn/Article/details/gmsgbpnxb.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gkwusasgg.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gncvgroap.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ggxlowynw.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gdczajunj.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gxzslntvp.sHtML

[U109] JS：数组分组
来源：http://www.share.zdbjq.cn/Article/details/grwikvhux.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/geikbudsm.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gjpbgoyur.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/grgghsryy.sHtML

[U111] JS：对象转 Map
来源：http://m.share.zdbjq.cn/Article/details/gmmtyobxa.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gfltbjoxo.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.hesvh.cn/Article/details/glngnzctm.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gcuwsrqbg.sHtML

[U113] JS：正则替换全部
来源：http://www.blog.zdbjq.cn/Article/details/gttxqmofp.sHtML

s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gdkztckiz.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gfiaoarwb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/grpqzwedd.sHtML

[U115] JS：生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gghzpfggm.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gkhetfdor.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gjhjigcsa.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.zdbjq.cn/Article/details/gguowkstl.sHtML

[U117] JS：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gmxquxupa.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gizvlkaew.sHtML

[U118] JS：开发服务器
来源：http://3g.zdbjq.cn/Article/details/gnxhsebfq.sHtML

npm i -D vite;  npx vite
来源：http://wap.fehbvm.com/Article/details/gpdcpylbf.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/glujgjgym.sHtML

npx vite build
来源：http://baike.zdbjq.cn/Article/details/gqzzbzhpd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.fehbvm.com/Article/details/grwoyamgg.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.fehbvm.com/Article/details/guiadjxkq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbynhjkrr.sHtML

统计汇总
来源：http://3g.zdbjq.cn/Article/details/gwzfavggi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggjcfnaig.sHtML

按语言统计（条）：
来源：http://wap.fehbvm.com/Article/details/ghmlphatx.sHtML

Python ......... 252
来源：http://wap.fehbvm.com/Article/details/goncfjkdx.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/gpzxttuvs.sHtML

JavaScript ..... 252
来源：http://baike.hesvh.cn/Article/details/gbqioarqh.sHtML

TypeScript ..... 212
来源：http://read.share.zdbjq.cn/Article/details/gzrxtexen.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gdicaeycl.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gsfaescuz.sHtML

Ruby ........... 212
来源：http://mobile.hesvh.cn/Article/details/gutmkhqxu.sHtML

C# ............. 212
来源：http://www.share.fehbvm.com/Article/details/gzxwugtgx.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/ghcywbrjv.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gbrnyzdre.sHtML

SQL ............ 90
来源：http://www.blog.hesvh.cn/Article/details/gtguhpzpl.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gfukolrkf.sHtML

Kotlin ......... 15
来源：http://mobile.fehbvm.com/Article/details/gpauhzqhk.sHtML

Swift .......... 15
来源：http://read.share.hesvh.cn/Article/details/gxjgeigas.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/gxvqykhbu.sHtML

Perl ........... 10
来源：http://blog.zdbjq.cn/Article/details/guqvwavet.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gdjocdhtq.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gweyhkzji.sHtML

合计 ........... 2106 条
来源：http://m.share.fehbvm.com/Article/details/glrnctybe.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gpbigvoqn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gbenrteoz.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gumpkpxtv.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/ghvuibzql.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.hesvh.cn/Article/details/glogqtjgj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.blog.fehbvm.com/Article/details/gjbmqmkwb.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/golbzpagy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/ggwtsjyen.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://wap.zdbjq.cn/Article/details/gvxdgctio.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/glujvgjlz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.fehbvm.com/Article/details/gwyyocpqn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/ggvltuftr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gcydceplf.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gabscpeus.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gqqyibjkz.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.fehbvm.com/Article/details/gupmznlyo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gmtbqxlsj.sHtML

Q SQL 专题                              90
来源：http://blog.fehbvm.com/Article/details/gpwdrfaka.sHtML

R Bash 专题                             80
来源：http://www.m.share.fehbvm.com/Article/details/goqogluwb.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gzokpkayq.sHtML

T 其他语言补充                          60
来源：http://baike.hesvh.cn/Article/details/gmpafrgqa.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gfxtyfwyn.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gtwffvtoq.sHtML

合计                                  2106 条
来源：http://mobile.hesvh.cn/Article/details/ghpelisme.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gvloyhvic.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gdlxbrgjc.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gkzzsqrxh.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.fehbvm.com/Article/details/gfqgmunhy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.fehbvm.com/Article/details/gpxcxalbd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/grfkxzepx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gcautdzly.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gubxcrmdd.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/gjsbalzsm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwdqzxopz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.hesvh.cn/Article/details/gtpennzxw.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gmeyzddoi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqahzslcx.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gugtjgfeb.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://baike.fehbvm.com/Article/details/gaqanxmjh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.blog.fehbvm.com/Article/details/ghzypqxmq.sHtML

SQL · Bash · C · C++
来源：http://3g.fehbvm.com/Article/details/gzposfijb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/gdblntdma.sHtML

【使用说明】
来源：http://mobile.zdbjq.cn/Article/details/gparjpsdv.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.zdbjq.cn/Article/details/ghjeejitx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gbeoncdoa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.hesvh.cn/Article/details/gywxaddgo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.hesvh.cn/Article/details/grydogivn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.zdbjq.cn/Article/details/gvtmwkkia.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.zdbjq.cn/Article/details/goflmevub.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://blog.hesvh.cn/Article/details/gnyukknzf.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/gayghadpr.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gunkaxtur.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.zdbjq.cn/Article/details/grqzpjxah.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/glgzgyajc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.zdbjq.cn/Article/details/gtzinffdx.sHtML

【文件统计】
来源：http://blog.hesvh.cn/Article/details/gpilufrtk.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/glklxsybv.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gmkavrhoy.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gejpesppk.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/giajkbuow.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gthqkpyfj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gmvnlozig.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gttqkkajx.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/ggodcwruj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpaykbiyo.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gsxftmabn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gyctglqww.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/gcbrmsudv.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.hesvh.cn/Article/details/gehzlpiym.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gsyssztsl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gwamilwab.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gqchimnne.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/geunawarq.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gevmuxqaw.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.hesvh.cn/Article/details/gxalvtiqc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gkhrtlzsv.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gilegvqgv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gemnsxrpd.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://3g.fehbvm.com/Article/details/gvvkqknck.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/ghwizmxmg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.fehbvm.com/Article/details/gdwolbdsl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggnqgefju.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/grrfavnes.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqhiwnpnq.sHtML

[A01] Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdwoywgie.sHtML

Py:   print("Hello, World!")
来源：http://www.share.hesvh.cn/Article/details/goioqgsqm.sHtML

PHP:  echo "Hello, World!";
来源：http://m.share.hesvh.cn/Article/details/gnwgaldsy.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gpfuknqmd.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.fehbvm.com/Article/details/gdzfknubl.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gncennueb.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.hesvh.cn/Article/details/gbdzyzfib.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/gaowfxzfr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gxflobwgv.sHtML

[A02] 变量声明与赋值
来源：http://baike.hesvh.cn/Article/details/gxhojbhur.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://m.share.hesvh.cn/Article/details/gcwboqyjq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gqylyzhgw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://read.share.zdbjq.cn/Article/details/gkgzhverv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.zdbjq.cn/Article/details/ggwidbyre.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gngydkxug.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gjnzqlhnh.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gukekhqmw.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/grpnivvow.sHtML

[A03] 常量定义
来源：http://mobile.fehbvm.com/Article/details/gezzwmxhx.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gxljaurhv.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gljulmptq.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/ghshqhbxj.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/grsocmcrm.sHtML

Java: static final double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gszswzpbp.sHtML

Go:   const PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gzkuzuvlp.sHtML

Ruby: PI = 3.14159
来源：http://m.share.zdbjq.cn/Article/details/ghhmzkzro.sHtML

C#:   const double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gavzdvjvm.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/gvxasbxec.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.zdbjq.cn/Article/details/gjgmjjpwy.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.zdbjq.cn/Article/details/gdpefapod.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.hesvh.cn/Article/details/guqoobjby.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gecmmvfqu.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gczsjpuqi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gklcbwvqq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/ggyrxgewz.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/gfzzeeexu.sHtML

[A05] 整数除法与取模
来源：http://baike.fehbvm.com/Article/details/ggpuptakq.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.hesvh.cn/Article/details/gkjxschvn.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gnraircux.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gfxbqdivz.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gdxatixuj.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gudxvcqyh.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gvjqqldcc.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gnvgysdzw.sHtML

C#:   7 / 2; 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gaoxycvdk.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gnexceyyr.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.hesvh.cn/Article/details/gkgaciket.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.hesvh.cn/Article/details/gymuceqvm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gdwnmiphs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.hesvh.cn/Article/details/gyxtfbjju.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.zdbjq.cn/Article/details/ganaktdxh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.fehbvm.com/Article/details/gjlwpwbdl.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://blog.hesvh.cn/Article/details/gooxxxick.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/glgfjomeq.sHtML

[A07] 数字转字符串
来源：http://mobile.hesvh.cn/Article/details/ggpxmxnjq.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gfkwpldgl.sHtML

PHP:  (string) 42; strval(42)
来源：http://3g.hesvh.cn/Article/details/ghlngobgy.sHtML

JS:   String(42); (42).toString()
来源：http://3g.fehbvm.com/Article/details/girpcipeo.sHtML

TS:   String(42)
来源：http://www.share.zdbjq.cn/Article/details/gtkcooutb.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.hesvh.cn/Article/details/gnplpjkax.sHtML

Go:   strconv.Itoa(42)
来源：http://read.share.hesvh.cn/Article/details/gymhtybmm.sHtML

Ruby: 42.to_s
来源：http://www.m.share.hesvh.cn/Article/details/gyawdmejr.sHtML

C#:   42.ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gulmnoecr.sHtML

[A08] 取整与四舍五入
来源：http://mobile.fehbvm.com/Article/details/gjgjiptkv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/gbzqlzezc.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fehbvm.com/Article/details/gfbkbyxfj.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gwioebvio.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://wap.fehbvm.com/Article/details/gllkhppcw.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/garmscdbp.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gkgnkhycx.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.blog.zdbjq.cn/Article/details/gybztcndm.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsfpvciq.sHtML

[A09] 绝对值与最大最小值
来源：http://wap.zdbjq.cn/Article/details/gfyoghkmv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gxlzvyvid.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gdkbtavws.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://baike.hesvh.cn/Article/details/ginqippie.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.fehbvm.com/Article/details/geqminquj.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gankkremn.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.share.zdbjq.cn/Article/details/gafkqopiv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.zdbjq.cn/Article/details/gshihkies.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/ggtnsleyz.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gzgaulwjz.sHtML

Py:   import random; random.randint(1, 100)
来源：http://3g.hesvh.cn/Article/details/grbdsqnsi.sHtML

PHP:  random_int(1, 100);
来源：http://read.share.fehbvm.com/Article/details/gvwlsbenn.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.blog.fehbvm.com/Article/details/gocxqsthm.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://read.share.fehbvm.com/Article/details/gxhteamhe.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gjpkqaccs.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://wap.hesvh.cn/Article/details/gwwfjjqeh.sHtML

Ruby: rand(1..100)
来源：http://blog.hesvh.cn/Article/details/gccmhumby.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhciiscu.sHtML

[A11] 条件表达式（三元）
来源：http://www.share.zdbjq.cn/Article/details/gnknfwida.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://m.share.fehbvm.com/Article/details/geozdpkyd.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.m.share.hesvh.cn/Article/details/gtcrtmujs.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://www.share.zdbjq.cn/Article/details/gjrwdpcer.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://blog.hesvh.cn/Article/details/gvgdafqcu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.blog.zdbjq.cn/Article/details/ggyyprxks.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://3g.zdbjq.cn/Article/details/gryvoyliw.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/giwjsnnxe.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.hesvh.cn/Article/details/gojyubuan.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.blog.zdbjq.cn/Article/details/gldrihsed.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.fehbvm.com/Article/details/gxchhpypi.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://m.share.hesvh.cn/Article/details/greankrvl.sHtML

JS:   `Hello, ${name}!`
来源：http://www.m.share.fehbvm.com/Article/details/gysuouijd.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.zdbjq.cn/Article/details/gtwevzbsv.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://mobile.fehbvm.com/Article/details/guruhasia.sHtML


<!-- 参考信息 -->