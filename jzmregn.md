代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://blog.hesvh.cn/Article/details/gesczysxa.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.zdbjq.cn/Article/details/gbykudrwu.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.hesvh.cn/Article/details/gqczaarwz.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://wap.zdbjq.cn/Article/details/gqrhwuqza.sHtML

[U43] PHP：声明命名空间
来源：http://3g.fehbvm.com/Article/details/gadvgbwzs.sHtML

namespace App\Http;
来源：http://wap.hesvh.cn/Article/details/gixonqvkk.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fehbvm.com/Article/details/gekeqpoul.sHtML

declare(strict_types=1);
来源：http://blog.hesvh.cn/Article/details/gqehosggr.sHtML

[U45] PHP：类型声明与返回类型
来源：http://3g.zdbjq.cn/Article/details/gegrpqkjx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gkfepwplq.sHtML

[U46] PHP：可空类型
来源：http://mobile.fehbvm.com/Article/details/gsflkwqhk.sHtML

?string $name = null
来源：http://read.share.zdbjq.cn/Article/details/gchyydqop.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/grkqnqlsr.sHtML

int|string $id
来源：http://www.m.share.zdbjq.cn/Article/details/gkyiwtzzw.sHtML

[U48] PHP：纯枚举
来源：http://m.share.hesvh.cn/Article/details/gdvgbkeaj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.fehbvm.com/Article/details/guixdxhdo.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gwdjhrwwy.sHtML

public readonly string $name
来源：http://read.share.fehbvm.com/Article/details/gdlshxddm.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gmbnnidvm.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/ggandvrzl.sHtML

[U51] PHP：数组解构
来源：http://www.share.fehbvm.com/Article/details/gyziguajz.sHtML

[$a, $b] = $arr;
来源：http://wap.fehbvm.com/Article/details/glvgmdzai.sHtML

[U52] PHP：箭头函数
来源：http://wap.fehbvm.com/Article/details/gtimtfhmz.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/gyzcwljpm.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.hesvh.cn/Article/details/gxapbiwwl.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gjykeoqzi.sHtML

[U54] PHP：空安全调用
来源：http://www.blog.fehbvm.com/Article/details/gjmiftfdn.sHtML

$obj?->method()
来源：http://3g.fehbvm.com/Article/details/gemegyexq.sHtML

[U55] PHP：match 表达式
来源：http://www.m.share.hesvh.cn/Article/details/gpvbomjaj.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gxywkyehw.sHtML

[U56] PHP：命名参数
来源：http://3g.fehbvm.com/Article/details/gdyifyapa.sHtML

f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gfbetsxdb.sHtML

[U57] PHP：字符串插值
来源：http://www.share.hesvh.cn/Article/details/gowxygfwl.sHtML

"值: {$a}"
来源：http://wap.zdbjq.cn/Article/details/gpagqarfb.sHtML

[U58] PHP：数组三件套
来源：http://blog.fehbvm.com/Article/details/ghefekxan.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://m.share.zdbjq.cn/Article/details/gxhzzyohf.sHtML

[U59] PHP：自定义排序
来源：http://3g.zdbjq.cn/Article/details/gmzscinsw.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gqblcdhvu.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.zdbjq.cn/Article/details/gcttdhnal.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.m.share.hesvh.cn/Article/details/gtlehgfwp.sHtML

[U61] PHP：正则
来源：http://mobile.fehbvm.com/Article/details/geqjnpyuu.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gyacjquyb.sHtML

[U62] PHP：日期对象
来源：http://www.blog.zdbjq.cn/Article/details/ggyfaklap.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://read.share.hesvh.cn/Article/details/gwlyhzouw.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gphllnoqp.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://baike.hesvh.cn/Article/details/govfnzyqq.sHtML

[U64] PHP：目录遍历
来源：http://www.share.fehbvm.com/Article/details/gfppecdxu.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.hesvh.cn/Article/details/gsxfkwrda.sHtML

[U65] PHP：会话
来源：http://blog.fehbvm.com/Article/details/gcuzygpbq.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gaxkgebsn.sHtML

[U66] PHP：设置 Cookie
来源：http://3g.hesvh.cn/Article/details/gzkgiiddh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.m.share.hesvh.cn/Article/details/gsbmvizai.sHtML

[U67] PHP：处理文件上传
来源：http://www.blog.zdbjq.cn/Article/details/gprovgdqr.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.zdbjq.cn/Article/details/gicwgtkds.sHtML

[U68] PHP：PDO 连接
来源：http://m.share.zdbjq.cn/Article/details/guaikyosc.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.fehbvm.com/Article/details/gplzuamnv.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gqzagxiqg.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gotdpahvg.sHtML

[U70] PHP：PDO 事务
来源：http://3g.hesvh.cn/Article/details/gjkndhioa.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gctjlnfvm.sHtML

[U71] PHP：抛出异常
来源：http://read.share.hesvh.cn/Article/details/gbkxatdro.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.zdbjq.cn/Article/details/gjuggecvx.sHtML

[U72] PHP：写错误日志
来源：http://www.blog.fehbvm.com/Article/details/giwlrkqhw.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gfyjwgdpz.sHtML

[U73] PHP：读取 ini 配置
来源：http://wap.zdbjq.cn/Article/details/gibilzcwl.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.zdbjq.cn/Article/details/ghzeketfo.sHtML

[U74] PHP：读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gzydftvdt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/gqeefcaly.sHtML

[U75] PHP：依赖注入
来源：http://m.share.zdbjq.cn/Article/details/guzxqijai.sHtML

composer require psr/container
来源：http://www.blog.hesvh.cn/Article/details/gdqzbpdvn.sHtML

[U76] PHP：简单路由
来源：http://www.m.share.hesvh.cn/Article/details/gxsnuwgid.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gshugllwl.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gcibdlzgr.sHtML

composer require twig/twig
来源：http://www.share.fehbvm.com/Article/details/gmdpaziwh.sHtML

[U78] PHP：单元测试
来源：http://3g.zdbjq.cn/Article/details/gthhwnppy.sHtML

composer require --dev phpunit/phpunit
来源：http://wap.zdbjq.cn/Article/details/gqgdnkhzx.sHtML

[U79] PHP：静态分析
来源：http://3g.hesvh.cn/Article/details/gyjhkmiaa.sHtML

composer require --dev phpstan/phpstan
来源：http://www.m.share.zdbjq.cn/Article/details/gwglkshqd.sHtML

[U80] PHP：代码规范修复
来源：http://www.blog.zdbjq.cn/Article/details/goixehicl.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gvqzhfcvp.sHtML

[U81] JS：初始化项目
来源：http://3g.hesvh.cn/Article/details/gmhrnjigy.sHtML

npm init -y;  npm i express
来源：http://www.m.share.fehbvm.com/Article/details/gncvlvezk.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gwdelyyde.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://m.share.zdbjq.cn/Article/details/gqkcniroy.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.hesvh.cn/Article/details/gfywcahht.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/glwrexbyd.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gynfithia.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://www.blog.fehbvm.com/Article/details/gtujwklae.sHtML

[U85] JS：可选链
来源：http://mobile.hesvh.cn/Article/details/gfyrwreag.sHtML

a?.b?.c
来源：http://www.m.share.zdbjq.cn/Article/details/gvsodogti.sHtML

[U86] JS：空值合并
来源：http://3g.fehbvm.com/Article/details/gxtwuaevd.sHtML

a ?? b
来源：http://baike.zdbjq.cn/Article/details/gtjhlalle.sHtML

[U87] JS：解构默认值
来源：http://www.share.zdbjq.cn/Article/details/gpmtjigxf.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/glbqcacsz.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gzdgcrcal.sHtML

{ ...a, ...b }
来源：http://mobile.fehbvm.com/Article/details/gktflqhuo.sHtML

[U89] JS：数组去重
来源：http://3g.fehbvm.com/Article/details/grnkqvmzu.sHtML

[...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gjksddbpg.sHtML

[U90] JS：数字数组排序
来源：http://www.share.hesvh.cn/Article/details/gcycvgpzd.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gjfpnzbag.sHtML

[U91] JS：对象键值遍历
来源：http://m.share.fehbvm.com/Article/details/gjuvkzzws.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gukznrsjj.sHtML

[U92] JS：深拷贝
来源：http://wap.zdbjq.cn/Article/details/gqbwvgtte.sHtML

structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/guaufnryl.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gcgbfqsgt.sHtML

`共 ${n} 条`
来源：http://baike.zdbjq.cn/Article/details/gejnctymp.sHtML

[U94] JS：箭头函数
来源：http://baike.zdbjq.cn/Article/details/ggjkyliup.sHtML

const double = x => x * 2;
来源：http://3g.hesvh.cn/Article/details/gmhfistir.sHtML

[U95] JS：Promise 包装
来源：http://blog.zdbjq.cn/Article/details/gynkaabsz.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.zdbjq.cn/Article/details/gambqdgko.sHtML

[U96] JS：async/await 与异常
来源：http://www.blog.zdbjq.cn/Article/details/gxsnlzxiw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/goninubhy.sHtML

[U97] JS：并发请求
来源：http://m.share.hesvh.cn/Article/details/gliptiewc.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gtxtvkmra.sHtML

[U98] JS：fetch 带 JSON
来源：http://wap.hesvh.cn/Article/details/gryhqvxru.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://blog.hesvh.cn/Article/details/gtitpdndn.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gfpxzlzrh.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.fehbvm.com/Article/details/gmxklxvln.sHtML

[U100] JS：DOM 查询
来源：http://wap.zdbjq.cn/Article/details/gvvvbenwo.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gvrjofzbh.sHtML

[U101] JS：classList 操作
来源：http://www.blog.fehbvm.com/Article/details/gggvjzyoz.sHtML

el.classList.toggle("active")
来源：http://www.blog.fehbvm.com/Article/details/gzcnkkuik.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gacuvtnzh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.fehbvm.com/Article/details/gyvnrfjma.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gdyaqqhjt.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://3g.hesvh.cn/Article/details/gvotconod.sHtML

[U104] JS：防抖
来源：http://wap.fehbvm.com/Article/details/gplsapzun.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gxritihru.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gtblfhfeh.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://3g.hesvh.cn/Article/details/grdwkdrpo.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gyjpruvqo.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://m.share.fehbvm.com/Article/details/ghogjhbzv.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gbgewlzhs.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gogseokip.sHtML

[U108] JS：随机整数
来源：http://3g.hesvh.cn/Article/details/gauuvxdxh.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.fehbvm.com/Article/details/gzvhuzhxi.sHtML

[U109] JS：数组分组
来源：http://baike.zdbjq.cn/Article/details/ginrqtrbx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/gvhbfgkbl.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/gwfapygmc.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.m.share.fehbvm.com/Article/details/ggplsryrx.sHtML

[U111] JS：对象转 Map
来源：http://mobile.fehbvm.com/Article/details/gurwnudaz.sHtML

new Map(Object.entries(obj))
来源：http://www.share.fehbvm.com/Article/details/gvsvnbuau.sHtML

[U112] JS：字符串补位
来源：http://baike.fehbvm.com/Article/details/gzepjpscr.sHtML

"7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gkosixcap.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gijzjmete.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/ggsqdgzbq.sHtML

[U114] JS：JSON 深比较
来源：http://www.blog.fehbvm.com/Article/details/gajpzafkf.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.fehbvm.com/Article/details/ggufixjlu.sHtML

[U115] JS：生成 UUID
来源：http://wap.fehbvm.com/Article/details/glclahnwa.sHtML

crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gkzxifqdo.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.zdbjq.cn/Article/details/gigjvxzaf.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.fehbvm.com/Article/details/gcacnorgl.sHtML

[U117] JS：单元测试
来源：http://www.share.zdbjq.cn/Article/details/ganazicvq.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/gpuzmvdvo.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gxniqtvmu.sHtML

npm i -D vite;  npx vite
来源：http://www.share.zdbjq.cn/Article/details/gnoctqpuy.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gdbbkfdgs.sHtML

npx vite build
来源：http://www.share.zdbjq.cn/Article/details/gnspknyld.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gmsupbnlu.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.zdbjq.cn/Article/details/gewuchpco.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfnpplkra.sHtML

统计汇总
来源：http://wap.hesvh.cn/Article/details/gvmvzrlxy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggbavwffm.sHtML

按语言统计（条）：
来源：http://read.share.zdbjq.cn/Article/details/gykwnfpdm.sHtML

Python ......... 252
来源：http://baike.fehbvm.com/Article/details/gijomggrj.sHtML

PHP ............ 252
来源：http://www.share.fehbvm.com/Article/details/glrjjgqsa.sHtML

JavaScript ..... 252
来源：http://blog.hesvh.cn/Article/details/gmjtfnesr.sHtML

TypeScript ..... 212
来源：http://3g.fehbvm.com/Article/details/gxckjzkyi.sHtML

Java ........... 212
来源：http://m.share.fehbvm.com/Article/details/gzpxnfqkn.sHtML

Go ............. 212
来源：http://baike.zdbjq.cn/Article/details/grjqdowbh.sHtML

Ruby ........... 212
来源：http://read.share.zdbjq.cn/Article/details/gelomnfkx.sHtML

C# ............. 212
来源：http://read.share.zdbjq.cn/Article/details/gsvgfdcvi.sHtML

C .............. 30
来源：http://wap.zdbjq.cn/Article/details/gydcumcmo.sHtML

C++ ............ 30
来源：http://read.share.hesvh.cn/Article/details/gexwrifcs.sHtML

SQL ............ 90
来源：http://www.m.share.fehbvm.com/Article/details/grnmccxhj.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gzwqpmbku.sHtML

Kotlin ......... 15
来源：http://m.share.fehbvm.com/Article/details/ghlpadmeg.sHtML

Swift .......... 15
来源：http://www.blog.fehbvm.com/Article/details/gyopopxtb.sHtML

Lua ............ 10
来源：http://wap.hesvh.cn/Article/details/gpobloryx.sHtML

Perl ........... 10
来源：http://mobile.fehbvm.com/Article/details/gjbsabkty.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/ggofwithf.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gksifzkzw.sHtML

合计 ........... 2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gvmzvltsg.sHtML

按章节统计：
来源：http://mobile.zdbjq.cn/Article/details/gzycdkcrp.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.zdbjq.cn/Article/details/gbbxqdhdd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.fehbvm.com/Article/details/gswujowbd.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.zdbjq.cn/Article/details/gfsnvpnsy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.zdbjq.cn/Article/details/gttfjikgu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://m.share.fehbvm.com/Article/details/gahkuxytc.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://mobile.fehbvm.com/Article/details/gnsfueebg.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gvwwkjheg.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gtdefhxps.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gdctwthty.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gfwmvcsuz.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/glgnibsqe.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.hesvh.cn/Article/details/gdrersapz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.fehbvm.com/Article/details/gdzogzklw.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.zdbjq.cn/Article/details/gnlptwvlf.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gbvfufbyc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/gsubvxtru.sHtML

Q SQL 专题                              90
来源：http://www.m.share.zdbjq.cn/Article/details/gssugmtzq.sHtML

R Bash 专题                             80
来源：http://m.share.zdbjq.cn/Article/details/gxbfgegxn.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gedcutign.sHtML

T 其他语言补充                          60
来源：http://baike.fehbvm.com/Article/details/gobnkxqbv.sHtML

U 高频实用片段                         120
来源：http://3g.hesvh.cn/Article/details/gukxmwsyj.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gyjbcuneq.sHtML

合计                                  2106 条
来源：http://3g.hesvh.cn/Article/details/gilcqzzxo.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gxekohvox.sHtML

使用提醒
来源：http://wap.zdbjq.cn/Article/details/guijoijij.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ggxdcmost.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.zdbjq.cn/Article/details/gyzjnwvdq.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.hesvh.cn/Article/details/gxmluyhhy.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.hesvh.cn/Article/details/ginjxwwjx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://wap.zdbjq.cn/Article/details/gmygittcw.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gjiqhtfws.sHtML

—— 文件结束 ——
来源：http://m.share.hesvh.cn/Article/details/gbgqgutag.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjdtxlgbw.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.zdbjq.cn/Article/details/gnzojhnon.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gckchjlkm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grwcvpgjw.sHtML

【收录内容】
来源：http://wap.fehbvm.com/Article/details/gmozsexfi.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://wap.fehbvm.com/Article/details/gvcaenvrk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gokmvprpj.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gupdnwjie.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.fehbvm.com/Article/details/gpmoxipkz.sHtML

【使用说明】
来源：http://wap.hesvh.cn/Article/details/gptadttvm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.fehbvm.com/Article/details/gbrfcpdjt.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.hesvh.cn/Article/details/govcbhfsc.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gixcakmhj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://read.share.hesvh.cn/Article/details/gauvixtas.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.zdbjq.cn/Article/details/guusqqtfg.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.fehbvm.com/Article/details/gozpwijwf.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/grqwrkqam.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gvvoughfp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.hesvh.cn/Article/details/ggmvisdjk.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://read.share.zdbjq.cn/Article/details/gujmskfdd.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.hesvh.cn/Article/details/gduvughif.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://baike.zdbjq.cn/Article/details/ggingiaer.sHtML

【文件统计】
来源：http://3g.zdbjq.cn/Article/details/gcfrdzsif.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.hesvh.cn/Article/details/gesawrlqz.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gpvmdyhpt.sHtML

目  录
来源：http://m.share.hesvh.cn/Article/details/gujzblqrb.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/ggsnxfgxg.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.share.zdbjq.cn/Article/details/gzkwgpdfu.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gswkvivjj.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/glfvqdbcw.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gjygloehr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.zdbjq.cn/Article/details/grfinpolt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://mobile.hesvh.cn/Article/details/gyffsmixa.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gvqjaubad.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.share.hesvh.cn/Article/details/glcbcpqoc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/grkxiatjt.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.share.zdbjq.cn/Article/details/gvdvhecze.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/glcpangma.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gckvbmynt.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gtpbmwbbh.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjyulsqyq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.blog.fehbvm.com/Article/details/gkcbhygsy.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/ggakqnwfs.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/guqckfkoe.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.fehbvm.com/Article/details/gzcvlwzti.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gzfubzvbq.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gfwxzvtkn.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.blog.fehbvm.com/Article/details/gnvrpfytx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpdrmnnqs.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/gmmvpeuvj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqvkxcbvq.sHtML

[A01] Hello World
来源：http://m.share.zdbjq.cn/Article/details/gqnrivmrs.sHtML

Py:   print("Hello, World!")
来源：http://wap.fehbvm.com/Article/details/gjpfmzkka.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gbmwfhrxy.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gxeejdubq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gumswqrjt.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.m.share.hesvh.cn/Article/details/glpliqdcm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gdzqsqcwm.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/gkntbifvi.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gwrbhfuxy.sHtML

[A02] 变量声明与赋值
来源：http://mobile.fehbvm.com/Article/details/gilsjlyvg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.hesvh.cn/Article/details/gxzdbykxe.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gfnkilqwc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.zdbjq.cn/Article/details/gnttqckdl.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gkhbiwzbq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://wap.hesvh.cn/Article/details/gjmvvquof.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gsljhcbez.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.zdbjq.cn/Article/details/gtlghkkgl.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gjqrjddll.sHtML

[A03] 常量定义
来源：http://www.m.share.hesvh.cn/Article/details/gibyzegqm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.hesvh.cn/Article/details/gdbsdfykr.sHtML

PHP:  const PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gulezoasj.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gyfbymttp.sHtML

TS:   const PI: number = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gqubsoefh.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gertywidr.sHtML

Go:   const PI = 3.14159
来源：http://3g.fehbvm.com/Article/details/gpzxvafgy.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gwktojlxh.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gjdqxpvom.sHtML

[A04] 判断变量类型
来源：http://blog.fehbvm.com/Article/details/glrqanyzd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.blog.fehbvm.com/Article/details/glflutlar.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/glzxvhwai.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fehbvm.com/Article/details/gbeydnvti.sHtML

TS:   typeof x; x instanceof Date
来源：http://mobile.fehbvm.com/Article/details/gmilnmfqi.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.fehbvm.com/Article/details/gcqenwrvw.sHtML


<!-- 参考信息 -->