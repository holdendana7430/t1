代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://m.share.fehbvm.com/Article/details/gplmkmmzk.sHtML

sys.stdout.isatty()
来源：http://mobile.fehbvm.com/Article/details/ghedirjor.sHtML

[U40] Py：打印到标准错误
来源：http://www.share.hesvh.cn/Article/details/govusvdsj.sHtML

print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gtyjmxsja.sHtML

[U41] PHP：初始化 Composer 项目
来源：http://baike.zdbjq.cn/Article/details/gufdnhlvx.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://3g.hesvh.cn/Article/details/gfufrdccb.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.hesvh.cn/Article/details/gybynqpxq.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.zdbjq.cn/Article/details/gqhajitjc.sHtML

[U43] PHP：声明命名空间
来源：http://3g.hesvh.cn/Article/details/gegkdghgp.sHtML

namespace App\Http;
来源：http://www.share.zdbjq.cn/Article/details/gqagjzyhk.sHtML

[U44] PHP：开启严格类型
来源：http://www.share.fehbvm.com/Article/details/gymyhejzq.sHtML

declare(strict_types=1);
来源：http://blog.fehbvm.com/Article/details/gmtowvzpx.sHtML

[U45] PHP：类型声明与返回类型
来源：http://read.share.hesvh.cn/Article/details/gazpjackb.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gnnuwwtcp.sHtML

[U46] PHP：可空类型
来源：http://www.share.zdbjq.cn/Article/details/gjchvtkej.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gmblahgpg.sHtML

[U47] PHP：联合类型
来源：http://www.blog.hesvh.cn/Article/details/geyvowcim.sHtML

int|string $id
来源：http://read.share.fehbvm.com/Article/details/gyexkxmuj.sHtML

[U48] PHP：纯枚举
来源：http://www.share.hesvh.cn/Article/details/glncratlf.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.hesvh.cn/Article/details/gdziwcmpd.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gwlvywnoq.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/glqpqqzhc.sHtML

[U50] PHP：构造器属性提升
来源：http://www.share.zdbjq.cn/Article/details/gexrabfia.sHtML

public function __construct(private int $id) {}
来源：http://m.share.fehbvm.com/Article/details/ggwebasbm.sHtML

[U51] PHP：数组解构
来源：http://www.share.hesvh.cn/Article/details/gajgczbya.sHtML

[$a, $b] = $arr;
来源：http://3g.zdbjq.cn/Article/details/gyczjdcco.sHtML

[U52] PHP：箭头函数
来源：http://m.share.fehbvm.com/Article/details/gosqjmefm.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.fehbvm.com/Article/details/gxvnpdoug.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gqelghvqg.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.hesvh.cn/Article/details/gkuqaxogr.sHtML

[U54] PHP：空安全调用
来源：http://blog.fehbvm.com/Article/details/gkbyenepq.sHtML

$obj?->method()
来源：http://blog.fehbvm.com/Article/details/giasyxmip.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/ggobzlnjs.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://3g.zdbjq.cn/Article/details/guiafnwey.sHtML

[U56] PHP：命名参数
来源：http://blog.fehbvm.com/Article/details/gsfebconn.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gnvtwjuxf.sHtML

[U57] PHP：字符串插值
来源：http://baike.fehbvm.com/Article/details/gfpbrvgza.sHtML

"值: {$a}"
来源：http://baike.zdbjq.cn/Article/details/gcxesgjli.sHtML

[U58] PHP：数组三件套
来源：http://blog.zdbjq.cn/Article/details/gynjvkrvc.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://3g.hesvh.cn/Article/details/geqhucahs.sHtML

[U59] PHP：自定义排序
来源：http://www.m.share.fehbvm.com/Article/details/grbxncadc.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/guaojmuft.sHtML

[U60] PHP：JSON 编解码
来源：http://www.m.share.fehbvm.com/Article/details/gsonofwhr.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gsldiirmp.sHtML

[U61] PHP：正则
来源：http://www.blog.zdbjq.cn/Article/details/gorqchqaf.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gpjvpyags.sHtML

[U62] PHP：日期对象
来源：http://3g.zdbjq.cn/Article/details/giiaxdtud.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://m.share.zdbjq.cn/Article/details/gdxejypfv.sHtML

[U63] PHP：文件读写
来源：http://read.share.fehbvm.com/Article/details/ggmpshjuf.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.hesvh.cn/Article/details/gyouefcel.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gdvhqijns.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gyhwxqrkw.sHtML

[U65] PHP：会话
来源：http://mobile.hesvh.cn/Article/details/ggnuxtiuc.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmtrpkefv.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.hesvh.cn/Article/details/gqribufdw.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.hesvh.cn/Article/details/ghsjbthxd.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.fehbvm.com/Article/details/gpguqqauj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.hesvh.cn/Article/details/gwmotxcst.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gtqrbbxry.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/glopzcsac.sHtML

[U69] PHP：PDO 预处理
来源：http://read.share.zdbjq.cn/Article/details/gpugnvzsm.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://baike.fehbvm.com/Article/details/gzhgrqrmv.sHtML

[U70] PHP：PDO 事务
来源：http://blog.zdbjq.cn/Article/details/gomwaehhm.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.hesvh.cn/Article/details/gdmodrcog.sHtML

[U71] PHP：抛出异常
来源：http://m.share.zdbjq.cn/Article/details/gopetzknf.sHtML

throw new RuntimeException("失败", 500);
来源：http://wap.fehbvm.com/Article/details/ghrbcmlnl.sHtML

[U72] PHP：写错误日志
来源：http://baike.hesvh.cn/Article/details/geismobiv.sHtML

error_log("失败: " . $e->getMessage());
来源：http://www.share.hesvh.cn/Article/details/gbsreaeqz.sHtML

[U73] PHP：读取 ini 配置
来源：http://mobile.zdbjq.cn/Article/details/gyivsvthx.sHtML

parse_ini_file("config.ini", true)
来源：http://www.m.share.hesvh.cn/Article/details/geootlzbj.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/glelovvsn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.zdbjq.cn/Article/details/gpnhsaqtg.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/ggjvjnckc.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/gbcrhzdvc.sHtML

[U76] PHP：简单路由
来源：http://wap.hesvh.cn/Article/details/gykqbxtai.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/gyskdemri.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/ghzpgddnh.sHtML

composer require twig/twig
来源：http://www.m.share.zdbjq.cn/Article/details/gpqefppzw.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gvsxwhhut.sHtML

composer require --dev phpunit/phpunit
来源：http://www.blog.hesvh.cn/Article/details/gvpvovhij.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/gzzwzjtsv.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gudzeybhi.sHtML

[U80] PHP：代码规范修复
来源：http://wap.hesvh.cn/Article/details/gmvpymcci.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.fehbvm.com/Article/details/gtsdslnky.sHtML

[U81] JS：初始化项目
来源：http://www.share.fehbvm.com/Article/details/guxihqgkj.sHtML

npm init -y;  npm i express
来源：http://baike.fehbvm.com/Article/details/gylcxvgic.sHtML

[U82] JS：package.json 脚本
来源：http://www.m.share.fehbvm.com/Article/details/gpyhdlqud.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.hesvh.cn/Article/details/gcbsbgiqo.sHtML

[U83] JS：ES Module 导入导出
来源：http://3g.hesvh.cn/Article/details/gtafvnfwt.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gshqglmym.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.hesvh.cn/Article/details/gguekwigl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.zdbjq.cn/Article/details/gbkkwvlvb.sHtML

[U85] JS：可选链
来源：http://m.share.fehbvm.com/Article/details/gipicjovu.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/gxthbcdsz.sHtML

[U86] JS：空值合并
来源：http://www.m.share.hesvh.cn/Article/details/gkdabwkaa.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gpdgnjjdq.sHtML

[U87] JS：解构默认值
来源：http://baike.hesvh.cn/Article/details/gssukwmbk.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.fehbvm.com/Article/details/gndapbkmf.sHtML

[U88] JS：对象展开合并
来源：http://mobile.zdbjq.cn/Article/details/gedvwjkit.sHtML

{ ...a, ...b }
来源：http://m.share.hesvh.cn/Article/details/gdrmpoeuf.sHtML

[U89] JS：数组去重
来源：http://baike.fehbvm.com/Article/details/gopmfjyjd.sHtML

[...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gjmpqjsrv.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gkjatckel.sHtML

[...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gjykaonhl.sHtML

[U91] JS：对象键值遍历
来源：http://baike.zdbjq.cn/Article/details/gdguszmws.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.zdbjq.cn/Article/details/gwxmmefqw.sHtML

[U92] JS：深拷贝
来源：http://m.share.hesvh.cn/Article/details/gutqkcrdw.sHtML

structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gzeaizbuk.sHtML

[U93] JS：模板字符串
来源：http://blog.fehbvm.com/Article/details/gueetynuu.sHtML

`共 ${n} 条`
来源：http://www.blog.zdbjq.cn/Article/details/gvokmsnae.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gwghgttqi.sHtML

const double = x => x * 2;
来源：http://wap.fehbvm.com/Article/details/ggiuufmqu.sHtML

[U95] JS：Promise 包装
来源：http://3g.hesvh.cn/Article/details/gqznwdidi.sHtML

new Promise((resolve, reject) => {})
来源：http://wap.hesvh.cn/Article/details/gcgafaxzy.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gbujqysaw.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gfnujcmfb.sHtML

[U97] JS：并发请求
来源：http://read.share.hesvh.cn/Article/details/gfhrosfce.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gboxwkdmx.sHtML

[U98] JS：fetch 带 JSON
来源：http://3g.zdbjq.cn/Article/details/gbndjjyqu.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://3g.fehbvm.com/Article/details/gmlashmfj.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/glupeyiva.sHtML

el.addEventListener("click", e => {})
来源：http://m.share.zdbjq.cn/Article/details/gmaqimmiw.sHtML

[U100] JS：DOM 查询
来源：http://m.share.hesvh.cn/Article/details/gulxmklej.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/ggfkycylk.sHtML

[U101] JS：classList 操作
来源：http://mobile.hesvh.cn/Article/details/gyzbgxdjo.sHtML

el.classList.toggle("active")
来源：http://www.m.share.hesvh.cn/Article/details/gucznvuvd.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/gpyfswejz.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://3g.hesvh.cn/Article/details/gyhpmwwku.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gaysvgomr.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/ggaihcxoc.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gorafjjov.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gjtgyvylh.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/grkyixhdz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/ggdvvocwz.sHtML

[U106] JS：日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gqygxjfur.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/gblexsrou.sHtML

[U107] JS：数字千分位
来源：http://3g.fehbvm.com/Article/details/gbvtsjgqn.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gzmmbfqje.sHtML

[U108] JS：随机整数
来源：http://blog.hesvh.cn/Article/details/gssvjzlme.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.share.zdbjq.cn/Article/details/gboaugpew.sHtML

[U109] JS：数组分组
来源：http://blog.zdbjq.cn/Article/details/grbluqxsw.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmzwnzjz.sHtML

[U110] JS：数组分块
来源：http://wap.zdbjq.cn/Article/details/giurrveju.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.zdbjq.cn/Article/details/gdydhporz.sHtML

[U111] JS：对象转 Map
来源：http://www.blog.fehbvm.com/Article/details/gkrjcpphq.sHtML

new Map(Object.entries(obj))
来源：http://mobile.fehbvm.com/Article/details/gumvicawb.sHtML

[U112] JS：字符串补位
来源：http://wap.zdbjq.cn/Article/details/ggipivphr.sHtML

"7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gosayxzje.sHtML

[U113] JS：正则替换全部
来源：http://read.share.zdbjq.cn/Article/details/gxissgivi.sHtML

s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gyilbbjud.sHtML

[U114] JS：JSON 深比较
来源：http://wap.zdbjq.cn/Article/details/geyxdilhx.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/grbfvsmsr.sHtML

[U115] JS：生成 UUID
来源：http://3g.zdbjq.cn/Article/details/gcymwvywv.sHtML

crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gijurcvdt.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://read.share.hesvh.cn/Article/details/gbjhqvklr.sHtML

/** @param {string} name */ function f(name) {}
来源：http://3g.hesvh.cn/Article/details/gpmtahoys.sHtML

[U117] JS：单元测试
来源：http://mobile.hesvh.cn/Article/details/gqfcpirpn.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/geknmklza.sHtML

[U118] JS：开发服务器
来源：http://read.share.fehbvm.com/Article/details/gwvnzmkkt.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gfbfunsac.sHtML

[U119] JS：生产构建
来源：http://baike.fehbvm.com/Article/details/ghamchdze.sHtML

npx vite build
来源：http://m.share.hesvh.cn/Article/details/gjmdvdmeu.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://baike.zdbjq.cn/Article/details/gqmuykfhx.sHtML

import.meta.env.VITE_API_URL
来源：http://mobile.zdbjq.cn/Article/details/gykjurwrl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gasbqcmyv.sHtML

统计汇总
来源：http://baike.zdbjq.cn/Article/details/gvexmjlgd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goosiwvoc.sHtML

按语言统计（条）：
来源：http://www.share.fehbvm.com/Article/details/gwkkjzqlg.sHtML

Python ......... 252
来源：http://www.m.share.zdbjq.cn/Article/details/gwnyttnpd.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gvmwmdscd.sHtML

JavaScript ..... 252
来源：http://www.share.zdbjq.cn/Article/details/gezjyuuha.sHtML

TypeScript ..... 212
来源：http://blog.fehbvm.com/Article/details/gjfkcijyt.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/gbjuuyylf.sHtML

Go ............. 212
来源：http://mobile.hesvh.cn/Article/details/gxsdzgktc.sHtML

Ruby ........... 212
来源：http://wap.fehbvm.com/Article/details/gidlmhrqd.sHtML

C# ............. 212
来源：http://www.blog.zdbjq.cn/Article/details/gykioicnf.sHtML

C .............. 30
来源：http://read.share.zdbjq.cn/Article/details/gvseffayw.sHtML

C++ ............ 30
来源：http://3g.hesvh.cn/Article/details/gaavlgsys.sHtML

SQL ............ 90
来源：http://wap.fehbvm.com/Article/details/gvsggfylb.sHtML

Bash ........... 80
来源：http://blog.zdbjq.cn/Article/details/gqegdamkn.sHtML

Kotlin ......... 15
来源：http://www.blog.fehbvm.com/Article/details/gwwsljhgi.sHtML

Swift .......... 15
来源：http://wap.hesvh.cn/Article/details/gwgcdncwt.sHtML

Lua ............ 10
来源：http://blog.fehbvm.com/Article/details/gbhmhebhg.sHtML

Perl ........... 10
来源：http://www.m.share.hesvh.cn/Article/details/gdwykxsdk.sHtML

Scala .......... 10
来源：http://m.share.fehbvm.com/Article/details/gwcordehm.sHtML

------------------------------------
来源：http://blog.zdbjq.cn/Article/details/ggzfcpgmc.sHtML

合计 ........... 2106 条
来源：http://baike.zdbjq.cn/Article/details/gzhrhdlul.sHtML

按章节统计：
来源：http://www.share.hesvh.cn/Article/details/gkzlyeaus.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/ggilibbdd.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://mobile.zdbjq.cn/Article/details/geykcqjwh.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/gtyvfkcag.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.zdbjq.cn/Article/details/gypajjdwr.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://wap.zdbjq.cn/Article/details/gdccmeyxs.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gwmbzvcsi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/goasfzciu.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.zdbjq.cn/Article/details/gujiaawjt.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gmqtfgfqv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://blog.hesvh.cn/Article/details/ggniorfzk.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/grwgagkwu.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gjtcukorh.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gbstnuldr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/ggevwhvvy.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.blog.fehbvm.com/Article/details/gymzypofa.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.hesvh.cn/Article/details/geiuyeyab.sHtML

Q SQL 专题                              90
来源：http://www.share.fehbvm.com/Article/details/gjfkcrsja.sHtML

R Bash 专题                             80
来源：http://blog.hesvh.cn/Article/details/ghzmkwxzj.sHtML

S C / C++ 专题                          60
来源：http://www.m.share.hesvh.cn/Article/details/gzmvcpgin.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/godmdzfgp.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/gegwpdjyu.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gfwvcufkj.sHtML

合计                                  2106 条
来源：http://mobile.fehbvm.com/Article/details/govryblgp.sHtML

--------------------------------------------------------------------------------
来源：http://blog.fehbvm.com/Article/details/guzcfogay.sHtML

使用提醒
来源：http://wap.hesvh.cn/Article/details/gzvcrtijb.sHtML

--------------------------------------------------------------------------------
来源：http://wap.zdbjq.cn/Article/details/gzgswyiun.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.fehbvm.com/Article/details/gjmttczgi.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://mobile.zdbjq.cn/Article/details/gxzrgvwdm.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://wap.zdbjq.cn/Article/details/gvxuxotqh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gheterngn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.m.share.fehbvm.com/Article/details/gpmjydyly.sHtML

—— 文件结束 ——
来源：http://www.blog.zdbjq.cn/Article/details/guecrxous.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goqfeqnma.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/gjzjtfmyh.sHtML

Common Programming Examples Cheat Book
来源：http://mobile.hesvh.cn/Article/details/gqzwjdxnk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyevviuzi.sHtML

【收录内容】
来源：http://baike.hesvh.cn/Article/details/gbunsxkdp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://blog.zdbjq.cn/Article/details/gboruosqf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://3g.hesvh.cn/Article/details/gmdjuoryr.sHtML

SQL · Bash · C · C++
来源：http://mobile.fehbvm.com/Article/details/gboasmpzu.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gjuqxeisr.sHtML

【使用说明】
来源：http://mobile.fehbvm.com/Article/details/gfybakzqu.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/greslwbnr.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://blog.fehbvm.com/Article/details/gtrxinqvz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/goqkjbqvz.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.zdbjq.cn/Article/details/gjwxfizta.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://blog.hesvh.cn/Article/details/gzmzxcxcp.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://wap.fehbvm.com/Article/details/gitjcwunv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.zdbjq.cn/Article/details/gzhicbzna.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://m.share.fehbvm.com/Article/details/gcofqxoah.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.share.zdbjq.cn/Article/details/ghjjtsoso.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://wap.zdbjq.cn/Article/details/gtfqennnm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://wap.fehbvm.com/Article/details/gbhzwixmy.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gkstvwjhq.sHtML

【文件统计】
来源：http://wap.fehbvm.com/Article/details/gaphylbiu.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.share.hesvh.cn/Article/details/gxztqmdgh.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gfilnbxii.sHtML

目  录
来源：http://read.share.hesvh.cn/Article/details/gothvrpaf.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gpvyyowsy.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://baike.zdbjq.cn/Article/details/gkrywscsd.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/glyyzuctq.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gbldxhcwo.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.m.share.zdbjq.cn/Article/details/ggengtlvj.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://wap.hesvh.cn/Article/details/gvdeeucbz.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.blog.hesvh.cn/Article/details/gdydibmpl.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://m.share.zdbjq.cn/Article/details/gkaitcvyq.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gocktdntb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gwhmcjubx.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.blog.zdbjq.cn/Article/details/gpwxqzhhu.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/gyexrfhoo.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gxxnzwbft.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gkcyxprje.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/ggaykordz.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.fehbvm.com/Article/details/ggfrzyipm.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gquhoscjh.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.fehbvm.com/Article/details/gerjgjhaj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://m.share.hesvh.cn/Article/details/glmgrkxcy.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.zdbjq.cn/Article/details/gmrxtpjhh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/gzdtjhibc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/gencfbpjh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grbkigage.sHtML

A. 基础语法与类型
来源：http://www.m.share.zdbjq.cn/Article/details/gjarxoykf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gaxmqfbdm.sHtML

[A01] Hello World
来源：http://blog.hesvh.cn/Article/details/gxzkalapq.sHtML

Py:   print("Hello, World!")
来源：http://wap.hesvh.cn/Article/details/gmziqxpci.sHtML

PHP:  echo "Hello, World!";
来源：http://read.share.zdbjq.cn/Article/details/gwsatfmej.sHtML

JS:   console.log("Hello, World!");
来源：http://www.m.share.fehbvm.com/Article/details/gjispxnlu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wap.zdbjq.cn/Article/details/gprxilbye.sHtML

Java: System.out.println("Hello, World!");
来源：http://wap.zdbjq.cn/Article/details/ggovkxmjo.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gdotmapwb.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/guuqlnzfm.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://m.share.fehbvm.com/Article/details/gwgiclblm.sHtML

[A02] 变量声明与赋值
来源：http://3g.fehbvm.com/Article/details/ghrjdwudg.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://baike.hesvh.cn/Article/details/glfifwybi.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/ghjqooxrp.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.blog.hesvh.cn/Article/details/gdmfrklpk.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.zdbjq.cn/Article/details/gbzzoooab.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.hesvh.cn/Article/details/gzxjjungg.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.share.fehbvm.com/Article/details/gwrmdapdn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.fehbvm.com/Article/details/gbhfopuwr.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gtzvxliwi.sHtML

[A03] 常量定义
来源：http://www.blog.hesvh.cn/Article/details/gxuxdolis.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://read.share.zdbjq.cn/Article/details/gufvdujbl.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/ghjoatjtg.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/guxqqxmoh.sHtML

TS:   const PI: number = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gqhmppmzh.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gyxonnoie.sHtML

Go:   const PI = 3.14159
来源：http://www.m.share.fehbvm.com/Article/details/glrlruirf.sHtML

Ruby: PI = 3.14159
来源：http://baike.fehbvm.com/Article/details/gotcdaqog.sHtML

C#:   const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gfkvotmxp.sHtML

[A04] 判断变量类型
来源：http://baike.zdbjq.cn/Article/details/gnsofwmwc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.hesvh.cn/Article/details/gdxgwavjh.sHtML


<!-- 参考信息 -->