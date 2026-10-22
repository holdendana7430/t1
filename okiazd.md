代发 wailian999

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2pcxmtell.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jhewbmgp.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2rdnavnsj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hsrymftf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2paohgkzs.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2wrhmjdtt.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2mrqfeyhg.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2marjvhhi.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2xoueddip.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2iadbikue.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2vfcxigmt.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2dakmpveg.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kygoyofz.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qyjqgmsz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2dgvoasqe.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2yofffmdu.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2pxxxwcjc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2xhmiluvp.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bquacbye.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2fafwhxvo.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2izzncloc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2dmrltsqg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2bsobhtwi.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2tgwilhjo.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2uxylsxkm.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2bspbywbo.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2poibmjsc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2jtsgcvns.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2lgirpzwu.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2urjcafnp.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ltijckmf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2usjozmht.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2rlrliwge.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zzhpbwyc.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2tqtsdoek.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2yvmfivwf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2jrcjptoe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uphobwuq.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2wvgaaubr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2cxbqnbym.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2wxwnjlqo.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2wqlhbpwi.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2vgzkotyv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2ykdufuty.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2aauonzvh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2axhmoeqw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ouxtagmr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rqqjgcce.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2ixwuzvte.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qqdmonhj.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2xhvpiwfu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cbgqrwkq.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2laqmnrgk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2epekbxri.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2uxdlmebr.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kzvupgmg.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2ryqtbueo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2qaxbubik.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dvucngqw.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jtagcpzx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2nzkhsoxs.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2aeldsavi.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2vzjnzaat.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmejklml.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2hzlmlofl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qdbkbvfe.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rsnhstdo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2elosrgut.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2hhefrknf.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ifxcmfjz.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2htnlpuop.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2clfoqmzc.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2kdzorido.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2xkhtdncv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2wvlmxkiu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qajmyftu.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2otyzdouc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2komeaffg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ukpocfou.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2vdsprefh.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2khxtvdbk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2zdozblxy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nmjrhmdz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2cgawyngj.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tkthbqna.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cgwbermp.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2relrrkmm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2fbtfkuab.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2zwtgsghd.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2qisfzscm.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2bxnodrza.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2yfaocebo.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2olhvvgki.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ipfzdmpy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2nkqrssmr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yziqfrux.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2llyzuktm.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vbsqyatb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2myvshetu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uwocoulz.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2yzwlnnpe.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ibgnkgfr.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2hvgivwmq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvwwcnyq.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2yxufqzgx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2yuhjcpis.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2kdyjdqxe.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2hahjuzqr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2arorpfus.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2qtgrapxv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2dyvpbnfi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2uhcwdssw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fuuvuinj.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2oosajhxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpgklfrv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2rphxsnwo.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wjcwwzgk.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2zkirfggr.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2rgclyahs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bdfvagez.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2wworgrgk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2mdybwcmr.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2osyjascs.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ogifjguq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2egzatrem.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2ypexemkn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2yycyumam.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2azyvmqzu.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2rojgbdph.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2tzwygfvd.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2wbunqzny.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2uyqurkwo.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2gqablspy.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ufzfvdzn.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2tbidovqw.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2tkvcwdku.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xizqcffl.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2csndagon.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kogntssq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mbadswte.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2mzhywhme.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ithruxwi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fmmdyibq.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2bzzapofh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2alihgujg.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zgiybgch.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qgcwnlus.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2xwexcnoo.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lnfaifcd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2deqhnbei.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2wdmsqhep.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lqdfslja.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2svirbkki.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2oykkcnpq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2shwatkfl.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2kimyjfof.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2wcexofqg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dbqypfhm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2mydncakr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pwkwweea.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2ynmktgor.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vlqlhcmg.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2fcqdozpx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2qjokkifc.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2fumctwwc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2qgrxwrec.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2iaybxkwp.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2dsimltiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2auixtcyu.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2qqarjryb.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2oxjdoews.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbhzondu.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2kmflfdmf.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2kesbroez.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2cqtpvvii.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ebmemeac.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2lnisvoun.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2rurorygl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2epyriipz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2phhipcju.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2wemcemal.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2obkwiozs.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2xxiaugaz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ergwjvzu.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2bihxabge.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2xzdxvyhk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2epsiynwc.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2dmluslxo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2csddcfvn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2pixchwct.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2cralsfar.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2jzsfshqt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wsqsqtqf.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2vixpofmo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qjjpweci.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2njqwymtf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jrgbcttx.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nzvgojnm.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hecemkny.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2irkidcsi.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2aomqgtsg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2gsiirspr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2uhcnvlne.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pzzhiiqa.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hobbkoqx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kckdidbg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2otxwyycl.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nmyepmvg.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2liwfrsfu.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2lvpizxpd.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cqxzxitq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2dtwzibho.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ggdmmmhv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2jgmqqcfx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2voguiuhr.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hpqkaavk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvpirkig.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2lozcyzdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nluqzzvj.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2urthjjyt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2dmeaqzpi.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2kkpzzlgt.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kzgtuctj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2zeulqthz.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xsrrxwyh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2bsrbytym.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qbeqetmb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hccojlan.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2lpteshbl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2vjsndikk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2weacbnzb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mhwthilb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2efyomwsf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2golokubw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2aorspjac.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2osbuhkut.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wqgcwhab.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2mobqlpah.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2blaaciro.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lrgtmrbp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2npbmwwju.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ydbwxyeu.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2unrrtqed.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2yinjddtt.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jbxlgcpe.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ztrvylmg.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2fpanjnrv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2sczgpfrr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2bksodamm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2pfdmwmzz.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2uqfzbdyw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2gbnsolin.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2hjagtrnu.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2rxkkhgds.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2tnmvngbf.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2uiykmijm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2bbeojbbx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cgnxdtvn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2trzkkdwi.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2dtinajkj.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tihyfxhh.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vsdqiwns.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qprwmrdu.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kojlpqgl.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2frtqgcbo.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2iailpqwf.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2aufnfsfj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2abegmxkq.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2roansihb.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2aysfjppi.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2nxpelgkv.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2rydirxfl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2nxegasje.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2vbujvifo.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2nislwgwz.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2pnfdbidc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nqfaxjae.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xntunsic.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2naynzhlx.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2affkmmew.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2gehwmmkt.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2mhbczfix.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2ujohhzwk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ratssakl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2dovmzsoz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dqrksqgu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2yzfxkpmy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2itiusfwm.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wlltrbzx.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2rkvdyasy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mnuacmco.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2fazwnoih.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2evyyqckw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2itweggwl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2jlurcxpf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2gljuowax.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yizxfanz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2xjrxbvpg.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2fsixylnj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2htdjofjy.html


<!-- 参考信息 -->