代发 wailian999

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/geanevpsw.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gdxasnqnu.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/ggesummpe.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gixiuvene.sHtML

[U75] PHP：依赖注入
来源：http://read.share.hesvh.cn/Article/details/gpnwboabj.sHtML

composer require psr/container
来源：http://wap.fehbvm.com/Article/details/gxircrkbu.sHtML

[U76] PHP：简单路由
来源：http://m.share.fehbvm.com/Article/details/gxhlmamml.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://baike.zdbjq.cn/Article/details/glivcxtqq.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/grylnrtzo.sHtML

composer require twig/twig
来源：http://baike.fehbvm.com/Article/details/gdfwnvpeo.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gregglndg.sHtML

composer require --dev phpunit/phpunit
来源：http://baike.zdbjq.cn/Article/details/guwtalegz.sHtML

[U79] PHP：静态分析
来源：http://m.share.hesvh.cn/Article/details/gemnrcpto.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.zdbjq.cn/Article/details/gslrwhnbr.sHtML

[U80] PHP：代码规范修复
来源：http://www.m.share.hesvh.cn/Article/details/gqgddbybn.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/garerxkyp.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/gfxlzsdbk.sHtML

npm init -y;  npm i express
来源：http://blog.fehbvm.com/Article/details/gczqkrjvl.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gtfmzfrxb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gifcgpgar.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gekmsszcv.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gjmrtfkzq.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gwsyprgay.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gmgkiwjnj.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gmlkzzbqx.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gexzjjmxj.sHtML

[U86] JS：空值合并
来源：http://m.share.fehbvm.com/Article/details/gnlsgcufv.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gjblcoxxy.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gscytqmkg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/gskdqkpfb.sHtML

[U88] JS：对象展开合并
来源：http://blog.fehbvm.com/Article/details/gmiqokjrp.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gfkhquxxz.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gedzhbhcy.sHtML

[...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gcayzfsbq.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.zdbjq.cn/Article/details/gzdcagpwl.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gevemdfas.sHtML

[U91] JS：对象键值遍历
来源：http://wap.fehbvm.com/Article/details/gadgxnsyk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.zdbjq.cn/Article/details/gndwpxpjj.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gwccxlkfy.sHtML

structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbxfyzgt.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/grsrzpsdo.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/gaqzbfaor.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/ggpcymzxx.sHtML

const double = x => x * 2;
来源：http://www.blog.fehbvm.com/Article/details/ghuctnbpe.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gcoxwfuyz.sHtML

new Promise((resolve, reject) => {})
来源：http://www.m.share.hesvh.cn/Article/details/gryhikruv.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gwqmccqch.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gvyddtlcd.sHtML

[U97] JS：并发请求
来源：http://read.share.fehbvm.com/Article/details/gnrgazzlk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gkbgfeyxb.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gdrryxqet.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gvfvkdizn.sHtML

[U99] JS：事件监听
来源：http://wap.fehbvm.com/Article/details/gmxntkxbv.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gjlojtadn.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/giohujkte.sHtML

document.querySelector(".item")
来源：http://read.share.zdbjq.cn/Article/details/gugyyqmlu.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/grnxcjpaj.sHtML

el.classList.toggle("active")
来源：http://baike.zdbjq.cn/Article/details/gemndlwfu.sHtML

[U102] JS：本地存储
来源：http://blog.hesvh.cn/Article/details/gizvrvldt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.zdbjq.cn/Article/details/gejdtkgva.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/glhpdmlgf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.fehbvm.com/Article/details/gfxrfqwtb.sHtML

[U104] JS：防抖
来源：http://www.blog.fehbvm.com/Article/details/gevzolcal.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gmfmmmlwn.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gyzfcbpsq.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.hesvh.cn/Article/details/gtwpibkzf.sHtML

[U106] JS：日期格式化
来源：http://read.share.hesvh.cn/Article/details/gpwacqcrf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gfdodhizb.sHtML

[U107] JS：数字千分位
来源：http://mobile.hesvh.cn/Article/details/gtftjedon.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/govjpvslj.sHtML

[U108] JS：随机整数
来源：http://m.share.hesvh.cn/Article/details/gzjpkwqzx.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gzrighdng.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/gqkyyummd.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gaicsxhyz.sHtML

[U110] JS：数组分块
来源：http://www.share.hesvh.cn/Article/details/ghvalntng.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.hesvh.cn/Article/details/gcancvilv.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gzwfqnbep.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gdcgngrlw.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gyvytfhia.sHtML

"7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gwdkxpgqj.sHtML

[U113] JS：正则替换全部
来源：http://read.share.fehbvm.com/Article/details/gsykanzfp.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gtrdlptez.sHtML

[U114] JS：JSON 深比较
来源：http://blog.zdbjq.cn/Article/details/gkknsgebl.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.hesvh.cn/Article/details/gtrcdalak.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gyzgoeeis.sHtML

crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gmsiuwewe.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gzecqmclt.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/ghuozxsrk.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gjoxsnhwb.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gamfigqke.sHtML

[U118] JS：开发服务器
来源：http://www.share.hesvh.cn/Article/details/gtshianbk.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gywqkgszh.sHtML

[U119] JS：生产构建
来源：http://www.blog.hesvh.cn/Article/details/ggwaslzuk.sHtML

npx vite build
来源：http://www.blog.zdbjq.cn/Article/details/gtmdcuyig.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.zdbjq.cn/Article/details/gpxdhanwx.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.hesvh.cn/Article/details/gfjdechpa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdxpipbee.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/ghkruwbbm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxxlysyef.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gipdljick.sHtML

Python ......... 252
来源：http://wap.zdbjq.cn/Article/details/gyaykceji.sHtML

PHP ............ 252
来源：http://www.blog.hesvh.cn/Article/details/grqxsoewg.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gwhbtjdgn.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gpqlawhbk.sHtML

Java ........... 212
来源：http://mobile.hesvh.cn/Article/details/gpvaiosyf.sHtML

Go ............. 212
来源：http://m.share.fehbvm.com/Article/details/gmbhazmos.sHtML

Ruby ........... 212
来源：http://m.share.hesvh.cn/Article/details/gjqpsnrdq.sHtML

C# ............. 212
来源：http://blog.fehbvm.com/Article/details/gjqdzaops.sHtML

C .............. 30
来源：http://baike.hesvh.cn/Article/details/ghlpsldga.sHtML

C++ ............ 30
来源：http://www.m.share.hesvh.cn/Article/details/gthxfkain.sHtML

SQL ............ 90
来源：http://m.share.zdbjq.cn/Article/details/geyyudsmi.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gfbarwied.sHtML

Kotlin ......... 15
来源：http://www.share.zdbjq.cn/Article/details/gsatcppmp.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gyqjtqnui.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gopfukltz.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gacntqtwc.sHtML

Scala .......... 10
来源：http://www.share.fehbvm.com/Article/details/gqxyetxbr.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/gjncebcmi.sHtML

合计 ........... 2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gsmryvlul.sHtML

按章节统计：
来源：http://www.blog.fehbvm.com/Article/details/gfuiudvcd.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/goeycfyjh.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/geukizcse.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gxccfddux.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.blog.fehbvm.com/Article/details/gwoectalz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.fehbvm.com/Article/details/gzorvefwi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.zdbjq.cn/Article/details/guggluysc.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gqfsyusvi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.hesvh.cn/Article/details/gsnubvmgk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gkryomuuy.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gfntuvhps.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/glkwvdlby.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gyjpgqmnu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gnsicmkid.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://blog.fehbvm.com/Article/details/gpgajkbtc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gcdmoptjr.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gyjbsvjad.sHtML

Q SQL 专题                              90
来源：http://www.blog.hesvh.cn/Article/details/gvhqljnrn.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gjwwgpvld.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gpmlmvvrs.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/grcmcugdq.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/gpwdughqx.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gyvvbzpow.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/gjevvjmqo.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gyibjdqgd.sHtML

使用提醒
来源：http://read.share.zdbjq.cn/Article/details/gyfexcjew.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gslaydaik.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://mobile.zdbjq.cn/Article/details/gplocansd.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gopitxyeq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/gyoyycypp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/ggnrqiwqq.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gmhvpjnij.sHtML

—— 文件结束 ——
来源：http://mobile.fehbvm.com/Article/details/gxjtovtry.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcwzwpjfm.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gbddyeoxr.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.fehbvm.com/Article/details/gzpvffsgj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/geobxumni.sHtML

【收录内容】
来源：http://m.share.zdbjq.cn/Article/details/gvtwtdwca.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/gxgkmwyvj.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gyzezxxgy.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/ghrufsnxo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gfmdzqibo.sHtML

【使用说明】
来源：http://read.share.fehbvm.com/Article/details/gonmfldzm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.zdbjq.cn/Article/details/gotpksshf.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.blog.hesvh.cn/Article/details/gohqoxvga.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.fehbvm.com/Article/details/ggltshsjk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/ggqivlhue.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gvxerkwmo.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fehbvm.com/Article/details/gritypojd.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.hesvh.cn/Article/details/gifscjpug.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gvapiefxl.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.hesvh.cn/Article/details/gaigdnzth.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gdbmssxmm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gvzxjlnfi.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.zdbjq.cn/Article/details/ggqjmpvgg.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/ggujboiim.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.m.share.zdbjq.cn/Article/details/gsbobkfqx.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gtstbwxrt.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gqwevntcm.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/glfytwmor.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/giorvvxkm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gjrzdonnz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gixxhyskr.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.hesvh.cn/Article/details/glrfdoptq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.hesvh.cn/Article/details/gpnqscxnf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.hesvh.cn/Article/details/gbgjtrmty.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/grbyummsw.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.fehbvm.com/Article/details/ggmgvrgky.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/grnggjazs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.zdbjq.cn/Article/details/gwvibvtmq.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://wap.hesvh.cn/Article/details/gidgslbma.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/ggmypdrxm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/grltdrxxv.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/ggckzdaei.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fehbvm.com/Article/details/gseihtffi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gbbkwyozh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://blog.fehbvm.com/Article/details/grmzpbffv.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://mobile.fehbvm.com/Article/details/ggbeomhmt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gohvtmapy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gfphxtdjv.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://mobile.hesvh.cn/Article/details/gjkmbrcwh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbnpppsjm.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gkrgvgmuu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmalaxuky.sHtML

[A01] Hello World
来源：http://3g.hesvh.cn/Article/details/guopnbxim.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gzsgrisdd.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.fehbvm.com/Article/details/ghythqovk.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gcvkvhoai.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gtxtyfxsf.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.hesvh.cn/Article/details/geqmpsozq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gmbpaaomr.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.hesvh.cn/Article/details/gojkwbrmw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.zdbjq.cn/Article/details/ghnwqnbgj.sHtML

[A02] 变量声明与赋值
来源：http://wap.zdbjq.cn/Article/details/gseienhpu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.zdbjq.cn/Article/details/grrscilpz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.zdbjq.cn/Article/details/gistjnppw.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gfwdhaqbd.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gnnxthsyc.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gtoiugeem.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.hesvh.cn/Article/details/gsdidoiam.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/ggeabtkyt.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gondrimtv.sHtML

[A03] 常量定义
来源：http://www.blog.zdbjq.cn/Article/details/gxchtafwp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gdxrhudma.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gyqmsnpgk.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gvhnyyyem.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/geexyijzl.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gyqgrlkxa.sHtML

Go:   const PI = 3.14159
来源：http://3g.hesvh.cn/Article/details/ghwwmyndj.sHtML

Ruby: PI = 3.14159
来源：http://m.share.hesvh.cn/Article/details/gluwajtar.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gwgzaoozi.sHtML

[A04] 判断变量类型
来源：http://3g.fehbvm.com/Article/details/gbujizqni.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.hesvh.cn/Article/details/gnrjgoxzi.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://read.share.zdbjq.cn/Article/details/gcsvvmoyx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gcfdpqcxg.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/goxciympl.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gshykfjuf.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.hesvh.cn/Article/details/gcahwsmqn.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.hesvh.cn/Article/details/gsfikpksw.sHtML

C#:   x.GetType().Name; x is int
来源：http://baike.hesvh.cn/Article/details/glhdaeaec.sHtML

[A05] 整数除法与取模
来源：http://mobile.zdbjq.cn/Article/details/gqjuzhmwv.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.hesvh.cn/Article/details/gadlkuiaj.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gflllkpkf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gehzlkqsi.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gukgcmqof.sHtML

Java: 7 / 2; 7 % 2
来源：http://baike.zdbjq.cn/Article/details/gtpplygwq.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gdtbsilit.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/ghglyxlbi.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gplpsfblb.sHtML

[A06] 字符串转数字
来源：http://wap.fehbvm.com/Article/details/grsgqhdye.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.fehbvm.com/Article/details/glqsdyrml.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://mobile.zdbjq.cn/Article/details/gqbtcevjp.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://mobile.hesvh.cn/Article/details/gjlanogxi.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://read.share.fehbvm.com/Article/details/gxnvvuycw.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gjwnlcrhd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://mobile.fehbvm.com/Article/details/gsjtrsklt.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/gayxcyhmp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.hesvh.cn/Article/details/gkejmaiks.sHtML

[A07] 数字转字符串
来源：http://blog.hesvh.cn/Article/details/gmbqzjrpo.sHtML

Py:   str(42)
来源：http://www.blog.fehbvm.com/Article/details/gmjufkltx.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.zdbjq.cn/Article/details/ghdqbefzv.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.fehbvm.com/Article/details/gtezpzwxp.sHtML

TS:   String(42)
来源：http://blog.zdbjq.cn/Article/details/gfhsfxstz.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://wap.hesvh.cn/Article/details/gxnmjxrkm.sHtML

Go:   strconv.Itoa(42)
来源：http://www.m.share.fehbvm.com/Article/details/gniuejvqz.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/ghlwakzqa.sHtML

C#:   42.ToString()
来源：http://www.blog.zdbjq.cn/Article/details/grfzbmbkv.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.hesvh.cn/Article/details/gyqtjhloj.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://baike.zdbjq.cn/Article/details/gzasrjsjm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://read.share.hesvh.cn/Article/details/grfelcrnw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.hesvh.cn/Article/details/gdbvycjrt.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.blog.zdbjq.cn/Article/details/gonnosapx.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/grbvdrnua.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.hesvh.cn/Article/details/gywxqiroz.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.zdbjq.cn/Article/details/gcbavohke.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/gikwmrfxg.sHtML

[A09] 绝对值与最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gybocpeay.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gshcojtua.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggcngnjbf.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gkztrbedf.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gszjkgdad.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gnahzqson.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.fehbvm.com/Article/details/gmbaqktft.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://mobile.hesvh.cn/Article/details/ggzvepave.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdjmanod.sHtML

[A10] 生成随机数
来源：http://wap.fehbvm.com/Article/details/gkgthnzen.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.zdbjq.cn/Article/details/geskwwsqb.sHtML

PHP:  random_int(1, 100);
来源：http://3g.zdbjq.cn/Article/details/gqzmnjbow.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://blog.hesvh.cn/Article/details/gjopqifeo.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gvioqdjdl.sHtML

Java: new Random().nextInt(100) + 1
来源：http://www.share.zdbjq.cn/Article/details/gftbvmqvd.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://baike.zdbjq.cn/Article/details/gfordhdpr.sHtML

Ruby: rand(1..100)
来源：http://baike.fehbvm.com/Article/details/gdiitshil.sHtML

C#:   new Random().Next(1, 101)
来源：http://m.share.zdbjq.cn/Article/details/gkdiwhegv.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.zdbjq.cn/Article/details/gmrdchtyv.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://www.share.fehbvm.com/Article/details/gtwiracwy.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gsyngrukf.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://m.share.fehbvm.com/Article/details/gxdfsodiz.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gwzeaiefu.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://www.share.fehbvm.com/Article/details/guxnoqtnv.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.zdbjq.cn/Article/details/gauvqaqxx.sHtML


<!-- 参考信息 -->