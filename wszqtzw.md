代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcvvzbpn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://m.share.fanxiaobao.xyz/Article/details/goocvqiph.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmongavu.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsauawpxh.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gggkcyvhz.sHtML

namespace App\Http;
来源：http://wap.fanxiaobao.xyz/Article/details/grhblgpzz.sHtML

[U44] PHP：开启严格类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjbufwzd.sHtML

declare(strict_types=1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqnckyho.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gclpiyopm.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxvmhhjlu.sHtML

[U46] PHP：可空类型
来源：http://wap.fanxiaobao.xyz/Article/details/gpngawwet.sHtML

?string $name = null
来源：http://m.share.fanxiaobao.xyz/Article/details/gbarrrapg.sHtML

[U47] PHP：联合类型
来源：http://wap.fanxiaobao.xyz/Article/details/ghlcwruzk.sHtML

int|string $id
来源：http://blog.fanxiaobao.xyz/Article/details/ggfueqzce.sHtML

[U48] PHP：纯枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbswpwwvd.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grilnmvdm.sHtML

[U49] PHP：只读属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyhzyabd.sHtML

public readonly string $name
来源：http://3g.fanxiaobao.xyz/Article/details/gzsauwwer.sHtML

[U50] PHP：构造器属性提升
来源：http://blog.fanxiaobao.xyz/Article/details/gavxunstf.sHtML

public function __construct(private int $id) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmfosjnn.sHtML

[U51] PHP：数组解构
来源：http://3g.fanxiaobao.xyz/Article/details/ggslapivk.sHtML

[$a, $b] = $arr;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnsddtzr.sHtML

[U52] PHP：箭头函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcefeower.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktycfpfz.sHtML

[U53] PHP：空合并运算符
来源：http://3g.fanxiaobao.xyz/Article/details/gaibfuvfa.sHtML

$v = $a ?? $b ?? "default";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygliizob.sHtML

[U54] PHP：空安全调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gllcuhdbr.sHtML

$obj?->method()
来源：http://wap.fanxiaobao.xyz/Article/details/gjeppkemx.sHtML

[U55] PHP：match 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/grsaphlsq.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsrskozp.sHtML

[U56] PHP：命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhabxjlh.sHtML

f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/glmqeykut.sHtML

[U57] PHP：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/glpmtakmb.sHtML

"值: {$a}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwnbfnuz.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gladdtzcb.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlsiyife.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcsekobc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/grfuvyqfc.sHtML

[U60] PHP：JSON 编解码
来源：http://www.share.fanxiaobao.xyz/Article/details/gitiseidf.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gugmjhrmn.sHtML

[U61] PHP：正则
来源：http://mobile.fanxiaobao.xyz/Article/details/gzceqqvfc.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsctbqga.sHtML

[U62] PHP：日期对象
来源：http://3g.fanxiaobao.xyz/Article/details/garyrudbj.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmufevqtz.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxuiprkx.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsflbqbw.sHtML

[U64] PHP：目录遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gmwuubxri.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fanxiaobao.xyz/Article/details/gledqutbb.sHtML

[U65] PHP：会话
来源：http://wap.fanxiaobao.xyz/Article/details/gelkhrtis.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyfqlufa.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzpktsdj.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtowjekl.sHtML

[U67] PHP：处理文件上传
来源：http://baike.fanxiaobao.xyz/Article/details/giplwmnaj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://blog.fanxiaobao.xyz/Article/details/gjzmndauo.sHtML

[U68] PHP：PDO 连接
来源：http://baike.fanxiaobao.xyz/Article/details/gdyueklbf.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.fanxiaobao.xyz/Article/details/ghtnlvsyn.sHtML

[U69] PHP：PDO 预处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gavktwbel.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.fanxiaobao.xyz/Article/details/gukyzyber.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gpduhykqw.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.fanxiaobao.xyz/Article/details/gmbtlmlxt.sHtML

[U71] PHP：抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyyzpnjd.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/gkxvdacgd.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fanxiaobao.xyz/Article/details/ghaziwwoe.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.fanxiaobao.xyz/Article/details/gkvzfdxmo.sHtML

[U73] PHP：读取 ini 配置
来源：http://blog.fanxiaobao.xyz/Article/details/gikepsjto.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaqlfoqw.sHtML

[U74] PHP：读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gphihwmsv.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmgmfknt.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fanxiaobao.xyz/Article/details/gehazjmuu.sHtML

composer require psr/container
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnszovqu.sHtML

[U76] PHP：简单路由
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnltrswh.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.fanxiaobao.xyz/Article/details/gwfptagwd.sHtML

[U77] PHP：模板渲染
来源：http://wap.fanxiaobao.xyz/Article/details/gzjydrphi.sHtML

composer require twig/twig
来源：http://baike.fanxiaobao.xyz/Article/details/gkfnqfabk.sHtML

[U78] PHP：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gcjoaebpi.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fanxiaobao.xyz/Article/details/gavotptqh.sHtML

[U79] PHP：静态分析
来源：http://read.share.fanxiaobao.xyz/Article/details/gneqrfnie.sHtML

composer require --dev phpstan/phpstan
来源：http://m.share.fanxiaobao.xyz/Article/details/gloabemyl.sHtML

[U80] PHP：代码规范修复
来源：http://3g.fanxiaobao.xyz/Article/details/giwounesd.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://wap.fanxiaobao.xyz/Article/details/gqucxutpn.sHtML

[U81] JS：初始化项目
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyvjkbpl.sHtML

npm init -y;  npm i express
来源：http://read.share.fanxiaobao.xyz/Article/details/gylgbnzdg.sHtML

[U82] JS：package.json 脚本
来源：http://baike.fanxiaobao.xyz/Article/details/gxdwhivtk.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldbjgfty.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.fanxiaobao.xyz/Article/details/ghnzaazob.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gtpzlvmoa.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnbqceci.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.fanxiaobao.xyz/Article/details/gbewzwmpa.sHtML

[U85] JS：可选链
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomaouiaq.sHtML

a?.b?.c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicbyxclf.sHtML

[U86] JS：空值合并
来源：http://m.share.fanxiaobao.xyz/Article/details/glzcrzvep.sHtML

a ?? b
来源：http://baike.fanxiaobao.xyz/Article/details/gvcgirxih.sHtML

[U87] JS：解构默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/grenopmsh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.fanxiaobao.xyz/Article/details/gqiwoeyru.sHtML

[U88] JS：对象展开合并
来源：http://3g.fanxiaobao.xyz/Article/details/gsnwlzdsy.sHtML

{ ...a, ...b }
来源：http://baike.fanxiaobao.xyz/Article/details/gpifasonz.sHtML

[U89] JS：数组去重
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdhgvbwh.sHtML

[...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gcxtzmdpp.sHtML

[U90] JS：数字数组排序
来源：http://wap.fanxiaobao.xyz/Article/details/gcnilnsag.sHtML

[...arr].sort((a, b) => a - b)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbbmxdcs.sHtML

[U91] JS：对象键值遍历
来源：http://blog.fanxiaobao.xyz/Article/details/glrvvgtef.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://blog.fanxiaobao.xyz/Article/details/galyzydjk.sHtML

[U92] JS：深拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/ggnewcqfv.sHtML

structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gvylmhodz.sHtML

[U93] JS：模板字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gcewrugra.sHtML

`共 ${n} 条`
来源：http://mobile.fanxiaobao.xyz/Article/details/gklhrypdq.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkbycwbx.sHtML

const double = x => x * 2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyinqxpv.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwhtljve.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiyfjkuq.sHtML

[U96] JS：async/await 与异常
来源：http://blog.fanxiaobao.xyz/Article/details/gidpsgqbe.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaztgear.sHtML

[U97] JS：并发请求
来源：http://3g.fanxiaobao.xyz/Article/details/gapmgxkyh.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gmyxxvcso.sHtML

[U98] JS：fetch 带 JSON
来源：http://baike.fanxiaobao.xyz/Article/details/goqkyqdcb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://baike.fanxiaobao.xyz/Article/details/gsfqpogwt.sHtML

[U99] JS：事件监听
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqqegprs.sHtML

el.addEventListener("click", e => {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gpruzrvzm.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxvkbxzqf.sHtML

document.querySelector(".item")
来源：http://baike.fanxiaobao.xyz/Article/details/gglqyylci.sHtML

[U101] JS：classList 操作
来源：http://blog.fanxiaobao.xyz/Article/details/gtsvogxnf.sHtML

el.classList.toggle("active")
来源：http://blog.fanxiaobao.xyz/Article/details/ggvqeqlea.sHtML

[U102] JS：本地存储
来源：http://wap.fanxiaobao.xyz/Article/details/goanpykru.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmujlpqy.sHtML

[U103] JS：定时器
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxthimcb.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fanxiaobao.xyz/Article/details/guyzsmqzb.sHtML

[U104] JS：防抖
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnfpnnjb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fanxiaobao.xyz/Article/details/goldfdjfq.sHtML

[U105] JS：节流
来源：http://www.share.fanxiaobao.xyz/Article/details/gluodcmto.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.fanxiaobao.xyz/Article/details/gwypalssv.sHtML

[U106] JS：日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gducebplq.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlhsnkpm.sHtML

[U107] JS：数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijdyceyh.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gwpurgeli.sHtML

[U108] JS：随机整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnznkdtkw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.fanxiaobao.xyz/Article/details/gkowxgxjh.sHtML

[U109] JS：数组分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gaozxbfla.sHtML

Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gexrjtlaf.sHtML

[U110] JS：数组分块
来源：http://3g.fanxiaobao.xyz/Article/details/gjnncjcis.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgyacmqf.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzthliwhb.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhgcmbbh.sHtML

[U112] JS：字符串补位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuiqmxbg.sHtML

"7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gidyyycaw.sHtML

[U113] JS：正则替换全部
来源：http://3g.fanxiaobao.xyz/Article/details/gmrxrsnbc.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmrbkbye.sHtML

[U114] JS：JSON 深比较
来源：http://baike.fanxiaobao.xyz/Article/details/gguytcbkb.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelepqqdn.sHtML

[U115] JS：生成 UUID
来源：http://blog.fanxiaobao.xyz/Article/details/gnfvimetq.sHtML

crypto.randomUUID()
来源：http://3g.fanxiaobao.xyz/Article/details/gvhpkzctw.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjbilytm.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctxvyvrq.sHtML

[U117] JS：单元测试
来源：http://3g.fanxiaobao.xyz/Article/details/gsmwsdrsr.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.fanxiaobao.xyz/Article/details/gkyfarvaj.sHtML

[U118] JS：开发服务器
来源：http://baike.fanxiaobao.xyz/Article/details/gcrmempio.sHtML

npm i -D vite;  npx vite
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkdxzvxa.sHtML

[U119] JS：生产构建
来源：http://baike.fanxiaobao.xyz/Article/details/gcejbmhtt.sHtML

npx vite build
来源：http://www.share.fanxiaobao.xyz/Article/details/gcivwhvix.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgowenny.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.fanxiaobao.xyz/Article/details/gagydbxmb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtnwhksg.sHtML

统计汇总
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmdgdfik.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaglbkgx.sHtML

按语言统计（条）：
来源：http://3g.fanxiaobao.xyz/Article/details/gxdfudxqc.sHtML

Python ......... 252
来源：http://baike.fanxiaobao.xyz/Article/details/gduhfdmyr.sHtML

PHP ............ 252
来源：http://m.share.fanxiaobao.xyz/Article/details/goxzmwejp.sHtML

JavaScript ..... 252
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmapefizo.sHtML

TypeScript ..... 212
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsaibepq.sHtML

Java ........... 212
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsssuhbk.sHtML

Go ............. 212
来源：http://mobile.fanxiaobao.xyz/Article/details/gceejryyu.sHtML

Ruby ........... 212
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeptfrhb.sHtML

C# ............. 212
来源：http://www.share.fanxiaobao.xyz/Article/details/grxmwwrbb.sHtML

C .............. 30
来源：http://3g.fanxiaobao.xyz/Article/details/guwkswmgw.sHtML

C++ ............ 30
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpxnrzex.sHtML

SQL ............ 90
来源：http://3g.fanxiaobao.xyz/Article/details/gsdpoaftt.sHtML

Bash ........... 80
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkowhqcca.sHtML

Kotlin ......... 15
来源：http://baike.fanxiaobao.xyz/Article/details/ghxaaqrgh.sHtML

Swift .......... 15
来源：http://m.share.fanxiaobao.xyz/Article/details/guxuvqlwg.sHtML

Lua ............ 10
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrwvqyis.sHtML

Perl ........... 10
来源：http://mobile.fanxiaobao.xyz/Article/details/gamwxfblk.sHtML

Scala .......... 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzxdhsvi.sHtML

------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsbbfxmm.sHtML

合计 ........... 2106 条
来源：http://wap.fanxiaobao.xyz/Article/details/gaopaarkm.sHtML

按章节统计：
来源：http://read.share.fanxiaobao.xyz/Article/details/gmexjzcfz.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwhchiwl.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjrfzshf.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gevfabscx.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.fanxiaobao.xyz/Article/details/goxmrqvhj.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.fanxiaobao.xyz/Article/details/gmnwsqvyo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.fanxiaobao.xyz/Article/details/gameldbwu.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.fanxiaobao.xyz/Article/details/gqdjkhapz.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhfgkhsy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcjwxhis.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://baike.fanxiaobao.xyz/Article/details/gwlixqizc.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhrzgwbl.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fanxiaobao.xyz/Article/details/gokvspnmr.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoxhizvi.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fanxiaobao.xyz/Article/details/goqkwlzgm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcksinlk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrwyprna.sHtML

Q SQL 专题                              90
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiefffrn.sHtML

R Bash 专题                             80
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnodapefy.sHtML

S C / C++ 专题                          60
来源：http://baike.fanxiaobao.xyz/Article/details/gcttdgsui.sHtML

T 其他语言补充                          60
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdhnipum.sHtML

U 高频实用片段                         120
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpskhnvcc.sHtML

------------------------------------
来源：http://baike.fanxiaobao.xyz/Article/details/gvuwojiil.sHtML

合计                                  2106 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywujmmud.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fanxiaobao.xyz/Article/details/gqztovhee.sHtML

使用提醒
来源：http://blog.fanxiaobao.xyz/Article/details/gnopvedcc.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuhjnebx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapkafuxe.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpixlbfa.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.fanxiaobao.xyz/Article/details/gwsosdxwp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttdxwgtb.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdsrdqyb.sHtML

—— 文件结束 ——
来源：http://baike.fanxiaobao.xyz/Article/details/gzkxxrjsp.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubiaphpy.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoptqkgq.sHtML

Common Programming Examples Cheat Book
来源：http://3g.fanxiaobao.xyz/Article/details/gqyrwfvid.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gciaxdjpf.sHtML

【收录内容】
来源：http://baike.fanxiaobao.xyz/Article/details/gszwbjztq.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhfisowh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://wap.fanxiaobao.xyz/Article/details/gztzisfir.sHtML

SQL · Bash · C · C++
来源：http://blog.fanxiaobao.xyz/Article/details/grqcwitkt.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fanxiaobao.xyz/Article/details/gahcjnhkt.sHtML

【使用说明】
来源：http://read.share.fanxiaobao.xyz/Article/details/gspkhcxyc.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsyvrtmn.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.fanxiaobao.xyz/Article/details/gryaljxyj.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://m.share.fanxiaobao.xyz/Article/details/goitycwuj.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fanxiaobao.xyz/Article/details/ggjuvozev.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fanxiaobao.xyz/Article/details/gisrtbrwd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtaywmue.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsjqhjpd.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.fanxiaobao.xyz/Article/details/gwufmrfal.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://baike.fanxiaobao.xyz/Article/details/gwiitazsh.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqxczydu.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fanxiaobao.xyz/Article/details/ggiqfvzxq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fanxiaobao.xyz/Article/details/gcfzaozwo.sHtML

【文件统计】
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyxbuzwf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://read.share.fanxiaobao.xyz/Article/details/ggovykfiu.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.fanxiaobao.xyz/Article/details/gvcawdfzk.sHtML

目  录
来源：http://www.share.fanxiaobao.xyz/Article/details/gncnvwsyv.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fanxiaobao.xyz/Article/details/gyusaiuds.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/grwkutdww.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gvyomsmry.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuujlbnh.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gtvawrihl.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gxycsmzpd.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwzefwce.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.fanxiaobao.xyz/Article/details/ggddoanpb.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gorravlsi.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzfhmlbb.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnfwpkac.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gfybwznud.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.fanxiaobao.xyz/Article/details/grvdraazg.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gqnnlbbou.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://baike.fanxiaobao.xyz/Article/details/gnuuehuzl.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwcwwznk.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gmhxydnhk.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://3g.fanxiaobao.xyz/Article/details/ggpunmisc.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gbyysocsb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwnsehil.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gotxxovpk.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/gjnunadrv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghyxbbjtv.sHtML

A. 基础语法与类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gioxtpqtq.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gjtkshehu.sHtML

[A01] Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gphgxgcve.sHtML

Py:   print("Hello, World!")
来源：http://3g.fanxiaobao.xyz/Article/details/gzylbomlm.sHtML

PHP:  echo "Hello, World!";
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnutajfz.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpthspqo.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fanxiaobao.xyz/Article/details/gramnlmnz.sHtML

Java: System.out.println("Hello, World!");
来源：http://m.share.fanxiaobao.xyz/Article/details/gilnxhcli.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfltkcatu.sHtML

Ruby: puts "Hello, World!"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzftkhxsf.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fanxiaobao.xyz/Article/details/gjbmecklb.sHtML

[A02] 变量声明与赋值
来源：http://3g.fanxiaobao.xyz/Article/details/gixwhbmln.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbiozuix.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fanxiaobao.xyz/Article/details/guuytbjxe.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://wap.fanxiaobao.xyz/Article/details/gotkwoywv.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://baike.fanxiaobao.xyz/Article/details/gzbspwfzo.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgoonnfl.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksaiseab.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.fanxiaobao.xyz/Article/details/gfspoowwv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fanxiaobao.xyz/Article/details/gchdliwya.sHtML

[A03] 常量定义
来源：http://baike.fanxiaobao.xyz/Article/details/goxlblbsc.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.fanxiaobao.xyz/Article/details/gbikwzlbn.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gspqfcttx.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gxpvlsaaa.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gieyyzstf.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjvfbupq.sHtML

Go:   const PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gfliibvqx.sHtML

Ruby: PI = 3.14159
来源：http://blog.fanxiaobao.xyz/Article/details/gdonkfkev.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gsqzkxawa.sHtML

[A04] 判断变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdzifcgk.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhuqdger.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gsdfxwdmt.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnwcgcdx.sHtML

TS:   typeof x; x instanceof Date
来源：http://m.share.fanxiaobao.xyz/Article/details/grwkaqvtn.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeqyfgjc.sHtML


<!-- 参考信息 -->