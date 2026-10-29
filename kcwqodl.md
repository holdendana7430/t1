代发 wailian999

[U49] PHP：只读属性
来源：http://m.share.hesvh.cn/Article/details/gzitxvqsp.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/gzluupxll.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.fehbvm.com/Article/details/gbgbgvprm.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gbdvywlex.sHtML

[U51] PHP：数组解构
来源：http://baike.fehbvm.com/Article/details/gcqlskbxw.sHtML

[$a, $b] = $arr;
来源：http://www.share.fehbvm.com/Article/details/gptuhocax.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gzqiiemap.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/gflzqtxfn.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gpguvqiom.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.share.zdbjq.cn/Article/details/ghjcbcoqf.sHtML

[U54] PHP：空安全调用
来源：http://blog.zdbjq.cn/Article/details/gxutuxpey.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/gkbzxnzme.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gzhymlggr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/gbwpauvhp.sHtML

[U56] PHP：命名参数
来源：http://blog.zdbjq.cn/Article/details/gkehquscl.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqjtdgyel.sHtML

[U57] PHP：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gihamxuav.sHtML

"值: {$a}"
来源：http://3g.hesvh.cn/Article/details/ghbresdou.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/gmblisjmr.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.zdbjq.cn/Article/details/gpumjwywa.sHtML

[U59] PHP：自定义排序
来源：http://3g.fehbvm.com/Article/details/gjwnclzzm.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gisyiejev.sHtML

[U60] PHP：JSON 编解码
来源：http://mobile.hesvh.cn/Article/details/gpcubcnff.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.zdbjq.cn/Article/details/gwbafhezs.sHtML

[U61] PHP：正则
来源：http://baike.hesvh.cn/Article/details/gmlxogguh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fehbvm.com/Article/details/gpdqbxugh.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gqzousfbf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/guwhrdrpd.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gdalinfyv.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://3g.hesvh.cn/Article/details/gzxevthzh.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gincsxbwo.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.fehbvm.com/Article/details/gibuxvclt.sHtML

[U65] PHP：会话
来源：http://baike.hesvh.cn/Article/details/gjqcxivec.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.hesvh.cn/Article/details/glaapgvrp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gaqsvrzhi.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.hesvh.cn/Article/details/gnndvcnkt.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.fehbvm.com/Article/details/gdplekive.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gxdjuugtq.sHtML

[U68] PHP：PDO 连接
来源：http://www.m.share.hesvh.cn/Article/details/gnuwueruy.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://blog.hesvh.cn/Article/details/gaxujwacn.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.fehbvm.com/Article/details/guouyexoo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.zdbjq.cn/Article/details/gmwiujjlk.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.hesvh.cn/Article/details/grjqxhwah.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.hesvh.cn/Article/details/gimmuvsxp.sHtML

[U71] PHP：抛出异常
来源：http://3g.hesvh.cn/Article/details/gjiuhkkpv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gbwtdzner.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gcuaigslw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gbgztgfyw.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.zdbjq.cn/Article/details/gzkaakuke.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.zdbjq.cn/Article/details/gdjiuvqan.sHtML

[U74] PHP：读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gneblndgr.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gwhxjwdlc.sHtML

[U75] PHP：依赖注入
来源：http://www.share.fehbvm.com/Article/details/gpolhoskx.sHtML

composer require psr/container
来源：http://mobile.fehbvm.com/Article/details/gorpslctp.sHtML

[U76] PHP：简单路由
来源：http://www.share.zdbjq.cn/Article/details/gzcozfeen.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gwwlplezy.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gsstbsdip.sHtML

composer require twig/twig
来源：http://3g.zdbjq.cn/Article/details/gtdsemeug.sHtML

[U78] PHP：单元测试
来源：http://mobile.zdbjq.cn/Article/details/gphlujobp.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.zdbjq.cn/Article/details/gqthmkpjd.sHtML

[U79] PHP：静态分析
来源：http://read.share.zdbjq.cn/Article/details/gvgkgnfni.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gycghugxv.sHtML

[U80] PHP：代码规范修复
来源：http://blog.zdbjq.cn/Article/details/gghozpyhl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.hesvh.cn/Article/details/ggvwgchbv.sHtML

[U81] JS：初始化项目
来源：http://3g.zdbjq.cn/Article/details/gqyajidcj.sHtML

npm init -y;  npm i express
来源：http://www.share.hesvh.cn/Article/details/gxqmtgihp.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.zdbjq.cn/Article/details/gcijmvshb.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://3g.hesvh.cn/Article/details/gnaopqbfz.sHtML

[U83] JS：ES Module 导入导出
来源：http://m.share.hesvh.cn/Article/details/gmkjyftnq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/geqezgavo.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gcryzgtaf.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.share.fehbvm.com/Article/details/gwlxdmyst.sHtML

[U85] JS：可选链
来源：http://www.m.share.zdbjq.cn/Article/details/gjmuifdke.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/gopqfksco.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/gpjhbwejd.sHtML

a ?? b
来源：http://3g.hesvh.cn/Article/details/giipvrnen.sHtML

[U87] JS：解构默认值
来源：http://www.m.share.hesvh.cn/Article/details/gwbexyyjf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://3g.fehbvm.com/Article/details/gzygxsvbr.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/geyedsnqj.sHtML

{ ...a, ...b }
来源：http://www.share.zdbjq.cn/Article/details/gglvwidyj.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/grtytvmyn.sHtML

[...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/gssgevgfj.sHtML

[U90] JS：数字数组排序
来源：http://baike.zdbjq.cn/Article/details/gyqmjlfyz.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gnvfqxfmb.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gjrevberw.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.share.zdbjq.cn/Article/details/gfvacditx.sHtML

[U92] JS：深拷贝
来源：http://www.share.hesvh.cn/Article/details/gykqnjvny.sHtML

structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gxqjihglg.sHtML

[U93] JS：模板字符串
来源：http://www.share.hesvh.cn/Article/details/gyaeaqxcu.sHtML

`共 ${n} 条`
来源：http://3g.hesvh.cn/Article/details/ggbpwtixg.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/gikzxksya.sHtML

const double = x => x * 2;
来源：http://baike.zdbjq.cn/Article/details/gizabtrdk.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.hesvh.cn/Article/details/ggucvcrgk.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.zdbjq.cn/Article/details/guwjswhuw.sHtML

[U96] JS：async/await 与异常
来源：http://m.share.fehbvm.com/Article/details/guwglpbzd.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gpcegzogw.sHtML

[U97] JS：并发请求
来源：http://m.share.fehbvm.com/Article/details/gevcusnlz.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gkenedenw.sHtML

[U98] JS：fetch 带 JSON
来源：http://mobile.zdbjq.cn/Article/details/gvoknvmrl.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/grlzgdonl.sHtML

[U99] JS：事件监听
来源：http://www.share.hesvh.cn/Article/details/ggmghkvuh.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.zdbjq.cn/Article/details/grpjitotw.sHtML

[U100] JS：DOM 查询
来源：http://www.share.zdbjq.cn/Article/details/gewblbekx.sHtML

document.querySelector(".item")
来源：http://www.blog.hesvh.cn/Article/details/gbiqbxmdh.sHtML

[U101] JS：classList 操作
来源：http://baike.fehbvm.com/Article/details/gqgrrgjxz.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gnncvmqif.sHtML

[U102] JS：本地存储
来源：http://m.share.fehbvm.com/Article/details/gwrdsuvqo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/giuhjnkvc.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/gusyhfihq.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/gdrwprzwx.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gaeulcluv.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gaxivazjp.sHtML

[U105] JS：节流
来源：http://3g.zdbjq.cn/Article/details/gbydkzuhh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.hesvh.cn/Article/details/glhbddlvc.sHtML

[U106] JS：日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gjbcecnfq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.fehbvm.com/Article/details/grjppoqjo.sHtML

[U107] JS：数字千分位
来源：http://wap.fehbvm.com/Article/details/gieluyuzw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/girmucgtx.sHtML

[U108] JS：随机整数
来源：http://mobile.hesvh.cn/Article/details/gfrkkoeoe.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/guqbznanf.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gnitpnhil.sHtML

Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gmgkpcedr.sHtML

[U110] JS：数组分块
来源：http://www.m.share.zdbjq.cn/Article/details/gfxqsxkai.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.zdbjq.cn/Article/details/gcitvufqs.sHtML

[U111] JS：对象转 Map
来源：http://www.share.hesvh.cn/Article/details/gxlvcuizc.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gfxqsvzdy.sHtML

[U112] JS：字符串补位
来源：http://blog.fehbvm.com/Article/details/gvpzxquhr.sHtML

"7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gxneozpzi.sHtML

[U113] JS：正则替换全部
来源：http://wap.fehbvm.com/Article/details/gzakfzcjz.sHtML

s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gnrcksbaf.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/gpbibevfd.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.fehbvm.com/Article/details/gjdxveytj.sHtML

[U115] JS：生成 UUID
来源：http://m.share.hesvh.cn/Article/details/gegtzlcab.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gmfvjoopl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.fehbvm.com/Article/details/gfhuwtjhg.sHtML

/** @param {string} name */ function f(name) {}
来源：http://read.share.zdbjq.cn/Article/details/gsenymkcs.sHtML

[U117] JS：单元测试
来源：http://wap.zdbjq.cn/Article/details/ggfxetbor.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.hesvh.cn/Article/details/giqcmeryv.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gqbegfxtx.sHtML

npm i -D vite;  npx vite
来源：http://wap.hesvh.cn/Article/details/gtoojruce.sHtML

[U119] JS：生产构建
来源：http://www.share.hesvh.cn/Article/details/ghcagqmpe.sHtML

npx vite build
来源：http://www.m.share.zdbjq.cn/Article/details/gvgfdkdef.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fehbvm.com/Article/details/guvzgpydm.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.zdbjq.cn/Article/details/gonpdwtuv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwlnzivkq.sHtML

统计汇总
来源：http://www.blog.fehbvm.com/Article/details/gykltbeua.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/golndisly.sHtML

按语言统计（条）：
来源：http://baike.hesvh.cn/Article/details/gaqanmwef.sHtML

Python ......... 252
来源：http://read.share.zdbjq.cn/Article/details/gctlfksfr.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gccsqhocr.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gbapkydqe.sHtML

TypeScript ..... 212
来源：http://www.m.share.zdbjq.cn/Article/details/ggqtkogri.sHtML

Java ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gcgdaueyc.sHtML

Go ............. 212
来源：http://read.share.fehbvm.com/Article/details/gtqfreojs.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gkhuevamm.sHtML

C# ............. 212
来源：http://m.share.zdbjq.cn/Article/details/geutcapst.sHtML

C .............. 30
来源：http://www.share.fehbvm.com/Article/details/ggkpjgjcs.sHtML

C++ ............ 30
来源：http://www.blog.hesvh.cn/Article/details/gkhwytnfy.sHtML

SQL ............ 90
来源：http://m.share.fehbvm.com/Article/details/gcktjkqzi.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gwiqlaktl.sHtML

Kotlin ......... 15
来源：http://www.m.share.hesvh.cn/Article/details/ggcgwusfu.sHtML

Swift .......... 15
来源：http://www.share.hesvh.cn/Article/details/gshodoetm.sHtML

Lua ............ 10
来源：http://www.share.zdbjq.cn/Article/details/ghkaikbvt.sHtML

Perl ........... 10
来源：http://baike.fehbvm.com/Article/details/gmossyfub.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/ghfuxjqwy.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gwwtrbsix.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gwhiemjhq.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gjeppfapk.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gdgssquaw.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/getfruecb.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.blog.fehbvm.com/Article/details/gjlcyuvyh.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gqudpykiv.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gcvzfljll.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/glfvtzkdn.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/gkmqdnsor.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.hesvh.cn/Article/details/givmuuxmg.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://mobile.hesvh.cn/Article/details/gqveqojtt.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.hesvh.cn/Article/details/gwaideler.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gxuioymes.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gqjetvksn.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gzgiakgrw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gzsfnclru.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.zdbjq.cn/Article/details/gghjstzut.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/ganknkfmj.sHtML

Q SQL 专题                              90
来源：http://m.share.zdbjq.cn/Article/details/gcrgyyssl.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gqyltvtrb.sHtML

S C / C++ 专题                          60
来源：http://wap.zdbjq.cn/Article/details/gbewkehrn.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gjnnvxoqp.sHtML

U 高频实用片段                         120
来源：http://www.blog.fehbvm.com/Article/details/gshedduaj.sHtML

------------------------------------
来源：http://wap.hesvh.cn/Article/details/gdngsmxhm.sHtML

合计                                  2106 条
来源：http://www.share.hesvh.cn/Article/details/gdnmsamqo.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gctslzmnv.sHtML

使用提醒
来源：http://www.m.share.zdbjq.cn/Article/details/gugoetigv.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gjqbwtqhb.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gkvevfxix.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://baike.zdbjq.cn/Article/details/gjgmtfafr.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.share.hesvh.cn/Article/details/gncgnmyjb.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gnoidxehw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/grahjfbbz.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gbvljqnuy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gepcwqrmu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://m.share.fehbvm.com/Article/details/ggwflukfm.sHtML

Common Programming Examples Cheat Book
来源：http://wap.zdbjq.cn/Article/details/gjgpjtqpv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glpvaqccg.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gfbecvhxs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/geyzttvop.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.fehbvm.com/Article/details/gyscgbhun.sHtML

SQL · Bash · C · C++
来源：http://blog.zdbjq.cn/Article/details/gvsfdevrf.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.hesvh.cn/Article/details/gxuvhpink.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gxqjgaioe.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gdnzlqrzb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.hesvh.cn/Article/details/gymjbcbbg.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.hesvh.cn/Article/details/gbtwkovtw.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://m.share.fehbvm.com/Article/details/gfioucjpk.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gcraxapdl.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.hesvh.cn/Article/details/gkocxgpmy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://m.share.fehbvm.com/Article/details/gyrpdsetp.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.zdbjq.cn/Article/details/gstyzdwyk.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/gmisalqfo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.fehbvm.com/Article/details/gehtrinuy.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://m.share.fehbvm.com/Article/details/gbwedgrpp.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.zdbjq.cn/Article/details/gpxelezdz.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/gkcxpispz.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.zdbjq.cn/Article/details/gvvfkkrfc.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gudvhnekd.sHtML

目  录
来源：http://mobile.zdbjq.cn/Article/details/gwneywxnu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gfyccqrpr.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.m.share.hesvh.cn/Article/details/gvlbkcjhf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gkqvpicrc.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/gjyhmtgyi.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://wap.hesvh.cn/Article/details/glfoagilh.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.fehbvm.com/Article/details/grpuerckp.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.hesvh.cn/Article/details/gtldxzpbl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gsfvfsnrm.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://m.share.fehbvm.com/Article/details/geyobroii.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/girfzcwww.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/givembtks.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.zdbjq.cn/Article/details/gdenjppep.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gbdkjdpwd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/geeftlzlw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gsbvtthup.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gdwmtuzvw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fehbvm.com/Article/details/gljwvsdar.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.zdbjq.cn/Article/details/gznivehlp.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gaeatlwmc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.fehbvm.com/Article/details/gwqelmdfd.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gemiuaozw.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://baike.fehbvm.com/Article/details/goomcgxzc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxynneacc.sHtML

A. 基础语法与类型
来源：http://read.share.fehbvm.com/Article/details/gcsmefqvi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giuqlpobe.sHtML

[A01] Hello World
来源：http://baike.hesvh.cn/Article/details/gxledsbun.sHtML

Py:   print("Hello, World!")
来源：http://mobile.zdbjq.cn/Article/details/gmziaulii.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.zdbjq.cn/Article/details/gmsmuedou.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gzyyqyapi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://blog.zdbjq.cn/Article/details/gacvbovvd.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/glaufwtrq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gydjgheah.sHtML

Ruby: puts "Hello, World!"
来源：http://read.share.fehbvm.com/Article/details/guklbtlcg.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/grhdqynix.sHtML

[A02] 变量声明与赋值
来源：http://www.share.hesvh.cn/Article/details/gxbztybms.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gnetyerkk.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.hesvh.cn/Article/details/geefinhqp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gailarreg.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gptuyteke.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.hesvh.cn/Article/details/gwtrejxdy.sHtML

Go:   name := "Alex"; age := 20
来源：http://read.share.fehbvm.com/Article/details/glllytkud.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.blog.zdbjq.cn/Article/details/gzcibgdks.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gndslmhaq.sHtML

[A03] 常量定义
来源：http://baike.fehbvm.com/Article/details/gvtmljpgp.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.fehbvm.com/Article/details/gtiatgenj.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gzsewksbp.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/glsalxous.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/grmjjlkxp.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gcxgamddn.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.hesvh.cn/Article/details/gdadzlhmi.sHtML

Ruby: PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gnolganvn.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/grqiuayzi.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gwroqqsql.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fehbvm.com/Article/details/gwovbpsgd.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.hesvh.cn/Article/details/gyaofkwur.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/grfnhivhy.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/ghmwekzqx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.hesvh.cn/Article/details/gbkzwfjvy.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gjsncgnsi.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/gyyxjzewu.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/gfxapdeze.sHtML

[A05] 整数除法与取模
来源：http://blog.hesvh.cn/Article/details/gknvymgnb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.zdbjq.cn/Article/details/gwovvrutk.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gnchchlqw.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/gwklpnfum.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://blog.zdbjq.cn/Article/details/gzffjatwe.sHtML

Java: 7 / 2; 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gxafhshuk.sHtML

Go:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gipywmdaj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://m.share.fehbvm.com/Article/details/giujcqrzp.sHtML

C#:   7 / 2; 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gjdcxskkd.sHtML

[A06] 字符串转数字
来源：http://baike.hesvh.cn/Article/details/gxndjgdgo.sHtML

Py:   int("42"); float("3.14")
来源：http://www.m.share.fehbvm.com/Article/details/grtdlxiuc.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.m.share.zdbjq.cn/Article/details/glzpyqvqs.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://3g.hesvh.cn/Article/details/gmqygjttm.sHtML


<!-- 参考信息 -->