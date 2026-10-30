代发 wailian999

[U67] PHP：处理文件上传
来源：http://3g.zdbjq.cn/Article/details/gvpcdhllf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.fehbvm.com/Article/details/gelaqgalr.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/gcboskbbc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.zdbjq.cn/Article/details/gghrvemsx.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/giuyxkmzu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.fehbvm.com/Article/details/gcoojckyd.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gqehpezzn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fehbvm.com/Article/details/gugmachmf.sHtML

[U71] PHP：抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gmipqjyjw.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gnjhracod.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.zdbjq.cn/Article/details/goqlmgrrr.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gihoqpgyf.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.fehbvm.com/Article/details/gdcrvvaap.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.zdbjq.cn/Article/details/gjvgtaogg.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/garwnnbdz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gnpukpark.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gckuvbrsp.sHtML

composer require psr/container
来源：http://m.share.hesvh.cn/Article/details/gdecnvfgc.sHtML

[U76] PHP：简单路由
来源：http://www.blog.zdbjq.cn/Article/details/gmsfunzce.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.fehbvm.com/Article/details/gohnjtgvk.sHtML

[U77] PHP：模板渲染
来源：http://baike.zdbjq.cn/Article/details/gqwyofrdt.sHtML

composer require twig/twig
来源：http://read.share.hesvh.cn/Article/details/guxlcrhny.sHtML

[U78] PHP：单元测试
来源：http://m.share.hesvh.cn/Article/details/gnfcvryki.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gjxkypctf.sHtML

[U79] PHP：静态分析
来源：http://www.blog.fehbvm.com/Article/details/gictbrocs.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.fehbvm.com/Article/details/gtiqfpman.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/guolvsefo.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.fehbvm.com/Article/details/gowtisbef.sHtML

[U81] JS：初始化项目
来源：http://mobile.fehbvm.com/Article/details/glfcaxsto.sHtML

npm init -y;  npm i express
来源：http://wap.hesvh.cn/Article/details/gdowvlmzl.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gloreynqv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gjovavgvo.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.zdbjq.cn/Article/details/gxihhypry.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gqdumqpde.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.hesvh.cn/Article/details/gunczwivx.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gnhlgslry.sHtML

[U85] JS：可选链
来源：http://mobile.zdbjq.cn/Article/details/gakfrxxsu.sHtML

a?.b?.c
来源：http://baike.hesvh.cn/Article/details/gknfycust.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/goxupxaxs.sHtML

a ?? b
来源：http://wap.zdbjq.cn/Article/details/gsmcviztw.sHtML

[U87] JS：解构默认值
来源：http://mobile.zdbjq.cn/Article/details/gfknsmviy.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.fehbvm.com/Article/details/gtdencryr.sHtML

[U88] JS：对象展开合并
来源：http://www.share.zdbjq.cn/Article/details/gvsnmqxzh.sHtML

{ ...a, ...b }
来源：http://mobile.hesvh.cn/Article/details/gkybdytze.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/gfbjgzzou.sHtML

[...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gnrysdveg.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gnviszsoq.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/glfmgihmy.sHtML

[U91] JS：对象键值遍历
来源：http://wap.zdbjq.cn/Article/details/gomdtudvo.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.fehbvm.com/Article/details/gsuleutpx.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/guvnbjvac.sHtML

structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvgoydsrv.sHtML

[U93] JS：模板字符串
来源：http://baike.fehbvm.com/Article/details/gxoxmylri.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/ggomrlnur.sHtML

[U94] JS：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gestetelg.sHtML

const double = x => x * 2;
来源：http://mobile.fehbvm.com/Article/details/gwdrjoqgn.sHtML

[U95] JS：Promise 包装
来源：http://read.share.hesvh.cn/Article/details/grscxewvl.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.fehbvm.com/Article/details/gywfsvaqo.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.hesvh.cn/Article/details/ghqzxzwed.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gaqxrruvg.sHtML

[U97] JS：并发请求
来源：http://baike.hesvh.cn/Article/details/gpkgqatnd.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/grztmlpgq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.hesvh.cn/Article/details/gejixwphy.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://read.share.hesvh.cn/Article/details/gdytvcpnz.sHtML

[U99] JS：事件监听
来源：http://m.share.fehbvm.com/Article/details/gmthfnsqn.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.hesvh.cn/Article/details/gqezfvgtv.sHtML

[U100] JS：DOM 查询
来源：http://3g.hesvh.cn/Article/details/gxlflpoae.sHtML

document.querySelector(".item")
来源：http://baike.hesvh.cn/Article/details/gsdxonxzt.sHtML

[U101] JS：classList 操作
来源：http://wap.zdbjq.cn/Article/details/gonojwdyh.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/gnvsvtjmy.sHtML

[U102] JS：本地存储
来源：http://3g.zdbjq.cn/Article/details/gulvpqbqt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/glpfaruxl.sHtML

[U103] JS：定时器
来源：http://wap.zdbjq.cn/Article/details/ghpkojozl.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gbajaacvb.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/gvwlwjelt.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gfvbcqmga.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gsmyijuxy.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.fehbvm.com/Article/details/gtkqvfivn.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gtardbkfs.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/gburoehxt.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/ganxmsrkq.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gbevrefnp.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/gyilnunxu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.zdbjq.cn/Article/details/ghzeaqwhe.sHtML

[U109] JS：数组分组
来源：http://mobile.fehbvm.com/Article/details/gcgkkuzlw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gonurgdfm.sHtML

[U110] JS：数组分块
来源：http://blog.zdbjq.cn/Article/details/grojzrrpt.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fehbvm.com/Article/details/gzxzdcbtd.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gpqskoupi.sHtML

new Map(Object.entries(obj))
来源：http://3g.hesvh.cn/Article/details/gimtncltg.sHtML

[U112] JS：字符串补位
来源：http://mobile.fehbvm.com/Article/details/gedkzhqqa.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gaegnwxdj.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.fehbvm.com/Article/details/gcsutxybc.sHtML

s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/georkvlxs.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gcnllfcvz.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/ggfbovjps.sHtML

[U115] JS：生成 UUID
来源：http://m.share.zdbjq.cn/Article/details/guadibbvt.sHtML

crypto.randomUUID()
来源：http://blog.hesvh.cn/Article/details/guklhwdod.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fehbvm.com/Article/details/gkmygyqwv.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.fehbvm.com/Article/details/gdnpnqpat.sHtML

[U117] JS：单元测试
来源：http://wap.hesvh.cn/Article/details/gaasjozpr.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fehbvm.com/Article/details/gcxacfvij.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gypzywnvl.sHtML

npm i -D vite;  npx vite
来源：http://3g.zdbjq.cn/Article/details/gsysnbzyu.sHtML

[U119] JS：生产构建
来源：http://3g.zdbjq.cn/Article/details/gqeqvdtvr.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/ggcblizkf.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gugpvibtb.sHtML

import.meta.env.VITE_API_URL
来源：http://3g.hesvh.cn/Article/details/gfepoaiwg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtzwgvtlh.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gwiyvcueq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzztpycty.sHtML

按语言统计（条）：
来源：http://wap.hesvh.cn/Article/details/ghcqsofev.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gkhdezbpn.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gsdhszicc.sHtML

JavaScript ..... 252
来源：http://mobile.fehbvm.com/Article/details/grgptqbnv.sHtML

TypeScript ..... 212
来源：http://www.m.share.fehbvm.com/Article/details/gmhumehgd.sHtML

Java ........... 212
来源：http://www.m.share.fehbvm.com/Article/details/gseyidbla.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gxjbgenuc.sHtML

Ruby ........... 212
来源：http://baike.hesvh.cn/Article/details/gqxdfsomz.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gaxaozyws.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/guvrnmfeq.sHtML

C++ ............ 30
来源：http://www.share.hesvh.cn/Article/details/gjetqzueb.sHtML

SQL ............ 90
来源：http://www.m.share.zdbjq.cn/Article/details/giftgqvye.sHtML

Bash ........... 80
来源：http://mobile.zdbjq.cn/Article/details/gjpvjdvvp.sHtML

Kotlin ......... 15
来源：http://baike.zdbjq.cn/Article/details/gdlspgpkk.sHtML

Swift .......... 15
来源：http://read.share.fehbvm.com/Article/details/gzvzfttjk.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/guhjpxuwu.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gjuykxuvd.sHtML

Scala .......... 10
来源：http://m.share.hesvh.cn/Article/details/govttojam.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gahuxwdou.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gffltjpwj.sHtML

按章节统计：
来源：http://blog.fehbvm.com/Article/details/gqnsgkrsc.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/gzdgphjie.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/grqtuyynd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/glqlvqouu.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gsmzcpeed.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.hesvh.cn/Article/details/gpitxujmg.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gbjouvzmm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gimfjxrub.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.zdbjq.cn/Article/details/gmrwuumsh.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gwetpstoz.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gzmhfanbj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gfumioyei.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gwrxvxans.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gezarebov.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://mobile.zdbjq.cn/Article/details/gdveuvmdj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.m.share.fehbvm.com/Article/details/gmwmggzqi.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gpuxtpgjf.sHtML

Q SQL 专题                              90
来源：http://m.share.hesvh.cn/Article/details/gwgllwkpd.sHtML

R Bash 专题                             80
来源：http://www.m.share.hesvh.cn/Article/details/gtuwqlytc.sHtML

S C / C++ 专题                          60
来源：http://www.blog.zdbjq.cn/Article/details/gjvcqeejk.sHtML

T 其他语言补充                          60
来源：http://www.share.hesvh.cn/Article/details/gfqrgigfx.sHtML

U 高频实用片段                         120
来源：http://www.blog.hesvh.cn/Article/details/gwqobbofm.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gutpiwpgb.sHtML

合计                                  2106 条
来源：http://wap.hesvh.cn/Article/details/gdwavwfgl.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gdkwxgvoi.sHtML

使用提醒
来源：http://baike.zdbjq.cn/Article/details/gkrawznej.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gspxbtxnf.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.hesvh.cn/Article/details/gglmhvicy.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.zdbjq.cn/Article/details/gbyicitsz.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gzvhgbygk.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://3g.fehbvm.com/Article/details/gxmleontm.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.hesvh.cn/Article/details/gkgrevbmy.sHtML

—— 文件结束 ——
来源：http://www.m.share.fehbvm.com/Article/details/gcowypaes.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbepmdamp.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.fehbvm.com/Article/details/gtnmczncw.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fehbvm.com/Article/details/gmcornuhu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbrhalutz.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/gbygayvqt.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.fehbvm.com/Article/details/ghividuxs.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/gkblwazyp.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gtfwqpneb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/ghelfthkt.sHtML

【使用说明】
来源：http://read.share.zdbjq.cn/Article/details/gqrxkvatb.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gflguzgmh.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gargwznao.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gtlujvfwq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.zdbjq.cn/Article/details/gxkkkntix.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://wap.fehbvm.com/Article/details/gsxpystaq.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/gejmewvvj.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gnxmbyett.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gyecalazw.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://mobile.hesvh.cn/Article/details/gqhsorawx.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gwsyyripv.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.fehbvm.com/Article/details/gplogzrmo.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.blog.hesvh.cn/Article/details/ggxyenyys.sHtML

【文件统计】
来源：http://www.share.hesvh.cn/Article/details/gwvhzvyry.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/grdumaxpw.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/glayngfzv.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gerwolkmh.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gmvbjgolo.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gjetfiusq.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gqhtchltg.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.fehbvm.com/Article/details/gxsxhnokn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gjyjcuaub.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gkfcimtot.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gxhlinwse.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gaunieydl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gpxerfekc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gzwcoiqto.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gztalvxbj.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gdezpfqog.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gxaucpclo.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gqrixjvvu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://m.share.zdbjq.cn/Article/details/gexneblia.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/gxskjbjys.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gpcnorzsj.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gjufxdgcl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/guwzhrhok.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.fehbvm.com/Article/details/gnwrkmccm.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gfqrnyzfy.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gxduxcycm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjlalpzwg.sHtML

A. 基础语法与类型
来源：http://3g.zdbjq.cn/Article/details/gxsjjdnzz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grpccggqj.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gyxtkfzck.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/goaxxvpbe.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.hesvh.cn/Article/details/gasecqrkn.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gonbaswou.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gywclpzth.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.fehbvm.com/Article/details/gdnnpqpgc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gixolbryz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.hesvh.cn/Article/details/gcudbyscr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/guozhpedo.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gjshsahrf.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://read.share.hesvh.cn/Article/details/gmftdunbm.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gqmkutdkf.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gqjmwwmoh.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://3g.fehbvm.com/Article/details/gwlyztrkv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/gnibveaby.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.hesvh.cn/Article/details/gymhljoxt.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/grnucjnaz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gmlydreht.sHtML

[A03] 常量定义
来源：http://www.blog.fehbvm.com/Article/details/gizgsfmfv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.fehbvm.com/Article/details/gdodcpzmj.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/ghmzaxeoi.sHtML

JS:   const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gylbjcduf.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gmadjcpgi.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gfgfsyxaq.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gpftwhufo.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gtwajjvyq.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/guorbkthf.sHtML

[A04] 判断变量类型
来源：http://m.share.hesvh.cn/Article/details/girfhdrxt.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://blog.hesvh.cn/Article/details/genyktfsc.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.fehbvm.com/Article/details/gsmraioyp.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/ggnobtogt.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/giluwlcqc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/glaukelmj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://3g.zdbjq.cn/Article/details/ggrjkfszu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/gyqudrywc.sHtML

C#:   x.GetType().Name; x is int
来源：http://3g.hesvh.cn/Article/details/greqpedij.sHtML

[A05] 整数除法与取模
来源：http://read.share.fehbvm.com/Article/details/gbbajdvjr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://read.share.hesvh.cn/Article/details/gysclewhv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.fehbvm.com/Article/details/geztwhvbu.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gwoplgeau.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gcrqnixfi.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gvmhhqtuf.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/grpcpvvvp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gchrvaibe.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.zdbjq.cn/Article/details/gjctwexmu.sHtML

[A06] 字符串转数字
来源：http://blog.fehbvm.com/Article/details/gcjzzhced.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.fehbvm.com/Article/details/gzdqpzglc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://baike.hesvh.cn/Article/details/gkdxnvduk.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.hesvh.cn/Article/details/gxjvmiodg.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.fehbvm.com/Article/details/gomuymwfn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/gxsqjlpja.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.hesvh.cn/Article/details/gzcbdxeae.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fehbvm.com/Article/details/gdvrydfid.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://read.share.fehbvm.com/Article/details/gcxcrmnqc.sHtML

[A07] 数字转字符串
来源：http://wap.zdbjq.cn/Article/details/gnzbdkrqx.sHtML

Py:   str(42)
来源：http://read.share.zdbjq.cn/Article/details/gwmmvfbpt.sHtML

PHP:  (string) 42; strval(42)
来源：http://www.m.share.zdbjq.cn/Article/details/gljoxoiiz.sHtML

JS:   String(42); (42).toString()
来源：http://wap.fehbvm.com/Article/details/ganmcvqrs.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gqnkmtsik.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.zdbjq.cn/Article/details/gabmilnnp.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.fehbvm.com/Article/details/ghcxlezgn.sHtML

Ruby: 42.to_s
来源：http://mobile.hesvh.cn/Article/details/gtehiriot.sHtML

C#:   42.ToString()
来源：http://www.share.fehbvm.com/Article/details/gezrmmxys.sHtML

[A08] 取整与四舍五入
来源：http://wap.fehbvm.com/Article/details/gojpmevlu.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/gbaiqnnlv.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.hesvh.cn/Article/details/gybvxbpim.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.m.share.zdbjq.cn/Article/details/genrlhrjr.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://m.share.fehbvm.com/Article/details/gqglgushe.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gstfaflsd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/gnctkvlsn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://baike.zdbjq.cn/Article/details/gfqibevcg.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gteuhqkkn.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.fehbvm.com/Article/details/gdcwfvewt.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gbvcnrwiq.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ggefcyueb.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gaoxewjna.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gjovyomnc.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gbdvoiyem.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://baike.hesvh.cn/Article/details/gvlqhrkrk.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://wap.hesvh.cn/Article/details/glahtzoao.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gzvivacpp.sHtML

[A10] 生成随机数
来源：http://www.m.share.hesvh.cn/Article/details/gzfcwakiw.sHtML

Py:   import random; random.randint(1, 100)
来源：http://m.share.zdbjq.cn/Article/details/gnrqalmom.sHtML

PHP:  random_int(1, 100);
来源：http://m.share.fehbvm.com/Article/details/gonekjzhs.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://m.share.fehbvm.com/Article/details/gjavldbyn.sHtML


<!-- 参考信息 -->