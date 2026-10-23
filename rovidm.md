代发 wailian999

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3bvvwipbw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3iqnbiuec.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3wqqbjhct.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3ripprlpq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3uvwnxhge.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3zlrokdon.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3owyxyprw.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3ronqckdw.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3nkdoznis.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3ajlbcvph.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3hgravqde.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ukjrvyar.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3krygwlcb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3tyflycoh.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3jillmfrz.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ajuonibv.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3kswrvfhr.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3jmtjpzki.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3fnaahtom.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ckgqfojs.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3yhojpylz.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3gumetrqd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3akobkiij.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3ucwmqyma.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3eelmoowr.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3otkdbqkp.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3lggcmjdo.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3gnedlzqr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3kvqvniai.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xpsvprxj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3nphldmdh.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3gwcgrcma.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3hllvhhws.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3qmiyidfc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3tzspktyd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3czbifyfl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xfyxiuhn.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3csbfuyew.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3ngdltclf.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3ahadttmx.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3gwylvxjq.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3eyagxrxr.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3fbeakcut.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wijmuxrx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bussevoo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3etxijpfp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3gccvtljv.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zlglxgng.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3hqtjasng.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3knmnkbwb.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3fekkfves.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3qiyoygqx.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3nwfyawxt.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ixszhehv.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3bvfuoumu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3retwpxwg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3cverkvvn.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3iinhvvmm.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3vvvmaypm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3bipzxews.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3cjdnqpvu.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3oysnbjeo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3tdsouvgq.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3xxyyrmol.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3winocvmo.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3mlrwzjsu.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3lxfqqqht.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3cdppnfhq.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3tpviymiy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3lbznxmuy.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3izfgsbjp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3pwpflclu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3itbxksrh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3aiyxtsod.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fnhxjiep.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3rzezgfbg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3feakuzcq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3irecsjso.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3smtzfvhh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3xonunije.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3uqbqtpel.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3imljuxhc.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3caqovjvw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3efqlqkxb.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3ygopvtjn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3pceytkgi.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ueqjerbw.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kzkzkhut.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3waxosies.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yfimcpiw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3btzfyilc.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3obbmtanh.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nqyqtvkq.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zmwxdsfo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3hwxvioqn.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3xgsliegz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3xnekwhit.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3bvovqder.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3itfiqusv.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3mexmhsbo.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3athvuzmn.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3jmhfxcwk.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3ynmekone.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3mfcxleuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3agmjynem.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3lyhgukwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3menfefrd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3fdadrzdp.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lxtdvkox.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3iqgmexxr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3rdokwzfp.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jlbydqkn.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ritgcvqb.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3whcrrbmq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kqkvgdxy.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gtfcblxy.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3jjecbequ.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3qgmzatfq.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3bqxadylt.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3zvufjjmy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3utwhrydm.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3xnnpzarc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3xhmvxeko.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3qolmikng.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3dfmkisnq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yorkztog.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3fsypoppl.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3wxherdpl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3kpymedhr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ugspbovn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3zxszjibu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3eylvidbh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3fwbpxzlo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ztajkmrf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3vlzjnbum.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uadmtdkh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xetihnym.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3uacqywvf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xbpmpmmf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hrjjfvoe.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3jaflqjqc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3goqbtmtm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3djgecztc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xoswrfkl.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3fxhnalzb.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3zxvinqxw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3jbahfsqd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3wkvlvuea.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3demsupwj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3wxxnfumt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3jjlnrtyq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3crmacrze.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3vgkcsowg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3sscvntzh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3qmejkzpw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3cisbihxr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ajktukae.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3vzkjfndg.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3javfmgic.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3girczwfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfeuqbzy.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3cwopqyer.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3tziyesyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unffwnom.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3zvekclit.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3kiewzltt.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3xkazpzyk.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3hnhocosb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3nzsbisfe.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3peqlisja.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3eakjscos.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3ktqjagof.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3eptddikn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3fduiehey.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3cguyfobd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3ipwnlssj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3kglgbaue.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3kqufzuci.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3eqhvyekq.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3kxuajiep.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3jvyykiyd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jxfrweeo.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3kcohelxl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3sdgzmznj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3cvwejoes.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3ydibknep.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yngjigmi.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3rzhfcpgj.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jnvwvxgf.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3sjgdejui.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3smocvtbs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tzxdgani.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3geefjdtl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vggvvgbo.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eofdvgcj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3crvmxcav.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3eclerybh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3boidumnt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ynozjown.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jetkflgv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3fcniliuu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vcmnmwxz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wymfulxv.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3bfgkpahi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3higeqcko.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3asydywxt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bshsgmpf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3qchozfum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mblinnwe.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3sbogaycz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djgorcgh.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qtlenqpd.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3sghgfydw.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3urftfbsl.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3jdbgpbvl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3vjlyaifj.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vzzevsaw.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3lamcinvb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ercwuzft.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fkuctcqk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3mvvvkqti.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3dskzgvdn.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3apejnfpy.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3erjnmszh.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3slrxlxnr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yxlgxpdz.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3eguefplk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3xvrmszte.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3cazikmka.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3tnyktzby.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3xjlbxuzy.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fjcnadme.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3latnvikm.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3burqzizf.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bqbpgbqv.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3fwedbigi.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3bokacxfs.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3nfcaehjr.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3goololmj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3znrkjydf.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3kigkqguu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xenluvqg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wvbnjezo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3bsgbkxvn.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3lanqlope.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ykgobhdu.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3bgodrcja.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3muhgfghz.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ktpmgttm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3twtuvgmd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vkxxlnlr.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3uwozldnb.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nwgrhzmq.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cttzxxpc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pykfykqr.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bupgxcsd.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vkqinxie.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dikgspld.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rthqjysq.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ilvtxsbl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3wczvfimp.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3skolkonu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3zghefdwk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3vsqzqhji.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xcfzvrpz.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3lmuexzud.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3einmxdhj.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vecccjuu.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3qraludft.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3erdiyxjv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3dendtpde.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xpgwcpyk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3qelzggxm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3wygemfsa.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3dpwwisks.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3epsxhoan.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3lorrtoky.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3xhwxjvca.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3pepeqbfx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ogvxlvbu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3iypbnxrs.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3ahydlfxx.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ehwtigtd.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jxcffqfl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oipnfuaa.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qhtalzcs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3lteqcvjx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dtlpsgxb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ytqayawv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3pumwihta.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3fvmtarkk.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oiievond.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3brhtpzgc.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3bkjthehy.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3wxbihdtd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hbtyrpkq.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3haltsqtd.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3zgxoycrj.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3xncftghz.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3qsngpyth.html


<!-- 参考信息 -->