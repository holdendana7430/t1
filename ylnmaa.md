代发 wailian999

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3azctfouf.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3yfmawvdx.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3kpnkutwn.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3eejmcyjr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rmqnfnjc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3mkohaoie.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3breshqkm.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3hsnymnlg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3fxotkref.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3tixodqag.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3scndtugn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3sgpgzzoi.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3vkpdwcfj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3mpnqipfu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xpvyywwe.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3tjrytsyd.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3biqauoct.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3zuiwygcp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3tufddihi.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3xkqgzimb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3yengosff.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ylogfyje.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3amvjgyqz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3lzudgtpu.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3zutesysj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3cwmjsotl.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3raegqdva.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3xtujrnra.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ndgzasss.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3pigpptwb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3lazzwvfq.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3rteppuyw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ojpzqipr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3qnedodef.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3uvjpcrun.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3gojqftwa.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qlskdzir.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3twatrtea.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3ufgfseos.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tmnpjmsn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3euwtnrcr.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3wjsxdgfu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vxufsurj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ojrvaxbh.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jvyvpvto.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3prceolwg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3jfcdtfag.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3uwycaamr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3jvkgsmhd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3berojjbt.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3evlkqziu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugnyotuj.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3nsflvfyb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jujdofjl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3edumzrlt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3gqzhgalp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3xkvxeuug.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3brlkzmdz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ddgjucpf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3cglusjmg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3xeoieetj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3hlluanre.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3bzcikqic.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3vhnspqrt.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3dtlqwiru.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3axayrdpq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3hpyikhax.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3wxdzhaba.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3pwhsnzlg.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3titfnyje.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xvgtaour.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3xbdrazwx.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3gxjyooyl.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lliqtxao.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3wlvqezcz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3bvyczdzs.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3lrxitjpx.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hhhygdgz.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3kbzqzzym.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3rvqwantk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3srsfkuop.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3cseqiplh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3hnefnsmj.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tzchyywt.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3emtlteys.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eetxomhy.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3xzexxuiy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hkktirnt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3opbslccv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jsjsnslo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3whiubepz.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scdffzvu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3yjlcokfh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3adlhoekq.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3unjdwjei.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3yewhpint.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3eghkqvqp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3bsdcfyyi.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3rmyyskqw.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3iojzuuqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggitymvp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3jizqutwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqykjoaf.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3zvnjncah.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3aratqzay.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ulpqiynj.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3mctmoemz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3xkuebxyd.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3luhflqzl.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qpmbvlch.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rtpmdcss.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3dluvjaxc.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3gglhjbsc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rpmfzaar.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3qpvcrivd.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wwadycvi.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3klsfbvod.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3nrykuvcw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3vonixafz.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3yltqsnek.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3jcebddvp.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lwnlakjo.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3urjpbtvi.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3rbxpozsd.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3axecfpqi.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ptxgsrtb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xmavqgjp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3yfuqqezm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3flemsqzd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3znrwaqzp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tyiogvnu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3rfswlqax.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wgxfaevy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3ycfunepk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3trbkmhvi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uuvsjiyy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ebwwtocq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lactpzeo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3elvxzltd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gjlrmriq.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3tojwxiou.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3dsgnjirc.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3jxgbfwsu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3qmvrstwn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3oxyxllta.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vdogrrqg.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3stimyriu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sbidlqqb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3gaxtjdiu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uaouimqv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3ttyhbnic.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3xrxstboq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3cqwvsvao.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3wrjvqjjt.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3jvpdbvsm.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3pwjbvpbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvtmidlv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3dqraxjop.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3thibdmmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kktmerei.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3jfubzavc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3wxvtwmoa.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3exfjlbsd.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3vjvnqsak.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3pkukfqoh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3znzkwdol.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3xcrbdxdm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3jdebaqni.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3bzcpqxmk.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3kzandaed.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3joczcgrt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3lrurucih.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3vsirysud.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3witxpamb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3scbimckk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3yuzeijgd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3jeiyolrr.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3cclstksk.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3hkbqxkyj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3cizstfeo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3wrwcunuk.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3qlxaqufm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3lurfbugy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3xmuxpdlm.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nevdmuoy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zxdgxyat.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cpkxcunn.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3otuvwlic.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xmzmwiys.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vhfjppvd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3svjtknha.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3llexdjim.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tgjthmsr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uisteqiq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hhuccdea.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3liaereay.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xmjtzeup.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gzusagpq.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nbtjnvbp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3abfjllng.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ibtqlgxt.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3khpleiqo.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3trblbifs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3iieiyaxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijwnwpta.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ekpczrqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xyhataur.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3zkvauroi.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3hamfmuxp.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3xbkddsaf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mnecfvkj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ybrqkfyd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xrgpqtsu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hjfwgoja.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3xxfwyrax.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3smsdpnus.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3tsazyylg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3kedjnmei.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3teptmorf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3khhrotsa.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yzdklmmw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cyptigpl.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ogjgszjk.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3begghxkh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vupzlflr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3piksrasd.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3djddxzpd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wgoftxgc.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kxgynncd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qfkmimvw.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ppahvybr.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mpiukglk.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3flbmobmn.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yslyakfq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3cyzxsnxs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3rddzqupd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hkjmbqot.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3bkozgooj.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ldcahmks.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3jubkksmo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3fxdzuytb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3jijwugwu.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3jhhsjenb.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3znzgnons.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3xzijaqly.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aaatgmvy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qyshfeah.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gxucvdxe.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hledawfs.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nnfrieiv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uplcbfyq.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3htvhtiwq.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3kbowdphv.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3nuvbsxte.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3odrrqcmc.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rnabuuzu.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tivuhpbd.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wsukmagu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3dzclgvzt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3wgfjtvjw.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3maqqdktw.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sdevkwoz.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zkycuqau.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3izfbkjgc.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3hazfufqp.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3fceruinv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iewbhpav.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qkvuocsl.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3pbdkxxmh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3qxpmfyvv.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ehxorduw.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3arjuyaws.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjzpprpk.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qzwcnufg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3jrydwjkk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3droxzidp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fcdcfvoa.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ysbfimkg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3aerxjwct.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pmhcltfk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oufleltx.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lcvovkwb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xfixxcap.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3sahurahx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dvpbprew.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3xfubvpsx.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3rdopmogf.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qfoomabx.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pcjjchem.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3ndtfbpmc.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3cwmtknbv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3vwqingwq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3xkqlqwzj.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3puygvats.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3cclqkwgd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3cghokdvo.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3sfwxonmd.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3dfywohbd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3koyojbvp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3wiieqsab.html


<!-- 参考信息 -->