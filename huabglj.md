代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://wap.zdbjq.cn/Article/details/gbniqimto.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://www.blog.fehbvm.com/Article/details/gwwyonvin.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://www.blog.zdbjq.cn/Article/details/gbwxbodjm.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://3g.fehbvm.com/Article/details/gxblexxpt.sHtML

[U43] PHP：声明命名空间
来源：http://m.share.zdbjq.cn/Article/details/gaffirdmd.sHtML

namespace App\Http;
来源：http://mobile.fehbvm.com/Article/details/grhgwfumu.sHtML

[U44] PHP：开启严格类型
来源：http://m.share.zdbjq.cn/Article/details/gmnrzlwhc.sHtML

declare(strict_types=1);
来源：http://m.share.hesvh.cn/Article/details/ghrftsewl.sHtML

[U45] PHP：类型声明与返回类型
来源：http://wap.zdbjq.cn/Article/details/gfxddyjea.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/gkrtztxcv.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gacceudsu.sHtML

?string $name = null
来源：http://www.share.hesvh.cn/Article/details/ggvasulwt.sHtML

[U47] PHP：联合类型
来源：http://www.share.zdbjq.cn/Article/details/gmwyotdqx.sHtML

int|string $id
来源：http://m.share.fehbvm.com/Article/details/gzoyrptdt.sHtML

[U48] PHP：纯枚举
来源：http://blog.fehbvm.com/Article/details/gtqytytme.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/goakygitn.sHtML

[U49] PHP：只读属性
来源：http://read.share.fehbvm.com/Article/details/gevscxuzm.sHtML

public readonly string $name
来源：http://baike.hesvh.cn/Article/details/gzdroasjd.sHtML

[U50] PHP：构造器属性提升
来源：http://www.m.share.hesvh.cn/Article/details/gkwecctll.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gejbsozkr.sHtML

[U51] PHP：数组解构
来源：http://wap.hesvh.cn/Article/details/ghknqrfxp.sHtML

[$a, $b] = $arr;
来源：http://3g.fehbvm.com/Article/details/gckxtmzur.sHtML

[U52] PHP：箭头函数
来源：http://www.m.share.zdbjq.cn/Article/details/gujidsefw.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.hesvh.cn/Article/details/gfdfgfxjd.sHtML

[U53] PHP：空合并运算符
来源：http://www.m.share.zdbjq.cn/Article/details/grffczvhq.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.hesvh.cn/Article/details/gikswbfti.sHtML

[U54] PHP：空安全调用
来源：http://read.share.zdbjq.cn/Article/details/gkzonrhlw.sHtML

$obj?->method()
来源：http://read.share.hesvh.cn/Article/details/gxwjfookt.sHtML

[U55] PHP：match 表达式
来源：http://3g.hesvh.cn/Article/details/gjafvxvvl.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gswtwyhkv.sHtML

[U56] PHP：命名参数
来源：http://baike.hesvh.cn/Article/details/gwuiwqzvp.sHtML

f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gmqripcra.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/guwfsyufz.sHtML

"值: {$a}"
来源：http://read.share.fehbvm.com/Article/details/gnvubzuqm.sHtML

[U58] PHP：数组三件套
来源：http://www.m.share.zdbjq.cn/Article/details/ggmbcbzgf.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/grspzewex.sHtML

[U59] PHP：自定义排序
来源：http://www.blog.fehbvm.com/Article/details/gplvtyqdo.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/giixwgsiq.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gjjnknizm.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://blog.fehbvm.com/Article/details/goxqlhmqi.sHtML

[U61] PHP：正则
来源：http://wap.hesvh.cn/Article/details/gxisjxipl.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/grdbvrweu.sHtML

[U62] PHP：日期对象
来源：http://3g.hesvh.cn/Article/details/guqzzpngr.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.blog.fehbvm.com/Article/details/gbgiomaeu.sHtML

[U63] PHP：文件读写
来源：http://wap.fehbvm.com/Article/details/gvjkooymq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/grpvjvjmo.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gmsgzxuvd.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://wap.zdbjq.cn/Article/details/gkuxvonuj.sHtML

[U65] PHP：会话
来源：http://wap.fehbvm.com/Article/details/gcyncnjta.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://wap.fehbvm.com/Article/details/gxsdgynms.sHtML

[U66] PHP：设置 Cookie
来源：http://www.share.hesvh.cn/Article/details/gvhhidbqh.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://read.share.fehbvm.com/Article/details/gvngfjzar.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gsvinjwas.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gtbiqkthb.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gtaebbtpq.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.hesvh.cn/Article/details/gmnbamrxh.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.hesvh.cn/Article/details/gxdopncuj.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkbozsoq.sHtML

[U70] PHP：PDO 事务
来源：http://wap.zdbjq.cn/Article/details/gtmikiewo.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.blog.hesvh.cn/Article/details/gnxnynbzm.sHtML

[U71] PHP：抛出异常
来源：http://wap.hesvh.cn/Article/details/gcrrdcjua.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.fehbvm.com/Article/details/glesjqgcx.sHtML

[U72] PHP：写错误日志
来源：http://www.share.zdbjq.cn/Article/details/gqqgbewmu.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/ggcdxjeue.sHtML

[U73] PHP：读取 ini 配置
来源：http://read.share.hesvh.cn/Article/details/gfbluzoep.sHtML

parse_ini_file("config.ini", true)
来源：http://blog.fehbvm.com/Article/details/gsuxrcqak.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gbfgsusbu.sHtML

getenv("APP_ENV") ?: "production"
来源：http://blog.zdbjq.cn/Article/details/gnqkquqvg.sHtML

[U75] PHP：依赖注入
来源：http://read.share.zdbjq.cn/Article/details/gfdxledlc.sHtML

composer require psr/container
来源：http://blog.hesvh.cn/Article/details/ggrflbrkr.sHtML

[U76] PHP：简单路由
来源：http://wap.zdbjq.cn/Article/details/gxwgdomzm.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://blog.hesvh.cn/Article/details/gabekpumd.sHtML

[U77] PHP：模板渲染
来源：http://blog.hesvh.cn/Article/details/gjvwxstmv.sHtML

composer require twig/twig
来源：http://wap.fehbvm.com/Article/details/gfvepzrwi.sHtML

[U78] PHP：单元测试
来源：http://www.share.zdbjq.cn/Article/details/grtwrbizj.sHtML

composer require --dev phpunit/phpunit
来源：http://blog.fehbvm.com/Article/details/gobxzxalj.sHtML

[U79] PHP：静态分析
来源：http://www.m.share.fehbvm.com/Article/details/gstbuxtsr.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.fehbvm.com/Article/details/gxbsbnbmv.sHtML

[U80] PHP：代码规范修复
来源：http://read.share.zdbjq.cn/Article/details/ghoeswwir.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://3g.fehbvm.com/Article/details/gvoeibrmr.sHtML

[U81] JS：初始化项目
来源：http://blog.hesvh.cn/Article/details/gltmocech.sHtML

npm init -y;  npm i express
来源：http://wap.zdbjq.cn/Article/details/gnqhqhlyj.sHtML

[U82] JS：package.json 脚本
来源：http://wap.zdbjq.cn/Article/details/gxudsquwt.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.share.hesvh.cn/Article/details/gxriukhtu.sHtML

[U83] JS：ES Module 导入导出
来源：http://blog.hesvh.cn/Article/details/ghlftmewh.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gaoaegsjr.sHtML

[U84] JS：CommonJS 写法
来源：http://www.blog.hesvh.cn/Article/details/gfdnmhnsm.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://3g.hesvh.cn/Article/details/gkmsrnbaw.sHtML

[U85] JS：可选链
来源：http://baike.zdbjq.cn/Article/details/gzsmxxvck.sHtML

a?.b?.c
来源：http://mobile.hesvh.cn/Article/details/ggibjpcia.sHtML

[U86] JS：空值合并
来源：http://read.share.hesvh.cn/Article/details/gqkykwrxk.sHtML

a ?? b
来源：http://mobile.hesvh.cn/Article/details/gbcuicakp.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gjwrzfbvh.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/gctvasaih.sHtML

[U88] JS：对象展开合并
来源：http://read.share.hesvh.cn/Article/details/gjpxyhjfo.sHtML

{ ...a, ...b }
来源：http://www.blog.fehbvm.com/Article/details/gxzmicggu.sHtML

[U89] JS：数组去重
来源：http://wap.hesvh.cn/Article/details/gzuyejebb.sHtML

[...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gjfqvydfi.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gomkowvxx.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gkwxksxua.sHtML

[U91] JS：对象键值遍历
来源：http://mobile.fehbvm.com/Article/details/gowhxlyfu.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://mobile.zdbjq.cn/Article/details/gucisdzqo.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gfvofdpid.sHtML

structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gtfthgyjf.sHtML

[U93] JS：模板字符串
来源：http://3g.hesvh.cn/Article/details/gvkwvxvcl.sHtML

`共 ${n} 条`
来源：http://3g.zdbjq.cn/Article/details/gfnzvxfiu.sHtML

[U94] JS：箭头函数
来源：http://www.blog.fehbvm.com/Article/details/gqclkxndh.sHtML

const double = x => x * 2;
来源：http://read.share.zdbjq.cn/Article/details/gsszrddqy.sHtML

[U95] JS：Promise 包装
来源：http://baike.fehbvm.com/Article/details/gibffogba.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.fehbvm.com/Article/details/gubwwgwjq.sHtML

[U96] JS：async/await 与异常
来源：http://3g.fehbvm.com/Article/details/gxazogbng.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/guexwbhnn.sHtML

[U97] JS：并发请求
来源：http://blog.zdbjq.cn/Article/details/gncptnkba.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gizjprktj.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gffszbyej.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.hesvh.cn/Article/details/gvitmmahz.sHtML

[U99] JS：事件监听
来源：http://www.m.share.fehbvm.com/Article/details/gsmsdoden.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gphchxcyi.sHtML

[U100] JS：DOM 查询
来源：http://baike.fehbvm.com/Article/details/gnjbxrzaj.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/grtgvjqcj.sHtML

[U101] JS：classList 操作
来源：http://baike.zdbjq.cn/Article/details/glxxaaven.sHtML

el.classList.toggle("active")
来源：http://blog.fehbvm.com/Article/details/gqnorwcww.sHtML

[U102] JS：本地存储
来源：http://3g.fehbvm.com/Article/details/gecrjoncb.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.blog.hesvh.cn/Article/details/gpkoqhkvb.sHtML

[U103] JS：定时器
来源：http://baike.hesvh.cn/Article/details/gwfrngvcu.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.zdbjq.cn/Article/details/gwoxbsjhb.sHtML

[U104] JS：防抖
来源：http://mobile.fehbvm.com/Article/details/gkevpuwdw.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/ghqkcbfkc.sHtML

[U105] JS：节流
来源：http://m.share.zdbjq.cn/Article/details/gcddxceaf.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://read.share.zdbjq.cn/Article/details/gevgyhmgx.sHtML

[U106] JS：日期格式化
来源：http://www.share.hesvh.cn/Article/details/gyhdnhdze.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://wap.hesvh.cn/Article/details/gyavkosji.sHtML

[U107] JS：数字千分位
来源：http://read.share.fehbvm.com/Article/details/gtdkuyehv.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://baike.zdbjq.cn/Article/details/ghcasemsi.sHtML

[U108] JS：随机整数
来源：http://read.share.zdbjq.cn/Article/details/gndvteadp.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/gxyxrgljy.sHtML

[U109] JS：数组分组
来源：http://3g.zdbjq.cn/Article/details/glqbwyxzx.sHtML

Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gvkieobsv.sHtML

[U110] JS：数组分块
来源：http://www.share.fehbvm.com/Article/details/gvungvtzi.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://wap.fehbvm.com/Article/details/gfzjrjnet.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gikgjrbol.sHtML

new Map(Object.entries(obj))
来源：http://blog.fehbvm.com/Article/details/gdsaujnco.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/goxkuyidd.sHtML

"7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gsunzegdk.sHtML

[U113] JS：正则替换全部
来源：http://www.m.share.hesvh.cn/Article/details/gvjmkdcac.sHtML

s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gzkafihxc.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.hesvh.cn/Article/details/gjglwpyys.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fehbvm.com/Article/details/gvstuywru.sHtML

[U115] JS：生成 UUID
来源：http://baike.hesvh.cn/Article/details/gobtqsjpu.sHtML

crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gzaqleamg.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.zdbjq.cn/Article/details/ghenzcspd.sHtML

/** @param {string} name */ function f(name) {}
来源：http://mobile.hesvh.cn/Article/details/gdocsrdtz.sHtML

[U117] JS：单元测试
来源：http://blog.zdbjq.cn/Article/details/gidqinfow.sHtML

npm i -D vitest;  npx vitest
来源：http://www.blog.zdbjq.cn/Article/details/gfpkmqgkt.sHtML

[U118] JS：开发服务器
来源：http://mobile.fehbvm.com/Article/details/gbwjswaxt.sHtML

npm i -D vite;  npx vite
来源：http://read.share.zdbjq.cn/Article/details/gbcsoxecn.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/goqziyhzn.sHtML

npx vite build
来源：http://m.share.zdbjq.cn/Article/details/gaoqhczsg.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.fehbvm.com/Article/details/gpxtdwmri.sHtML

import.meta.env.VITE_API_URL
来源：http://read.share.fehbvm.com/Article/details/giawcbfqz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtpxhhqvh.sHtML

统计汇总
来源：http://3g.fehbvm.com/Article/details/gxmsgncwk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glcdzgahp.sHtML

按语言统计（条）：
来源：http://m.share.hesvh.cn/Article/details/gfschqdhx.sHtML

Python ......... 252
来源：http://mobile.fehbvm.com/Article/details/gzhmjcujb.sHtML

PHP ............ 252
来源：http://www.m.share.fehbvm.com/Article/details/ghcjsglkx.sHtML

JavaScript ..... 252
来源：http://www.blog.fehbvm.com/Article/details/gvbxatqgc.sHtML

TypeScript ..... 212
来源：http://wap.hesvh.cn/Article/details/ghsvvyfyx.sHtML

Java ........... 212
来源：http://www.share.fehbvm.com/Article/details/gyzawkrai.sHtML

Go ............. 212
来源：http://blog.zdbjq.cn/Article/details/gxkvtnaiw.sHtML

Ruby ........... 212
来源：http://read.share.hesvh.cn/Article/details/gowksdvvg.sHtML

C# ............. 212
来源：http://www.share.hesvh.cn/Article/details/gfnhhlofv.sHtML

C .............. 30
来源：http://3g.zdbjq.cn/Article/details/gacjlfwqh.sHtML

C++ ............ 30
来源：http://mobile.hesvh.cn/Article/details/gwfjcdvfs.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gfmkkkoge.sHtML

Bash ........... 80
来源：http://wap.hesvh.cn/Article/details/gvsgtgngy.sHtML

Kotlin ......... 15
来源：http://read.share.fehbvm.com/Article/details/geaqybqlk.sHtML

Swift .......... 15
来源：http://wap.zdbjq.cn/Article/details/gnlcctvts.sHtML

Lua ............ 10
来源：http://www.m.share.hesvh.cn/Article/details/gynctkilv.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gzvzelhjh.sHtML

Scala .......... 10
来源：http://3g.zdbjq.cn/Article/details/gbypwkipq.sHtML

------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/gpbqkifkt.sHtML

合计 ........... 2106 条
来源：http://mobile.zdbjq.cn/Article/details/gdqmvgwzx.sHtML

按章节统计：
来源：http://read.share.hesvh.cn/Article/details/gqcrefmnu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.blog.hesvh.cn/Article/details/gexwpjkkr.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.m.share.fehbvm.com/Article/details/gwlletczp.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gpddffwkc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/gfssrdklf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://3g.fehbvm.com/Article/details/gjaezfegq.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gnzmzpmtm.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://mobile.hesvh.cn/Article/details/gzzuwynuo.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gnxhnacuk.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.hesvh.cn/Article/details/gkcmnpqcv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://m.share.hesvh.cn/Article/details/gypwsblca.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://baike.fehbvm.com/Article/details/graruhbmr.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.share.zdbjq.cn/Article/details/gjbdowkgt.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gldlffdpj.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.fehbvm.com/Article/details/gtkpgmucj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gyhsiwgoh.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.fehbvm.com/Article/details/gzjdtxflw.sHtML

Q SQL 专题                              90
来源：http://mobile.zdbjq.cn/Article/details/gqlxojidm.sHtML

R Bash 专题                             80
来源：http://mobile.hesvh.cn/Article/details/gglciwpgd.sHtML

S C / C++ 专题                          60
来源：http://baike.zdbjq.cn/Article/details/garbtwrud.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/ghbpvrwqa.sHtML

U 高频实用片段                         120
来源：http://blog.zdbjq.cn/Article/details/gmulklzzi.sHtML

------------------------------------
来源：http://mobile.fehbvm.com/Article/details/gcqdwfahm.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gjqiszktp.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.zdbjq.cn/Article/details/gcimszrpc.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gscxowtce.sHtML

--------------------------------------------------------------------------------
来源：http://blog.zdbjq.cn/Article/details/gdqakuzhp.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.blog.hesvh.cn/Article/details/gzzitsonu.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gyrsnksrf.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://blog.zdbjq.cn/Article/details/grcoufzuh.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gnbiswffn.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.fehbvm.com/Article/details/gcalrkqlq.sHtML

—— 文件结束 ——
来源：http://wap.hesvh.cn/Article/details/gqpaqgjjs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbnnsxbgz.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://3g.zdbjq.cn/Article/details/gobkuliuj.sHtML

Common Programming Examples Cheat Book
来源：http://baike.zdbjq.cn/Article/details/gqwytkthp.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsuwfjdhe.sHtML

【收录内容】
来源：http://www.blog.fehbvm.com/Article/details/gjgggupql.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://read.share.zdbjq.cn/Article/details/gmeosfyce.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.share.hesvh.cn/Article/details/gupyhicqs.sHtML

SQL · Bash · C · C++
来源：http://www.blog.hesvh.cn/Article/details/gdhkjzbaa.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.hesvh.cn/Article/details/gzpzblhdf.sHtML

【使用说明】
来源：http://www.m.share.fehbvm.com/Article/details/ggwyhgmes.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.m.share.zdbjq.cn/Article/details/gdgdcihsj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.m.share.hesvh.cn/Article/details/gdlytcxng.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.hesvh.cn/Article/details/gpkstiueo.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.fehbvm.com/Article/details/gtzqdmqkg.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/gisploplr.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gbehewxdv.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.fehbvm.com/Article/details/gonzvhegh.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.hesvh.cn/Article/details/gubteqkjg.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://blog.fehbvm.com/Article/details/gpcmkjcbf.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://3g.hesvh.cn/Article/details/gmuibjnom.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.zdbjq.cn/Article/details/gufgtocrw.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gmorxnpzf.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/gcxazjqsb.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.fehbvm.com/Article/details/gbbfrjiln.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gxlwluflh.sHtML

目  录
来源：http://blog.zdbjq.cn/Article/details/gmjzitccm.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.hesvh.cn/Article/details/geyfyilgf.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gfbjiqjuf.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gjqslhypt.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://m.share.fehbvm.com/Article/details/gyzpilcyn.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.hesvh.cn/Article/details/gicsfnybu.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.hesvh.cn/Article/details/gtyvhhhek.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.fehbvm.com/Article/details/gzwvcwrep.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://baike.fehbvm.com/Article/details/gbnrzhucn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gshappwgx.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.blog.zdbjq.cn/Article/details/gkeszcemz.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gklmnoesl.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://m.share.fehbvm.com/Article/details/gpyfnyxef.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://read.share.fehbvm.com/Article/details/ggyzhcbct.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/glktizztz.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gmoxfunbq.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://read.share.fehbvm.com/Article/details/gwcmxxdrw.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.hesvh.cn/Article/details/gejnmpkfa.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://baike.fehbvm.com/Article/details/gfpnejzej.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.blog.fehbvm.com/Article/details/gnlqbyadb.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://mobile.fehbvm.com/Article/details/gbuglpwop.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/georwoapl.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.share.hesvh.cn/Article/details/gazomnihv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvixiiuhv.sHtML

A. 基础语法与类型
来源：http://m.share.fehbvm.com/Article/details/ghqrbpnnr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghnxeowhf.sHtML

[A01] Hello World
来源：http://read.share.fehbvm.com/Article/details/gkbvlpgtl.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gfbtxgnmd.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.fehbvm.com/Article/details/gbvkfzuid.sHtML

JS:   console.log("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gakwlvanb.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gamwyagis.sHtML

Java: System.out.println("Hello, World!");
来源：http://read.share.hesvh.cn/Article/details/gsvkvmdzy.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gdmhmktqy.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.hesvh.cn/Article/details/gvgjxccim.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/ganbmfzhd.sHtML

[A02] 变量声明与赋值
来源：http://m.share.fehbvm.com/Article/details/gmqviayll.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gizhcoczs.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.hesvh.cn/Article/details/gpkbnxnnu.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.fehbvm.com/Article/details/gcpxptzfy.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gewrhklki.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gptjdhobr.sHtML

Go:   name := "Alex"; age := 20
来源：http://baike.zdbjq.cn/Article/details/ghkndrfit.sHtML

Ruby: name = "Alex"; age = 20
来源：http://m.share.hesvh.cn/Article/details/gqdorbxav.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gxuiuxqnm.sHtML

[A03] 常量定义
来源：http://www.m.share.fehbvm.com/Article/details/geaupcvta.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.zdbjq.cn/Article/details/guidulfwd.sHtML

PHP:  const PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gtibkszvm.sHtML

JS:   const PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gosdvmdik.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/grosboaix.sHtML

Java: static final double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gycjajtca.sHtML

Go:   const PI = 3.14159
来源：http://wap.hesvh.cn/Article/details/guobujpos.sHtML

Ruby: PI = 3.14159
来源：http://www.share.hesvh.cn/Article/details/grpvalmsg.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gkobxbqnb.sHtML

[A04] 判断变量类型
来源：http://read.share.zdbjq.cn/Article/details/gydrtqmyb.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/glpfvpdlw.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.zdbjq.cn/Article/details/gpwcoarph.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://wap.fehbvm.com/Article/details/gweafytxz.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gxkgzymuz.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gydesdnvb.sHtML


<!-- 参考信息 -->