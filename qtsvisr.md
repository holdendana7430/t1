代发 wailian999

[U47] PHP：联合类型
来源：http://3g.hesvh.cn/Article/details/gwunxgeiv.sHtML

int|string $id
来源：http://mobile.fehbvm.com/Article/details/gfmcngkuc.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gwgmyqjjg.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/gqeybadsr.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gnthejbig.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gmefcliuw.sHtML

[U50] PHP：构造器属性提升
来源：http://baike.hesvh.cn/Article/details/gexlygbfo.sHtML

public function __construct(private int $id) {}
来源：http://read.share.fehbvm.com/Article/details/gmcyrzvbt.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gwwqfqtpn.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/gwkoeepah.sHtML

[U52] PHP：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gqvxluxxp.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gerdsyafa.sHtML

[U53] PHP：空合并运算符
来源：http://www.share.hesvh.cn/Article/details/ginomptvr.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/gyyawixrn.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gvmyttvjl.sHtML

$obj?->method()
来源：http://www.m.share.fehbvm.com/Article/details/gcsfyvfzp.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gfnugwohf.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/gbmkzixrh.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/gahfhebrt.sHtML

f(a: 1, b: 2)
来源：http://3g.zdbjq.cn/Article/details/giqglbljs.sHtML

[U57] PHP：字符串插值
来源：http://3g.fehbvm.com/Article/details/gvdfgyfrj.sHtML

"值: {$a}"
来源：http://blog.fehbvm.com/Article/details/gtpsjzcci.sHtML

[U58] PHP：数组三件套
来源：http://m.share.fehbvm.com/Article/details/gbqatiwar.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.hesvh.cn/Article/details/gavzsfatc.sHtML

[U59] PHP：自定义排序
来源：http://wap.fehbvm.com/Article/details/gdtvwkkup.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gzmvvyjgs.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/ghrplnhlm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.fehbvm.com/Article/details/gavwemmyu.sHtML

[U61] PHP：正则
来源：http://www.m.share.zdbjq.cn/Article/details/gmzqegobx.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gztjklzmj.sHtML

[U62] PHP：日期对象
来源：http://www.m.share.zdbjq.cn/Article/details/gbrtvggil.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.hesvh.cn/Article/details/gtocanhar.sHtML

[U63] PHP：文件读写
来源：http://www.blog.zdbjq.cn/Article/details/gtncrrdzu.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.share.fehbvm.com/Article/details/gmbgquyzb.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.fehbvm.com/Article/details/ggnbhloro.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/grhryeptp.sHtML

[U65] PHP：会话
来源：http://m.share.zdbjq.cn/Article/details/grmlngbgd.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.hesvh.cn/Article/details/gfhgjvuww.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.zdbjq.cn/Article/details/gbodymngc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gylecktcp.sHtML

[U67] PHP：处理文件上传
来源：http://3g.hesvh.cn/Article/details/gnhuyigtf.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://read.share.hesvh.cn/Article/details/gsfuhwevz.sHtML

[U68] PHP：PDO 连接
来源：http://blog.zdbjq.cn/Article/details/gcbtjkmmx.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.hesvh.cn/Article/details/gbipkofeu.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/gfjiojfno.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://blog.hesvh.cn/Article/details/gkhjlajkl.sHtML

[U70] PHP：PDO 事务
来源：http://mobile.zdbjq.cn/Article/details/gsdsricdw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.hesvh.cn/Article/details/gfvicjbbs.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/gnehzqenj.sHtML

throw new RuntimeException("失败", 500);
来源：http://blog.fehbvm.com/Article/details/gwlqczxfh.sHtML

[U72] PHP：写错误日志
来源：http://m.share.zdbjq.cn/Article/details/gzxbgslmm.sHtML

error_log("失败: " . $e->getMessage());
来源：http://wap.fehbvm.com/Article/details/gtnemsqdy.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.fehbvm.com/Article/details/gtrkxmhka.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gggaejquw.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/gyfmdrqjz.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.hesvh.cn/Article/details/ghozttxiv.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gizxuieqy.sHtML

composer require psr/container
来源：http://www.m.share.zdbjq.cn/Article/details/gudbhblyq.sHtML

[U76] PHP：简单路由
来源：http://baike.zdbjq.cn/Article/details/gvmzprmpu.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://mobile.zdbjq.cn/Article/details/gnfcgmlyk.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.hesvh.cn/Article/details/gevyastnf.sHtML

composer require twig/twig
来源：http://m.share.fehbvm.com/Article/details/gxgskxwpp.sHtML

[U78] PHP：单元测试
来源：http://blog.hesvh.cn/Article/details/gdupqsusq.sHtML

composer require --dev phpunit/phpunit
来源：http://read.share.hesvh.cn/Article/details/gbzdvtusx.sHtML

[U79] PHP：静态分析
来源：http://blog.fehbvm.com/Article/details/grghcgwtw.sHtML

composer require --dev phpstan/phpstan
来源：http://read.share.zdbjq.cn/Article/details/gzwrzfyqm.sHtML

[U80] PHP：代码规范修复
来源：http://3g.zdbjq.cn/Article/details/gfxdsqmty.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://baike.hesvh.cn/Article/details/gmalltung.sHtML

[U81] JS：初始化项目
来源：http://mobile.zdbjq.cn/Article/details/groeccald.sHtML

npm init -y;  npm i express
来源：http://www.m.share.hesvh.cn/Article/details/gkgoxmfqz.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gkzlqhqwa.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gobehneby.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fehbvm.com/Article/details/goysjrdgx.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/geaualwpm.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.zdbjq.cn/Article/details/guifrzbii.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fehbvm.com/Article/details/gkbkmkvoe.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gyevwntpz.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gqxadjgmp.sHtML

[U86] JS：空值合并
来源：http://blog.hesvh.cn/Article/details/gogblcwig.sHtML

a ?? b
来源：http://www.share.zdbjq.cn/Article/details/gohcaiawi.sHtML

[U87] JS：解构默认值
来源：http://www.share.fehbvm.com/Article/details/ghfswvasp.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fehbvm.com/Article/details/gzgfaudqf.sHtML

[U88] JS：对象展开合并
来源：http://mobile.hesvh.cn/Article/details/gtuajhfhc.sHtML

{ ...a, ...b }
来源：http://m.share.fehbvm.com/Article/details/gjnzrnxrz.sHtML

[U89] JS：数组去重
来源：http://www.m.share.fehbvm.com/Article/details/geehepbtz.sHtML

[...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gpbzlhlyb.sHtML

[U90] JS：数字数组排序
来源：http://m.share.hesvh.cn/Article/details/grarvrzez.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gmluspyng.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.zdbjq.cn/Article/details/guqmzeztx.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://m.share.fehbvm.com/Article/details/guzitepho.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gsvnzckqn.sHtML

structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gtfzohfas.sHtML

[U93] JS：模板字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmuatmyoq.sHtML

`共 ${n} 条`
来源：http://3g.fehbvm.com/Article/details/gxftdwkuv.sHtML

[U94] JS：箭头函数
来源：http://read.share.hesvh.cn/Article/details/gmtasljdp.sHtML

const double = x => x * 2;
来源：http://mobile.zdbjq.cn/Article/details/grpeoiavg.sHtML

[U95] JS：Promise 包装
来源：http://3g.fehbvm.com/Article/details/gwkgxvrpl.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.fehbvm.com/Article/details/gggqjqysj.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fehbvm.com/Article/details/gizqdvtra.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gzcrihqzu.sHtML

[U97] JS：并发请求
来源：http://read.share.zdbjq.cn/Article/details/gsyeleyym.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gmsdjduoz.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.hesvh.cn/Article/details/gimxrsern.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.share.hesvh.cn/Article/details/gqyjormev.sHtML

[U99] JS：事件监听
来源：http://blog.fehbvm.com/Article/details/gxgfslttt.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gitnqbglf.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/geubxhafm.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gurkvundd.sHtML

[U101] JS：classList 操作
来源：http://www.blog.hesvh.cn/Article/details/ggvmryaiu.sHtML

el.classList.toggle("active")
来源：http://m.share.fehbvm.com/Article/details/gycvqkvgv.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gxtopnsqa.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.m.share.fehbvm.com/Article/details/gisaeaolc.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gjdjcsgsw.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://wap.zdbjq.cn/Article/details/grpqxeear.sHtML

[U104] JS：防抖
来源：http://blog.zdbjq.cn/Article/details/gmoowxoog.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gxjjfolcw.sHtML

[U105] JS：节流
来源：http://baike.zdbjq.cn/Article/details/gwfjwnuon.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://mobile.hesvh.cn/Article/details/gbuvtskme.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/getqmtedy.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gdeajyvee.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gzjkenxud.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gadhewiuv.sHtML

[U108] JS：随机整数
来源：http://3g.zdbjq.cn/Article/details/gbyfiypjo.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/gxgqzthov.sHtML

[U109] JS：数组分组
来源：http://www.blog.fehbvm.com/Article/details/gcnzvgtgh.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/grlbysoqa.sHtML

[U110] JS：数组分块
来源：http://www.blog.hesvh.cn/Article/details/gaggykqna.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/glvrohuaz.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.hesvh.cn/Article/details/givpupdkv.sHtML

new Map(Object.entries(obj))
来源：http://m.share.fehbvm.com/Article/details/geejpdcbr.sHtML

[U112] JS：字符串补位
来源：http://www.share.fehbvm.com/Article/details/gektowtpu.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gcvowodgj.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gyoklxmex.sHtML

s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gsvpvqevg.sHtML

[U114] JS：JSON 深比较
来源：http://www.share.fehbvm.com/Article/details/gexxxfevr.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/ggsvwrhpt.sHtML

[U115] JS：生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gewtsbfta.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gnxytrjyz.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gibttnmtw.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gclzqzsja.sHtML

[U117] JS：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gdhwrsdfa.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.zdbjq.cn/Article/details/ghpgeiiiw.sHtML

[U118] JS：开发服务器
来源：http://3g.hesvh.cn/Article/details/gwygtgbpk.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.hesvh.cn/Article/details/ghzgamcdl.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gzdluuibw.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gvpljxkrn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gktegvfif.sHtML

import.meta.env.VITE_API_URL
来源：http://www.m.share.fehbvm.com/Article/details/gwnrakrak.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guggdndog.sHtML

统计汇总
来源：http://mobile.hesvh.cn/Article/details/ghjgqhqee.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyqryrrth.sHtML

按语言统计（条）：
来源：http://wap.zdbjq.cn/Article/details/gumpnzhej.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gsxzablnv.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gyewwohcv.sHtML

JavaScript ..... 252
来源：http://www.share.fehbvm.com/Article/details/gwfwefnfw.sHtML

TypeScript ..... 212
来源：http://www.share.fehbvm.com/Article/details/gumaznpil.sHtML

Java ........... 212
来源：http://m.share.zdbjq.cn/Article/details/gocughehp.sHtML

Go ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/golkvsecp.sHtML

Ruby ........... 212
来源：http://read.share.fehbvm.com/Article/details/gxquanfly.sHtML

C# ............. 212
来源：http://www.share.zdbjq.cn/Article/details/gqrxdxund.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gyoegjlyb.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gwnjzgrmt.sHtML

SQL ............ 90
来源：http://baike.hesvh.cn/Article/details/gikpoxbvw.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gqywpciel.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gywlxhpff.sHtML

Swift .......... 15
来源：http://www.m.share.fehbvm.com/Article/details/gofvnqbxf.sHtML

Lua ............ 10
来源：http://www.blog.zdbjq.cn/Article/details/godlfntku.sHtML

Perl ........... 10
来源：http://3g.hesvh.cn/Article/details/ggzmzjqeg.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gctnwuogj.sHtML

------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gellxepwl.sHtML

合计 ........... 2106 条
来源：http://read.share.fehbvm.com/Article/details/gwxwrwlbz.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gyupbqfon.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/gskkqzkhp.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gbdbagsfp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/gkjmsfrez.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.zdbjq.cn/Article/details/gehnfzcdn.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fehbvm.com/Article/details/gicolsrqd.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gkgcrhikv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://read.share.fehbvm.com/Article/details/ghkphqvoi.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gfwknehjm.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gzshrvwky.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://mobile.zdbjq.cn/Article/details/giujpcutc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gitlivqpe.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/gfevqbrer.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.hesvh.cn/Article/details/gukyyulfo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.hesvh.cn/Article/details/gkwrqewks.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://blog.hesvh.cn/Article/details/gkveejukk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gojofevql.sHtML

Q SQL 专题                              90
来源：http://wap.zdbjq.cn/Article/details/gzcmrtsym.sHtML

R Bash 专题                             80
来源：http://3g.zdbjq.cn/Article/details/gzgutzroh.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gkbgbloyw.sHtML

T 其他语言补充                          60
来源：http://read.share.zdbjq.cn/Article/details/gljirugvn.sHtML

U 高频实用片段                         120
来源：http://baike.fehbvm.com/Article/details/gnplpzgrg.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gyklkxita.sHtML

合计                                  2106 条
来源：http://mobile.zdbjq.cn/Article/details/grexpphlm.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.zdbjq.cn/Article/details/gempupcfa.sHtML

使用提醒
来源：http://read.share.fehbvm.com/Article/details/guwccahwj.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fehbvm.com/Article/details/gkejmzncp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.m.share.hesvh.cn/Article/details/gnqziinhi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://read.share.hesvh.cn/Article/details/gvvjfbkjw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.m.share.hesvh.cn/Article/details/gfekfekqx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.fehbvm.com/Article/details/gihngppmw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gmmhmbpvt.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gkttuvhpf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxdtvfxak.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/gidbwmwpp.sHtML

Common Programming Examples Cheat Book
来源：http://blog.zdbjq.cn/Article/details/geawngpxt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwavakpic.sHtML

【收录内容】
来源：http://wap.hesvh.cn/Article/details/gwojbgryg.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.zdbjq.cn/Article/details/gfelfwcoz.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/gcxjzoepo.sHtML

SQL · Bash · C · C++
来源：http://www.share.zdbjq.cn/Article/details/gfrnrfuig.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/getosamua.sHtML

【使用说明】
来源：http://www.blog.fehbvm.com/Article/details/gokcpqbuk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fehbvm.com/Article/details/gxcnjkeym.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.fehbvm.com/Article/details/gryibfdpf.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.m.share.fehbvm.com/Article/details/gapttjujm.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gnwjdnmne.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://baike.fehbvm.com/Article/details/gnskpaoid.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gjgdwewti.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gxljespni.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://3g.fehbvm.com/Article/details/glyxffkte.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.fehbvm.com/Article/details/gfxivbegi.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://blog.fehbvm.com/Article/details/gyfxgihpk.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gjmskgykr.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.fehbvm.com/Article/details/gcenesdth.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gqgtavbsm.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://mobile.fehbvm.com/Article/details/gqnghucnu.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gvrdquffd.sHtML

目  录
来源：http://www.blog.zdbjq.cn/Article/details/gdmechpva.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/gsfdixzkd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.fehbvm.com/Article/details/gvcbalyog.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gfhscdgef.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gjocyldjy.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.fehbvm.com/Article/details/gjksrsbbf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://read.share.fehbvm.com/Article/details/gmowgticf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gnxplfefj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.blog.hesvh.cn/Article/details/grghqnctv.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gfrhhrzqj.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gzoqdqano.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.zdbjq.cn/Article/details/gwjhujcre.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/gokbngxey.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/grdzpcfxt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://mobile.zdbjq.cn/Article/details/ghajostlp.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gaxpjcxkf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gltmicwwd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://blog.fehbvm.com/Article/details/gmpnjkifp.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/grmjuwxwu.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/grbrvkevb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbdomuthr.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/ghbgsqtuz.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.zdbjq.cn/Article/details/gdxwmpxai.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glksjegdm.sHtML

A. 基础语法与类型
来源：http://baike.zdbjq.cn/Article/details/grddvfpqx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzbrqpiql.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/grnsfxfmm.sHtML

Py:   print("Hello, World!")
来源：http://www.m.share.zdbjq.cn/Article/details/gykzakzzf.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.fehbvm.com/Article/details/gmlpirerb.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/gqwdtwkka.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.zdbjq.cn/Article/details/gzsgydhfe.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.fehbvm.com/Article/details/gmnkkneug.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.fehbvm.com/Article/details/gwqehouef.sHtML

Ruby: puts "Hello, World!"
来源：http://m.share.zdbjq.cn/Article/details/gkxbnvsuz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.m.share.zdbjq.cn/Article/details/gvzjjxvqk.sHtML

[A02] 变量声明与赋值
来源：http://blog.zdbjq.cn/Article/details/gmjzapumk.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.share.fehbvm.com/Article/details/gevfyhcxc.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.hesvh.cn/Article/details/gzurrdqsp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.hesvh.cn/Article/details/gcenmgasb.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.share.zdbjq.cn/Article/details/gfrstwdus.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gjnaxnfab.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.fehbvm.com/Article/details/gyxwfaxzf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.m.share.hesvh.cn/Article/details/ghgdzqnno.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.fehbvm.com/Article/details/guhwiaben.sHtML

[A03] 常量定义
来源：http://read.share.zdbjq.cn/Article/details/gktvhyxfi.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.fehbvm.com/Article/details/gbfjtmzdt.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gqwlgqtun.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gjpkeqydi.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.hesvh.cn/Article/details/givsxbysl.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gtzkhlqem.sHtML

Go:   const PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/gwsvtckyc.sHtML

Ruby: PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gvoyzkzmz.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gwkurskmn.sHtML

[A04] 判断变量类型
来源：http://wap.hesvh.cn/Article/details/gbjsmuwjg.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/goerhgaoz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/gjhztwhrv.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gqvlbjqwi.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/ggwbjbono.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/gvzvceljt.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.fehbvm.com/Article/details/gclreoxfw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://read.share.hesvh.cn/Article/details/gmmfgxsnf.sHtML

C#:   x.GetType().Name; x is int
来源：http://m.share.hesvh.cn/Article/details/gcmpthwvq.sHtML

[A05] 整数除法与取模
来源：http://m.share.fehbvm.com/Article/details/gievjqvyb.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://baike.hesvh.cn/Article/details/gzknkjhzo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/grerkwatg.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gmncgxuan.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.share.fehbvm.com/Article/details/gwnecyhna.sHtML

Java: 7 / 2; 7 % 2
来源：http://m.share.zdbjq.cn/Article/details/gnhheuriu.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/glldjecrj.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/gsgceuifu.sHtML

C#:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gkjetwpsv.sHtML


<!-- 参考信息 -->