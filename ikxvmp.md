代发 wailian999

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2qlruxzwi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2dzvemzjs.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2uxarawpf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2miiehlrc.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2sdouozjg.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2uyorudlq.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xaphwwkd.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2egpjdwra.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2cyflxkqu.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2bhyoroas.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2blmmlvvf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2ngajwsxg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2kehbpgbh.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2evgdndla.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2kdxchdqc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2emgahmdo.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2pmuysfoe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ebiudfzk.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2eqppfyon.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2favrhicd.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2hksegmov.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2rwffhbzj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2jplecazz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2pwcgefww.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2tbmipoko.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2rdpjsrcw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ycspylar.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2oucmutel.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2eaznnsgg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2siwicamt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2idfujhvc.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qjpnreit.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2kvcstieg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2ysqkroga.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2gwltehgs.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2esuipiex.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2zumxigdj.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ofraenbt.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2bkrckuzn.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2epsxbvrk.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2vymuwteo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fbdnmlyq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ltactxxw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsroqjoi.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2amvprlrd.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iacqwqav.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jntvtcnx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2bwrqflee.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2bdcrpoua.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ycpcnyoi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2juymauwh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2gvjgamhx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2kjuqtqmo.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2zeeuapwb.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2emwasbkj.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2nkfjjhzm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2pbdqywbg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2bdacatmx.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2xgutopep.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2efvbracn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2kbbdkdil.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2khzjniul.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2arciqdpa.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2jspyjvzq.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pbcfjdlg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lflzahpz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2lqqkxzza.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2dtmijixm.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ozldmagu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2unlcbzde.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2zlvqdvsb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2tyjwaeij.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2qjqxoorl.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2unihtvqm.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2vxqxaydp.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ighsubxc.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2vuxhbdgb.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nyeqwvpq.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2nqokaqgw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qppswlwt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vnfdcpjp.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2illeitvg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2nwyohvke.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lidhslzl.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2dyhyfqpt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2sokzfqrk.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2zkhehngp.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2snsichsf.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ppfkosgz.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2sbizxcab.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2nvpqidac.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2cvmiskjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyhsdcsf.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2qmjybxyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzhgymyb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2mxtxbwki.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ccmrwdxg.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2rjfnvkip.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2fcqolwjd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2yqgwoofs.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2rsjfrawh.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2lveadleb.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pchndhuu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2waizlxjv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2swtkeavc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2slnejzxp.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2wwzulvoc.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2jbtforpq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qovpwbdg.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2yewwajie.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2zkguwuls.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xkxkgexo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2vmnvhnzl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2disukbbn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2caoazwdy.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2crtkmtxk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mynrqjuo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ltblihvd.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ndkoentb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2uqhtrvsk.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ttzfvlbw.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2yxktwsrx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ugnkndss.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dkxtlnnh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2apdolqeg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2gnokxnnm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2novctjjj.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2febgcdrp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lyzpnjoq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2geuefkzp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2bnwfgsoa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uylbpavw.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2oisbmkvw.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2aqycizfe.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2pgvuvvst.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2iijupbkx.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2rgfzqoea.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dvagjuoo.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2wywywswb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ddcwmvnn.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ghgwzonk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sbsucrxs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2bynrkcva.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ixpvrtth.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2bhshilqj.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ekcrobki.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2cbvlpnqp.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2wxybldtf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfiydsnk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2mjutzleg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2truzzddq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prwoxlpf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2cflxsldk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2aupatwba.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2urxijzbe.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2dsqnodre.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2vfxknmrl.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2kuxpauoc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2jmjwyxcm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2mwjmbyhe.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2whoavtdp.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2xxygopyc.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2bvztguif.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ipqrhzxg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2qopxnnxh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2levrzdlw.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2occjglwo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2wjawanaw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2slpzozbw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2uyysviwv.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2bdqaagop.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2kfvtihgy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lznysxum.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2zkxezjjv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xojahruf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2yqyiiyfa.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2aumkdjwi.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kieuhhpb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fpqusjtu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mxjhtnhs.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2syhyebhc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xvkyxxzw.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dnpqqwtx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2loogdnle.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ulthxhao.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hwewirtz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dosdtjkf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yyvbccbw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jxqaquek.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2krfkyffo.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yvhtfecp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2yqrtvszx.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2yvcrpfpg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2nhkvrefi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2qvxilqth.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2gfuriizv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxmnyzuh.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2pzsujqhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hclsuojl.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ibnckhgg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vulddkud.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2olxxcsck.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vrvyaguo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ptmuotjs.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ugqeompx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2kuhiulhj.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2dtsbtjtu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2nzdmjmdp.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2neezpiyw.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2fspxvxwq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dpyjauyc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rblyvhfj.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2yaefpalx.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nbjhendl.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2pzayqcxt.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2otjwkfuj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hulmyrny.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2ocookiny.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2aqawgbka.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eattfgcp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2yajoykzx.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2crgobhjx.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zxktvazi.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2tklntdnl.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2kwgogxca.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vkeyacva.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zjewwfiv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2mgvrklxk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2oqrnuhux.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2slwtadru.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2lwiqasto.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2fqzkxdpo.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2vuibywhe.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2zcfiempy.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2koaiuuut.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2ilzrrihp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2gorrotid.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2anpnvwek.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rdfuqdtl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qrmboqdn.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qalslfmv.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vydimsut.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2coknjjjb.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nhtjphnm.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nprkrybn.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rmdpxnxf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xxggswho.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2pfltytxx.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ssbfnird.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rddqlxgl.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2djkyfrqo.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2xjkzbbpo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pdhqdike.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ysagmwmi.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2adbwdaxb.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2eathoelt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2xpmpttcy.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2dajtvsas.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2kyhluohe.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2twqtekmf.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2tcogdiqf.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2qgmnhwiw.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2sjytgaxy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wbwjgxbz.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2hbfovpoo.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2htpjnnoi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2kqljnehg.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zmrukqmc.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2crzasway.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2vjvtnrbb.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2utxsysij.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kbzbifpu.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uppzomvj.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bbydxhjl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vlgvakzc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2qyiuuucv.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ienbsuqq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2gzwhnqlt.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2gfcvpzqp.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2axpbkpol.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2zmtabezq.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2okaejsra.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2jokiihtk.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jjosqqlt.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jadcuebc.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2aiokuhhd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2uppxrnvk.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2jhnsgzma.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2knrnmvmt.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2cpaoabrm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2lnogihdz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2alvilrfd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2iybbxouq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2chyuwmaf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xxwppqhk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2wrbeavun.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hxtmtalo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ptjuszbh.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hmntjptf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqfjhdrs.html


<!-- 参考信息 -->