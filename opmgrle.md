代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://blog.fehbvm.com/Article/details/gegjoipnc.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://blog.hesvh.cn/Article/details/gkaqpfbqf.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://mobile.fehbvm.com/Article/details/gmyxrnmib.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://read.share.fehbvm.com/Article/details/gbhusbwqc.sHtML

[U43] PHP：声明命名空间
来源：http://mobile.fehbvm.com/Article/details/gygtbgihl.sHtML

namespace App\Http;
来源：http://blog.zdbjq.cn/Article/details/gyjfwusab.sHtML

[U44] PHP：开启严格类型
来源：http://wap.hesvh.cn/Article/details/ghffbywow.sHtML

declare(strict_types=1);
来源：http://3g.zdbjq.cn/Article/details/gtihwtsny.sHtML

[U45] PHP：类型声明与返回类型
来源：http://blog.fehbvm.com/Article/details/gbdgocpom.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gujqxxtik.sHtML

[U46] PHP：可空类型
来源：http://read.share.zdbjq.cn/Article/details/gkyxlkwnu.sHtML

?string $name = null
来源：http://mobile.fehbvm.com/Article/details/gvrhczgju.sHtML

[U47] PHP：联合类型
来源：http://3g.zdbjq.cn/Article/details/gvauavdbx.sHtML

int|string $id
来源：http://read.share.zdbjq.cn/Article/details/gvyeruhoy.sHtML

[U48] PHP：纯枚举
来源：http://read.share.hesvh.cn/Article/details/gbxbkeklj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.share.hesvh.cn/Article/details/gzphbbkyp.sHtML

[U49] PHP：只读属性
来源：http://mobile.fehbvm.com/Article/details/ghwtqthnp.sHtML

public readonly string $name
来源：http://www.share.fehbvm.com/Article/details/gbupljngq.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.hesvh.cn/Article/details/gqgxtzhhd.sHtML

public function __construct(private int $id) {}
来源：http://blog.zdbjq.cn/Article/details/gxuaageer.sHtML

[U51] PHP：数组解构
来源：http://m.share.fehbvm.com/Article/details/gpwvwurlu.sHtML

[$a, $b] = $arr;
来源：http://www.m.share.hesvh.cn/Article/details/gbzdlwpyy.sHtML

[U52] PHP：箭头函数
来源：http://mobile.hesvh.cn/Article/details/ghprjbmiy.sHtML

$double = fn($x) => $x * 2;
来源：http://wap.fehbvm.com/Article/details/gewbwpulj.sHtML

[U53] PHP：空合并运算符
来源：http://www.blog.zdbjq.cn/Article/details/grihakiof.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.zdbjq.cn/Article/details/gskeuigkk.sHtML

[U54] PHP：空安全调用
来源：http://read.share.fehbvm.com/Article/details/grzuipxaj.sHtML

$obj?->method()
来源：http://wap.zdbjq.cn/Article/details/gmidjjxdz.sHtML

[U55] PHP：match 表达式
来源：http://mobile.hesvh.cn/Article/details/gxxucmyrg.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.hesvh.cn/Article/details/gyyyeamwe.sHtML

[U56] PHP：命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gewkimrnq.sHtML

f(a: 1, b: 2)
来源：http://read.share.fehbvm.com/Article/details/gnwwkafoi.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gppuaadbu.sHtML

"值: {$a}"
来源：http://mobile.fehbvm.com/Article/details/gcdzhomby.sHtML

[U58] PHP：数组三件套
来源：http://www.share.fehbvm.com/Article/details/gxtrmqltx.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://blog.zdbjq.cn/Article/details/gthhfardg.sHtML

[U59] PHP：自定义排序
来源：http://mobile.zdbjq.cn/Article/details/gnhtuinpn.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gpgombhcz.sHtML

[U60] PHP：JSON 编解码
来源：http://3g.fehbvm.com/Article/details/gnxtnqdjh.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://m.share.hesvh.cn/Article/details/gkgtvompv.sHtML

[U61] PHP：正则
来源：http://www.m.share.hesvh.cn/Article/details/glndgexaw.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gecbntcwe.sHtML

[U62] PHP：日期对象
来源：http://mobile.zdbjq.cn/Article/details/gqegaypqo.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.fehbvm.com/Article/details/gdixwjzea.sHtML

[U63] PHP：文件读写
来源：http://3g.zdbjq.cn/Article/details/ggxcvxwnk.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.m.share.fehbvm.com/Article/details/gshwrgtjy.sHtML

[U64] PHP：目录遍历
来源：http://blog.zdbjq.cn/Article/details/gnwayoffy.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/ggtcbkewp.sHtML

[U65] PHP：会话
来源：http://baike.fehbvm.com/Article/details/gpzwvbkri.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gawbwjehr.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.hesvh.cn/Article/details/gfcwbowgc.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://blog.fehbvm.com/Article/details/gpdbsxgik.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.zdbjq.cn/Article/details/gtbttilro.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://m.share.fehbvm.com/Article/details/gpexjhpkg.sHtML

[U68] PHP：PDO 连接
来源：http://read.share.hesvh.cn/Article/details/gulznihep.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://wap.hesvh.cn/Article/details/gdejcface.sHtML

[U69] PHP：PDO 预处理
来源：http://baike.zdbjq.cn/Article/details/gellowuny.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://read.share.zdbjq.cn/Article/details/gpevicmez.sHtML

[U70] PHP：PDO 事务
来源：http://www.share.hesvh.cn/Article/details/gwksjokza.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://wap.fehbvm.com/Article/details/gieadykjo.sHtML

[U71] PHP：抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gggvkbbof.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gmzgxdnlw.sHtML

[U72] PHP：写错误日志
来源：http://www.m.share.fehbvm.com/Article/details/gdkydspqq.sHtML

error_log("失败: " . $e->getMessage());
来源：http://mobile.zdbjq.cn/Article/details/gfpkcnkho.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.blog.hesvh.cn/Article/details/gdptrutis.sHtML

parse_ini_file("config.ini", true)
来源：http://read.share.fehbvm.com/Article/details/gnwgngnfv.sHtML

[U74] PHP：读取环境变量
来源：http://3g.zdbjq.cn/Article/details/glllxtljg.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.m.share.zdbjq.cn/Article/details/guqghbiia.sHtML

[U75] PHP：依赖注入
来源：http://mobile.fehbvm.com/Article/details/gdzatgkhy.sHtML

composer require psr/container
来源：http://baike.hesvh.cn/Article/details/gvismgpjy.sHtML

[U76] PHP：简单路由
来源：http://3g.zdbjq.cn/Article/details/gqdeaaqzf.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.m.share.fehbvm.com/Article/details/greipsdsv.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/glceasdlb.sHtML

composer require twig/twig
来源：http://blog.fehbvm.com/Article/details/guyvkfqne.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/gmgbbkjph.sHtML

composer require --dev phpunit/phpunit
来源：http://mobile.fehbvm.com/Article/details/gzzpuxnlk.sHtML

[U79] PHP：静态分析
来源：http://read.share.hesvh.cn/Article/details/gqiszrqog.sHtML

composer require --dev phpstan/phpstan
来源：http://baike.hesvh.cn/Article/details/gttdnkjwj.sHtML

[U80] PHP：代码规范修复
来源：http://3g.hesvh.cn/Article/details/gppfrjmbf.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://read.share.fehbvm.com/Article/details/goojzszwq.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/gsgphvnsq.sHtML

npm init -y;  npm i express
来源：http://www.share.fehbvm.com/Article/details/gwiqsglrs.sHtML

[U82] JS：package.json 脚本
来源：http://mobile.hesvh.cn/Article/details/gtghwrrjp.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gumwlbmwx.sHtML

[U83] JS：ES Module 导入导出
来源：http://wap.zdbjq.cn/Article/details/gtzmpxkxm.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/ggwhnhhal.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/grprwberl.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://wap.fehbvm.com/Article/details/gantcswmf.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gvtradtui.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gerjyqtzj.sHtML

[U86] JS：空值合并
来源：http://www.share.zdbjq.cn/Article/details/gjojexzkt.sHtML

a ?? b
来源：http://blog.zdbjq.cn/Article/details/glcervnat.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gjuciqjny.sHtML

const { a = 1, b = 2 } = obj;
来源：http://mobile.zdbjq.cn/Article/details/gnthapkxg.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gudlzetep.sHtML

{ ...a, ...b }
来源：http://3g.hesvh.cn/Article/details/gujspzjja.sHtML

[U89] JS：数组去重
来源：http://www.share.fehbvm.com/Article/details/glwaoiium.sHtML

[...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gkohfigjm.sHtML

[U90] JS：数字数组排序
来源：http://wap.hesvh.cn/Article/details/gpyawfawj.sHtML

[...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gvkshtewj.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/gnxfxthvz.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://read.share.fehbvm.com/Article/details/gadumfeyw.sHtML

[U92] JS：深拷贝
来源：http://m.share.fehbvm.com/Article/details/gfwgnpyeo.sHtML

structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/godfwgioy.sHtML

[U93] JS：模板字符串
来源：http://mobile.zdbjq.cn/Article/details/gqmokkxuy.sHtML

`共 ${n} 条`
来源：http://blog.hesvh.cn/Article/details/gfvqadxzs.sHtML

[U94] JS：箭头函数
来源：http://www.share.fehbvm.com/Article/details/ghlhlfsew.sHtML

const double = x => x * 2;
来源：http://baike.fehbvm.com/Article/details/gawoklzus.sHtML

[U95] JS：Promise 包装
来源：http://www.m.share.zdbjq.cn/Article/details/grhmzdjrg.sHtML

new Promise((resolve, reject) => {})
来源：http://mobile.hesvh.cn/Article/details/gmswxckoh.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.hesvh.cn/Article/details/gexexwdqs.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gzjnlfhpr.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gqvfhfqdq.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gixnofewi.sHtML

[U98] JS：fetch 带 JSON
来源：http://m.share.fehbvm.com/Article/details/gbginsihx.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gwpaiinmo.sHtML

[U99] JS：事件监听
来源：http://mobile.zdbjq.cn/Article/details/gcrlycvjf.sHtML

el.addEventListener("click", e => {})
来源：http://wap.zdbjq.cn/Article/details/gowwqwaig.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gpvamrbvs.sHtML

document.querySelector(".item")
来源：http://3g.hesvh.cn/Article/details/gtwchsrwb.sHtML

[U101] JS：classList 操作
来源：http://3g.fehbvm.com/Article/details/gonwtcuut.sHtML

el.classList.toggle("active")
来源：http://www.share.zdbjq.cn/Article/details/gzbcnartk.sHtML

[U102] JS：本地存储
来源：http://baike.hesvh.cn/Article/details/gepokumgf.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gaawewigi.sHtML

[U103] JS：定时器
来源：http://m.share.zdbjq.cn/Article/details/giaoebdag.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://m.share.fehbvm.com/Article/details/gaaknrtop.sHtML

[U104] JS：防抖
来源：http://blog.hesvh.cn/Article/details/gkiodrbud.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gczoovhhu.sHtML

[U105] JS：节流
来源：http://baike.hesvh.cn/Article/details/gnvojefbv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://wap.fehbvm.com/Article/details/gdupdpmsa.sHtML

[U106] JS：日期格式化
来源：http://baike.hesvh.cn/Article/details/goalbbvlf.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.zdbjq.cn/Article/details/gryjowbdk.sHtML

[U107] JS：数字千分位
来源：http://www.share.hesvh.cn/Article/details/gtoaebhgw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://blog.fehbvm.com/Article/details/ggqbpmrlv.sHtML

[U108] JS：随机整数
来源：http://blog.zdbjq.cn/Article/details/gralpsqke.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://m.share.fehbvm.com/Article/details/ghfsirjwx.sHtML

[U109] JS：数组分组
来源：http://m.share.zdbjq.cn/Article/details/gvbuhxlsn.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gnawkprzu.sHtML

[U110] JS：数组分块
来源：http://m.share.hesvh.cn/Article/details/gxvdkhfam.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gfpjqwteg.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gspobkdkb.sHtML

new Map(Object.entries(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gwsngwbbg.sHtML

[U112] JS：字符串补位
来源：http://3g.fehbvm.com/Article/details/gkpycmsun.sHtML

"7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gjxxmcaiy.sHtML

[U113] JS：正则替换全部
来源：http://m.share.fehbvm.com/Article/details/gvofekjgk.sHtML

s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gnzokmmkf.sHtML

[U114] JS：JSON 深比较
来源：http://3g.hesvh.cn/Article/details/grhcvdhou.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.zdbjq.cn/Article/details/gddvyyyfh.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gpstnmwgg.sHtML

crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gzmfkxrod.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://mobile.hesvh.cn/Article/details/ghlodklvq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.share.hesvh.cn/Article/details/gqpcusjyf.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gpkvvrrzo.sHtML

npm i -D vitest;  npx vitest
来源：http://www.m.share.zdbjq.cn/Article/details/gvqjpzdci.sHtML

[U118] JS：开发服务器
来源：http://www.m.share.hesvh.cn/Article/details/gwkhsvysd.sHtML

npm i -D vite;  npx vite
来源：http://www.m.share.fehbvm.com/Article/details/gixgktlao.sHtML

[U119] JS：生产构建
来源：http://read.share.hesvh.cn/Article/details/gfvpkqkyh.sHtML

npx vite build
来源：http://read.share.hesvh.cn/Article/details/ghthpcmrs.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://3g.hesvh.cn/Article/details/gmyylrdqi.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gqnytmjbl.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkwclxnai.sHtML

统计汇总
来源：http://www.share.hesvh.cn/Article/details/grjwhjfap.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwxqmawng.sHtML

按语言统计（条）：
来源：http://www.m.share.hesvh.cn/Article/details/gvksvjyyw.sHtML

Python ......... 252
来源：http://www.blog.zdbjq.cn/Article/details/gywsdghls.sHtML

PHP ............ 252
来源：http://www.share.zdbjq.cn/Article/details/gyrrydijq.sHtML

JavaScript ..... 252
来源：http://mobile.hesvh.cn/Article/details/gzkhodyci.sHtML

TypeScript ..... 212
来源：http://baike.zdbjq.cn/Article/details/glhzjzccz.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gdjllfcnd.sHtML

Go ............. 212
来源：http://wap.fehbvm.com/Article/details/gwwlawmxi.sHtML

Ruby ........... 212
来源：http://baike.zdbjq.cn/Article/details/gujhepksp.sHtML

C# ............. 212
来源：http://wap.hesvh.cn/Article/details/gljyfqupn.sHtML

C .............. 30
来源：http://www.m.share.hesvh.cn/Article/details/gouczbsyn.sHtML

C++ ............ 30
来源：http://wap.fehbvm.com/Article/details/gurmlbblq.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gnqcfhhre.sHtML

Bash ........... 80
来源：http://wap.zdbjq.cn/Article/details/gokxskckh.sHtML

Kotlin ......... 15
来源：http://m.share.hesvh.cn/Article/details/grntlwkdb.sHtML

Swift .......... 15
来源：http://www.blog.hesvh.cn/Article/details/ggaqsjsrs.sHtML

Lua ............ 10
来源：http://3g.fehbvm.com/Article/details/gqotmeboj.sHtML

Perl ........... 10
来源：http://www.m.share.zdbjq.cn/Article/details/gisekfliv.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/glxwdsvqz.sHtML

------------------------------------
来源：http://blog.fehbvm.com/Article/details/gqoifxtdd.sHtML

合计 ........... 2106 条
来源：http://mobile.hesvh.cn/Article/details/gkkwbxran.sHtML

按章节统计：
来源：http://www.blog.zdbjq.cn/Article/details/gwvvxxwjl.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.share.zdbjq.cn/Article/details/gbkfybmpv.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gbildpsjy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/geypxrxgy.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://blog.hesvh.cn/Article/details/gsvadcocz.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://read.share.fehbvm.com/Article/details/gpuuycxjv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.hesvh.cn/Article/details/gbdsgtpgo.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://blog.hesvh.cn/Article/details/gvfotdnws.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://mobile.hesvh.cn/Article/details/gsrjftaly.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gfnxmcifb.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gndfuqkyx.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gzlgltnch.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://wap.fehbvm.com/Article/details/gnsgwjrcv.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gtwgxpsky.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.m.share.fehbvm.com/Article/details/gyqiumbir.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://read.share.hesvh.cn/Article/details/gzkjhyzlc.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.blog.zdbjq.cn/Article/details/gjjbwezhq.sHtML

Q SQL 专题                              90
来源：http://baike.hesvh.cn/Article/details/gqhpbobao.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gecngwvrc.sHtML

S C / C++ 专题                          60
来源：http://mobile.fehbvm.com/Article/details/gzqgpzmsb.sHtML

T 其他语言补充                          60
来源：http://wap.fehbvm.com/Article/details/gzrkijlmb.sHtML

U 高频实用片段                         120
来源：http://baike.zdbjq.cn/Article/details/goidqbkde.sHtML

------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/grvtebeyq.sHtML

合计                                  2106 条
来源：http://www.m.share.fehbvm.com/Article/details/gxhyftdhs.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gfdcmtwln.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gnlccjfzk.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.zdbjq.cn/Article/details/gxmdavjra.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://wap.hesvh.cn/Article/details/gnmkmzimv.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.zdbjq.cn/Article/details/gsnpboxjq.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/ghjdbpmtx.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://mobile.zdbjq.cn/Article/details/gpnmiebdh.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.blog.hesvh.cn/Article/details/gonklpndk.sHtML

—— 文件结束 ——
来源：http://www.m.share.zdbjq.cn/Article/details/gkdqglfdd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gytijeyon.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.hesvh.cn/Article/details/gzsyunknh.sHtML

Common Programming Examples Cheat Book
来源：http://www.blog.zdbjq.cn/Article/details/gchjygtee.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grzoghcop.sHtML

【收录内容】
来源：http://wap.zdbjq.cn/Article/details/gswjbauzo.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.fehbvm.com/Article/details/gzmmkluvf.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://m.share.zdbjq.cn/Article/details/gftggpxxd.sHtML

SQL · Bash · C · C++
来源：http://www.blog.fehbvm.com/Article/details/gnzmmiuac.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.zdbjq.cn/Article/details/gljrphpgt.sHtML

【使用说明】
来源：http://www.share.fehbvm.com/Article/details/gcmcxzadk.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://baike.hesvh.cn/Article/details/gyqutqcrb.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://read.share.zdbjq.cn/Article/details/gygwgyepq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.zdbjq.cn/Article/details/gvelmbilq.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://3g.zdbjq.cn/Article/details/ghfzztcno.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/glqchvdge.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.m.share.hesvh.cn/Article/details/gsblqwozq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://baike.zdbjq.cn/Article/details/gkdcxkepv.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://blog.fehbvm.com/Article/details/gjtxovrxp.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/gwechbxkm.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gqrzypvvm.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://mobile.fehbvm.com/Article/details/gkocuaiuq.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://mobile.hesvh.cn/Article/details/gmpduteyn.sHtML

【文件统计】
来源：http://mobile.fehbvm.com/Article/details/ggslpyvvn.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://m.share.zdbjq.cn/Article/details/gnyfhkrny.sHtML

--------------------------------------------------------------------------------
来源：http://blog.hesvh.cn/Article/details/gzihvnecu.sHtML

目  录
来源：http://mobile.fehbvm.com/Article/details/gzcvexesi.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gpjexdodd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gxoljkqgy.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://blog.hesvh.cn/Article/details/gpnxqdmoz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.fehbvm.com/Article/details/gigcjjhri.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://m.share.fehbvm.com/Article/details/gaztdnatx.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://m.share.zdbjq.cn/Article/details/gagmpbtba.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://blog.fehbvm.com/Article/details/ghghnwyqt.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/gvweduohc.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://mobile.fehbvm.com/Article/details/gtcdaffwb.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gavohlmic.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.fehbvm.com/Article/details/gzmhkawrx.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://3g.hesvh.cn/Article/details/gklaltoen.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.share.hesvh.cn/Article/details/gubpizuer.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gakjefnvk.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.fehbvm.com/Article/details/ghnnhvoyu.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.fehbvm.com/Article/details/gznpryrrp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/gxpvldlqg.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://m.share.zdbjq.cn/Article/details/grurkuptl.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gnvaohmhq.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.blog.fehbvm.com/Article/details/gvwcztugy.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gypwmfadc.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gdidzgolw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsztuebmb.sHtML

A. 基础语法与类型
来源：http://wap.zdbjq.cn/Article/details/gjolaifqo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gunaqdbxp.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gwswixmqc.sHtML

Py:   print("Hello, World!")
来源：http://wap.zdbjq.cn/Article/details/gmrnfczor.sHtML

PHP:  echo "Hello, World!";
来源：http://3g.hesvh.cn/Article/details/gbjxgagmf.sHtML

JS:   console.log("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gmwjrhgpu.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://mobile.zdbjq.cn/Article/details/gerrwubad.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gzsfgusfw.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/gnhzmccmm.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/ghrrvzoww.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://read.share.zdbjq.cn/Article/details/gmvhjtjot.sHtML

[A02] 变量声明与赋值
来源：http://baike.zdbjq.cn/Article/details/gslqbxisn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.blog.zdbjq.cn/Article/details/govaofnlr.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://wap.fehbvm.com/Article/details/gihlvygqm.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gaqpzyjst.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.hesvh.cn/Article/details/ghmnffdpi.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/gbdorkrka.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/gbitxvwzo.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/grlkkxsxq.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://www.blog.fehbvm.com/Article/details/ggwygmofe.sHtML

[A03] 常量定义
来源：http://read.share.hesvh.cn/Article/details/gapkccvtm.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gahyksmnn.sHtML

PHP:  const PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gxfuapfjx.sHtML

JS:   const PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/gjsaonczd.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/ghmubjycp.sHtML

Java: static final double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gqcnzsfrb.sHtML

Go:   const PI = 3.14159
来源：http://blog.zdbjq.cn/Article/details/gyfewxyit.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/gzakxhprq.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/geetplwsy.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gosrvunxd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.hesvh.cn/Article/details/gyievxnjk.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.share.hesvh.cn/Article/details/ggvbamaqs.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://read.share.hesvh.cn/Article/details/gjzarawoc.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gtjqlsevj.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://m.share.zdbjq.cn/Article/details/grwxabdhw.sHtML


<!-- 参考信息 -->