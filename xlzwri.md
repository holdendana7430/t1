代发 wailian999

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2fnlfqwey.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ylgsdspz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2ydvymwpy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2fsyzbxml.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2ypyvqtub.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wtdelbjf.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2juhndblx.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ojkpppym.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2truaswon.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2osgcxzhc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2kmttsomk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2qdjduvcq.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2sjdmaonk.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qonrdsso.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ooyqtmuk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2pidljcws.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2zvzzzlwb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gkegtxdu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ywtdzfta.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2wtlnsrza.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ojvqtsgy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2wkdwzanx.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2yktppwgi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2jucbnhwi.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2bjuuibnk.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2jpfrpupq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2hvydznbg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ynpfeuoo.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2aoghtqar.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2naqlzqii.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2aqxylgqf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oqgiaohc.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dakjmnuh.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ztmddnyz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zzqhjxfu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2uwirrkfs.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sqzmerpf.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2ocsdiyrl.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2hxuunkje.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mkliljrr.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vqroyjuf.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2qttpotwo.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2lfcidphl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2trdkqvwf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2eeltyhve.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2swkuxtcc.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2dkcnsgha.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2rffaycqc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2mbpltbod.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kmcpfjlo.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2mflpvwsq.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2xtxoakmi.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2bzhmamfs.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2ipmxtfgz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2ahjizvhg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2uhggqgpj.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2bstsepnv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2hemtdkxj.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2kerelzqh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2edktlfna.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2hriicikc.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2azcxnvdc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2whtilbzx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2smmahuza.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rtcrtexj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hldkxxix.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2mlqcziwm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2oupgnrvh.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2xpysydab.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2uywtsorm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2bdlyyrqx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2dfjhjuch.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2hnielpny.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2pcfjtxub.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2czisbgxc.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jviycare.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ksngrozv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2btrztyzo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2vyytyxkt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2meykytnj.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2diqkvywv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qjgpqrey.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2gcxhalph.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2seckzuww.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ddbgkkrr.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2qzesvhem.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2fzxhzege.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ewkzxcdc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2mfdjusyt.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2nemdhzhb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jxzidrjl.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ntlitzbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bummvocw.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2avktkrir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtolseop.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2fvzelwbd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2uwjbbppi.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2hxojmygb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2cnkjauec.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2wjdhvgdo.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wizarsot.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qtdkeihr.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2igsgkoab.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2wtkwoika.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2zefhwasr.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2tewikpue.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2jddmossr.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2bbfqkgav.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2lcvgmiza.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2pflpbjdq.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2mpwholdq.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2dkgoeuei.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zkiekgot.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uscfsigb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2elytbywj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2phfmysgv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wihqweob.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yvdzckkl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2prlkiqmc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2mhbarnro.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ybkznvbk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ylitnagd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2twyifjxu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2eprqtkph.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xmmpkowd.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2hjntaids.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2krdnmnpg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2effoivxx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ypbvzqoz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2bfgfqdrq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2cveotmjk.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ruganbri.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2snfydvgh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2rilzxqaf.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ppieimsn.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2sxmztfyb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2bdeumsfa.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rqucebta.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2nkwvwbwd.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2yygremwo.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ipxugvmb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2dslwnjzz.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2qrgkjcms.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2xcfkqcqh.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2kgwmgtcj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2pdkkdvez.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2ghrrzjel.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2xpfofsnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vflmbjci.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2zqfngcmu.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2tvatipbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwlsxzuz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2bpohnguz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2uogcchdz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2xvlhspul.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2fptqbizx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2jrekacpb.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2gwxvsnwx.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2rcjkjgwb.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2nkbhkgod.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2rhhnzqez.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2qqwxxlab.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2zzxgcstn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2djajmzyk.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ylsycnkq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2febnckxe.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2cdsorwep.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2fuihobzz.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2ufyeafgb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2mxsgxeqg.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2jjlegtkc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2xnfcpslz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2owbsjnbg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2hiddibrv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wafxpeen.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lofhduem.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tbhpoaey.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hxbswjof.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cozggkee.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jniqddfr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2taqdkulz.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2btlmbnvg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2uwlydbpv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2injizrmo.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vdxduohu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2frcvksed.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2quaaugpa.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jfvqhpof.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2shdjrjzr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2mnfttuhw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ynccjzxm.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yusnrjvm.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2zzuyocyc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bwtgryjy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2svuflewg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ehhgddqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xxlrdafz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2tmgpncbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttjabfpq.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2jbybxgfr.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2swziunti.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2javksdzu.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qmhkofmj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2upzijbrq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2htnzocct.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mdcsxrkt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2swoiiomo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zsawxcnn.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2kagswqgr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2wnrgrlui.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2thncxygf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ddsqtown.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2reiclrdx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2thjxgwfx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2zglreeim.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2bwqqoujt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wooprtlu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2xecfehqs.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2nvvtanna.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ujqqsmjw.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gsvqsjgk.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2keejgcpz.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wtaxqgsm.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2vcjaxbsb.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2asgwacya.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qyuuaazp.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2csaiwprx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2ktucjqfy.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jwpcrwyx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jphshmnv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2zjvtowav.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2hotdcyep.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2wchsbxrq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2cxirwdfw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2yqgkdaxf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2jonwbxot.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2qhvakono.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sbzsxqza.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ejvfnhxe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vtpobprc.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2numaunpi.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fhftmnjt.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cndbkezq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zutvhotj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nfhpwnll.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2pzlkzgbj.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ihqekjly.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bcjgltqc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2uyduxfjq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lgcwkgwa.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2kefklmoo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2kbohafas.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2alhhcraf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2leclncvu.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2mesrnarv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2pnkgyufz.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wyjgdsdj.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ywbfauda.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yxjhwmac.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2wncknzzw.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2jepmnhyb.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wpfixqyc.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2qxepcevm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ztfwzses.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2dqydhzzg.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rqhmsgvp.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2uznqlpkj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gtnwemvx.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tzrbqboh.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2tfjwjnnr.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2smnjduug.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ixnxecya.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2toeyallf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oreirxme.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jwaqgkur.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uhankrgp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jqlszlke.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ykvtpeln.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ymttbrsw.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2epulbqoq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2dezujzun.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2fujemxkv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2wlgzdoab.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2npwidual.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2iaiqjsrd.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2yrrycort.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2zeunfwfm.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2bjmleink.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2notkkxoj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2zjcwvdfz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2aafizcuc.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2afaaimzz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pmppmmol.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2arikghtx.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2shnlknow.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2oekndooa.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nvexuwjy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mcprbdbo.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2twchoyjq.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2iuxyonbi.html


<!-- 参考信息 -->