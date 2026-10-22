代发 wailian999

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2oqdqacpr.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2liwmbaeh.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ucrawhqz.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2ixjkfonl.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ixrcweds.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fjigdjev.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2xivyurso.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2rbcfdkko.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2phwupion.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2nvwykjzp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2fwxaktqp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ykauxsbt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2kjndsyjw.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2hbvttveq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2jidhncjp.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2cqxfrskm.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ahnhshyt.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2uckgwikv.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2oohsageh.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2zelrohcc.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2xgclzljc.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2kcpuktkt.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ygceerjj.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2jirtyhyt.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2hhfbrskb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ewlyrcfa.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2axezngfi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ryukhwly.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2fgwrbkjx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2xpdoukyt.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2aboglggm.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2qmoftwwr.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2zwqhjbzl.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2nlotsjua.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2hiotuajq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2fjononje.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2abyqazef.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2ulbmczni.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2bbhhgsrn.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2drlvhzuz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2sunpxanv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jeraubxr.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2wrwgrgje.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2kihuehmk.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2uvtpvzfj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2efxdrxwe.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2mryolbrb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2yiiyheeh.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2nusvgfwl.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ylssjrmq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2fwgcdjwr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2alaimfjn.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2xfeqdpey.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bhtrikcq.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2bsuwkxla.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ejzcvogc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2reogrfig.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2vxwmhfiz.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2ompysziu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2xkdmurni.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2bvuulfol.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2cxpnubpc.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xikqbdbw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zponweug.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2iizzuhrc.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ckxvmxdw.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dzgzghpj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohyumkmg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2xobecuka.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zjrnoupn.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2reezobvs.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2yiqisyhw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2eoghqfih.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2oacjpmzu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2fhacibbv.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2szsyfzrj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2qxoiiwyk.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2okndxixb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2pbmevthv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2bpbbjxjf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2fghhecyk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2bpeoqzxz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ilmepoce.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qlrvghgz.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2oojjhlub.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2kfacwrxi.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ncxyuohn.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2hrbjfwsl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2urqwwwyx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wahisgoy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2gkoubhal.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2lwynkzgu.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2fuzasiod.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2grergehe.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2tffwgwcd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2omxqlkic.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2imfdqych.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qecrseqs.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2dyslrjxz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2umvlkrcn.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2joinubjp.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cmkbqdsz.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2kuqyfezb.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xfikbjwi.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pelslrns.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fsqxzqbz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2bnuszmfa.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2abptafun.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2yduysjeg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2yyrhtbcw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2rkcvugsw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2lynutmez.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2qkqniref.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2idfmgrrx.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2hoqzczkf.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2btafjgzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jheqdwdp.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2gifkqtwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfjidctx.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2gffuuzme.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2yogpivea.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2ognfxxat.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lmvkvhwh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2belpqzhl.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ponsnmim.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2sxyddcfx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2pusdwxtc.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2prfrujxy.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2dagacgdu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2nngtsvnf.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ktwlzewh.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2feinmmvd.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qiujdrqw.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2khqikfkp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bdxvsxws.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zgfdbhcg.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qbihfetz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2azdbzxix.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2miclayzp.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2yecyluwt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xyzxqezv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2tknpswbp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2qvipicjx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2qsbjbhgg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2lyaekubc.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ivvhdfmu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ivmrxgeg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jiuitezi.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vprdzqbz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2wxsiislj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fmrjbkld.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ihdsjfjz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ottmwvuw.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2nlnvvosh.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2spmlblhv.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2wpizorzm.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2hovwkwvr.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2mpiplcue.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kyrvrrca.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2uqgdvawp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2oazbvyad.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rpeesxhn.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ejyyevii.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iqetqaip.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2yevtrcjm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xxokwwge.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2kcybwgpc.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2vuhmzdoy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2oeykjqzr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2wknlpgqs.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2urazoiqd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2hsftjgmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjbdodcz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2fbniqces.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2tlgsxufr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jobrvbqr.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2nsqegidq.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ssxyataf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2dbvtrihc.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2zzryqhwe.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2fjvcvwfz.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2rviwrxol.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2wdfmqdqd.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2vyplrgwu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2lmagngfj.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2uqtjjude.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ylpgohdq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2vheldvuy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2yfrphewb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2kgfdjafq.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2pvsgilak.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2efoaipnp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2beobrcns.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2bnedtvlt.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2egwlaqmb.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2sotuvkee.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rqvuiezh.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2rtybdklu.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iazoamsf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xgtgtsww.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yfnambai.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zqcfbxic.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jtnfvkyb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2vpssfhrt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2imrabsbu.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rzlufmky.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2jfqipvnr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cvjthcpc.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2oxfwpguj.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2slcbfire.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2romugqdi.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fejrpcmi.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2phlyziju.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wyviyyvz.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qrtqunzy.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ldilwcyz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wljyruzp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2odvttjcd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jjzvpuau.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2rezwegug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjpnphpj.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2opucenha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wuhxjexi.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2qpckilnb.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2lmazfbig.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2bcrnwetv.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zthfeunk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2cpgbixpb.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2llwjglti.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2qvtrjyox.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2omsscvyc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2oeviqlwh.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2rgujsjet.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2gybcapla.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2upnadcjh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pvczrblq.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2rmoibjxs.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nxbsslcr.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2bvwikfnz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2occqiawp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2shklbvfq.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2gpxaudyx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ouaenynr.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2taowfece.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2srusjwse.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eibckiws.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kkjpyygu.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2lcfnjuxe.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2cqspwpia.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wcvebzhd.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zsmpguyg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2nooshque.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kswbwant.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2olmowwzx.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2axdjzkfk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2sjqwtfzq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2cetiafnq.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ruwkbxwu.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2sqvnrmpq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2zmftdqzf.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ktowgqjx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qnnnqrgp.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zyqmuhvz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2daodkxxa.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wsiuxzuo.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ilwmsyav.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nfadoswk.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vfewlhan.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qbqxzhkv.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ycysohjb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2hzinfrul.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zayoxbvc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ommxsela.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2inevoxxb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2tpizntms.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2teqdpmmf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ptbwzsff.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2jxxixcdb.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2txqkvqeo.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ogoyjsmb.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uffkwtqr.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2xyulqhrg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2rgypdbmt.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2swgtzmxr.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2dafgnlmm.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2zblxqnmn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2nwcfyrby.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fkiqfqgx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2hdouybcq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ubthbwil.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2kcgdfwhk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wwnfkupo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2fpwrgiea.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2iecfgoeo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2btekwlxk.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2oscderyx.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nsjibzfo.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eldqknlr.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kwetzxjt.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jmbikwsf.html


<!-- 参考信息 -->