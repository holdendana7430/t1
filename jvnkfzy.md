代发 wailian999

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/gkvocwkwq.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gsfwcgmwi.sHtML

[U62] PHP：日期对象
来源：http://wap.zdbjq.cn/Article/details/gaebjtgsa.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.zdbjq.cn/Article/details/gfvflfscq.sHtML

[U63] PHP：文件读写
来源：http://www.share.zdbjq.cn/Article/details/gfwmauuiq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fehbvm.com/Article/details/gprdkterk.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/gtelsfuxp.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gucungyhj.sHtML

[U65] PHP：会话
来源：http://www.blog.zdbjq.cn/Article/details/gjmxaiceo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.zdbjq.cn/Article/details/glcmmzfac.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gksqbchfx.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.hesvh.cn/Article/details/gfajfukwd.sHtML

[U67] PHP：处理文件上传
来源：http://www.share.fehbvm.com/Article/details/geowgqcmi.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.hesvh.cn/Article/details/gudrjlpou.sHtML

[U68] PHP：PDO 连接
来源：http://baike.hesvh.cn/Article/details/gagsicnha.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/graqyemqe.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gjchkdmiu.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/ggpuplrlk.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/gcbyqbire.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gfxusxrps.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gohkbfxmu.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gacthwswt.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.zdbjq.cn/Article/details/gsrnypzqg.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.hesvh.cn/Article/details/gvlmvxkyt.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gdsgrmpws.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.zdbjq.cn/Article/details/gybsrahgp.sHtML

[U74] PHP：读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gmtdcwjim.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.fehbvm.com/Article/details/gwjofivpy.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gwkbotorr.sHtML

composer require psr/container
来源：http://mobile.hesvh.cn/Article/details/gskkxntrj.sHtML

[U76] PHP：简单路由
来源：http://baike.hesvh.cn/Article/details/gdsiqqinb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fehbvm.com/Article/details/gnuzoamax.sHtML

[U77] PHP：模板渲染
来源：http://mobile.zdbjq.cn/Article/details/gbjhwoero.sHtML

composer require twig/twig
来源：http://wap.hesvh.cn/Article/details/golcgkgls.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/grumvhgbj.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.zdbjq.cn/Article/details/geyoxdwpi.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.zdbjq.cn/Article/details/gwqdncrpv.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.hesvh.cn/Article/details/gywzyufco.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fehbvm.com/Article/details/gpkpjobuc.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gazbjbkqy.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gqcqmkpos.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gkbtkwjpf.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.hesvh.cn/Article/details/gqekjibyq.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gloftufgt.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.share.fehbvm.com/Article/details/gddlgjjki.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gogimrjdr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.fehbvm.com/Article/details/gtscqgykj.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.zdbjq.cn/Article/details/gwfobmrvq.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gpgorzlql.sHtML

a?.b?.c
来源：http://www.blog.fehbvm.com/Article/details/gbjacehno.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gjxghuvsj.sHtML

a ?? b
来源：http://m.share.zdbjq.cn/Article/details/gxztdxbxu.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.fehbvm.com/Article/details/gldvsvxkk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gyftbywty.sHtML

[U88] JS：对象展开合并
来源：http://m.share.zdbjq.cn/Article/details/gdnvyxchr.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gkpfrnjvd.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gglvgbhbb.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gheiumubl.sHtML

[U90] JS：数字数组排序
来源：http://www.share.zdbjq.cn/Article/details/gzgpatcta.sHtML

[...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gaqclennk.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/guedrdugp.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gsnajiufm.sHtML

[U92] JS：深拷贝
来源：http://www.blog.hesvh.cn/Article/details/gkodeqovz.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/ghrtrazrr.sHtML

[U93] JS：模板字符串
来源：http://www.blog.fehbvm.com/Article/details/gnavjjpoc.sHtML

`共 ${n} 条`
来源：http://www.blog.fehbvm.com/Article/details/gswgzdacj.sHtML

[U94] JS：箭头函数
来源：http://mobile.hesvh.cn/Article/details/gtvedollx.sHtML

const double = x => x * 2;
来源：http://baike.hesvh.cn/Article/details/gzxuovawo.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gmgsonrdz.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.fehbvm.com/Article/details/geugopiqr.sHtML

[U96] JS：async/await 与异常
来源：http://baike.fehbvm.com/Article/details/gytkmkhgx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/glfphqsvp.sHtML

[U97] JS：并发请求
来源：http://blog.hesvh.cn/Article/details/gaegkdusn.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gnhsmrmjh.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gtwmgrwxu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/ggjpbdlec.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/glqtrmwxx.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.hesvh.cn/Article/details/gcqwsnqxn.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fehbvm.com/Article/details/gczoeqlrg.sHtML

document.querySelector(".item")
来源：http://baike.zdbjq.cn/Article/details/gbyksetsx.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gzzvsfytd.sHtML

el.classList.toggle("active")
来源：http://baike.fehbvm.com/Article/details/grrjvqsyj.sHtML

[U102] JS：本地存储
来源：http://blog.zdbjq.cn/Article/details/glifgnida.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.fehbvm.com/Article/details/gfxjcgtvp.sHtML

[U103] JS：定时器
来源：http://baike.zdbjq.cn/Article/details/gksqlvots.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gmxdutzdf.sHtML

[U104] JS：防抖
来源：http://m.share.hesvh.cn/Article/details/gwoekvstw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gxpuqjwrd.sHtML

[U105] JS：节流
来源：http://www.blog.zdbjq.cn/Article/details/gsjqvbdth.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/gsowdkqng.sHtML

[U106] JS：日期格式化
来源：http://blog.hesvh.cn/Article/details/gbezmiaac.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gkbijqbcm.sHtML

[U107] JS：数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gpucctria.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gvwjlcbkv.sHtML

[U108] JS：随机整数
来源：http://www.share.zdbjq.cn/Article/details/gyhtcouws.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/gvyjcgbtd.sHtML

[U109] JS：数组分组
来源：http://www.m.share.hesvh.cn/Article/details/gzsneqrhp.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gqxllvofn.sHtML

[U110] JS：数组分块
来源：http://read.share.hesvh.cn/Article/details/gddcrvorm.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.hesvh.cn/Article/details/gdqzimfla.sHtML

[U111] JS：对象转 Map
来源：http://3g.fehbvm.com/Article/details/goxoknrtz.sHtML

new Map(Object.entries(obj))
来源：http://mobile.hesvh.cn/Article/details/gmllaguqt.sHtML

[U112] JS：字符串补位
来源：http://m.share.zdbjq.cn/Article/details/glnpqtzux.sHtML

"7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gqgavluge.sHtML

[U113] JS：正则替换全部
来源：http://www.share.zdbjq.cn/Article/details/gyvfoivjl.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gsmmynphl.sHtML

[U114] JS：JSON 深比较
来源：http://mobile.zdbjq.cn/Article/details/gwfxyvrkw.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gnjsxxhrf.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gcrmdbzgy.sHtML

crypto.randomUUID()
来源：http://blog.fehbvm.com/Article/details/gpxbiriwb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.hesvh.cn/Article/details/glatxlwgo.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gcyulmtrn.sHtML

[U117] JS：单元测试
来源：http://m.share.fehbvm.com/Article/details/ghjfgvaem.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.hesvh.cn/Article/details/gixcbjlfj.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gncugwnya.sHtML

npm i -D vite;  npx vite
来源：http://m.share.zdbjq.cn/Article/details/gxrmxsbyw.sHtML

[U119] JS：生产构建
来源：http://wap.fehbvm.com/Article/details/goqojhcwx.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gcsuvgijy.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.hesvh.cn/Article/details/gfmmmykso.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.hesvh.cn/Article/details/ghszvkikj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwpgthmru.sHtML

统计汇总
来源：http://m.share.fehbvm.com/Article/details/glnavzdwe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghljiszsf.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/gkeokedqj.sHtML

Python ......... 252
来源：http://blog.fehbvm.com/Article/details/gbsbgcphe.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gmiwpeewt.sHtML

JavaScript ..... 252
来源：http://blog.fehbvm.com/Article/details/gtqzctahr.sHtML

TypeScript ..... 212
来源：http://www.blog.fehbvm.com/Article/details/gmrzontqk.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gclpbkudi.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/gnpitgacj.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gkrsokyyq.sHtML

C# ............. 212
来源：http://wap.fehbvm.com/Article/details/gilgboolx.sHtML

C .............. 30
来源：http://blog.fehbvm.com/Article/details/gslfdkufw.sHtML

C++ ............ 30
来源：http://baike.zdbjq.cn/Article/details/gaqunsdqc.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gtrtrnkqw.sHtML

Bash ........... 80
来源：http://www.share.hesvh.cn/Article/details/gwphszdew.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/gybszvnlw.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/guvrswuqq.sHtML

Lua ............ 10
来源：http://blog.hesvh.cn/Article/details/gxclrcxmh.sHtML

Perl ........... 10
来源：http://www.share.fehbvm.com/Article/details/gnesiqkqe.sHtML

Scala .......... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gutweyoez.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gyrwvucfc.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gqpnomjim.sHtML

按章节统计：
来源：http://blog.zdbjq.cn/Article/details/gnmcgglne.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/ghyocrndo.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gadtcznmm.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/grzhgvpae.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gcthxnsik.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.fehbvm.com/Article/details/gfqybevvl.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/ghmttskln.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.share.fehbvm.com/Article/details/goxrrpxvg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gvgsuedhc.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.hesvh.cn/Article/details/ghzyfgehx.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gcjjatmyo.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gohksxtxq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gxualcfiy.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gphihivhh.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gtdxbguai.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.fehbvm.com/Article/details/gseohldev.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/guuliksjf.sHtML

Q SQL 专题                              90
来源：http://mobile.fehbvm.com/Article/details/gnmlrbotp.sHtML

R Bash 专题                             80
来源：http://mobile.fehbvm.com/Article/details/gpmadxauc.sHtML

S C / C++ 专题                          60
来源：http://www.share.zdbjq.cn/Article/details/gzdgfmwom.sHtML

T 其他语言补充                          60
来源：http://www.blog.fehbvm.com/Article/details/goukzokvs.sHtML

U 高频实用片段                         120
来源：http://wap.fehbvm.com/Article/details/grzsfxyqc.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gkkcfdhaf.sHtML

合计                                  2106 条
来源：http://3g.zdbjq.cn/Article/details/gdftsgdsm.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gawouyruo.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gaynxonpc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gmzkmjspr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.hesvh.cn/Article/details/gflkxrxcv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.hesvh.cn/Article/details/gddqxjijp.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gxhekrmtr.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gwttzzbwi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.fehbvm.com/Article/details/gfcmexgdu.sHtML

—— 文件结束 ——
来源：http://blog.hesvh.cn/Article/details/gqtqfzvhu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goegtrrae.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.fehbvm.com/Article/details/ggjidylfa.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gwtooyulu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvwjkaiov.sHtML

【收录内容】
来源：http://m.share.fehbvm.com/Article/details/gdhwjzysi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.hesvh.cn/Article/details/gqmdttpqe.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.zdbjq.cn/Article/details/gwmbjhurb.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gxakvlrhb.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://read.share.zdbjq.cn/Article/details/gltropfly.sHtML

【使用说明】
来源：http://blog.zdbjq.cn/Article/details/gltntjbhf.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.fehbvm.com/Article/details/gajtmxsbl.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/gpqvgvpjt.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fehbvm.com/Article/details/gwrdmxmjv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/grqhzagrf.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.hesvh.cn/Article/details/gwwnnolkb.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.zdbjq.cn/Article/details/gkusrhzeu.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fehbvm.com/Article/details/grsoxxqff.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gcmmunsrm.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.hesvh.cn/Article/details/gjuagdlap.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.zdbjq.cn/Article/details/gcrcncujn.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.zdbjq.cn/Article/details/gjdofichy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.zdbjq.cn/Article/details/gdusywoni.sHtML

【文件统计】
来源：http://www.blog.zdbjq.cn/Article/details/gemqhsbwz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gmdoavkoc.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.fehbvm.com/Article/details/guavhutiz.sHtML

目  录
来源：http://blog.fehbvm.com/Article/details/gpzsqqhly.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gxsvavppt.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.zdbjq.cn/Article/details/guiiamqcc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.share.zdbjq.cn/Article/details/gdsueuqeq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gntbdixao.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gyohpxqmm.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://baike.hesvh.cn/Article/details/gfksccngw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gcghexbxg.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gnkrmwbgl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gbebebzkk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gzbzvtelf.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/grchrgcun.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/glrdzsrjg.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gqdpjuovm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gytzkhqun.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/grorsrzph.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.zdbjq.cn/Article/details/gzyyyhqzq.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gogxqsuiy.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.fehbvm.com/Article/details/gbjagavsm.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gitjszumw.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gtmnrkuwx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gjjlqawfw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/gbgkzanur.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvlhcfpio.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/ghxkgxopj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmleefzjr.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/gqujcjqbb.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gzcottvzf.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/ghggbuitp.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gawwfbxfg.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.zdbjq.cn/Article/details/gmillzole.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.zdbjq.cn/Article/details/gidgobivi.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/gukbkwtaf.sHtML

Ruby: puts "Hello, World!"
来源：http://www.blog.zdbjq.cn/Article/details/gzsixiamh.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gclppeork.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gqkxtvgxs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gsakfishf.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://read.share.hesvh.cn/Article/details/gwzhrjres.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gxnkqzskw.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.hesvh.cn/Article/details/gqnzmymgv.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://read.share.zdbjq.cn/Article/details/grcqhznwr.sHtML

Go:   name := "Alex"; age := 20
来源：http://m.share.zdbjq.cn/Article/details/groryagad.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.zdbjq.cn/Article/details/gnsauaroz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.zdbjq.cn/Article/details/gwobpndjx.sHtML

[A03] 常量定义
来源：http://m.share.hesvh.cn/Article/details/gsbzldkhl.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.zdbjq.cn/Article/details/gfjmjcwnk.sHtML

PHP:  const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gqufccqzk.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gzoqhaazw.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gxmrulqwb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gezlitheh.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gzpzemqxz.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gblhswtyw.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gzozdetha.sHtML

[A04] 判断变量类型
来源：http://m.share.zdbjq.cn/Article/details/gfurwbtai.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.m.share.zdbjq.cn/Article/details/giymzcxsr.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.hesvh.cn/Article/details/giekouoim.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/grkbevuzw.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gmvmcyrlx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.zdbjq.cn/Article/details/gctexivrq.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://wap.fehbvm.com/Article/details/gdmzgxjkb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.hesvh.cn/Article/details/gofbwchpp.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gaieuvbbq.sHtML

[A05] 整数除法与取模
来源：http://wap.fehbvm.com/Article/details/golpvyyht.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gqvhegzpx.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/glmhartry.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gmirototo.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/gvhzssjwp.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gdeddzxcx.sHtML

Go:   7 / 2; 7 % 2
来源：http://3g.fehbvm.com/Article/details/gtoxjvege.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gdravmgpa.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gvijtqwbl.sHtML

[A06] 字符串转数字
来源：http://3g.fehbvm.com/Article/details/ghuoidgyf.sHtML

Py:   int("42"); float("3.14")
来源：http://www.share.zdbjq.cn/Article/details/gdrjgzszr.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.zdbjq.cn/Article/details/ghhnlejbu.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.fehbvm.com/Article/details/gplxriabx.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://3g.zdbjq.cn/Article/details/grsxvhtaf.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.zdbjq.cn/Article/details/ggdkgjjsb.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://3g.fehbvm.com/Article/details/gqaawsxqg.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://read.share.fehbvm.com/Article/details/gbgfbmyvh.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.blog.fehbvm.com/Article/details/gnixkugqn.sHtML

[A07] 数字转字符串
来源：http://mobile.fehbvm.com/Article/details/getwgivry.sHtML

Py:   str(42)
来源：http://3g.zdbjq.cn/Article/details/ggsirfgfs.sHtML

PHP:  (string) 42; strval(42)
来源：http://baike.zdbjq.cn/Article/details/gikeivgtl.sHtML

JS:   String(42); (42).toString()
来源：http://www.share.hesvh.cn/Article/details/gikksgicv.sHtML

TS:   String(42)
来源：http://wap.fehbvm.com/Article/details/gvzggbvlm.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://baike.zdbjq.cn/Article/details/gaujtioid.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gecbqafji.sHtML

Ruby: 42.to_s
来源：http://read.share.zdbjq.cn/Article/details/gxnenmzwp.sHtML

C#:   42.ToString()
来源：http://baike.hesvh.cn/Article/details/gtjnhrcqv.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.zdbjq.cn/Article/details/gjarsyzba.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.m.share.fehbvm.com/Article/details/gkfxtojly.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://3g.zdbjq.cn/Article/details/gyyinzqmq.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.hesvh.cn/Article/details/gvdwcpirz.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://3g.zdbjq.cn/Article/details/gwjhomfia.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://read.share.hesvh.cn/Article/details/gbdnxjiox.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gnyshdddn.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.m.share.zdbjq.cn/Article/details/gfjdsdpvr.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://read.share.zdbjq.cn/Article/details/gnwraucfo.sHtML

[A09] 绝对值与最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gdpkipdvc.sHtML


<!-- 参考信息 -->