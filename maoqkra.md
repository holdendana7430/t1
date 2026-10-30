代发 wailian999

[U43] PHP：声明命名空间
来源：http://m.share.hesvh.cn/Article/details/ghowlneps.sHtML

namespace App\Http;
来源：http://baike.hesvh.cn/Article/details/ggfswlmut.sHtML

[U44] PHP：开启严格类型
来源：http://3g.fehbvm.com/Article/details/gyveicekl.sHtML

declare(strict_types=1);
来源：http://wap.fehbvm.com/Article/details/gwuvxmiek.sHtML

[U45] PHP：类型声明与返回类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmbnigypx.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gmfcyjpfh.sHtML

[U46] PHP：可空类型
来源：http://wap.zdbjq.cn/Article/details/gvldezkhf.sHtML

?string $name = null
来源：http://wap.fehbvm.com/Article/details/gowombnsx.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/gqrlqhwok.sHtML

int|string $id
来源：http://3g.zdbjq.cn/Article/details/gutjnqocg.sHtML

[U48] PHP：纯枚举
来源：http://mobile.zdbjq.cn/Article/details/gwcdpbbvj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://m.share.fehbvm.com/Article/details/gauklhfve.sHtML

[U49] PHP：只读属性
来源：http://www.share.zdbjq.cn/Article/details/gsmplhkhd.sHtML

public readonly string $name
来源：http://mobile.fehbvm.com/Article/details/gnzlnypnp.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gbsjxgucb.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gymredlyv.sHtML

[U51] PHP：数组解构
来源：http://mobile.fehbvm.com/Article/details/gluhexrex.sHtML

[$a, $b] = $arr;
来源：http://blog.hesvh.cn/Article/details/gcmgfwlxu.sHtML

[U52] PHP：箭头函数
来源：http://blog.hesvh.cn/Article/details/goxldsong.sHtML

$double = fn($x) => $x * 2;
来源：http://mobile.fehbvm.com/Article/details/gobiewctg.sHtML

[U53] PHP：空合并运算符
来源：http://m.share.hesvh.cn/Article/details/glgjbipwt.sHtML

$v = $a ?? $b ?? "default";
来源：http://baike.fehbvm.com/Article/details/ggylskxjh.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gokxdbpon.sHtML

$obj?->method()
来源：http://www.blog.zdbjq.cn/Article/details/grbcwyayb.sHtML

[U55] PHP：match 表达式
来源：http://baike.zdbjq.cn/Article/details/ggelqwhtr.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://blog.fehbvm.com/Article/details/geeebqrsk.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gaafwwmdj.sHtML

f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/grxpeymfq.sHtML

[U57] PHP：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gzkiydlwi.sHtML

"值: {$a}"
来源：http://www.blog.fehbvm.com/Article/details/goccpwwea.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.hesvh.cn/Article/details/ggrixjzrk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gwqksxjsv.sHtML

[U59] PHP：自定义排序
来源：http://blog.fehbvm.com/Article/details/gevboqsaj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/guemwwjrc.sHtML

[U60] PHP：JSON 编解码
来源：http://read.share.fehbvm.com/Article/details/gnbcuarvz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://mobile.fehbvm.com/Article/details/gizpirheh.sHtML

[U61] PHP：正则
来源：http://blog.hesvh.cn/Article/details/guynhynpk.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gvymhywhl.sHtML

[U62] PHP：日期对象
来源：http://read.share.zdbjq.cn/Article/details/gdmbhvaeg.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gdstvlflj.sHtML

[U63] PHP：文件读写
来源：http://m.share.hesvh.cn/Article/details/gsvbgzwuc.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://wap.zdbjq.cn/Article/details/gpobnswkx.sHtML

[U64] PHP：目录遍历
来源：http://blog.fehbvm.com/Article/details/ghnsourev.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.hesvh.cn/Article/details/gaxaghrri.sHtML

[U65] PHP：会话
来源：http://m.share.hesvh.cn/Article/details/grefozxli.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://blog.fehbvm.com/Article/details/gqjlwtojp.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.zdbjq.cn/Article/details/gigxpprgn.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.zdbjq.cn/Article/details/gwvoqcoti.sHtML

[U67] PHP：处理文件上传
来源：http://blog.hesvh.cn/Article/details/gugafwrxx.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gfsygggfz.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.zdbjq.cn/Article/details/ghkwynpig.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.zdbjq.cn/Article/details/grkbzuroj.sHtML

[U69] PHP：PDO 预处理
来源：http://blog.zdbjq.cn/Article/details/guxdsrznl.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.hesvh.cn/Article/details/gekifvtpn.sHtML

[U70] PHP：PDO 事务
来源：http://baike.fehbvm.com/Article/details/guznpphfd.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://m.share.fehbvm.com/Article/details/gawvlzisr.sHtML

[U71] PHP：抛出异常
来源：http://blog.zdbjq.cn/Article/details/gnvxkzfdf.sHtML

throw new RuntimeException("失败", 500);
来源：http://m.share.fehbvm.com/Article/details/gvjserewd.sHtML

[U72] PHP：写错误日志
来源：http://read.share.fehbvm.com/Article/details/gibfaabnb.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.hesvh.cn/Article/details/gekbmbgtx.sHtML

[U73] PHP：读取 ini 配置
来源：http://3g.hesvh.cn/Article/details/gqxvmcksq.sHtML

parse_ini_file("config.ini", true)
来源：http://www.blog.hesvh.cn/Article/details/gfnkaiogq.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/ghpxvywnt.sHtML

getenv("APP_ENV") ?: "production"
来源：http://3g.fehbvm.com/Article/details/ghwptrpbm.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.hesvh.cn/Article/details/gwhoslbhe.sHtML

composer require psr/container
来源：http://3g.zdbjq.cn/Article/details/guqzhoncl.sHtML

[U76] PHP：简单路由
来源：http://mobile.hesvh.cn/Article/details/gaazlbwdb.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://wap.hesvh.cn/Article/details/gioacmpar.sHtML

[U77] PHP：模板渲染
来源：http://www.m.share.zdbjq.cn/Article/details/gczvtndwu.sHtML

composer require twig/twig
来源：http://www.blog.zdbjq.cn/Article/details/gmtinqyii.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gwawkchpm.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gxqbvvwfi.sHtML

[U79] PHP：静态分析
来源：http://read.share.fehbvm.com/Article/details/gebsrmcxh.sHtML

composer require --dev phpstan/phpstan
来源：http://3g.fehbvm.com/Article/details/gikzmautc.sHtML

[U80] PHP：代码规范修复
来源：http://mobile.zdbjq.cn/Article/details/gvbsiczdr.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.zdbjq.cn/Article/details/gsuxvamlj.sHtML

[U81] JS：初始化项目
来源：http://read.share.hesvh.cn/Article/details/gduqhxzfk.sHtML

npm init -y;  npm i express
来源：http://www.blog.zdbjq.cn/Article/details/gvrhwfqbe.sHtML

[U82] JS：package.json 脚本
来源：http://www.blog.hesvh.cn/Article/details/gpcwafdjf.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gpbgkmqqh.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.zdbjq.cn/Article/details/gmfpymkzd.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gaukqjpdt.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.fehbvm.com/Article/details/gypzknxbk.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://baike.hesvh.cn/Article/details/gbkvaiafv.sHtML

[U85] JS：可选链
来源：http://3g.fehbvm.com/Article/details/gkgegfmcz.sHtML

a?.b?.c
来源：http://read.share.zdbjq.cn/Article/details/gnsidzbxb.sHtML

[U86] JS：空值合并
来源：http://baike.zdbjq.cn/Article/details/gjkdijcki.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/gitvspjlj.sHtML

[U87] JS：解构默认值
来源：http://wap.hesvh.cn/Article/details/gtidcbzqc.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.hesvh.cn/Article/details/giktydcwz.sHtML

[U88] JS：对象展开合并
来源：http://read.share.fehbvm.com/Article/details/gfanpmjei.sHtML

{ ...a, ...b }
来源：http://read.share.fehbvm.com/Article/details/gtblxlctl.sHtML

[U89] JS：数组去重
来源：http://blog.fehbvm.com/Article/details/gqmocmmys.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/ggazxaykt.sHtML

[U90] JS：数字数组排序
来源：http://3g.zdbjq.cn/Article/details/geyfbyquw.sHtML

[...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gnnyyodfa.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gftzyxyza.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/gfnphtysh.sHtML

[U92] JS：深拷贝
来源：http://baike.fehbvm.com/Article/details/gsjxlncax.sHtML

structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gifsslilz.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gvazzvvsx.sHtML

`共 ${n} 条`
来源：http://wap.hesvh.cn/Article/details/gkykwbwtz.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gfxrebbuw.sHtML

const double = x => x * 2;
来源：http://m.share.hesvh.cn/Article/details/gbaesuagm.sHtML

[U95] JS：Promise 包装
来源：http://blog.fehbvm.com/Article/details/giidegmav.sHtML

new Promise((resolve, reject) => {})
来源：http://blog.zdbjq.cn/Article/details/gtuzxwrsj.sHtML

[U96] JS：async/await 与异常
来源：http://www.m.share.fehbvm.com/Article/details/giyqtjjnb.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/ggipbjmgi.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gmpjlcuaf.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gxezlyxnq.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.fehbvm.com/Article/details/grqsjuydf.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gllkelesk.sHtML

[U99] JS：事件监听
来源：http://baike.fehbvm.com/Article/details/gmwqcgzag.sHtML

el.addEventListener("click", e => {})
来源：http://wap.fehbvm.com/Article/details/gahemaaei.sHtML

[U100] JS：DOM 查询
来源：http://read.share.hesvh.cn/Article/details/gguqzwaex.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/ghhckwwfi.sHtML

[U101] JS：classList 操作
来源：http://m.share.fehbvm.com/Article/details/gzkuvztix.sHtML

el.classList.toggle("active")
来源：http://www.blog.zdbjq.cn/Article/details/glbudkvxc.sHtML

[U102] JS：本地存储
来源：http://www.m.share.zdbjq.cn/Article/details/grrukpfhm.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.fehbvm.com/Article/details/gzysgyhov.sHtML

[U103] JS：定时器
来源：http://www.blog.hesvh.cn/Article/details/gmcevvjmv.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://read.share.hesvh.cn/Article/details/gdctjxpik.sHtML

[U104] JS：防抖
来源：http://mobile.zdbjq.cn/Article/details/gdvqdtizz.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gnickslho.sHtML

[U105] JS：节流
来源：http://www.m.share.fehbvm.com/Article/details/gyyhelqyi.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.share.zdbjq.cn/Article/details/gxouufdei.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gmennruhj.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://read.share.hesvh.cn/Article/details/gvlpuwdjp.sHtML

[U107] JS：数字千分位
来源：http://wap.hesvh.cn/Article/details/gvwpouswc.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/glxyeyysv.sHtML

[U108] JS：随机整数
来源：http://blog.fehbvm.com/Article/details/gffjullit.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.blog.hesvh.cn/Article/details/ghjikfuog.sHtML

[U109] JS：数组分组
来源：http://www.m.share.zdbjq.cn/Article/details/ganfuzqic.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gyjxmfxbw.sHtML

[U110] JS：数组分块
来源：http://read.share.fehbvm.com/Article/details/guwchwyum.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/glzdvamkg.sHtML

[U111] JS：对象转 Map
来源：http://read.share.fehbvm.com/Article/details/gxtomkxfu.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gtfbxxyay.sHtML

[U112] JS：字符串补位
来源：http://www.share.hesvh.cn/Article/details/gylpsmuyd.sHtML

"7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/geharlpqr.sHtML

[U113] JS：正则替换全部
来源：http://3g.fehbvm.com/Article/details/gsnbedsza.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gpczfkjud.sHtML

[U114] JS：JSON 深比较
来源：http://baike.zdbjq.cn/Article/details/ghovyhggv.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/ghqdoxzdh.sHtML

[U115] JS：生成 UUID
来源：http://3g.fehbvm.com/Article/details/ghsqypgou.sHtML

crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gaemiruqr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.fehbvm.com/Article/details/gvcopxfqy.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.hesvh.cn/Article/details/gcrqwpyto.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gyaiffaim.sHtML

npm i -D vitest;  npx vitest
来源：http://baike.hesvh.cn/Article/details/girxqznux.sHtML

[U118] JS：开发服务器
来源：http://blog.fehbvm.com/Article/details/gkswhmahh.sHtML

npm i -D vite;  npx vite
来源：http://mobile.hesvh.cn/Article/details/gttgpofdu.sHtML

[U119] JS：生产构建
来源：http://blog.fehbvm.com/Article/details/gwyocnmcx.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/gtszafjpn.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.share.hesvh.cn/Article/details/gznetfqco.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/ghvnhtgfk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/godmlvphm.sHtML

统计汇总
来源：http://www.m.share.hesvh.cn/Article/details/ghrkcduhi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdcrmhqbt.sHtML

按语言统计（条）：
来源：http://www.share.hesvh.cn/Article/details/geoxjyaby.sHtML

Python ......... 252
来源：http://baike.hesvh.cn/Article/details/gnasbdlml.sHtML

PHP ............ 252
来源：http://wap.hesvh.cn/Article/details/gfylgxwez.sHtML

JavaScript ..... 252
来源：http://wap.hesvh.cn/Article/details/gcjuqwzff.sHtML

TypeScript ..... 212
来源：http://m.share.zdbjq.cn/Article/details/gkugiuora.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/gbhemujaz.sHtML

Go ............. 212
来源：http://3g.hesvh.cn/Article/details/gzxbtrura.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gpqzectaq.sHtML

C# ............. 212
来源：http://www.m.share.fehbvm.com/Article/details/gqfhodlxa.sHtML

C .............. 30
来源：http://m.share.fehbvm.com/Article/details/gaguhrjqe.sHtML

C++ ............ 30
来源：http://www.m.share.fehbvm.com/Article/details/gqnqrnuax.sHtML

SQL ............ 90
来源：http://3g.zdbjq.cn/Article/details/gvyelktgv.sHtML

Bash ........... 80
来源：http://3g.fehbvm.com/Article/details/gstctzygm.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gnihzkzzx.sHtML

Swift .......... 15
来源：http://mobile.fehbvm.com/Article/details/gtznqkyrq.sHtML

Lua ............ 10
来源：http://www.blog.hesvh.cn/Article/details/grblvctqn.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gyesihdka.sHtML

Scala .......... 10
来源：http://baike.fehbvm.com/Article/details/gdpozagvf.sHtML

------------------------------------
来源：http://www.m.share.zdbjq.cn/Article/details/gviajynpt.sHtML

合计 ........... 2106 条
来源：http://www.blog.zdbjq.cn/Article/details/gjnernddf.sHtML

按章节统计：
来源：http://www.blog.hesvh.cn/Article/details/gdlaaumun.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://read.share.fehbvm.com/Article/details/giwpaqiet.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://m.share.hesvh.cn/Article/details/gxvbvlvir.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://m.share.zdbjq.cn/Article/details/gekepgjfi.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://3g.hesvh.cn/Article/details/gipbjjkyu.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.m.share.hesvh.cn/Article/details/gjtjobrao.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gsoqxmgbw.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://baike.fehbvm.com/Article/details/grvsvbrqf.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.share.fehbvm.com/Article/details/gkxemreoj.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.share.hesvh.cn/Article/details/gnkpiwmes.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/garazyict.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://mobile.zdbjq.cn/Article/details/gpnktovwf.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gpprowozs.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gqoeemrkl.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://baike.hesvh.cn/Article/details/gybjbgmns.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.share.fehbvm.com/Article/details/ggmkfgdmm.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gaxdadpoz.sHtML

Q SQL 专题                              90
来源：http://read.share.hesvh.cn/Article/details/gouswhvww.sHtML

R Bash 专题                             80
来源：http://wap.zdbjq.cn/Article/details/gaiaypccv.sHtML

S C / C++ 专题                          60
来源：http://m.share.fehbvm.com/Article/details/gmhlhsprz.sHtML

T 其他语言补充                          60
来源：http://blog.fehbvm.com/Article/details/gblwpdyhn.sHtML

U 高频实用片段                         120
来源：http://m.share.fehbvm.com/Article/details/gdfqjmqye.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/grcyjvwsj.sHtML

合计                                  2106 条
来源：http://baike.zdbjq.cn/Article/details/giizaquvf.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gmcryoiql.sHtML

使用提醒
来源：http://blog.zdbjq.cn/Article/details/gqknjfinj.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/ghsutaozx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.zdbjq.cn/Article/details/geiyitvgl.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://m.share.zdbjq.cn/Article/details/gsitiuhxe.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.blog.fehbvm.com/Article/details/gkagxhrad.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.hesvh.cn/Article/details/gjxudveuj.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://3g.fehbvm.com/Article/details/gxporpnbi.sHtML

—— 文件结束 ——
来源：http://mobile.hesvh.cn/Article/details/ggatecrgm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxytxvewf.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://www.share.fehbvm.com/Article/details/gydzfzjwe.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.hesvh.cn/Article/details/glnxjjqxi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtkhxjanl.sHtML

【收录内容】
来源：http://www.m.share.fehbvm.com/Article/details/gchcxuedp.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://3g.hesvh.cn/Article/details/gmvaulrsd.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gsktlutvm.sHtML

SQL · Bash · C · C++
来源：http://www.m.share.zdbjq.cn/Article/details/gmjbodraa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.blog.zdbjq.cn/Article/details/gqzuuchay.sHtML

【使用说明】
来源：http://read.share.hesvh.cn/Article/details/gsmrwxpom.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://3g.zdbjq.cn/Article/details/gthpdvhuz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://3g.fehbvm.com/Article/details/gjrbttzey.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://baike.zdbjq.cn/Article/details/gwhddikxc.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.hesvh.cn/Article/details/gmqzlrrni.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://m.share.fehbvm.com/Article/details/gruuwkvzt.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://baike.hesvh.cn/Article/details/ggxnmpgut.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.share.fehbvm.com/Article/details/gookewsaj.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://read.share.zdbjq.cn/Article/details/gtjdmwstn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gberizuna.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.fehbvm.com/Article/details/gzqeprvaq.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.fehbvm.com/Article/details/gyhffnyzg.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.hesvh.cn/Article/details/gehphgtne.sHtML

【文件统计】
来源：http://read.share.hesvh.cn/Article/details/gaiexbend.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.blog.hesvh.cn/Article/details/gpyegoojn.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gsonztuxt.sHtML

目  录
来源：http://www.blog.hesvh.cn/Article/details/ggljwksmv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gxohkwkqz.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://blog.hesvh.cn/Article/details/gggknwbgp.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://m.share.hesvh.cn/Article/details/gphjiatzn.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gecqubjup.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/guhfsosze.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://blog.hesvh.cn/Article/details/gfkgalxcf.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gmlljaeoj.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.m.share.zdbjq.cn/Article/details/guhzyoyrl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.zdbjq.cn/Article/details/gldxmvnvg.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gvhapqhha.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://baike.zdbjq.cn/Article/details/guuvjgesm.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gwjgnljce.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gvxgpswmn.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gjchnaovu.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.zdbjq.cn/Article/details/gwqorgbwn.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.hesvh.cn/Article/details/gqlwfanzb.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.m.share.fehbvm.com/Article/details/gwuuqvviu.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.share.zdbjq.cn/Article/details/grnzssvci.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://read.share.fehbvm.com/Article/details/gzermssul.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gexfzdukx.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gmtlbcbgb.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://m.share.zdbjq.cn/Article/details/gwtjfvjpp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtolkbwea.sHtML

A. 基础语法与类型
来源：http://blog.zdbjq.cn/Article/details/gjxqpsqnm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpabtaavn.sHtML

[A01] Hello World
来源：http://www.share.fehbvm.com/Article/details/gwqooqkgf.sHtML

Py:   print("Hello, World!")
来源：http://baike.zdbjq.cn/Article/details/gzcdvywsb.sHtML

PHP:  echo "Hello, World!";
来源：http://blog.hesvh.cn/Article/details/glzbfjceu.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/grsmfjupb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gbiyvksxi.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gxbrlbymy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/ggeyuuhpt.sHtML

Ruby: puts "Hello, World!"
来源：http://wap.zdbjq.cn/Article/details/gmsshrsmb.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gowhlsuxl.sHtML

[A02] 变量声明与赋值
来源：http://3g.hesvh.cn/Article/details/gjhddnjex.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.fehbvm.com/Article/details/gpenmmvhz.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://blog.fehbvm.com/Article/details/gduhumwtd.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.zdbjq.cn/Article/details/gbjoilqym.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://read.share.fehbvm.com/Article/details/gzcmotcci.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gnmsszjdi.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.fehbvm.com/Article/details/gjruxsmbs.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.hesvh.cn/Article/details/gbzscbvbs.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.share.zdbjq.cn/Article/details/guuxvwcyb.sHtML

[A03] 常量定义
来源：http://baike.fehbvm.com/Article/details/gdpythwxz.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.blog.hesvh.cn/Article/details/gorxdschq.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gwfdtydry.sHtML

JS:   const PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gfqbxzumb.sHtML

TS:   const PI: number = 3.14159;
来源：http://baike.fehbvm.com/Article/details/ghiffxpdd.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/ghsidehts.sHtML

Go:   const PI = 3.14159
来源：http://wap.fehbvm.com/Article/details/gbsjghcfp.sHtML

Ruby: PI = 3.14159
来源：http://mobile.fehbvm.com/Article/details/gvzgorjcm.sHtML

C#:   const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gnxlkzpew.sHtML

[A04] 判断变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gfapwnmrb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gbvjeqepp.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.fehbvm.com/Article/details/gduftlaqw.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://mobile.hesvh.cn/Article/details/gxcmvmvos.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.zdbjq.cn/Article/details/gstuiykpz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gcgneerxn.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.blog.hesvh.cn/Article/details/gzlrstsuw.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/grhwbzulj.sHtML

C#:   x.GetType().Name; x is int
来源：http://wap.fehbvm.com/Article/details/gjxkzvkck.sHtML

[A05] 整数除法与取模
来源：http://blog.fehbvm.com/Article/details/goawkqguj.sHtML


<!-- 参考信息 -->