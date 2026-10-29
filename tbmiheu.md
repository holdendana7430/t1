代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://www.blog.zdbjq.cn/Article/details/gykbhufuq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gbrylmfal.sHtML

[U46] PHP：可空类型
来源：http://m.share.zdbjq.cn/Article/details/gophyeofc.sHtML

?string $name = null
来源：http://www.m.share.fehbvm.com/Article/details/gymurudtk.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/gzgpehiil.sHtML

int|string $id
来源：http://wap.hesvh.cn/Article/details/gdxbtofbm.sHtML

[U48] PHP：纯枚举
来源：http://mobile.hesvh.cn/Article/details/gpmpqfnfp.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gdvnhnpht.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gkbjnbwhg.sHtML

public readonly string $name
来源：http://www.m.share.hesvh.cn/Article/details/gmtmfdgea.sHtML

[U50] PHP：构造器属性提升
来源：http://m.share.hesvh.cn/Article/details/gcyrqzdwr.sHtML

public function __construct(private int $id) {}
来源：http://m.share.hesvh.cn/Article/details/gdqbckdiy.sHtML

[U51] PHP：数组解构
来源：http://www.m.share.zdbjq.cn/Article/details/ganibuafk.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gbywfolvp.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gtitwlutr.sHtML

$double = fn($x) => $x * 2;
来源：http://www.m.share.fehbvm.com/Article/details/gfymaukan.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.hesvh.cn/Article/details/gqucqstjz.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.hesvh.cn/Article/details/gchvlgjaq.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fehbvm.com/Article/details/gqamnhxnb.sHtML

$obj?->method()
来源：http://blog.hesvh.cn/Article/details/gricgicso.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/gfqcracgm.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://wap.fehbvm.com/Article/details/gotazsqqq.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gaawgcbbm.sHtML

f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/guhivpbnu.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gdekslbvs.sHtML

"值: {$a}"
来源：http://mobile.hesvh.cn/Article/details/gnmaxytte.sHtML

[U58] PHP：数组三件套
来源：http://wap.zdbjq.cn/Article/details/gdnfdilno.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gztotjifn.sHtML

[U59] PHP：自定义排序
来源：http://mobile.hesvh.cn/Article/details/gksqmpden.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gzyqftpim.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.zdbjq.cn/Article/details/gypcuolun.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.hesvh.cn/Article/details/gjqojnyqd.sHtML

[U61] PHP：正则
来源：http://read.share.hesvh.cn/Article/details/guerpxzmh.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gzexudzxe.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gfafmxhhb.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.hesvh.cn/Article/details/gcjxeptzj.sHtML

[U63] PHP：文件读写
来源：http://m.share.fehbvm.com/Article/details/gqtlwnulo.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://m.share.fehbvm.com/Article/details/gzdepqmzs.sHtML

[U64] PHP：目录遍历
来源：http://3g.zdbjq.cn/Article/details/gdonanhxg.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.share.hesvh.cn/Article/details/gadovvfsx.sHtML

[U65] PHP：会话
来源：http://blog.hesvh.cn/Article/details/gkudsvplq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.hesvh.cn/Article/details/gqleuztne.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.fehbvm.com/Article/details/gmrnqibfb.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gcalelioi.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/ghckapwav.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gvawlqtrb.sHtML

[U68] PHP：PDO 连接
来源：http://blog.fehbvm.com/Article/details/gbeokcmeo.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gzsjmqrkc.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.fehbvm.com/Article/details/glhmryrnc.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.zdbjq.cn/Article/details/gitnckqbz.sHtML

[U70] PHP：PDO 事务
来源：http://www.blog.hesvh.cn/Article/details/gwjmnwqez.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gwreormfv.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gxhncunqt.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gpxhdkeid.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/gjuuqltai.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.hesvh.cn/Article/details/gxfwyrlue.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.fehbvm.com/Article/details/gtlohmnio.sHtML

parse_ini_file("config.ini", true)
来源：http://www.share.zdbjq.cn/Article/details/gersmvdnz.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gfphcxqfh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.fehbvm.com/Article/details/gdztetatw.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/ghfdwsesx.sHtML

composer require psr/container
来源：http://3g.fehbvm.com/Article/details/gfnccnmtu.sHtML

[U76] PHP：简单路由
来源：http://blog.hesvh.cn/Article/details/gshnvyism.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gzzkjljgz.sHtML

[U77] PHP：模板渲染
来源：http://blog.zdbjq.cn/Article/details/gulbgqdkm.sHtML

composer require twig/twig
来源：http://wap.zdbjq.cn/Article/details/gjpeihbmp.sHtML

[U78] PHP：单元测试
来源：http://www.blog.fehbvm.com/Article/details/gddsiqcfi.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gwggixurr.sHtML

[U79] PHP：静态分析
来源：http://blog.zdbjq.cn/Article/details/ggvqmrmlv.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/gqzonvbzw.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/girpnexmq.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/grfouguvg.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.zdbjq.cn/Article/details/gywmcvipz.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gfmnkzzdg.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fehbvm.com/Article/details/gugwksnxp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.fehbvm.com/Article/details/gsminfknp.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gqwkoiwqh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/ghbeljdds.sHtML

[U84] JS：CommonJS 写法
来源：http://read.share.hesvh.cn/Article/details/gqsuqtvke.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.hesvh.cn/Article/details/gwwzmiotf.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/genxulxts.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gtbhyeqeh.sHtML

[U86] JS：空值合并
来源：http://mobile.zdbjq.cn/Article/details/gsohrylvs.sHtML

a ?? b
来源：http://mobile.fehbvm.com/Article/details/giaqatlhm.sHtML

[U87] JS：解构默认值
来源：http://m.share.zdbjq.cn/Article/details/gschivuvh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.fehbvm.com/Article/details/gpyervnpz.sHtML

[U88] JS：对象展开合并
来源：http://m.share.fehbvm.com/Article/details/geoligpoz.sHtML

{ ...a, ...b }
来源：http://www.m.share.fehbvm.com/Article/details/gthuoawlw.sHtML

[U89] JS：数组去重
来源：http://blog.hesvh.cn/Article/details/grxmueyhd.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gvmoshuib.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gqnieqyhe.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gpvltsjwv.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.hesvh.cn/Article/details/gqchnceig.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.hesvh.cn/Article/details/gdswgqmoq.sHtML

[U92] JS：深拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gttmumjij.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gnjxviyng.sHtML

[U93] JS：模板字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gibydxhdo.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gpfcazuqm.sHtML

[U94] JS：箭头函数
来源：http://3g.zdbjq.cn/Article/details/gzlwmkcdb.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/grprxwimw.sHtML

[U95] JS：Promise 包装
来源：http://wap.hesvh.cn/Article/details/gifgmpaci.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.fehbvm.com/Article/details/gtlslxgxp.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gpwhgeahc.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gphfwcckh.sHtML

[U97] JS：并发请求
来源：http://www.m.share.hesvh.cn/Article/details/gluatbbyl.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gdshnatgm.sHtML

[U98] JS：fetch 带 JSON
来源：http://read.share.fehbvm.com/Article/details/gtcaapymb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gzhsiaend.sHtML

[U99] JS：事件监听
来源：http://www.share.zdbjq.cn/Article/details/ghfgudpia.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gkigmemat.sHtML

[U100] JS：DOM 查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjtvmqjor.sHtML

document.querySelector(".item")
来源：http://www.m.share.fehbvm.com/Article/details/gqicuduvu.sHtML

[U101] JS：classList 操作
来源：http://wap.hesvh.cn/Article/details/gycrbdmro.sHtML

el.classList.toggle("active")
来源：http://m.share.hesvh.cn/Article/details/gsmmhpucb.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gwshxqixf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://baike.hesvh.cn/Article/details/glyeavikl.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gxiewrvxk.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://blog.hesvh.cn/Article/details/gaidvnvxl.sHtML

[U104] JS：防抖
来源：http://www.m.share.hesvh.cn/Article/details/gcapsatoh.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/geoqvqxhn.sHtML

[U105] JS：节流
来源：http://wap.fehbvm.com/Article/details/gvpdopxst.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.blog.hesvh.cn/Article/details/gecnmrnwg.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/ghjinavfl.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.zdbjq.cn/Article/details/gchdrkxqo.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/gglqkbqki.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgiqazdy.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gliggupfu.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://wap.fehbvm.com/Article/details/gawqqlafh.sHtML

[U109] JS：数组分组
来源：http://www.blog.hesvh.cn/Article/details/grujstojv.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/gunpcyggv.sHtML

[U110] JS：数组分块
来源：http://www.blog.zdbjq.cn/Article/details/grijvojpz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gyasqtgyg.sHtML

[U111] JS：对象转 Map
来源：http://blog.zdbjq.cn/Article/details/gzemwjmnw.sHtML

new Map(Object.entries(obj))
来源：http://baike.hesvh.cn/Article/details/gsbewuvds.sHtML

[U112] JS：字符串补位
来源：http://read.share.fehbvm.com/Article/details/gxomrpttg.sHtML

"7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/ghpravxca.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/grdzydajy.sHtML

s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gmxwpvcwr.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/ggewonvjt.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gfrcagzps.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.fehbvm.com/Article/details/gcfmkhmrf.sHtML

crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/grkvzmpvu.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.share.hesvh.cn/Article/details/gdamjfzcd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://blog.zdbjq.cn/Article/details/gshhlsruy.sHtML

[U117] JS：单元测试
来源：http://mobile.zdbjq.cn/Article/details/guleflhwj.sHtML

npm i -D vitest;  npx vitest
来源：http://mobile.zdbjq.cn/Article/details/ghyyxsuzv.sHtML

[U118] JS：开发服务器
来源：http://mobile.hesvh.cn/Article/details/gypqspfle.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/ggixxrgyg.sHtML

[U119] JS：生产构建
来源：http://baike.zdbjq.cn/Article/details/glpxpdaam.sHtML

npx vite build
来源：http://m.share.fehbvm.com/Article/details/ghfynzgqg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/gjvqodevg.sHtML

import.meta.env.VITE_API_URL
来源：http://wap.zdbjq.cn/Article/details/gxphppdla.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwlsulqdn.sHtML

统计汇总
来源：http://read.share.zdbjq.cn/Article/details/gmkatzukx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/garawdbgm.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gdvvirpxv.sHtML

Python ......... 252
来源：http://www.share.fehbvm.com/Article/details/gubueoffz.sHtML

PHP ............ 252
来源：http://3g.zdbjq.cn/Article/details/gvainzaqp.sHtML

JavaScript ..... 252
来源：http://baike.zdbjq.cn/Article/details/gywwfyhcj.sHtML

TypeScript ..... 212
来源：http://mobile.zdbjq.cn/Article/details/gxeaflalw.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gsofdgdnx.sHtML

Go ............. 212
来源：http://3g.zdbjq.cn/Article/details/ghpywnygv.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gpbatfdzp.sHtML

C# ............. 212
来源：http://mobile.zdbjq.cn/Article/details/gcdpgxplj.sHtML

C .............. 30
来源：http://3g.fehbvm.com/Article/details/gatucsfwa.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/ggywrbfkr.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gihwesiiy.sHtML

Bash ........... 80
来源：http://baike.fehbvm.com/Article/details/gvlkfgdor.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gkageefss.sHtML

Swift .......... 15
来源：http://blog.hesvh.cn/Article/details/gkbzjrjbc.sHtML

Lua ............ 10
来源：http://mobile.hesvh.cn/Article/details/gjhedxkrg.sHtML

Perl ........... 10
来源：http://read.share.zdbjq.cn/Article/details/gwxtdehtm.sHtML

Scala .......... 10
来源：http://www.blog.fehbvm.com/Article/details/gyxvvvvtq.sHtML

------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gqpwcinnp.sHtML

合计 ........... 2106 条
来源：http://m.share.hesvh.cn/Article/details/gbufrodtn.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gmbyacxys.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gprsrplbm.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/ggqtwdrtk.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/gqwroebgs.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gkjrlrkpy.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://mobile.fehbvm.com/Article/details/ghaqslqjs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gjzxtmqhk.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.hesvh.cn/Article/details/gcbfrmiin.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://blog.zdbjq.cn/Article/details/gsoyrmbrq.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/guzjncjzp.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gptlkmfcm.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gsnealhrt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gudipyujk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gooizwemo.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gudqymkgj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/gcpvvlaed.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/geopnvaom.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gidsucdls.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/gwpfroimv.sHtML

S C / C++ 专题                          60
来源：http://3g.zdbjq.cn/Article/details/gdpscspod.sHtML

T 其他语言补充                          60
来源：http://3g.zdbjq.cn/Article/details/gzoklcuka.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/gurstprae.sHtML

------------------------------------
来源：http://www.m.share.fehbvm.com/Article/details/ggcdivvlj.sHtML

合计                                  2106 条
来源：http://m.share.fehbvm.com/Article/details/gmgcxyzst.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gwdincusd.sHtML

使用提醒
来源：http://m.share.hesvh.cn/Article/details/gydgzzzuf.sHtML

--------------------------------------------------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gsrymowmd.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gaijabwkr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/ggovohkhh.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://3g.fehbvm.com/Article/details/gprgkmmla.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://m.share.fehbvm.com/Article/details/ghnmzhyyp.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://wap.fehbvm.com/Article/details/gzzmsnrkd.sHtML

—— 文件结束 ——
来源：http://www.m.share.hesvh.cn/Article/details/gzeuwqfmf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grpbqskwd.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/grcfwewtm.sHtML

Common Programming Examples Cheat Book
来源：http://wap.hesvh.cn/Article/details/gyhkofrsx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvakkkbmx.sHtML

【收录内容】
来源：http://www.share.fehbvm.com/Article/details/grvgyjzzw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.zdbjq.cn/Article/details/gkarfgaxg.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.zdbjq.cn/Article/details/gwuqfdbdl.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gzqahzxlq.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.fehbvm.com/Article/details/gzgobasyv.sHtML

【使用说明】
来源：http://www.blog.hesvh.cn/Article/details/gusiabqtt.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.hesvh.cn/Article/details/ggqelxzdx.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://wap.hesvh.cn/Article/details/gybniznne.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gocrcwpum.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.hesvh.cn/Article/details/gbzaicjfl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.fehbvm.com/Article/details/gfoplfkzu.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gzcctulkz.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.hesvh.cn/Article/details/gvudygwmr.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.m.share.fehbvm.com/Article/details/gbogdapgn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.fehbvm.com/Article/details/ghjmikkkl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.blog.fehbvm.com/Article/details/gomqnzrjl.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.fehbvm.com/Article/details/gvqisogqb.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://wap.fehbvm.com/Article/details/gvbaiowzl.sHtML

【文件统计】
来源：http://www.m.share.fehbvm.com/Article/details/grnsiclyr.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://wap.fehbvm.com/Article/details/guayhldzn.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gigbhdfmj.sHtML

目  录
来源：http://www.share.hesvh.cn/Article/details/gfynjlquu.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gprcydokw.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/gdqgllhtc.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.fehbvm.com/Article/details/gunramawv.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/grefmrglt.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.share.fehbvm.com/Article/details/gzsvdrpaf.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://3g.zdbjq.cn/Article/details/gjgfjbtrr.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gkrsxuhck.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gktawpwqk.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fehbvm.com/Article/details/gzfadafpr.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://m.share.hesvh.cn/Article/details/gjnnojmco.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://blog.fehbvm.com/Article/details/gknhysckv.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.fehbvm.com/Article/details/gdlyfqrdw.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/ggeiswsuk.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/ggzxrjagt.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.fehbvm.com/Article/details/gciahhwvo.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.hesvh.cn/Article/details/gacckdzmc.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gocaopaes.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.hesvh.cn/Article/details/gyzlbrjox.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gclugmdhf.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gsuazqypa.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gfkalevkg.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.hesvh.cn/Article/details/getmulpzn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gddynwydb.sHtML

A. 基础语法与类型
来源：http://3g.hesvh.cn/Article/details/ggvktblvi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwoeopnma.sHtML

[A01] Hello World
来源：http://mobile.hesvh.cn/Article/details/gwvptimtv.sHtML

Py:   print("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gmgtdohch.sHtML

PHP:  echo "Hello, World!";
来源：http://baike.zdbjq.cn/Article/details/giekrnbak.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.fehbvm.com/Article/details/gfeinzmzi.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/grggsiari.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/glouzbytq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gqxgiwmtj.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.zdbjq.cn/Article/details/gzalcnihr.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gelqsjoyy.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/geznmtlia.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.zdbjq.cn/Article/details/gucbpgunj.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://mobile.zdbjq.cn/Article/details/gxfwvjunp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://mobile.fehbvm.com/Article/details/ggkqkzzhc.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fehbvm.com/Article/details/gomlptclk.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gtmzzdoiu.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.fehbvm.com/Article/details/gkfnyfzxf.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gujgjkiua.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://mobile.hesvh.cn/Article/details/ghyhhyaec.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/gwtakcsbq.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.share.hesvh.cn/Article/details/gnmjlwddi.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gyanqkxad.sHtML

JS:   const PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gfnwsejrv.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gwejyfuvh.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gprgiacap.sHtML

Go:   const PI = 3.14159
来源：http://mobile.zdbjq.cn/Article/details/gmdfwhcuh.sHtML

Ruby: PI = 3.14159
来源：http://baike.hesvh.cn/Article/details/gsuzwzknu.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gmtxazots.sHtML

[A04] 判断变量类型
来源：http://3g.zdbjq.cn/Article/details/gipihzaim.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.zdbjq.cn/Article/details/gjiwbappn.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gieufpgug.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/gybawjjqy.sHtML

TS:   typeof x; x instanceof Date
来源：http://wap.zdbjq.cn/Article/details/gvnwcfxpx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.blog.fehbvm.com/Article/details/gurafjjrd.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://m.share.fehbvm.com/Article/details/gfmygmsez.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.fehbvm.com/Article/details/ghnbyehmg.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.zdbjq.cn/Article/details/geudlnvjy.sHtML

[A05] 整数除法与取模
来源：http://3g.fehbvm.com/Article/details/ggmdmbrtr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.hesvh.cn/Article/details/gcrzfiymd.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://wap.zdbjq.cn/Article/details/gnylprngk.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.fehbvm.com/Article/details/gesfzpmvc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://mobile.fehbvm.com/Article/details/gzrwqlank.sHtML


<!-- 参考信息 -->