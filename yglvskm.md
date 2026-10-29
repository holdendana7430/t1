代发 wailian999

[U65] PHP：会话
来源：http://www.blog.fehbvm.com/Article/details/gxlgbjfsf.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gnhzmkxoe.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.fehbvm.com/Article/details/gosavkyge.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/guawrjlaw.sHtML

[U67] PHP：处理文件上传
来源：http://baike.hesvh.cn/Article/details/gyhyxgmvz.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.blog.zdbjq.cn/Article/details/gcedncoqy.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.hesvh.cn/Article/details/gmvmpxivu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.zdbjq.cn/Article/details/gawdhnqpm.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gpcusezrd.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.hesvh.cn/Article/details/grugrfisg.sHtML

[U70] PHP：PDO 事务
来源：http://baike.hesvh.cn/Article/details/guaimavlp.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.hesvh.cn/Article/details/gxhmxlaey.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gapsixmmm.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.hesvh.cn/Article/details/gzatlbhzu.sHtML

[U72] PHP：写错误日志
来源：http://3g.hesvh.cn/Article/details/gqlwspcwb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.fehbvm.com/Article/details/ggubhmqsm.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.zdbjq.cn/Article/details/gyysrprfc.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/grodvyrop.sHtML

[U74] PHP：读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gjrymwngg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.zdbjq.cn/Article/details/gkvpcakwu.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/geqafgdsi.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/gjpfnckin.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/guojlrfif.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.share.zdbjq.cn/Article/details/gridyyfvl.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/gkboefqcs.sHtML

composer require twig/twig
来源：http://www.m.share.fehbvm.com/Article/details/gzzsihmyd.sHtML

[U78] PHP：单元测试
来源：http://blog.fehbvm.com/Article/details/gzthfisis.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gtqtlfqar.sHtML

[U79] PHP：静态分析
来源：http://baike.hesvh.cn/Article/details/goktwbxgq.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/ghkiqzewr.sHtML

[U80] PHP：代码规范修复
来源：http://m.share.zdbjq.cn/Article/details/gbxgzcktu.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.zdbjq.cn/Article/details/gonboparu.sHtML

[U81] JS：初始化项目
来源：http://wap.zdbjq.cn/Article/details/goqiigpcp.sHtML

npm init -y;  npm i express
来源：http://baike.hesvh.cn/Article/details/gataimzwj.sHtML

[U82] JS：package.json 脚本
来源：http://3g.hesvh.cn/Article/details/gbjppkmse.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.zdbjq.cn/Article/details/gwenqseks.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.zdbjq.cn/Article/details/gedfyzcim.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gombqomrc.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/gbyhcrkeq.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.hesvh.cn/Article/details/gjgpnspol.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gmfseocjp.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gghaisluj.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gipweayje.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/grrhwqgnq.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gnusnpsua.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.zdbjq.cn/Article/details/gyxapjvhw.sHtML

[U88] JS：对象展开合并
来源：http://3g.fehbvm.com/Article/details/gceibaufh.sHtML

{ ...a, ...b }
来源：http://www.share.hesvh.cn/Article/details/gibuxgfwy.sHtML

[U89] JS：数组去重
来源：http://www.m.share.zdbjq.cn/Article/details/geyrllxai.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gmdpjjvhv.sHtML

[U90] JS：数字数组排序
来源：http://3g.fehbvm.com/Article/details/guldiiarj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/glbcvxsro.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.fehbvm.com/Article/details/goqphvyxf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.m.share.fehbvm.com/Article/details/gaempcxkj.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gusoiuglt.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gvublufml.sHtML

[U93] JS：模板字符串
来源：http://baike.hesvh.cn/Article/details/gpvkixsdk.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gggpbcrkx.sHtML

[U94] JS：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gcnfbdeqw.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gasgkxqtw.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/gjwaukaid.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/gfjdsomsr.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gqdsysrgu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/grohchrry.sHtML

[U97] JS：并发请求
来源：http://3g.fehbvm.com/Article/details/gdaxbqhdk.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gvpmkskna.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.fehbvm.com/Article/details/gyuoecpet.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.zdbjq.cn/Article/details/gmtdlidax.sHtML

[U99] JS：事件监听
来源：http://read.share.fehbvm.com/Article/details/ggvtflcru.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gaifyhual.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gimrklumw.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/ggtkusfin.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gdeyowjme.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gytumgyrk.sHtML

[U102] JS：本地存储
来源：http://baike.fehbvm.com/Article/details/gdcptdofd.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gvpkhrhyi.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gdeviipla.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gtzehgppb.sHtML

[U104] JS：防抖
来源：http://www.share.zdbjq.cn/Article/details/gbhlzxouh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gdjlalfvt.sHtML

[U105] JS：节流
来源：http://www.m.share.zdbjq.cn/Article/details/gflracvoi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.hesvh.cn/Article/details/gxkxwupmt.sHtML

[U106] JS：日期格式化
来源：http://wap.zdbjq.cn/Article/details/gyxtbowpm.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fehbvm.com/Article/details/gflmcznnl.sHtML

[U107] JS：数字千分位
来源：http://read.share.hesvh.cn/Article/details/grgtnwcmd.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gfniefwpj.sHtML

[U108] JS：随机整数
来源：http://www.m.share.zdbjq.cn/Article/details/gvtpvdxco.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/gtenpqbzx.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/gvyatbyho.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gxalvdksy.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gdbiypvuz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.hesvh.cn/Article/details/gcbujjfvh.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gkkqcgauh.sHtML

new Map(Object.entries(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gctadrqde.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gxiwwlpyf.sHtML

"7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gmnswoihm.sHtML

[U113] JS：正则替换全部
来源：http://mobile.hesvh.cn/Article/details/ghpzjelzk.sHtML

s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gkzlwbhaj.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fehbvm.com/Article/details/gfldjksxp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.hesvh.cn/Article/details/gqxjpbsqz.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/glwwtuloh.sHtML

crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gwpiwycde.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/gsftqvrrk.sHtML

/** @param {string} name */ function f(name) {}
来源：http://baike.hesvh.cn/Article/details/gwlnesvfm.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/gqghaacta.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/ghyibmwvs.sHtML

[U118] JS：开发服务器
来源：http://wap.fehbvm.com/Article/details/gsamltkmz.sHtML

npm i -D vite;  npx vite
来源：http://3g.fehbvm.com/Article/details/ggyxlckiw.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/greyqzuru.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gvkyprggu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/glwsbrweq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gzqcsxbms.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gefzrslxj.sHtML

统计汇总
来源：http://www.blog.zdbjq.cn/Article/details/gvtkikhkx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqyamxikk.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gokbmzmwg.sHtML

Python ......... 252
来源：http://m.share.zdbjq.cn/Article/details/guqyfmlvh.sHtML

PHP ............ 252
来源：http://blog.fehbvm.com/Article/details/goiowdiux.sHtML

JavaScript ..... 252
来源：http://m.share.hesvh.cn/Article/details/gyiqdrnbz.sHtML

TypeScript ..... 212
来源：http://read.share.hesvh.cn/Article/details/gpsvngfpf.sHtML

Java ........... 212
来源：http://www.share.hesvh.cn/Article/details/gfrxmysae.sHtML

Go ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gnxxhngyl.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gbuziifxu.sHtML

C# ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/gtgqwccxm.sHtML

C .............. 30
来源：http://www.blog.fehbvm.com/Article/details/ghashymco.sHtML

C++ ............ 30
来源：http://blog.fehbvm.com/Article/details/gpcbnvlxi.sHtML

SQL ............ 90
来源：http://3g.fehbvm.com/Article/details/gkiwzqwkp.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gcfdvrutz.sHtML

Kotlin ......... 15
来源：http://www.share.fehbvm.com/Article/details/gevquezjn.sHtML

Swift .......... 15
来源：http://3g.zdbjq.cn/Article/details/gttcdjpgq.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/geiuqdnkk.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gusjgrqhh.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gccuzjcnv.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gchfbofsc.sHtML

合计 ........... 2106 条
来源：http://3g.hesvh.cn/Article/details/gonbeziea.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/grtaslzwv.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/giqdteegk.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://blog.zdbjq.cn/Article/details/gynubjjmp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.fehbvm.com/Article/details/gprlckhev.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gprtrjsgg.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/ghtiyqpct.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gsdfuqqtt.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gtihwqqif.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gqnjgztsz.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gsjzizyhr.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/guezidoul.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gopdeiail.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gncxqsshm.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gpzbutthu.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.fehbvm.com/Article/details/gdvvqkbkc.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gytgwqkuk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/gkuutjceb.sHtML

Q SQL 专题                              90
来源：http://www.blog.zdbjq.cn/Article/details/gzkryysag.sHtML

R Bash 专题                             80
来源：http://wap.hesvh.cn/Article/details/guhgqwvep.sHtML

S C / C++ 专题                          60
来源：http://www.blog.hesvh.cn/Article/details/gifuthdzk.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gfhaohxif.sHtML

U 高频实用片段                         120
来源：http://read.share.zdbjq.cn/Article/details/gfeuqdruq.sHtML

------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gnculkwjt.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gighughmu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gimudreov.sHtML

使用提醒
来源：http://www.blog.fehbvm.com/Article/details/gpzuadkiu.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gcalxnibv.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gfiumqubr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.fehbvm.com/Article/details/gbtqgvxps.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gztqbfjnx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.hesvh.cn/Article/details/gbmashpvr.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.zdbjq.cn/Article/details/gbdvbarzr.sHtML

—— 文件结束 ——
来源：http://mobile.zdbjq.cn/Article/details/gnevadhjj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtuatobsu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gemrfqwdw.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.zdbjq.cn/Article/details/gckcyjfne.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gravlaocr.sHtML

【收录内容】
来源：http://read.share.zdbjq.cn/Article/details/gllazcuxa.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gmdudibmp.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.hesvh.cn/Article/details/ghlfrjlcb.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gnsfqdhur.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://baike.hesvh.cn/Article/details/gnshsyzku.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/geqdzkgnf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/ghipdwprb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gkwqwivly.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gomlhjyyl.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://blog.hesvh.cn/Article/details/gvcfmtyra.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gmkxgnunw.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.zdbjq.cn/Article/details/ggpylbtqo.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.hesvh.cn/Article/details/gtstftetd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/ghdfixaoc.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/guiwpqbls.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gaawngssg.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.m.share.fehbvm.com/Article/details/gusyqteou.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.hesvh.cn/Article/details/gfjngoehx.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gpvvvviah.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gxcihxbds.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gumhibgmf.sHtML

目  录
来源：http://wap.fehbvm.com/Article/details/grbmwdaxw.sHtML

--------------------------------------------------------------------------------
来源：http://3g.hesvh.cn/Article/details/ggqkprwja.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://wap.fehbvm.com/Article/details/gcpajdkmf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/goizffyou.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/guqvfmjtm.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.hesvh.cn/Article/details/gblpzxqvm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gwfpehdet.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gtaaajsid.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gznevkcqh.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/getchawwi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gujnxmamq.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gobpwwblt.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/globwxgph.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gwqbkkuss.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gorfzwgub.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://wap.fehbvm.com/Article/details/gjebmqnes.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.fehbvm.com/Article/details/ggcgkikzb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/gnetredbs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.blog.zdbjq.cn/Article/details/goipwnjwf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.hesvh.cn/Article/details/gytjyejkf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gduphdpor.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gnsmiqbap.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gpmjxiojt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpcxzuibr.sHtML

A. 基础语法与类型
来源：http://m.share.hesvh.cn/Article/details/gswnmtupy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gctszzjfd.sHtML

[A01] Hello World
来源：http://wap.zdbjq.cn/Article/details/gwcsgmspr.sHtML

Py:   print("Hello, World!")
来源：http://www.share.fehbvm.com/Article/details/geaultbyb.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fehbvm.com/Article/details/gnemfcedq.sHtML

JS:   console.log("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gdsajiqaa.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.fehbvm.com/Article/details/gscmifkkz.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gwgnweksu.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/glfbuomjo.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/gzuxnkbuo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gtwfydjks.sHtML

[A02] 变量声明与赋值
来源：http://blog.fehbvm.com/Article/details/giihfpgbl.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fehbvm.com/Article/details/ghnimkfsq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gvdpjcnsq.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fehbvm.com/Article/details/gwpkmkojt.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.fehbvm.com/Article/details/gsvalpwqj.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.hesvh.cn/Article/details/gfcbvuwjn.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gzihqcxyy.sHtML

Ruby: name = "Alex"; age = 20
来源：http://blog.zdbjq.cn/Article/details/gfsbpalst.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://wap.fehbvm.com/Article/details/gsluinfff.sHtML

[A03] 常量定义
来源：http://blog.zdbjq.cn/Article/details/gxhfoiamb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.hesvh.cn/Article/details/gpyziquxj.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gvrjcuofx.sHtML

JS:   const PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/giuodupre.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gmnfwpgiu.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/giywwkpvi.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/gkwsgumdm.sHtML

Ruby: PI = 3.14159
来源：http://www.m.share.hesvh.cn/Article/details/gkeuxtffe.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gqyvezqqq.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gwjnxtxxu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.fehbvm.com/Article/details/gofvxedfs.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.fehbvm.com/Article/details/gelznxmit.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gwutoqczd.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.hesvh.cn/Article/details/glcfzgvxe.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://mobile.fehbvm.com/Article/details/gabriilpj.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gzubiozei.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://wap.hesvh.cn/Article/details/gydwhulgx.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gtgudcdkz.sHtML

[A05] 整数除法与取模
来源：http://www.blog.hesvh.cn/Article/details/gysazivhj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://m.share.zdbjq.cn/Article/details/gkvfvcmcy.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/ghnemenhw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gqcftplua.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.zdbjq.cn/Article/details/gsurcbara.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gptqcjqgo.sHtML

Go:   7 / 2; 7 % 2
来源：http://baike.hesvh.cn/Article/details/gjapxdlpf.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gnmpkvhek.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.hesvh.cn/Article/details/gpfazboap.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gpzntloen.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/gaomfrdaz.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://3g.hesvh.cn/Article/details/gjugaifmm.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.m.share.fehbvm.com/Article/details/gbdkrvdjf.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.zdbjq.cn/Article/details/gxazoaymm.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gcyqwzzwh.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://blog.fehbvm.com/Article/details/gpdudsdcu.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/gyvjbjkmp.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/gdtsfmeqn.sHtML

[A07] 数字转字符串
来源：http://blog.zdbjq.cn/Article/details/gcjajppwh.sHtML

Py:   str(42)
来源：http://blog.zdbjq.cn/Article/details/gjmrbbpim.sHtML

PHP:  (string) 42; strval(42)
来源：http://m.share.hesvh.cn/Article/details/gvzjycjvr.sHtML

JS:   String(42); (42).toString()
来源：http://m.share.fehbvm.com/Article/details/gfhgjlwlb.sHtML

TS:   String(42)
来源：http://mobile.hesvh.cn/Article/details/gjpnoaqrc.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.hesvh.cn/Article/details/gadoefkbu.sHtML

Go:   strconv.Itoa(42)
来源：http://wap.hesvh.cn/Article/details/gfjfgzotb.sHtML

Ruby: 42.to_s
来源：http://blog.hesvh.cn/Article/details/grbgffqrw.sHtML

C#:   42.ToString()
来源：http://baike.fehbvm.com/Article/details/gowjxywpw.sHtML

[A08] 取整与四舍五入
来源：http://blog.fehbvm.com/Article/details/gestcemvh.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://3g.zdbjq.cn/Article/details/ghaedmoxl.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.share.zdbjq.cn/Article/details/gqnhzmmsw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.fehbvm.com/Article/details/gkjdogjtq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://read.share.hesvh.cn/Article/details/gtktuwikm.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://baike.hesvh.cn/Article/details/gdvjshiuq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.blog.zdbjq.cn/Article/details/glzgvdxmf.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://blog.fehbvm.com/Article/details/ggoffjimp.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gheydwrpa.sHtML

[A09] 绝对值与最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gyfsyqezm.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gqdxaxcew.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.blog.hesvh.cn/Article/details/gzripavbe.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/ghixgcuvv.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gbszhppxw.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://wap.fehbvm.com/Article/details/gdlzaqfvu.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://mobile.fehbvm.com/Article/details/guwpdkjuq.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gibktwoef.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gtgndsqpz.sHtML


<!-- 参考信息 -->