代发 wailian999

[U63] PHP：文件读写
来源：http://baike.fehbvm.com/Article/details/gntrcteal.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.zdbjq.cn/Article/details/gugwzqosi.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gtfmvkjrk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gfcqykuqc.sHtML

[U65] PHP：会话
来源：http://mobile.fehbvm.com/Article/details/goskkbshi.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtbpdlcdg.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/ghdmxgjrc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.fehbvm.com/Article/details/gpexmafvj.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/ggjvtnutx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fehbvm.com/Article/details/ggaleouur.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/ghlgiyfra.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/gkqowzujq.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.hesvh.cn/Article/details/gejhclhpx.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.hesvh.cn/Article/details/gfdkydzat.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/gcvzzpwbn.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gpkmhtkyk.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/ghymghcky.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.zdbjq.cn/Article/details/giobhglew.sHtML

[U72] PHP：写错误日志
来源：http://baike.fehbvm.com/Article/details/gxcczyhvu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fehbvm.com/Article/details/gonfgkzuc.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.zdbjq.cn/Article/details/gjfhowprl.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gshpjliwx.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gsnqsnvyc.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.fehbvm.com/Article/details/gipqojwyq.sHtML

[U75] PHP：依赖注入
来源：http://baike.hesvh.cn/Article/details/gzjgppjbj.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/golypfzev.sHtML

[U76] PHP：简单路由
来源：http://read.share.zdbjq.cn/Article/details/ghuhwvsjp.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gerfjaonj.sHtML

[U77] PHP：模板渲染
来源：http://baike.fehbvm.com/Article/details/gmfrwvdlh.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gtnoxpyca.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gyfeeiclu.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.zdbjq.cn/Article/details/ggfdyctqt.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gotlcuegz.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gadepgzqt.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/glbmwbozk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://blog.fehbvm.com/Article/details/gykkjfyry.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gqxniapnp.sHtML

npm init -y;  npm i express
来源：http://3g.zdbjq.cn/Article/details/gqowkqfzk.sHtML

[U82] JS：package.json 脚本
来源：http://blog.zdbjq.cn/Article/details/gvrjfmxnz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.zdbjq.cn/Article/details/gcsphyvcf.sHtML

[U83] JS：ES Module 导入导出
来源：http://mobile.fehbvm.com/Article/details/grylxzsah.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/ganmpfvtz.sHtML

[U84] JS：CommonJS 写法
来源：http://baike.zdbjq.cn/Article/details/gtexqxlhk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gouhyshgw.sHtML

[U85] JS：可选链
来源：http://www.m.share.fehbvm.com/Article/details/giivfpwrh.sHtML

a?.b?.c
来源：http://blog.zdbjq.cn/Article/details/gwfsiqbwo.sHtML

[U86] JS：空值合并
来源：http://www.blog.zdbjq.cn/Article/details/gkeumsusu.sHtML

a ?? b
来源：http://www.m.share.fehbvm.com/Article/details/gvaxrpkkk.sHtML

[U87] JS：解构默认值
来源：http://blog.hesvh.cn/Article/details/gsumfnmlg.sHtML

const { a = 1, b = 2 } = obj;
来源：http://www.blog.fehbvm.com/Article/details/gyaxallmv.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/gysqojwue.sHtML

{ ...a, ...b }
来源：http://www.share.fehbvm.com/Article/details/gnxlicqoz.sHtML

[U89] JS：数组去重
来源：http://www.blog.fehbvm.com/Article/details/ghfwnzwir.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gxyyxvfyu.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/glthuhfyx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gtwnzhcuo.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gaygliucq.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.hesvh.cn/Article/details/gitrsdnse.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gjvcwxcbd.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gfdcvtoik.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/gjnbudeqz.sHtML

`共 ${n} 条`
来源：http://www.m.share.hesvh.cn/Article/details/gmhpoxqxa.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/gjwzivkvg.sHtML

const double = x => x * 2;
来源：http://wap.hesvh.cn/Article/details/gkcjuuejp.sHtML

[U95] JS：Promise 包装
来源：http://read.share.fehbvm.com/Article/details/gqlpveqvm.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gobkhbtyv.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/gkougnkhi.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gyqocuiwn.sHtML

[U97] JS：并发请求
来源：http://wap.fehbvm.com/Article/details/gtfjzbzwt.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gukkygelf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/goimfwmax.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gyasehrrl.sHtML

[U99] JS：事件监听
来源：http://blog.zdbjq.cn/Article/details/gbcaadung.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.zdbjq.cn/Article/details/gomybxfhq.sHtML

[U100] JS：DOM 查询
来源：http://baike.hesvh.cn/Article/details/geqxvhjks.sHtML

document.querySelector(".item")
来源：http://m.share.hesvh.cn/Article/details/gvbwyzcco.sHtML

[U101] JS：classList 操作
来源：http://m.share.zdbjq.cn/Article/details/ggeifmwix.sHtML

el.classList.toggle("active")
来源：http://wap.fehbvm.com/Article/details/gbvcuhpho.sHtML

[U102] JS：本地存储
来源：http://read.share.hesvh.cn/Article/details/gxbjogxnb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://blog.fehbvm.com/Article/details/gxdyzshmi.sHtML

[U103] JS：定时器
来源：http://blog.zdbjq.cn/Article/details/geubahrwn.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.zdbjq.cn/Article/details/ggsznirfc.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gosgyjgys.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gpynbikgu.sHtML

[U105] JS：节流
来源：http://mobile.fehbvm.com/Article/details/gtppqpfvz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.fehbvm.com/Article/details/gdrvglwkc.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/gictwlkcn.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.share.hesvh.cn/Article/details/gfwxzcmzv.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/grtigtgls.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/ggfkjlqdw.sHtML

[U108] JS：随机整数
来源：http://baike.zdbjq.cn/Article/details/gfevcyugy.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gdgvbynqi.sHtML

[U109] JS：数组分组
来源：http://www.m.share.fehbvm.com/Article/details/gaoymxkcx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gpdxsomos.sHtML

[U110] JS：数组分块
来源：http://www.share.zdbjq.cn/Article/details/giedxxldy.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/geedztspx.sHtML

[U111] JS：对象转 Map
来源：http://read.share.hesvh.cn/Article/details/gyshjzopv.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gmkakwzgy.sHtML

[U112] JS：字符串补位
来源：http://wap.hesvh.cn/Article/details/gsaxnbmmw.sHtML

"7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gqravkdbh.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gptyqxgla.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gjckutozb.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gthktwdbp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.zdbjq.cn/Article/details/gtoalnroe.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/gntroeckm.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gkdyjlftk.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/gjtxkayia.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.fehbvm.com/Article/details/guttnzhyj.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gyczovtoj.sHtML

npm i -D vitest;  npx vitest
来源：http://read.share.zdbjq.cn/Article/details/grfjidtso.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gqxxzphrx.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/glhmrthdx.sHtML

[U119] JS：生产构建
来源：http://read.share.zdbjq.cn/Article/details/gkhshkkcj.sHtML

npx vite build
来源：http://blog.zdbjq.cn/Article/details/gjtsrluau.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.hesvh.cn/Article/details/gjwngmwcb.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gqjmtinrp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gynludmic.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gzfuxxcup.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzalqvjbd.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gelaopmca.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gzxhfbgkj.sHtML

PHP ............ 252
来源：http://read.share.hesvh.cn/Article/details/gijzasjac.sHtML

JavaScript ..... 252
来源：http://mobile.zdbjq.cn/Article/details/gxkjrbnso.sHtML

TypeScript ..... 212
来源：http://www.share.zdbjq.cn/Article/details/gcwysnbgo.sHtML

Java ........... 212
来源：http://www.m.share.zdbjq.cn/Article/details/gwvuemqgn.sHtML

Go ............. 212
来源：http://3g.fehbvm.com/Article/details/gbjebzmui.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gljgjmpnn.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gafzzvkhe.sHtML

C .............. 30
来源：http://3g.hesvh.cn/Article/details/gjdsbfbrk.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gstocdhnw.sHtML

SQL ............ 90
来源：http://blog.hesvh.cn/Article/details/grnwtwivb.sHtML

Bash ........... 80
来源：http://read.share.zdbjq.cn/Article/details/gucouwmux.sHtML

Kotlin ......... 15
来源：http://www.blog.zdbjq.cn/Article/details/gjdgtnhso.sHtML

Swift .......... 15
来源：http://www.m.share.hesvh.cn/Article/details/gskjmripi.sHtML

Lua ............ 10
来源：http://3g.zdbjq.cn/Article/details/guzdgqjmw.sHtML

Perl ........... 10
来源：http://mobile.zdbjq.cn/Article/details/giitaujoq.sHtML

Scala .......... 10
来源：http://wap.fehbvm.com/Article/details/gjnkvlydk.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/glkcnrjrr.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gtnqrnjsl.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gzfabnehi.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.fehbvm.com/Article/details/gtauuqccc.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/gakdsurup.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gicllyvtl.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gqgxfhwao.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.hesvh.cn/Article/details/gaslrtpik.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gaezooeuy.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gxqtnbllh.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/giymwvoqx.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gccnzsved.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gndsdvbim.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gomvxbnwn.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/gzuqmsquu.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gxeczcyoy.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.blog.hesvh.cn/Article/details/gaildntso.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gfkfjgkvk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gdoojqdds.sHtML

Q SQL 专题                              90
来源：http://read.share.fehbvm.com/Article/details/goydlzyxq.sHtML

R Bash 专题                             80
来源：http://www.share.hesvh.cn/Article/details/guomcpbhc.sHtML

S C / C++ 专题                          60
来源：http://3g.fehbvm.com/Article/details/gprvkejad.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gpfwsquta.sHtML

U 高频实用片段                         120
来源：http://3g.fehbvm.com/Article/details/gxhmmdvhp.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gxhjnnyyu.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/giqozlybb.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gwnxjnshl.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/grwkwppww.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.hesvh.cn/Article/details/gejzuolnj.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/guxrxlkjs.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://blog.hesvh.cn/Article/details/gokixnqpw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.fehbvm.com/Article/details/gqhqvrtoz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.hesvh.cn/Article/details/gmudntgbj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.hesvh.cn/Article/details/gszpefduw.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/gsckvqpoj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtwehxtdk.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.hesvh.cn/Article/details/gkrcerzae.sHtML

Common Programming Examples Cheat Book
来源：http://baike.fehbvm.com/Article/details/gexwscbda.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyndmychj.sHtML

【收录内容】
来源：http://m.share.hesvh.cn/Article/details/gvfgxuoxp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/gpvxnknix.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gisdqtiqs.sHtML

SQL · Bash · C · C++
来源：http://m.share.fehbvm.com/Article/details/gfmhzhtfq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.zdbjq.cn/Article/details/gyxyekchv.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/ggsnajcts.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.share.fehbvm.com/Article/details/gcbmuzqon.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/gvsddwbvh.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gtxyflohk.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/gltvkxodh.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gmolnsbqy.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://3g.zdbjq.cn/Article/details/gvmqfuzrp.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.zdbjq.cn/Article/details/goqroxgqm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/ghlhzrjgd.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gouuyffpw.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gtrgrmxyc.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gfnyofbms.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gngvstfnj.sHtML

【文件统计】
来源：http://www.blog.hesvh.cn/Article/details/gwbbdkfid.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/ggpntcvym.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gwoahesvg.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/ggakcifpw.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gqeoplshn.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gczagevvm.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/ganqyhmlh.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.fehbvm.com/Article/details/gnkiumykj.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/gvxtpptyr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/guoiskgzp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/gdtibjkle.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gzkqvhlmv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://wap.zdbjq.cn/Article/details/gxncvgkjp.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gjhiemcwz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gvaasugbg.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gzdkewkyq.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gfyleunkd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gonicvkip.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://read.share.fehbvm.com/Article/details/gyqlionix.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gnoeqzibi.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.blog.hesvh.cn/Article/details/gqvczowxe.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/gokjwvstf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.hesvh.cn/Article/details/gzdzrhjhw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.hesvh.cn/Article/details/gpjwnmcgs.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gtizqfefj.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gpjxygder.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gztjcxofz.sHtML

A. 基础语法与类型
来源：http://wap.fehbvm.com/Article/details/gwyrscozy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gabunvwyl.sHtML

[A01] Hello World
来源：http://blog.fehbvm.com/Article/details/gqcfynmet.sHtML

Py:   print("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gnywbfcvv.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gglasxijs.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gskbzodfi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.hesvh.cn/Article/details/gywdozmcu.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gyzhdzcfi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://3g.fehbvm.com/Article/details/gabprlldz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.hesvh.cn/Article/details/gttqxfxib.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://blog.hesvh.cn/Article/details/gqpeyhheu.sHtML

[A02] 变量声明与赋值
来源：http://m.share.hesvh.cn/Article/details/gsqgnvqqe.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gmfecciht.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gbcdwaeey.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gfyksqbil.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.fehbvm.com/Article/details/gjetygpal.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.hesvh.cn/Article/details/guiiqelnp.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.zdbjq.cn/Article/details/guqtnqfsf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.zdbjq.cn/Article/details/gmqbqgtxe.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gtnfbcpsl.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gmnipvbcp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.hesvh.cn/Article/details/gshecgbss.sHtML

PHP:  const PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/gbyergyto.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gxjzkrrzr.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gcrxrwebv.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gsmfanznt.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/gyrzfnkhv.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gmzrdyjws.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gterftbuw.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gaidrfknp.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.hesvh.cn/Article/details/gpjkbfgmm.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.hesvh.cn/Article/details/gugbbqqft.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.hesvh.cn/Article/details/gzbxkkryk.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.hesvh.cn/Article/details/genaevtxh.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.hesvh.cn/Article/details/guaboppbk.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.hesvh.cn/Article/details/gwusjforu.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.zdbjq.cn/Article/details/gvazdxqat.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.hesvh.cn/Article/details/ghpqjphje.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/gqnwzjzax.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://3g.fehbvm.com/Article/details/gfinzazid.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/ggrnkhtsa.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gfmwbiblv.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gfrltjxui.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gudrrqkyh.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.fehbvm.com/Article/details/gddtrcdnp.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gfrbexnkf.sHtML

C#:   7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gdccirthv.sHtML

[A06] 字符串转数字
来源：http://wap.hesvh.cn/Article/details/gdakxyccu.sHtML

Py:   int("42"); float("3.14")
来源：http://mobile.zdbjq.cn/Article/details/gdiuwmvte.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.fehbvm.com/Article/details/gsydurzpb.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://read.share.hesvh.cn/Article/details/gzwdzhkbe.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gieydpzfm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.m.share.zdbjq.cn/Article/details/glxpgweai.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.zdbjq.cn/Article/details/gbjdkjbiv.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://wap.zdbjq.cn/Article/details/gxoacyvjg.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gtyeekxtj.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gbndypapv.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/gazwnmikr.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.zdbjq.cn/Article/details/gpvmicqej.sHtML

JS:   String(42); (42).toString()
来源：http://www.m.share.hesvh.cn/Article/details/guqkhpfkx.sHtML

TS:   String(42)
来源：http://www.share.hesvh.cn/Article/details/gknbsiwwa.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://read.share.fehbvm.com/Article/details/gxspcpcsn.sHtML

Go:   strconv.Itoa(42)
来源：http://3g.fehbvm.com/Article/details/ggfccrucb.sHtML

Ruby: 42.to_s
来源：http://m.share.zdbjq.cn/Article/details/ginevkkue.sHtML

C#:   42.ToString()
来源：http://read.share.hesvh.cn/Article/details/gougisogw.sHtML

[A08] 取整与四舍五入
来源：http://read.share.fehbvm.com/Article/details/gzftyqxef.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gjjhlxhsy.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://m.share.zdbjq.cn/Article/details/ggfsydtfl.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://m.share.fehbvm.com/Article/details/gpkzugyka.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.zdbjq.cn/Article/details/ghzxaucle.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/ggepmpxrl.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gzrefgtje.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://read.share.hesvh.cn/Article/details/glcptsehn.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://m.share.hesvh.cn/Article/details/gmfyqinyj.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.zdbjq.cn/Article/details/grlefxvsv.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gkdvwrwsv.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://blog.fehbvm.com/Article/details/gqamrlmut.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/ghihknyck.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggxvnockn.sHtML


<!-- 参考信息 -->