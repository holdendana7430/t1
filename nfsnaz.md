代发 wailian999

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2bzkozbds.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2otgopfhb.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2bbxyjyzl.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2pydsbmmm.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2nlsqxtmn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2htlaacsv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2tljhbquw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2esyjrhtn.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2kjklqhdg.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2ykznhwkf.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zjdbfhca.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2yqyrylso.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2howxyqyz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ajcrobzk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2nxuhuqox.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jywumjdp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2giaflmxz.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2frmevoxt.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2jvmfvrlq.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2xzwwnvqx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gyzouvns.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2qggxbota.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2tfihncrs.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2kxjfmtgi.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2jguckmoa.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qjhxpacj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2mzufxkoh.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rkpffpzg.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zjgmpdub.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2qhqlouwc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ulzpvhbj.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mcrlymty.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ptzisrnd.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2cgwsfiqh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wgwoytgi.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2tgunohum.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2lgusdekc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2pvmfpocl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ibbnrbsz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdqyhjgs.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2mzgfaatg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ukvlftvf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jbjsvlae.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xshycahe.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2ughnhypp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2crpfrgtn.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2qqrmjqlh.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2anrjkbdl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2npoxeatn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2idcoinyu.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2htgaishd.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2gihtfyzw.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2nlzgxjop.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2qezappps.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2oodnsbgp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bxjamuzj.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2fibcwdkj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cjfshkta.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wdgwceaj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xjvoqmdc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qcdgmkdt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ypbumydg.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2gyenldon.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2cpehqmsz.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2rzefbcfq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2uflbdrvy.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2egzhfzhd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2aoqwrvep.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2bkcnekip.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2dmjlbnif.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2tyjntymo.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ktgittoy.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2zeimbknz.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ncqrkrjb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2xyqnsfcx.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2kbkcukmz.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ksdkdfsb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jdoourmz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2vlyfoblm.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2hblaalra.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2zotlntjo.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ikdspddl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2plxwjrho.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2dlvsqelp.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2bxbmmlas.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2lwvbiiyq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2aldapdxc.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2cteddzja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2indtmxrh.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2injaqpla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgoshgwe.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2rqdiogkq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2zzlzzvxw.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2mzjemoxt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2oaddtbnj.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2osomugqw.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2gsvziiqm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qyptrllv.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zghcdtfd.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zluwoeys.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2nxjvttqq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2yejttpme.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2blofkfac.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2opnyhzrz.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2faarctos.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2naizlglb.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2rgwqcjbm.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2oxypryco.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lwnntrnl.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lvqaglxd.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2uhbicgyo.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2jjsndhtc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dfjorrcj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2nptazcay.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2edndfdou.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2znbykoti.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2jswdtknv.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tmouldsp.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2thobhtwr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2niijfseg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sbbsnzbu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2krvyufbn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2uvphhidg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2advjyypt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2kqbpvvws.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ouhpsakq.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2copzkndp.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ursouxjn.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2vjlrtyfp.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ccyyzsah.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2jcixqgih.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2lhxwovga.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2wdnqpgjc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fzploqtp.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2owvwylxt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2enmcqugw.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2wcaailjr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zvbtiyuu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2mjfqmqjz.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2pfbdozoa.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2qvrouzzt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2wbfkugfl.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2crlgukbl.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2qkxyeetd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfifzlgf.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2ejvairln.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2qvwjwwtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ecqiiqva.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2galerbvq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2dfshoxij.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2gvjmzkej.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2msyanmyh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2evcqwtyl.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2bqoccjwt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2ilvdzbfm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2qjpsoxtb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2wrcuybsl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2twovcthw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2ptiadbwt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2mqinaaom.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2lyqduoxc.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2vlevhiam.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2gkdvidhj.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2arrarbvd.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2opjadxwk.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2dozzqnmx.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2hadbtjeg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2uqilzklc.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eodollzu.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2mwtxlnsv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gprwmwuw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qiswtqtq.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2heqhhxqj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2siwhyayt.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ctpgusma.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tkbvmaek.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ecbwltwj.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2fvyxaerd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dgrlftqi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2perxqyhg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xmggljvs.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2iyqzwewf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kuxokxoz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fyobpobw.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gvmojvmd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ocszmfio.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2seaxcbaj.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2vdmvdfqv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uunqvewd.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nxsxtwai.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rxlwyumw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qaevcfii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kanoxhzq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2nbwulsqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xavsfbrg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rnelsnve.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2tivvoasw.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2mgnatxwj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ksqmprlh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2jnjwfnty.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2vvhytfzn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2krlsuals.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2knwkzjwb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hwsxzxet.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2gggyfaus.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2xpbkzrnx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rarksawl.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tuurjfha.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gjiawdmo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2vwmwyfas.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2bwmtdbbw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2jxgjvqxt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hqzlarlp.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2bkvompfa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2xaexajps.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2eqtkbkad.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2effgtkir.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ynanlwqd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zmsiagra.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2emcjmrhw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2uwwxlkao.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2widrxiot.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2oujzfess.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2jpptahno.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tkmyisck.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2aophhxxw.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2amiiqnzy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2nglwijfw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2odmwhfvm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2mhpvwwzc.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2cdjohkil.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ccvdlebu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2hbmbztrd.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2rxuvcqkg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fwmhqykl.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wmsndiow.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2byabniev.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xuhhcskq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2notwecrf.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ywqfrmdp.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rvxcppdt.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2cbbfaouh.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2nmtkodmy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2eaolzptw.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2ovjozppe.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hngcgsha.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2moylsybi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2ckzszktb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2yimszyoe.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2mrtzskip.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rjpnuhep.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mpnpzfnf.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lmmaegoy.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tvpnruea.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2mgzqdpbq.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2trnsoqgr.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2gujnpxkk.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2lvtvtcyc.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2fbzygbua.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2grqrbfwt.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgynaqna.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2npxgvftv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2gaczwucn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2hsdidose.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yxwifpsv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2vazonwdp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xdsrrglv.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2wcmfijcc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yxzqjcii.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kqdbxtlk.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uttpdsgm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hydmhzwd.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uhfzhwgh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2zwhefuoz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2rtreptft.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2debxqnoi.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2cwquywul.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2yskbpxnh.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2hcdzfyiq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fnepimxg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ixavbnni.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qvfgbqsb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2fdrmwmgl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2dsbhjhsw.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2fmswlrnc.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2jhkjrdym.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zgpmetrq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2rxipymwq.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fgoydyax.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bgpfzznb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2meropxcl.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2kkqgoxql.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2riwwsbhw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tfkfvdyw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sgzclorz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2xajwsmgt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2frntgval.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2hrlnwbpu.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2yvnhcaph.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cywkbfae.html


<!-- 参考信息 -->