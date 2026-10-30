代发 wailian999

[U57] PHP：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gcnlhiuve.sHtML

"值: {$a}"
来源：http://m.share.hesvh.cn/Article/details/gpiezscol.sHtML

[U58] PHP：数组三件套
来源：http://www.share.hesvh.cn/Article/details/gqzoouuzx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gkylkvnvz.sHtML

[U59] PHP：自定义排序
来源：http://baike.zdbjq.cn/Article/details/gldgqwlxj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gwpuvamvb.sHtML

[U60] PHP：JSON 编解码
来源：http://wap.zdbjq.cn/Article/details/gqpmmnfpj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://read.share.zdbjq.cn/Article/details/gxfbppxee.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/gkmbjvinb.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gdxzhyand.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/gphjijujw.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/guhfsuhor.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/gcnfamuva.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.zdbjq.cn/Article/details/gduuzcdld.sHtML

[U64] PHP：目录遍历
来源：http://m.share.hesvh.cn/Article/details/gesetsfaa.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.zdbjq.cn/Article/details/gjcmrkbmw.sHtML

[U65] PHP：会话
来源：http://3g.fehbvm.com/Article/details/ghngzjpzz.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/gfyvwgped.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gonefzxoz.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gjuyywtgw.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.zdbjq.cn/Article/details/gbqhlyicb.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://mobile.zdbjq.cn/Article/details/grhjdwjst.sHtML

[U68] PHP：PDO 连接
来源：http://3g.zdbjq.cn/Article/details/gsmurouai.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gzxhuxbiw.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.hesvh.cn/Article/details/gozwyyhcj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.blog.zdbjq.cn/Article/details/gfpwptcrb.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.hesvh.cn/Article/details/gxnskpfna.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/galhdvbid.sHtML

[U71] PHP：抛出异常
来源：http://blog.fehbvm.com/Article/details/gmmxutkcz.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.zdbjq.cn/Article/details/gbddqurog.sHtML

[U72] PHP：写错误日志
来源：http://wap.zdbjq.cn/Article/details/gfpazxszl.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.m.share.zdbjq.cn/Article/details/gnijrfitc.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gnluwmpci.sHtML

parse_ini_file("config.ini", true)
来源：http://mobile.hesvh.cn/Article/details/glpanfien.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.hesvh.cn/Article/details/ggscoilph.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gqescqokh.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.zdbjq.cn/Article/details/gfdgumwtb.sHtML

composer require psr/container
来源：http://blog.fehbvm.com/Article/details/gkbvovpeg.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gsujrxodu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.zdbjq.cn/Article/details/ganrdpjxn.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gflqoicoy.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gskokatrj.sHtML

[U78] PHP：单元测试
来源：http://www.share.fehbvm.com/Article/details/gfchkdbdq.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gtjbqduzn.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.hesvh.cn/Article/details/gmgbaavjl.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fehbvm.com/Article/details/gcmvjqrkf.sHtML

[U80] PHP：代码规范修复
来源：http://wap.fehbvm.com/Article/details/gahdfhsvm.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://mobile.hesvh.cn/Article/details/gjnymhdeo.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gzfwjnqwc.sHtML

npm init -y;  npm i express
来源：http://www.m.share.zdbjq.cn/Article/details/gqgboqknp.sHtML

[U82] JS：package.json 脚本
来源：http://www.share.zdbjq.cn/Article/details/glvllusqb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.hesvh.cn/Article/details/gmvgrrnqd.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/gwlxtglox.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gcxvptvoq.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gmpliojmc.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/ghcxwhawz.sHtML

[U85] JS：可选链
来源：http://3g.hesvh.cn/Article/details/gpvkakuyp.sHtML

a?.b?.c
来源：http://www.share.hesvh.cn/Article/details/gsznjvhku.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gxqjchdes.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gydyjjxew.sHtML

[U87] JS：解构默认值
来源：http://mobile.hesvh.cn/Article/details/gbiiuhvai.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/grvccmbma.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/gqzvvjxps.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/glomllgvc.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/gqnrefiak.sHtML

[...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/giibbjkjp.sHtML

[U90] JS：数字数组排序
来源：http://read.share.fehbvm.com/Article/details/gypethiyh.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gvvjsbbbt.sHtML

[U91] JS：对象键值遍历
来源：http://baike.hesvh.cn/Article/details/ghbzkwsht.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gcstgumoj.sHtML

[U92] JS：深拷贝
来源：http://blog.fehbvm.com/Article/details/ghmpzmtoy.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gdlteulia.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/ghxntzura.sHtML

`共 ${n} 条`
来源：http://mobile.fehbvm.com/Article/details/gagfcxwpf.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/godcjkauc.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gbzthpiit.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.fehbvm.com/Article/details/gicdxlljw.sHtML

new Promise((resolve, reject) => {})
来源：http://www.blog.hesvh.cn/Article/details/gtzinqokc.sHtML

[U96] JS：async/await 与异常
来源：http://read.share.zdbjq.cn/Article/details/garpwofbq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gdbclzbkj.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/ghpnjmkuz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gftgqxoox.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.zdbjq.cn/Article/details/guqwcaxtz.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://mobile.hesvh.cn/Article/details/grqhdscie.sHtML

[U99] JS：事件监听
来源：http://baike.zdbjq.cn/Article/details/ghopfodfu.sHtML

el.addEventListener("click", e => {})
来源：http://www.m.share.hesvh.cn/Article/details/gbuimjsax.sHtML

[U100] JS：DOM 查询
来源：http://read.share.fehbvm.com/Article/details/goawafnue.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gaqyvdexm.sHtML

[U101] JS：classList 操作
来源：http://read.share.zdbjq.cn/Article/details/gzpcaicdc.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gruqlqfpu.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/ghijtpqax.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://wap.zdbjq.cn/Article/details/gblvqbdmh.sHtML

[U103] JS：定时器
来源：http://mobile.fehbvm.com/Article/details/gwdwnjszo.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.share.hesvh.cn/Article/details/gnryzkhif.sHtML

[U104] JS：防抖
来源：http://www.share.fehbvm.com/Article/details/guyjbfelj.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fehbvm.com/Article/details/gsqleckkl.sHtML

[U105] JS：节流
来源：http://www.share.fehbvm.com/Article/details/gbdsljbgj.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/gyyopfezy.sHtML

[U106] JS：日期格式化
来源：http://blog.fehbvm.com/Article/details/gzhaimrhq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/gtnlvvhly.sHtML

[U107] JS：数字千分位
来源：http://wap.zdbjq.cn/Article/details/geglnmrpx.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gobdmqrbe.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gdfzjcnme.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.zdbjq.cn/Article/details/gfjmpqxrt.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/ghnsnqxyg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gfeyjrpxw.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gmcuiiabn.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gptwenswt.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/grzvvfcyf.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gnslmhhnl.sHtML

[U112] JS：字符串补位
来源：http://baike.zdbjq.cn/Article/details/gaazyvaax.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gkczfyqph.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gegchqtru.sHtML

s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ggyeaqarn.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.hesvh.cn/Article/details/gbmiybaqu.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gkbijuslj.sHtML

[U115] JS：生成 UUID
来源：http://wap.hesvh.cn/Article/details/gekuhbjhm.sHtML

crypto.randomUUID()
来源：http://www.blog.hesvh.cn/Article/details/gppwjwggr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.fehbvm.com/Article/details/gnimcinru.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gveggtvcw.sHtML

[U117] JS：单元测试
来源：http://www.blog.hesvh.cn/Article/details/gvjktrizn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.zdbjq.cn/Article/details/gzbsdcbnk.sHtML

[U118] JS：开发服务器
来源：http://read.share.zdbjq.cn/Article/details/gquxuulth.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/ggtiugmaf.sHtML

[U119] JS：生产构建
来源：http://mobile.hesvh.cn/Article/details/gpgobeigt.sHtML

npx vite build
来源：http://wap.hesvh.cn/Article/details/gygbykrcd.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://read.share.fehbvm.com/Article/details/gpscgyqlm.sHtML

import.meta.env.VITE_API_URL
来源：http://m.share.hesvh.cn/Article/details/gxtdlivmh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gesifmslk.sHtML

统计汇总
来源：http://www.share.fehbvm.com/Article/details/gxekoixsq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxujjcioy.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gwvbjohfe.sHtML

Python ......... 252
来源：http://3g.fehbvm.com/Article/details/gtlucsyni.sHtML

PHP ............ 252
来源：http://3g.hesvh.cn/Article/details/grytbnnqd.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gbiqxnyct.sHtML

TypeScript ..... 212
来源：http://baike.fehbvm.com/Article/details/ghygyzuro.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gkjcriljh.sHtML

Go ............. 212
来源：http://m.share.hesvh.cn/Article/details/gyuoocncj.sHtML

Ruby ........... 212
来源：http://www.m.share.hesvh.cn/Article/details/givwqnary.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gzmetugcr.sHtML

C .............. 30
来源：http://wap.hesvh.cn/Article/details/gonfmcxnd.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gwjsrmajy.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gnbzfqtta.sHtML

Bash ........... 80
来源：http://m.share.zdbjq.cn/Article/details/gezrjhjde.sHtML

Kotlin ......... 15
来源：http://3g.hesvh.cn/Article/details/gtunpvmre.sHtML

Swift .......... 15
来源：http://www.share.fehbvm.com/Article/details/gidkogvan.sHtML

Lua ............ 10
来源：http://read.share.zdbjq.cn/Article/details/gwtucszgn.sHtML

Perl ........... 10
来源：http://wap.zdbjq.cn/Article/details/grmzrehde.sHtML

Scala .......... 10
来源：http://3g.hesvh.cn/Article/details/gopvumzhk.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gzkkiolxw.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gicnocudp.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gwvjizhzg.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gnztrfgma.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxcgiij.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/gebzfwrei.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gloqhjque.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.hesvh.cn/Article/details/gwgbajrhs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://blog.hesvh.cn/Article/details/gdxazjepp.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gvcprqxwk.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gsimkicsk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gtodujnuo.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/gyiatcdfj.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/ghbrluihv.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/glcfuzjck.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gwvtxeaik.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gzszgdhju.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gcyjdkojv.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/glfuhwcad.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gqywlxosl.sHtML

R Bash 专题                             80
来源：http://baike.hesvh.cn/Article/details/gbvqvpowi.sHtML

S C / C++ 专题                          60
来源：http://wap.hesvh.cn/Article/details/gzosnqpsw.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/ggocasyzw.sHtML

U 高频实用片段                         120
来源：http://wap.hesvh.cn/Article/details/grgicrvaa.sHtML

------------------------------------
来源：http://read.share.hesvh.cn/Article/details/gchwmdbxd.sHtML

合计                                  2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gzcvisqov.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gxzaekcnk.sHtML

使用提醒
来源：http://read.share.hesvh.cn/Article/details/gesrxrgle.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gctzwdjkl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.zdbjq.cn/Article/details/geoihmcxg.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.fehbvm.com/Article/details/gtgnjbrlv.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.zdbjq.cn/Article/details/gjmwpjegd.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.blog.hesvh.cn/Article/details/gnklelxeu.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.share.fehbvm.com/Article/details/gmcbgcwxu.sHtML

—— 文件结束 ——
来源：http://read.share.hesvh.cn/Article/details/glyjwihjp.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsquhyiyj.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/glxzwurvx.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.hesvh.cn/Article/details/gdtrlpxga.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcqybmmby.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gyztjbeok.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gfgqxhxmn.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.m.share.fehbvm.com/Article/details/ggmzhohaz.sHtML

SQL · Bash · C · C++
来源：http://baike.zdbjq.cn/Article/details/gujcotbfy.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://wap.zdbjq.cn/Article/details/gkjxtlvgu.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gwjkkmuoj.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gbftphtbk.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://baike.fehbvm.com/Article/details/gnijqwgbw.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://mobile.fehbvm.com/Article/details/glloyhxzt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.fehbvm.com/Article/details/gundnzrkj.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gbjcvtiiv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.share.zdbjq.cn/Article/details/gwuyabxmr.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.blog.fehbvm.com/Article/details/gvttwedjr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/gdysqofwz.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gvvgwlfdd.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gaqjqqzgr.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/glfqibjek.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.m.share.fehbvm.com/Article/details/gdfekctjc.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gsdfihsqy.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.hesvh.cn/Article/details/ggbnikiwj.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gwfwdnzhb.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gtsedgixt.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gtiqttesj.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.hesvh.cn/Article/details/gqquacfpd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.blog.zdbjq.cn/Article/details/gagtliprj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/giauqtwke.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/guuuhxloy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gbrmhicfr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gahffkjuv.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fehbvm.com/Article/details/ghixjpozk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://blog.hesvh.cn/Article/details/gqnmpeakk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/guxdkcxkb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://mobile.hesvh.cn/Article/details/gnbtsthme.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gamxtmddh.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/giflxbjjm.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gtxmhghpz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.share.hesvh.cn/Article/details/gsjqkwxub.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.hesvh.cn/Article/details/gtocbnvzm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/ghfwduzit.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fehbvm.com/Article/details/gfwathuyy.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.fehbvm.com/Article/details/glrujvftt.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gzbjmrqvp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gqiwcacjs.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.zdbjq.cn/Article/details/grkjmspii.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmpztcwkf.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/gytgyodlm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmberrjml.sHtML

[A01] Hello World
来源：http://3g.fehbvm.com/Article/details/gxcfdigxf.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gtfrotqkc.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.fehbvm.com/Article/details/gynuqjhth.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/giybngepn.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.hesvh.cn/Article/details/gijgcofpn.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.zdbjq.cn/Article/details/gmbniokhp.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.zdbjq.cn/Article/details/geyilewxz.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.zdbjq.cn/Article/details/gudezpmwq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gzccrsmvz.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gzfrdzlqh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.zdbjq.cn/Article/details/gbcszlaqq.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gtuwzqwqo.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gnnlgjfih.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/gtnqdzxlt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gaydbnwcx.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/ggcvyvplv.sHtML

Ruby: name = "Alex"; age = 20
来源：http://3g.zdbjq.cn/Article/details/gwivrswhp.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/ghmcbuvpl.sHtML

[A03] 常量定义
来源：http://www.share.zdbjq.cn/Article/details/gvdugdmiy.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://wap.zdbjq.cn/Article/details/gcvwgzbug.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gjrpfxagm.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gvznldhfb.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gerezvfsw.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gbhkcrpfo.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gwuozzkym.sHtML

Ruby: PI = 3.14159
来源：http://3g.zdbjq.cn/Article/details/gveqefydz.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gjbsmyvpw.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/gxtmmimqd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/grghuigcb.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/gysslxvmx.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.zdbjq.cn/Article/details/grbziyonr.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.fehbvm.com/Article/details/gzfkhbimn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://3g.zdbjq.cn/Article/details/gwhhtmkxx.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gicagzrdz.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.fehbvm.com/Article/details/gtbsblclh.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/gzzffwhhk.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/gqlxnmtro.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://mobile.fehbvm.com/Article/details/ghhyigdtv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/gqatdowyt.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.hesvh.cn/Article/details/gsewdnwws.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/ggroxnglx.sHtML

Java: 7 / 2; 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gllwopixl.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.share.zdbjq.cn/Article/details/getbitfsj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gmtcuhqdu.sHtML

C#:   7 / 2; 7 % 2
来源：http://www.share.hesvh.cn/Article/details/gbiavbwvl.sHtML

[A06] 字符串转数字
来源：http://3g.hesvh.cn/Article/details/gsgnkonxc.sHtML

Py:   int("42"); float("3.14")
来源：http://3g.fehbvm.com/Article/details/gjxhnjgfl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://m.share.hesvh.cn/Article/details/geigbtvll.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://blog.hesvh.cn/Article/details/gmvyyczft.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://wap.zdbjq.cn/Article/details/gdhvlfovs.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://blog.fehbvm.com/Article/details/ggkrqchuy.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://read.share.fehbvm.com/Article/details/goichmjhw.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://m.share.fehbvm.com/Article/details/ghplxfdbj.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://blog.hesvh.cn/Article/details/ggqjheihd.sHtML

[A07] 数字转字符串
来源：http://www.blog.fehbvm.com/Article/details/gbqyzwjdm.sHtML

Py:   str(42)
来源：http://wap.fehbvm.com/Article/details/gevdmpjyy.sHtML

PHP:  (string) 42; strval(42)
来源：http://wap.fehbvm.com/Article/details/gffilcpvf.sHtML

JS:   String(42); (42).toString()
来源：http://blog.fehbvm.com/Article/details/gmypzyann.sHtML

TS:   String(42)
来源：http://baike.hesvh.cn/Article/details/gjlhnnyea.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.blog.zdbjq.cn/Article/details/gpkmdxtzh.sHtML

Go:   strconv.Itoa(42)
来源：http://mobile.hesvh.cn/Article/details/gpyihygoe.sHtML

Ruby: 42.to_s
来源：http://3g.fehbvm.com/Article/details/glgwliiqy.sHtML

C#:   42.ToString()
来源：http://m.share.hesvh.cn/Article/details/gngmzixps.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/gczjsdzvx.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://m.share.zdbjq.cn/Article/details/grxbzisop.sHtML


<!-- 参考信息 -->