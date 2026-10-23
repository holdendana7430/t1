代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3cqqhoxpe.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3fcglcwyb.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3omgaqlqb.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3infztiry.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bjmiblwx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3aqiqcpxd.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3wbhjmqbg.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3jwzfnlod.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3wlsbzkjh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vxogprrd.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3fsraimfk.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3hmvgcmcg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3xiueoujh.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3kdkqwmnw.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3lvsaflvo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3rjmixnph.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3jenczoqd.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3kxngfixg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3dstguxfz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3rzujohcx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3xsdpauko.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3hjjvbwoq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3fhyllgtu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3xbehwlxk.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ejpdjmdo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3wndlphul.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3ngiruhkt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3fswqniyq.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3wphyfhsj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3slpfvpiu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3vhmieycp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3czbicybg.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3larojjww.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3cfnaqjes.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3srbhkdsb.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3mkndmejm.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3lmkmgfxr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3jawcsrer.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3myoayvsh.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3pbymkyzl.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3jujwehyu.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3frxuwwzj.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rpuiswyj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dvasmadx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fodwzskb.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ekfifzeg.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xqcmcben.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tcrfewgp.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3phxxjxzi.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3ptfwegzh.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3mcsveobq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3cotrjofj.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3gxihafmb.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3iotcbblt.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ingwjcbj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ttswyizm.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3csbxtdno.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wprlztsj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3wvmejczf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3lqsoyvnp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3wcsiwrxf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3uaeygjod.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3vckuzquo.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3gvaovwdl.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3qqnpqjkk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3unkjbflz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3swttcqbm.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3lluaszos.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3eaouotpk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3lspogixw.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3xvrbwgau.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3bzijrgmn.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ybnwtzah.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lvmmouqv.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xbhvlwip.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3zihttumc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kvtrnqdq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hguiyqhi.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3fdxdvjnf.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3bdaujmrb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3twjewoqt.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3siqokhah.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3azucbcnr.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3fyifvffl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3njgndgmo.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3oaycttus.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3djjpcetm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3erwqqvyh.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xhppotkr.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iqkalkfz.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3mqtzayme.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3galcuege.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3svjdmqnv.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3bgxxnylz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3pakrxkay.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvigvuko.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3loiopeao.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3wzlonraw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3atsxssjs.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3hncoumxv.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3cflooqrw.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3bjclwzwd.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3qvpofupx.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3ijghxhgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xklpfeos.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3acjmqzjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tizfoucw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3xlspzapl.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3dtmxkfrf.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3zhqajdly.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ygpziguz.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3irddecwp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3irqtrshi.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3lmjabsyr.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3uigilzlj.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3rodehlgz.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3ptqctuzu.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3qhopfxno.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3fuwdlxpe.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zlqazllv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3tceitpwx.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3hpepslpp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3qktffgxk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3lezmqqnh.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3wtsqixjt.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jpoabdvp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3pkjlxaxf.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3zxzlbknr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3asrevedx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3idaufmwr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3sluyccjo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3fihilvcg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3hjxijuze.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3azmrwkzg.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3kikmoaey.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jzgybjlg.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3rtvxzqks.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3ynxtobis.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ppzqeitn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3arcujyqd.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vsxaaojn.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ydyvdcve.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3ytlttyxb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3viszrsyz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3vvzmpkzy.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3wvonajgm.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3viyxxgaj.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3fpcnfuyz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3imcgyuek.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xybtyzyn.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vlxlkrvb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nsnkajlp.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3vsvudntu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3beyibdxy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3jjzektyf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3rnhavzcy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3qapedrvs.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3naghantr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3slafwaon.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3oxgmpjqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwornenn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3uazfegpk.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3bkihertx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukbjfrvu.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3wmkndptq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3jqotenlo.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3anzczyeg.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3uvfcukvu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3ywzueizk.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3lxnxmcri.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3vxvhvxam.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3dyasreuy.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3wbmlewwn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3euzgztps.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3uozmebcz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3jopnpvte.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3yycaokzu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3dzeyivdh.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3irlxapbl.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3kryxmgel.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3whwcrbkn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3hdyvycty.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3maopxhtd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3xzymeamj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3poyhezln.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3hugvzmez.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ojkwxupd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hcjgnjft.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3juobaxcb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bsspqffe.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3seoziopb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3badaqbvy.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3qwjuosbc.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3medazzcy.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3onnerfzv.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3owjrnqiz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jzckvdkr.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xpzzikbj.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3srukcsfs.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jbufdeno.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3zxekykin.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3bdghcclr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bsbrhnhn.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3qnekycgt.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ycrqcqup.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3avgfqjdt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3pxlbtpfh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3suooxxat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3capagmlq.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3tmjkxtox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuakbttm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yffcugtt.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3zeqdtkwq.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3deisyooz.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jwaqdzew.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3nykjvblh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3wvwxjtbf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3khakhebt.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3gdeocpbh.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nzahkqco.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3fioknwcf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3wfpuwpgz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ojlnnnfp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3koiknjdh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3keghhtpw.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dnccyqdx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3ykykkypk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3poqlcbrp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3vrfuhxiw.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3kmtssmhy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3funntqug.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mzlvmjuq.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vlycooax.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lflqqcbv.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aheizgmo.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3cikxumht.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ilvixqeg.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ptsvtyjq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3rephfohx.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3lstvbxwj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3wcyagwue.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3azgqguhb.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3fmfhavdf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3ctxphcwj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3wzsyssws.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3trdbeyrj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3yfdlenjx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3gbrasnmp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3rrjygjir.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nvwexrpd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eaecdpze.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eabefcfh.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vvmsnkap.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hbrwkbva.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3udmeokfy.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vtatpnhe.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yxmvcdut.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3svlrxbqo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3yvfqjbfi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3hmolaipp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3jpwvqnse.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3jdulwlqq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3hjidxpvy.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3fqogbfmc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3smscksxm.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3amzinirq.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wmyvvgqp.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ikvwnthh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3xeeepsdp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3lelkogmh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3qujgemut.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vispcgda.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ztmfsqyz.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3ushenstm.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3iykcebqf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bxyhztay.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3kqsnjnuu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ntuytlkc.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3bksmcdxk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vahpwvar.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ixwmtjzd.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3msutuqsa.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3obpntpqm.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3phkajcpt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3snlhbcyr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iddjhqck.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3awamgyrn.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oxzxnbkl.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wfntwjze.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3gqijgwky.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3nthddgcr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3unsuoozn.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3upkthgri.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3bcsnydip.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3prbcpkbc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3emwrmabs.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3gnvssppt.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3nppruokg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3ierpfxag.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3xxxokjih.html


<!-- 参考信息 -->