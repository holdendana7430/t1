代发 wailian999

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2hcupnoog.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2mnqhvuuv.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2qvbhaipn.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qkruscrz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2eivsnikp.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2cixwcudl.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2zrpszcyk.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2zwsfnnrc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2qteeitjt.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2dqtnxosi.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2ipwbegsl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2htfmurpg.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2yqhivzuv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2igtdshtz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2xeoxejvf.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2iekhvwoa.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2azsbozrg.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2gomrzlbh.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2fipujvnw.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2rpuwkovh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2riguacwt.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2opytftdw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2mstnqznb.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2defrqwwt.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2jeijkwnf.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gpufnqew.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2qevspydy.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jspibhoz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pssedkpg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2kmyufqhx.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kykoqlnk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kstrhelf.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ygubdunz.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ywsihrcd.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2iemrynix.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2fzggvova.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ppcomsjt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2dfizastn.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xbosvnfg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yzcuvuhw.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2sbdpoiea.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2eyregpuu.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xmorlsvb.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ramotnuh.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2lajecfom.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2wsqwtssf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2ijkfffdf.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2wvdgpqbu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2dbonxxka.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zlqkjtgo.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2cpysqsrb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2zcqesnmk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2eackdcmm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2ottnnerq.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ybqnedct.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2zfbqmeim.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ggmobjcl.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2ynkusfrx.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nfxgfngw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2nknwhlek.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cdljtyke.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2yzdskdyx.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2wusklkkn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2druivzqu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2mqgmjnqy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qhjnmbvb.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2txupbevb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2edsvznrh.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2mrinkrwq.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cflysitq.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2qilfkaga.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mkffwboa.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ypvgpnmv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ktonnrsv.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2dcctmmim.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wwywzguk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gpocnboq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ljfiwcve.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2oyzblyvh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2grkwhdhd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2spfvqwpw.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ocqysbsc.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2zodtnmfo.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2rjfwyxoy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2pepeoeai.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2lijsvync.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2tuvptrws.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2anrfryme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epczwkvi.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2ybkpzfse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfgkvfkb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2uhtykmqa.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2htezdnfy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2ehhpkyzp.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2dulrcosm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2ishzpwrg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gesejcme.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hefyyowp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2gencimyh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2hfkdzvwn.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2rbfeljju.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2klsngkwv.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2jzulyqhy.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2sghkcsao.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2exqnbsng.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2crffjnqk.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2bhqzczjm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2vubaakml.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2enshuvfu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fyjesoel.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2tkvbynfz.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2dgvdixpi.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2cosseuew.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2swuzpinx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zfcazkzc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2iifdraeo.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2xfvecjpt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hvyvxtbc.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2mzqbuooc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2dwcelzcr.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mvtzgshz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zomntxsf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2amvhfyix.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uiaqewxw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2elunykvq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2byxzalbg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2apgsaclp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qhulwpni.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2hjxsjjhr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2nhuqhfqr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2reiyulfg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ihyoxsyf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2bwkobqok.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ohifenfu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2ltjoeecm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2thwdeedr.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2iekufxny.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jnzasbah.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2mqzmpjnv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ukzgiztu.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ibpndjcm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2qzcrfzve.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2nwaydcxn.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ygtxoxov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpuiojay.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2vcrbagxg.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2uwhvbayq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnmlcbxj.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2svvlfmjp.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2iilaczkx.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2gwzsxhfy.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2kmmncayc.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2mdovuexd.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2vcchrsqi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2keoehxyo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2luvpkotg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2rjyfhgxo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2rfrettik.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ygnuvkqh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2qqurwrix.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2cjvhwsnq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2edweipdc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2vsqvjjpa.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2uabtgbum.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2pvfedcfw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2xkterapt.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2jbsbkezz.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2xbsrznum.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xoxlpzvm.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2enenjrqj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mzcpwvha.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hpimlnpx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2dmgirfxn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2hnqrduiv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2emwjzzdt.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2zxxflsmk.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xxuhuflj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2jpwmwxwg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yytjgfdv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hcaltzab.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hnqhimfv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2enrrxwte.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kcnhirvm.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hjwtsbxz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2doqlwxma.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2wccdukpe.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2oztxzslp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2pnjvbjkp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2figrersc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qlbkuexr.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2drixugbc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2yaarjtgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfdblovl.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2hdzaukwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dootpgjx.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pzcosgbs.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2nnalkdpt.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2yhhiyfef.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vlgwmhgh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2vezfjxfv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2lbapjyyf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2djxpsaik.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qrdwlnpt.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2auunqkyf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2lgolqkvg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2wjyculuo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2yugbrizj.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ljgkgsec.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2xcegmkut.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lhkcwjfg.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2udlvnvsw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2pgkvsybu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ugwigivo.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2hshdtmrt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ziyqehun.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ctxyhzef.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2sfxbfirl.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ycxsdffn.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rwyrzkrf.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qgqaniyp.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2botudpre.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gpakducy.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2jplryqeh.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ydjyidyp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2afbxovzj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2kmqwokea.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ktkiditx.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2ztxxpffz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ktjucyfr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2qcojvsqm.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2ftgcbxuh.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2gsuzctqy.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2oemppybo.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2metzkwfy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2awfhyfwg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2gcbeaqwb.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dtpdmrwo.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gdnydkba.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2egihogcr.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2moasrjio.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2yzuujvlp.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ancuecug.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xywqrfbo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2uzjobmxy.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2vuaqynwv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2umllbxlh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2jmyjaakc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2uflaionl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rkeqqvyl.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kvmvtadb.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2fcegolrq.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2fyuatprx.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oinvrcdj.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nhpuedqj.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jofuarjp.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2hxqcdpqk.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2ioiggclp.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2kfotbmbf.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2rlerbvii.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qebblald.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2reqrmuzm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xlthhcsj.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ecbqtiur.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2tymmwsbn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2loboclxx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2uqfdepfx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vrtdltdh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qlwocbyu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2auhhbfyq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xskbqgfd.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gxgaobkr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2biugrfbm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bivvmjso.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2sfuzggis.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2elcfptbb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bwsmlzgx.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2mmaunqqj.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2djzalyiv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2alhifhjx.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2rzixmpra.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qoipttwa.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2mjfxgakt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2xhlaidsg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2xqpnjlfx.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2pinkpzcz.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ehujqptq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2acknpgkt.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xyadccrf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ucamikyh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fkhjafgg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2umxpirah.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2wvciidyh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2emgyoqlo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ffbpbgbh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2boqaomse.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2ivfvehgo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2zhzpywsu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kpiafern.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wylqdrkz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2chniqhjc.html


<!-- 参考信息 -->