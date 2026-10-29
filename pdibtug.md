代发 wailian999

[U37] Py：读写 Excel
来源：http://3g.zdbjq.cn/Article/details/gzdmnaygl.sHtML

pandas.read_excel / DataFrame.to_excel
来源：http://www.m.share.fehbvm.com/Article/details/glufguzru.sHtML

[U38] Py：获取脚本所在目录
来源：http://3g.fehbvm.com/Article/details/gnwagdtvy.sHtML

Path(__file__).resolve().parent
来源：http://www.share.fehbvm.com/Article/details/gunpmopbb.sHtML

[U39] Py：判断是否在交互环境
来源：http://baike.fehbvm.com/Article/details/gzxloenys.sHtML

sys.stdout.isatty()
来源：http://mobile.zdbjq.cn/Article/details/gpxqocvyb.sHtML

[U40] Py：打印到标准错误
来源：http://blog.hesvh.cn/Article/details/gbrcennul.sHtML

print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gjvgnrmwh.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://wap.fehbvm.com/Article/details/gtzxznmog.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.share.fehbvm.com/Article/details/galcpkaoc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gtrxytkza.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://mobile.hesvh.cn/Article/details/grgwueczg.sHtML

[U43] PHP：声明命名空间
来源：http://read.share.zdbjq.cn/Article/details/gjgzqshso.sHtML

namespace App\Http;
来源：http://m.share.fehbvm.com/Article/details/gquapzpab.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.zdbjq.cn/Article/details/gzxenrulg.sHtML

declare(strict_types=1);
来源：http://www.share.hesvh.cn/Article/details/gwiqdzuuf.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.share.hesvh.cn/Article/details/ghzaqaxmq.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gtzeoddha.sHtML

[U46] PHP：可空类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpcohwtmr.sHtML

?string $name = null
来源：http://m.share.zdbjq.cn/Article/details/gtqtmachl.sHtML

[U47] PHP：联合类型
来源：http://blog.fehbvm.com/Article/details/gwsrxyuqv.sHtML

int|string $id
来源：http://baike.hesvh.cn/Article/details/gjdlifbfd.sHtML

[U48] PHP：纯枚举
来源：http://wap.zdbjq.cn/Article/details/goohpmyut.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdnercfrn.sHtML

[U49] PHP：只读属性
来源：http://blog.fehbvm.com/Article/details/gdiizydld.sHtML

public readonly string $name
来源：http://baike.zdbjq.cn/Article/details/grzcqpoaq.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.hesvh.cn/Article/details/gopzzzxcd.sHtML

public function __construct(private int $id) {}
来源：http://baike.hesvh.cn/Article/details/gqzvrsuyz.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/gmxxfjenw.sHtML

[$a, $b] = $arr;
来源：http://wap.zdbjq.cn/Article/details/gzpuxqmjf.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/gqggowaxh.sHtML

$double = fn($x) => $x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gcbhlldkf.sHtML

[U53] PHP：空合并运算符
来源：http://baike.hesvh.cn/Article/details/gitfbkman.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gutqzjsgi.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/gcjmhopsx.sHtML

$obj?->method()
来源：http://www.blog.hesvh.cn/Article/details/guqljdiep.sHtML

[U55] PHP：match 表达式
来源：http://blog.hesvh.cn/Article/details/gvbwbfpeh.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/gechzwykq.sHtML

[U56] PHP：命名参数
来源：http://read.share.zdbjq.cn/Article/details/gaxxvqdkf.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gtmiahduo.sHtML

[U57] PHP：字符串插值
来源：http://read.share.hesvh.cn/Article/details/gvkhvmcgw.sHtML

"值: {$a}"
来源：http://blog.hesvh.cn/Article/details/gcyisrnly.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gbbfnfdxv.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.zdbjq.cn/Article/details/glwnpzkjp.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/gipmwuycv.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gboaqvdjs.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/gfgylyoxn.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.share.fehbvm.com/Article/details/gsopzrdae.sHtML

[U61] PHP：正则
来源：http://blog.fehbvm.com/Article/details/gbwurtpku.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/gencgnckh.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/gjjlexmwo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.hesvh.cn/Article/details/gkjiwhwab.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.zdbjq.cn/Article/details/ghntjsbqw.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.hesvh.cn/Article/details/ggnbhlpjp.sHtML

[U64] PHP：目录遍历
来源：http://mobile.zdbjq.cn/Article/details/gjmmktfmk.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://m.share.zdbjq.cn/Article/details/gkfxkceji.sHtML

[U65] PHP：会话
来源：http://mobile.zdbjq.cn/Article/details/gexbgwzpu.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://baike.hesvh.cn/Article/details/goigcrhpp.sHtML

[U66] PHP：设置 Cookie
来源：http://www.m.share.hesvh.cn/Article/details/gynovyuxc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.share.zdbjq.cn/Article/details/gqwepxnve.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gvhujlmae.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gzgcertpj.sHtML

[U68] PHP：PDO 连接
来源：http://blog.hesvh.cn/Article/details/guwomuwyh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://m.share.fehbvm.com/Article/details/gfloomfiy.sHtML

[U69] PHP：PDO 预处理
来源：http://wap.hesvh.cn/Article/details/gnbwicxyo.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.hesvh.cn/Article/details/gddantjxv.sHtML

[U70] PHP：PDO 事务
来源：http://blog.fehbvm.com/Article/details/garodmrxj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://3g.zdbjq.cn/Article/details/gehksgzuv.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gkjwxpkwz.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.share.hesvh.cn/Article/details/gjbhictlh.sHtML

[U72] PHP：写错误日志
来源：http://m.share.hesvh.cn/Article/details/gsupjnmvc.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/ghdpicyaa.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gvzrhhhrs.sHtML

parse_ini_file("config.ini", true)
来源：http://wap.hesvh.cn/Article/details/gcfkfuraf.sHtML

[U74] PHP：读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gmfvlbpsh.sHtML

getenv("APP_ENV") ?: "production"
来源：http://wap.hesvh.cn/Article/details/galmftmmg.sHtML

[U75] PHP：依赖注入
来源：http://www.m.share.hesvh.cn/Article/details/gxxldbein.sHtML

composer require psr/container
来源：http://baike.fehbvm.com/Article/details/gxziaopbm.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/ggrjuupdm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://read.share.hesvh.cn/Article/details/gugqbezpq.sHtML

[U77] PHP：模板渲染
来源：http://read.share.zdbjq.cn/Article/details/gkftlpime.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/gevtxmxfv.sHtML

[U78] PHP：单元测试
来源：http://wap.zdbjq.cn/Article/details/gciccubud.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.hesvh.cn/Article/details/gffxfilbi.sHtML

[U79] PHP：静态分析
来源：http://mobile.hesvh.cn/Article/details/ggkelbsol.sHtML

composer require --dev phpstan/phpstan
来源：http://wap.hesvh.cn/Article/details/ghzztyizq.sHtML

[U80] PHP：代码规范修复
来源：http://wap.zdbjq.cn/Article/details/gmxnzmzjb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gicvgxnzc.sHtML

[U81] JS：初始化项目
来源：http://mobile.hesvh.cn/Article/details/gvznfnvve.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gvxkhrcvz.sHtML

[U82] JS：package.json 脚本
来源：http://blog.hesvh.cn/Article/details/gkbejprti.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://wap.hesvh.cn/Article/details/gulxsxhho.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gbtatmpgw.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/grlujfptg.sHtML

[U84] JS：CommonJS 写法
来源：http://mobile.zdbjq.cn/Article/details/grxuxapve.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/guoinysef.sHtML

[U85] JS：可选链
来源：http://www.blog.zdbjq.cn/Article/details/gxjwfapvr.sHtML

a?.b?.c
来源：http://baike.fehbvm.com/Article/details/gfsyupxvj.sHtML

[U86] JS：空值合并
来源：http://blog.zdbjq.cn/Article/details/gpcfdtmht.sHtML

a ?? b
来源：http://read.share.hesvh.cn/Article/details/gfyqoidkg.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/guqahvegk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://m.share.fehbvm.com/Article/details/gpaothrxg.sHtML

[U88] JS：对象展开合并
来源：http://www.share.hesvh.cn/Article/details/gwotfofhj.sHtML

{ ...a, ...b }
来源：http://blog.zdbjq.cn/Article/details/gzpcostsx.sHtML

[U89] JS：数组去重
来源：http://read.share.fehbvm.com/Article/details/gnksjjehz.sHtML

[...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/guqebmron.sHtML

[U90] JS：数字数组排序
来源：http://www.m.share.hesvh.cn/Article/details/gvtirygxx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gxppcuhoz.sHtML

[U91] JS：对象键值遍历
来源：http://read.share.zdbjq.cn/Article/details/gllzpvhbi.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.zdbjq.cn/Article/details/gihgwcvwk.sHtML

[U92] JS：深拷贝
来源：http://mobile.hesvh.cn/Article/details/gwrqdsjip.sHtML

structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gwnlzwecx.sHtML

[U93] JS：模板字符串
来源：http://www.share.zdbjq.cn/Article/details/gukesjbov.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gkfxofipd.sHtML

[U94] JS：箭头函数
来源：http://3g.fehbvm.com/Article/details/giacenepe.sHtML

const double = x => x * 2;
来源：http://wap.zdbjq.cn/Article/details/gjoerskft.sHtML

[U95] JS：Promise 包装
来源：http://www.blog.zdbjq.cn/Article/details/gstsjoxtq.sHtML

new Promise((resolve, reject) => {})
来源：http://www.share.zdbjq.cn/Article/details/gklajejqn.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/ghxlmevac.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gwbkxnfgd.sHtML

[U97] JS：并发请求
来源：http://www.share.hesvh.cn/Article/details/gdkzjnzye.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gleygdafh.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.share.hesvh.cn/Article/details/gsyonwidb.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gdvyuabtf.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/glxizxqjs.sHtML

el.addEventListener("click", e => {})
来源：http://mobile.zdbjq.cn/Article/details/glvribkwe.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gcujyczfw.sHtML

document.querySelector(".item")
来源：http://3g.fehbvm.com/Article/details/gojqurgry.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/ggweyophs.sHtML

el.classList.toggle("active")
来源：http://read.share.fehbvm.com/Article/details/gohgmjnww.sHtML

[U102] JS：本地存储
来源：http://read.share.zdbjq.cn/Article/details/gjzkeayzu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://mobile.zdbjq.cn/Article/details/gorglbvwm.sHtML

[U103] JS：定时器
来源：http://m.share.hesvh.cn/Article/details/gtgpdnoca.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/gepaesvts.sHtML

[U104] JS：防抖
来源：http://read.share.zdbjq.cn/Article/details/gomlawoef.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gvgsmghwc.sHtML

[U105] JS：节流
来源：http://www.share.zdbjq.cn/Article/details/gejtiulbw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/guiiswgro.sHtML

[U106] JS：日期格式化
来源：http://www.share.fehbvm.com/Article/details/ggqepgflh.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://baike.fehbvm.com/Article/details/gcnmwkifo.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/glnrtgpav.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gunzweqfy.sHtML

[U108] JS：随机整数
来源：http://wap.zdbjq.cn/Article/details/gkshhqnkf.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://3g.fehbvm.com/Article/details/ghydrxwxc.sHtML

[U109] JS：数组分组
来源：http://read.share.zdbjq.cn/Article/details/gnvhgcfzq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gljwopkgk.sHtML

[U110] JS：数组分块
来源：http://baike.fehbvm.com/Article/details/ggzdzrydj.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.blog.zdbjq.cn/Article/details/gkamwpjpo.sHtML

[U111] JS：对象转 Map
来源：http://baike.zdbjq.cn/Article/details/gdmrivnfn.sHtML

new Map(Object.entries(obj))
来源：http://3g.zdbjq.cn/Article/details/gjijpvtxd.sHtML

[U112] JS：字符串补位
来源：http://blog.hesvh.cn/Article/details/getayaifb.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/grxliyxue.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gwvygkuby.sHtML

s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gnvdxvnnl.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gvuxknjgh.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.hesvh.cn/Article/details/gwwuqarlr.sHtML

[U115] JS：生成 UUID
来源：http://www.share.fehbvm.com/Article/details/glaavexvg.sHtML

crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gcggorfxy.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.zdbjq.cn/Article/details/gxjfehmsx.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gasxptnln.sHtML

[U117] JS：单元测试
来源：http://www.share.hesvh.cn/Article/details/gpxqzombg.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.zdbjq.cn/Article/details/gtsaekyqc.sHtML

[U118] JS：开发服务器
来源：http://m.share.hesvh.cn/Article/details/gdhxbjkrw.sHtML

npm i -D vite;  npx vite
来源：http://mobile.fehbvm.com/Article/details/gwsanfiuc.sHtML

[U119] JS：生产构建
来源：http://wap.zdbjq.cn/Article/details/grxymazxk.sHtML

npx vite build
来源：http://www.blog.hesvh.cn/Article/details/gpxurkehg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.fehbvm.com/Article/details/ghbzigjym.sHtML

import.meta.env.VITE_API_URL
来源：http://www.share.zdbjq.cn/Article/details/giorvekvp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggwstiqmx.sHtML

统计汇总
来源：http://www.share.zdbjq.cn/Article/details/gbrmeruun.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpaomnmny.sHtML

按语言统计（条）：
来源：http://mobile.zdbjq.cn/Article/details/gilblklnl.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gnqxuuykx.sHtML

PHP ............ 252
来源：http://m.share.hesvh.cn/Article/details/goxiahiak.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gzwtupsnm.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/gnzduxtuz.sHtML

Java ........... 212
来源：http://blog.zdbjq.cn/Article/details/gaxpownan.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gcuuitcio.sHtML

Ruby ........... 212
来源：http://www.blog.zdbjq.cn/Article/details/gozqbsjrj.sHtML

C# ............. 212
来源：http://blog.hesvh.cn/Article/details/gcxqtgczp.sHtML

C .............. 30
来源：http://mobile.fehbvm.com/Article/details/gbqufoveo.sHtML

C++ ............ 30
来源：http://mobile.zdbjq.cn/Article/details/gjsldysqm.sHtML

SQL ............ 90
来源：http://wap.hesvh.cn/Article/details/gpxjozjfd.sHtML

Bash ........... 80
来源：http://blog.fehbvm.com/Article/details/gbgbllewc.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/gbampzlmh.sHtML

Swift .......... 15
来源：http://baike.fehbvm.com/Article/details/gxgosvunj.sHtML

Lua ............ 10
来源：http://www.share.hesvh.cn/Article/details/gvrbypgtp.sHtML

Perl ........... 10
来源：http://m.share.fehbvm.com/Article/details/gowchgzqe.sHtML

Scala .......... 10
来源：http://blog.zdbjq.cn/Article/details/gvssqlvwq.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gqjkernzv.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gsfzokruh.sHtML

按章节统计：
来源：http://3g.hesvh.cn/Article/details/gxkgorgbn.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/gkizjasxg.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/ggmwmjiht.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gwrfozsky.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://read.share.hesvh.cn/Article/details/gnvnfvbzr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/grmlvwpbi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gysrpqqyv.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gfhbfbvbm.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gsmrnhzgn.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gxjwwmoxd.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/ggejafahu.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gihmrssbt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://read.share.hesvh.cn/Article/details/gibrqyrzh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gwrlqplhk.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.fehbvm.com/Article/details/ggkaydazo.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.fehbvm.com/Article/details/ggmwjsndb.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gshwowvbl.sHtML

Q SQL 专题                              90
来源：http://wap.fehbvm.com/Article/details/gkjehzoht.sHtML

R Bash 专题                             80
来源：http://www.blog.fehbvm.com/Article/details/gpldwgzzw.sHtML

S C / C++ 专题                          60
来源：http://blog.zdbjq.cn/Article/details/ggfcawfgl.sHtML

T 其他语言补充                          60
来源：http://3g.fehbvm.com/Article/details/gaajzynvb.sHtML

U 高频实用片段                         120
来源：http://read.share.hesvh.cn/Article/details/gldoywvnx.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gfcfdfnaw.sHtML

合计                                  2106 条
来源：http://3g.fehbvm.com/Article/details/gsdugygow.sHtML

--------------------------------------------------------------------------------
来源：http://3g.zdbjq.cn/Article/details/gzbsacesg.sHtML

使用提醒
来源：http://m.share.fehbvm.com/Article/details/gvfbbqcha.sHtML

--------------------------------------------------------------------------------
来源：http://baike.hesvh.cn/Article/details/gfglzmsfl.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gjjwrxhwr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.share.zdbjq.cn/Article/details/gcrigyooj.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/gojagzeob.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.fehbvm.com/Article/details/gmfkzcvhx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://baike.hesvh.cn/Article/details/gxjnlkqba.sHtML

—— 文件结束 ——
来源：http://www.share.zdbjq.cn/Article/details/gluiupoyz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmpoueriu.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://wap.hesvh.cn/Article/details/gfmrxuzrv.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gwfhekgle.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsfljwgbd.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gthggchvw.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.hesvh.cn/Article/details/gikvtmekf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.hesvh.cn/Article/details/gluqbqpdt.sHtML

SQL · Bash · C · C++
来源：http://read.share.zdbjq.cn/Article/details/gwaxzjmmi.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.zdbjq.cn/Article/details/gzagfgxsp.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gnjqkgwtx.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://m.share.zdbjq.cn/Article/details/gfxoofnup.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.zdbjq.cn/Article/details/gqmhzgqnl.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gzexnafub.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://baike.hesvh.cn/Article/details/gdvbmkvyn.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gilwtiegr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.zdbjq.cn/Article/details/gcftacavh.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gxotcqfxo.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.fehbvm.com/Article/details/guywrwshu.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.m.share.fehbvm.com/Article/details/geahwfmlo.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://m.share.fehbvm.com/Article/details/gjmgaqpil.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.share.fehbvm.com/Article/details/gipidsmrm.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://read.share.zdbjq.cn/Article/details/gogfsekyi.sHtML

【文件统计】
来源：http://baike.hesvh.cn/Article/details/gnkoddyzf.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.hesvh.cn/Article/details/gsljfwoyc.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/glzoucpzk.sHtML

目  录
来源：http://www.m.share.fehbvm.com/Article/details/gsfvxsbyg.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gwpdtbdgb.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gfnscemad.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://read.share.hesvh.cn/Article/details/grwlljlwm.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.hesvh.cn/Article/details/glnknlooc.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gvhklrpfr.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.zdbjq.cn/Article/details/gphlhiwqt.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://read.share.hesvh.cn/Article/details/gyjhehqrs.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.fehbvm.com/Article/details/gjanxwebj.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.hesvh.cn/Article/details/gtihkqvxm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gcabwqubs.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.hesvh.cn/Article/details/ggwztuuqf.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/ggswchhqv.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://3g.fehbvm.com/Article/details/gndiaukjd.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gshfdukqw.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.blog.zdbjq.cn/Article/details/gjqlwxrfv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.share.zdbjq.cn/Article/details/grciovwlz.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gvhfxlhfg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.hesvh.cn/Article/details/gihzgjyfs.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.fehbvm.com/Article/details/gcwjsnfet.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gygazzcpi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.fehbvm.com/Article/details/gfxzhyxqi.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gpgyiltnc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjkpibxjj.sHtML

A. 基础语法与类型
来源：http://read.share.zdbjq.cn/Article/details/grxxejngc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxnfqryff.sHtML

[A01] Hello World
来源：http://mobile.zdbjq.cn/Article/details/gvgmjpush.sHtML

Py:   print("Hello, World!")
来源：http://m.share.fehbvm.com/Article/details/gmfbuppqd.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/goteormnx.sHtML

JS:   console.log("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/gurkzqkiz.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.zdbjq.cn/Article/details/gehymrzgc.sHtML

Java: System.out.println("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gqgmmklsq.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gnhhmeknd.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/guowmrroo.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/gqklecqku.sHtML

[A02] 变量声明与赋值
来源：http://read.share.hesvh.cn/Article/details/ggsrnpouc.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.hesvh.cn/Article/details/gpwctyeet.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.fehbvm.com/Article/details/gotmkdbct.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.hesvh.cn/Article/details/gzmpxzjhf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gdlmpnbsp.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://baike.hesvh.cn/Article/details/gvehdvzwd.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.zdbjq.cn/Article/details/gmytivibz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://read.share.zdbjq.cn/Article/details/gurnrkjmx.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://baike.fehbvm.com/Article/details/gcnqiksix.sHtML

[A03] 常量定义
来源：http://wap.hesvh.cn/Article/details/gydgsvkda.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://blog.fehbvm.com/Article/details/gtzggqwts.sHtML

PHP:  const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gcksjrbhp.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gcjmwnetj.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/ghnunljzf.sHtML

Java: static final double PI = 3.14159;
来源：http://www.share.zdbjq.cn/Article/details/gwujspcan.sHtML

Go:   const PI = 3.14159
来源：http://blog.hesvh.cn/Article/details/gdupqfndb.sHtML


<!-- 参考信息 -->