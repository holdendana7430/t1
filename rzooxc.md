代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3ybmzpcig.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3qggadcfo.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3munmppmt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ityewdgc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yuzvczom.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wfzncmng.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3cvjxgmxd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3siwkkorv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3hsgosyak.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3xwfbxvts.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3crrzhvhf.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3osnmuhgn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3cvoegxpi.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3fnoiqelg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3mvqxauzm.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3madtmjev.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3iiszjrbz.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3tubvhdsh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3rfxxvpps.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3mpmyzyus.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3itehmvao.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3mvdjdbsi.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3uyczbgjx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3kmypmkub.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ilzmwckt.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3aqncecjy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3vhljjktj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3crjpehld.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3cdddnxcj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tognneby.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3htmmgekx.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3qqxgwkgr.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qoibrgme.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3nhgvbgxj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3hbiyydhb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3aomubmpt.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3veslsyio.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3qnabcdha.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3vakcjjbp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3giobyjxo.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3wjvyaozn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ugyuabds.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3vcluzzwo.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3eudhrkbw.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3xrmkyuzo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3hyoiorjk.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3amjlneao.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3shhneexz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3txtcxtdd.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3osfyuwqa.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3gswzdoyv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3brpuudhw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3eisaaleo.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3zqncvykm.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3cooflhtp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivkpvbkp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3ylxvfigj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dgepnlel.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lvdthpbt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3jntijynp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3swmqmhlw.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3fkixpnam.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3bpfrdcbd.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3einfmsjo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3cupzwpky.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3aqqyiqox.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3pmrmihpt.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3sopekurc.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3kqcxnlar.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3pcutsvoa.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3jgxlijwl.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3nqelepix.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3abzblxxu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3tceqfygc.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hsdtfxis.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3qkxjspny.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3alahbzwg.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3rfdertbc.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3vkmmxgov.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3jonjjwou.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3onkitdyc.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nihtftsx.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3xykqyqyv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xruyclbl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3iievwjoo.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3mdfuqadn.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3mojcvxdl.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3evpkvgxk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3nhsegugm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3clxddrgs.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3krpxnpte.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3muvaryoy.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3gbtaqlmo.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3vzmbmvmt.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3culyzyxu.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3shsqyooh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mtcrmyrb.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3axbjmqzl.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3vwzuljji.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3ccfxevst.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3iznctdfp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3vwwasvqy.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3utfqodqq.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ajyppxox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3meijehij.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3tvfwpnce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umzlgnxq.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3hhccihqt.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3bcwydvog.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3vuduivin.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3pmarcbfl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xouonqqo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3bbpuslfp.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xejiqchp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xzuinhbw.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vokjpoab.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ysjedyct.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3sobovpnw.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3sdgecscr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wajjfrdg.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3imumovdo.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3tlpusruf.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3vkwbbtml.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tyvanvqq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3grfvdlfe.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jtpyawcj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3ulgovwxj.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ylgtwtpc.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3hafwabol.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3lthizcby.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3cxmklrdh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tqdbahet.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3ejcfrnwm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ybqwhswj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ijmquhuc.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3firyvzaq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3beroofpg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tgmyrerq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gcuozgtt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3qntgkvvw.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bvahqvtl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nvzckuce.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3shoxqqvb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ykhybjao.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3vxcjncxt.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3wotiofuq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3pefkpzxe.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3zfrogtjk.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3junnkraj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ttxubnqi.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3ezqzfkan.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jhwqxelg.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3hybhobyr.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ypxphifl.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3hrkllsbp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3vulidjcy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3xkxuqgoi.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3qggaoguc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3uvpqmnpd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3mryoamio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nytcrqcx.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3zmbdgiea.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3raxennju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3veoefiku.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3tohiqaod.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3yfwenvmz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3pcwplxdi.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3iiepjlsl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3tmspnhbe.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3cqhzgefj.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3gpsvxkda.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3ailxmplv.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3jkvqdsso.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3hzuluuhq.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3gcvzmzyp.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3vnqlmssv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3ejwqivar.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3karxlxwt.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3vhjvzwjh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3kkvhxuvw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3xfhirvon.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3aiaitctq.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3koslgykw.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3igdcbelq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pyakrqoh.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3szvhabsm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3pcjxhygn.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3memdqnht.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ssruaioj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3knslxpmz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3agtsnlze.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3gyxbtgfc.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3atvtxsga.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rfsddzdd.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3eaitqtte.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3irjrjfjn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3blpcatyl.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqevqpcp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cpksfwef.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jjodudbp.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3rxikqjgc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tfxfxric.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lsnptlla.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ppgsfhmt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rgggqewu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3scwuqjkx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zsxomwjn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ccgcbotp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ninocnks.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3kqqxwyuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcekelnm.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3xllfhhgq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3vrqiderj.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3kvuoukzd.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3irxllldq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3galgalxp.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3clzajqxt.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qbfvaovj.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3oxtoekwm.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3mvqekgzx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3nkbbxvkl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3eadjnkol.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3uapvgsiz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ndjlffcl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3orfmicwf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tmhsrkbo.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3bfyekocm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3zlqixjsi.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rlfpcrzl.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3npcltngq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3peokzeiq.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iunigtlm.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3framezzy.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3lvmyczxh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hnwpvuxb.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3qmvfqfpg.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gruafhvk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bhgqcqaz.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3lxjeeonf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3rfkwathp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ijitedzx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wfvbwhxe.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3mjzoklhw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3tjhejfrl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3mpcdadjj.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3zfaovgow.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3xxkceism.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3glfflhvd.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3lmebgmkm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pvreskrj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pmzvwret.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lkdtlwtv.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yenedluk.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ugwxyhli.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3klygsjtp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hrcpuzio.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hpkjibfv.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3khsvwoha.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3wmiplfiw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3dgbwumot.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qooyfovx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3czsaodke.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3nucwewve.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3tdnfalcp.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wwiiqqme.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3reelfqcv.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3mblvesvp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3abtowiis.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3oxftxgxl.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ffurixbv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3qkspegxy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bpdxspmb.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3kifsbetp.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3zuamjneh.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3xvsjnjrc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vlbklzae.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3kpkaapdl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3onspytnt.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3eucraxjm.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hyfqjtew.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sxhdajuu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3afcdxutq.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ucvdnerv.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ghgamwll.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3itjoupwm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mgupgefe.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mbbwlsdm.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dolcteon.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3dsdojjwo.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3fwzideen.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3pydglwpq.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jpypelxg.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3kduemwhf.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3njavxkef.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3mrjrnnqj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3setrzpay.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jlnhqxif.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vignoerb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3fwtuxhha.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3ftiwkset.html


<!-- 参考信息 -->