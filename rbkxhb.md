代发 wailian999

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3bdnisnln.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3wghgqrze.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3oorojolr.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3kpnhszfw.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3aremvbsa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tepfzlol.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3gcqhznjb.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3juqiqtse.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3eondzpjw.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3maulbkcr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3crovpiil.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3uspxdozw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3cijzyrmj.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3mdroozka.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3fhvwhpax.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3pzurvpcg.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3lrpppwmv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xsxecshf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3sonissoo.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mlfyetqp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kzduuvfm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lsvqzeew.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vcmarsoy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xzuuxbkz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3xyvvqbbs.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3djyobyxg.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3zjxmgoqi.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vzkixwue.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3mtttdsyq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3iorguuyh.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3yurzhxsu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qnunwvjy.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3edporrsj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3unljnoxw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3fiduhuwj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3svxobnby.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3yvgzetai.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3mapexohu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3sarvuzya.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3nsspkbok.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3diimttri.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3tboztidt.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3dnqfuvgl.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3uxspmgzz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3kjutgltc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3jbtsjzvp.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3qcqhrxeb.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jocbfzrq.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3frhahefq.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3aamotxyx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xyalgjfz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3vnrtarkz.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3muaoihwo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gdbcvhol.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3cxkkvguf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jnaizbwr.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3rfptgtch.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3llaczphf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3igfoprcu.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3vormgfle.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3huhdywmb.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hiakabaw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3smsklata.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pdcjmjcl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3yavsmtyo.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xyugwoax.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3ycdjseyf.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pdsneycs.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ddtlaghv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fbpuaaum.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3njguondt.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfovgsgm.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3buadmcll.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3powqpmph.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3udveybsq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3hglyybeu.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3stlepnnm.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3zbsjsapw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3jzkhukad.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ezbvfeog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvawfoub.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3nmcctzuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjfmfqvg.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3rtnkievt.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3tptolaag.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3ugssfnqz.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3dhxonjkw.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3wfmcigmf.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3rofacaab.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3lrbktbib.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3sqysmwrm.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lbrkatfw.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3qrtrjaga.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3bdxaikin.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3pocrkqlf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3mujluzay.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3zeszmwkl.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3icqkkvif.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3jteafrui.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3arqiawkm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3nsedlimx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3orwltffi.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3qfeemzft.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3rhmuakfg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jfddxziv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ynobbdav.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xdgirejz.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3lmxuoqey.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3gcnjpfty.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3oojomfyr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3mbkiwhax.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3pnguthnq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wsyexglf.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3gunzutkj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3bccosmai.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3koaimrkq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lwqhvnjf.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3rfnxmfdp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3nzbevddq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uuegzumm.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3edmvnmdw.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3fzrafuad.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3dknzmjow.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3afvmrwox.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3egpqipyr.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hyyohhwh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3kpcoddsr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3upvxbwdf.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3grnmtlpi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xvgapmaq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3mrthwwut.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3jyeuxcac.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3pftqygjq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ugjiaasf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3vyntbysd.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3nlsuhore.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgyaksdl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3iloauueq.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3uhkjlaoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3savbblgv.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3lrbwfexu.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3dwmwxfef.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3aydushat.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3xjpnbpkr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3bimuvfxy.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3tczeyatm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3kmhlbgxr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3raobtdcb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3rpntijyn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3gnezbztn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3fcwitwgt.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3dkzgltdg.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3spbzggjw.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3pveuzlbn.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3nznpexsh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3okzngmmv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3xjbvucjh.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jhvbbxhy.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3kjojbcgx.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3avyeqfkb.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3uvdilnux.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3emfhwdgh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3whpmykyb.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3oklegfdu.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3plyrmbar.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hhpejhiv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3voekugaj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3zshbyzqb.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3kbltjvhn.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3swnvzbde.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qhqqqohm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3otcpjtzs.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ujvtpcqq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3nqgyrkjl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jawuvjfv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jmkempnt.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3vxjlfvwn.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uedelghn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3onjrigas.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bbsmijfd.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zfwmuljz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cpapjmps.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zwhifisw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mkbcfqqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlflpzal.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3tffpqgtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tofhqygs.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uplmlxax.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wlrhzbxu.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3adbeppur.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3olqrlapk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3hkewkxdl.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mamurmsw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qfeyufwt.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3fnwovskb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3juarcfqu.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3eylkfpgb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3imahfstz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yeqtyugr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ndlxkyju.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mrcfqmnf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3yrknebll.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3oynaagmz.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3opvjdvyb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zndmxbuk.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ygufwzal.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3sbvnkumd.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3aiicersx.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dpeczdtt.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lnypoadv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bvbpkfdt.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ilpleboo.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3rpmhdwwq.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vysixrxw.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3rkdzwtsv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3oidpyiga.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3cuatyphh.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3yusdbgtj.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3anucepwi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ihcxfegc.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3zlkbxhip.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3xkcbpfff.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3mhxwdlzv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3wknjdbtw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3ozprawjk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fmsadjkq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3uenzajmd.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bolxlptq.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zkmaflzt.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3muzofgsc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mxvmyqkp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zjaszczy.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3vsgnhczv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3whbshior.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3linkisbj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qbrkawch.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kbihrkzl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3nrjaqxip.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3nsbgvsci.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3dqojjkks.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vduelado.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mnwbxphv.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kpcerdae.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3jzidotjj.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3abwdcivn.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3qrphlwfy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jsxfdnyh.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wzulazqt.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3xllwxtnd.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ockaymaz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3lzbxpfuc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hnkximyg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3gnsswfko.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3mrmrqpmm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3dqssihbs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tfehzkli.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3avaybkxp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3eiukagqh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3kqfryylc.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3tvynodps.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fqsyqzvm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qixjfcbx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vbldgasj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3quziryci.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdqmlsbv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3kajuzkte.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3fbsfiyvr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3skoxmons.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3qxffujmq.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3vncasjin.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3fbyzjvvu.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qxqitwpc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3arjhfzoq.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3notqasjl.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ntvfjlrf.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3amaheapa.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3jgcesnbk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3hjxgdnlr.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hgfvfknv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jbjbtzdt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kvwwzahd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3rcfiyufg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3uaqisykc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3nhlqsohe.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nffqnojh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gkevaeqi.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3tcmcqyyt.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3bucdtmic.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3kepoirxb.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3fmqrfypr.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3uupqzwyt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3sxcidfrx.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rnoodteg.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3vplwnjfv.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3dupaaqrp.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3zqrvogyj.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jblztbcn.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jfmjcdbl.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qlykhsas.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jgmxdbfv.html


<!-- 参考信息 -->