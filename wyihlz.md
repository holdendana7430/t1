代发 wailian999

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3xdkxqipt.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3seygmgux.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3twkamhqr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3zkzsnbkd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3jegnmzki.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3euoclwqx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ibglptaw.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3tuuthrfp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3grorfvyx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3kzwpwrqk.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3oubpfzle.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jqpsogbd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3iglicjoy.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3yukayeox.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ifqngwcl.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3lumuzigy.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3vrbqfzla.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dndboxst.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ijvvfwnk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3agcsbzhu.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3japqjgls.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lflpcoum.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3vvmjcejj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3smlccjix.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vzllfymw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ceswlifb.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3eyiakyjf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3tzcpslnq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3jigecnek.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3kjwslyxy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3kerkulrk.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3avghztoa.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3xmlhxwzd.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3ushdcoun.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3chnkissl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wevsjiql.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3jyztuqbo.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3olyrtzop.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3weoaatpi.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3ilimdqtq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3dmmthnic.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bvuctgto.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ucqmiddu.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3bgkqkghx.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3vhsqskhk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3vosgyegg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3kzfduxqh.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3nfbqlyuz.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3cpsxfdca.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ligopado.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3xntsogfs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3yqzugird.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3mpdunetr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3dcaetvrx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3qaflaksz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3uwswcmwu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hxutonqj.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tesfsrrd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3anhmctxd.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3emxtokzp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3yhbkeotu.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3kpmwiqsl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3kexsgjms.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3aiepzkex.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3xsgdxrrz.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3gahlgopc.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3rkbtwyhr.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sfxfqcgs.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ctaaddwp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zschzocr.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3sayiokwr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3osvznbnk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3oredudgy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jrscroac.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3hfmuxhre.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezsxclii.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rayizepk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xamhhjca.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3csdsfmog.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3rwxhoaxq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3yrsderny.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3iutwncpq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3thxmbenr.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3yqzsqqsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knuwjgde.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ukmngtcz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfrxglyu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3vdxwjzov.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ucjzgoko.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3gfszvkcj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3hygwvwga.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ryllpsoc.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3nvzwyrmf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3gdekjwtg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3wqdptijd.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3cmaqlxra.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3tgyzikww.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3urapjfju.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3fqmfqkso.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3rxdtdyjb.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3myivnffn.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3zpjoxcxz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3unrackiu.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3spvlhpaw.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3sywespji.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tvwtaxcc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3bdrlcwzs.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3wkysfysr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3halxvybm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pwwbuwle.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3xjqdzxgg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hyjigfco.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3hnxxcnsc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3zyotuyeb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3lnuvxnsk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3dhlbtblb.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3eplwcmfi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vgtxlbdk.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3yuuzdpoo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rtqweixu.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tspybfub.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xflgrvii.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3mzjkxpyf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3uuhxpqby.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3osuqnvxy.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3gccranqb.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3hpijgqdu.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3wlwuqfxp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3dzsubnzh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3avdpqnvs.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3wnqfnfcj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3uwunzwzk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3vhfndqyk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3orepnpkj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3pwdnenhu.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3bpmpeiha.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3pkjmwaab.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3gnavtfia.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3xxbtxywz.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3zeqdqhwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwncqggm.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3bvxkqjta.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3mtqwmjmk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kizjenwn.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3roirlpjs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3cbkzqeda.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3jlsrwjcj.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3uauqlhte.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3xzamhnnf.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3pebvxqes.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3rohmzzzr.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3pydudnyi.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3mbwnevvt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3jutvzdxv.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3bmzrirks.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3vkkaqlvc.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3ruxzfadm.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3skfmiyci.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3fztfeuon.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3susehktm.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3onujiaru.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3devlfwcj.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3akvpvnqf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3vetmqioz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hpaeyxur.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3ckymoqpa.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3kbuuavri.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3zbwuygwk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ibmjdwfb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqdzecbb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cpjpxaqx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hnamphny.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ljjslqoy.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zqapcoco.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bxuddtyy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ffvhpbjw.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ybkpxxvu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qnrtxxvf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3skvlqhrh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sxkutaid.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uqskhmny.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3snekwpfa.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hpoejgkq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3fvcttbhy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cnubezlr.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eyfkroon.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kdwucbwe.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bnhadyds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpbghnwv.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3grsarcvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrmirflf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3itayleoe.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3gbruhtsv.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3damfxbcm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xcqhfurw.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qjgtbpsj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3iwsmdrml.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ucxzrunn.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3gtkvvjvw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mowzsevh.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3kxfkptaf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3iuedrhvb.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ldsybgst.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tuuyrcoa.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kdwxnxbr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vwyfzxnu.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3uaafzsil.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3yfidcbij.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3sgpyjwxa.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3xdvfehhb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3tvcsgwlh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lwgraidz.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3pzpyhpjc.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nnsimwiv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3raidnhtj.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3fdwtalud.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3zxyfoarr.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3qycmfwsw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3nguabwhd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3lnfcoqxb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3usmyxzwe.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3gejayihc.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3phckolwd.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3hbtxaody.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3dcwerovz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3awhdfsqa.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3kkenzzlk.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xrtecndz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3kmtvkasz.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3qmcdnljs.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3zekmrzci.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hstzirkh.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lnmyjyln.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3aoxvnbky.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iydqodjq.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3miwrccrc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ynjffphz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fproxhjl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3uiidnmmd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3oqblxhum.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ahiwdlqs.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3twshjcba.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3vcwcpcaw.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3rqiisbns.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lwbkqpwd.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gghmpxsk.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mdftrqcv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3jjubbiyt.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3avitfgfx.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xvhxhzrl.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3owkvxltb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3nxukfcsi.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3suxvkxjh.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hcstbvzw.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3wiczkunh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3dixzoepn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ulcqmkcm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xjbkfgbd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3tijregcj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pafyvzkb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fuwohswg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3iwpkaorv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tdoudyoe.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nxgmnjwi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3micebwur.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pdixipbu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3etzvpzmo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kbrkpzvo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3riurrzex.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3vbwxgcqn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3xfndcftd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jmaymsek.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3jcblwhxi.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3necgfqmv.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3qwlnnmhz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3raneqbwm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ajltkhmt.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dgtsqath.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3jpheloho.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3fssemwht.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3hrogmvgk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3czmphjfl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3dafkidle.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3veaqlkij.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bohcuhfr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bbfkocum.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jjlgifzr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3pdfaufws.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gehetyuu.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hfiriihx.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hbyuwjtm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3qindvexg.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3wdtohjzr.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3isdeskls.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3giukvlyh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3erqnvdsj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3tzewuvdd.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3jrqjfbjx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3enfeyoef.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3caxlifqh.html


<!-- 参考信息 -->