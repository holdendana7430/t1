代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.share.hesvh.cn/Article/details/gdjeafnpn.sHtML

composer init;  composer require guzzlehttp/guzzle
来源：http://baike.zdbjq.cn/Article/details/gvhlynlkc.sHtML

[U42] PHP：PSR-4 自动加载
来源：http://blog.fehbvm.com/Article/details/gvotokuck.sHtML

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.share.fehbvm.com/Article/details/gkbhtiamp.sHtML

[U43] PHP：声明命名空间
来源：http://wap.zdbjq.cn/Article/details/gmyfxakga.sHtML

namespace App\Http;
来源：http://www.share.fehbvm.com/Article/details/gksdjkhwo.sHtML

[U44] PHP：开启严格类型
来源：http://read.share.hesvh.cn/Article/details/gjagaqkjo.sHtML

declare(strict_types=1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdydamceu.sHtML

[U45] PHP：类型声明与返回类型
来源：http://m.share.hesvh.cn/Article/details/geacqhiid.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gvsaujyul.sHtML

[U46] PHP：可空类型
来源：http://mobile.hesvh.cn/Article/details/gkgypxatg.sHtML

?string $name = null
来源：http://blog.hesvh.cn/Article/details/gckfctbvk.sHtML

[U47] PHP：联合类型
来源：http://mobile.zdbjq.cn/Article/details/gmvaaclek.sHtML

int|string $id
来源：http://blog.zdbjq.cn/Article/details/gktnniora.sHtML

[U48] PHP：纯枚举
来源：http://www.blog.fehbvm.com/Article/details/gtyszypkm.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfxolvwjx.sHtML

[U49] PHP：只读属性
来源：http://www.m.share.fehbvm.com/Article/details/gyjllntkn.sHtML

public readonly string $name
来源：http://www.blog.fehbvm.com/Article/details/gpktbaoem.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gycdbzwlb.sHtML

public function __construct(private int $id) {}
来源：http://wap.fehbvm.com/Article/details/gavrtdouj.sHtML

[U51] PHP：数组解构
来源：http://3g.zdbjq.cn/Article/details/ggeqrlbgm.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gktyohfwc.sHtML

[U52] PHP：箭头函数
来源：http://www.share.zdbjq.cn/Article/details/gpthjnvdw.sHtML

$double = fn($x) => $x * 2;
来源：http://www.blog.zdbjq.cn/Article/details/ggmwwpczv.sHtML

[U53] PHP：空合并运算符
来源：http://wap.hesvh.cn/Article/details/gjsfrnfvj.sHtML

$v = $a ?? $b ?? "default";
来源：http://mobile.fehbvm.com/Article/details/gsklnbrls.sHtML

[U54] PHP：空安全调用
来源：http://baike.zdbjq.cn/Article/details/gvoyiiubn.sHtML

$obj?->method()
来源：http://mobile.zdbjq.cn/Article/details/grfnazcxw.sHtML

[U55] PHP：match 表达式
来源：http://www.blog.fehbvm.com/Article/details/gbaudbsds.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://m.share.zdbjq.cn/Article/details/gferasodu.sHtML

[U56] PHP：命名参数
来源：http://mobile.zdbjq.cn/Article/details/gvcblqvsb.sHtML

f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gfepwmuox.sHtML

[U57] PHP：字符串插值
来源：http://wap.fehbvm.com/Article/details/gjbqdqlze.sHtML

"值: {$a}"
来源：http://wap.hesvh.cn/Article/details/gutzrvdrx.sHtML

[U58] PHP：数组三件套
来源：http://read.share.fehbvm.com/Article/details/gjafzytqk.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gimlgvoky.sHtML

[U59] PHP：自定义排序
来源：http://blog.zdbjq.cn/Article/details/gicucsizb.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gbhnvtcbg.sHtML

[U60] PHP：JSON 编解码
来源：http://www.blog.fehbvm.com/Article/details/gyravaslx.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://baike.fehbvm.com/Article/details/gbtzpjied.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/gygcibeli.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gkligniik.sHtML

[U62] PHP：日期对象
来源：http://blog.fehbvm.com/Article/details/gmavofbtu.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/ghnouhfqi.sHtML

[U63] PHP：文件读写
来源：http://m.share.zdbjq.cn/Article/details/guajqsivn.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.zdbjq.cn/Article/details/gqfgyjdep.sHtML

[U64] PHP：目录遍历
来源：http://read.share.hesvh.cn/Article/details/gsnxhyoad.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.fehbvm.com/Article/details/gvpvfdrxv.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gpdduugmo.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/galpzsywj.sHtML

[U66] PHP：设置 Cookie
来源：http://mobile.zdbjq.cn/Article/details/gnwnozwno.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://m.share.fehbvm.com/Article/details/gmvyqbkor.sHtML

[U67] PHP：处理文件上传
来源：http://www.m.share.hesvh.cn/Article/details/gxgotuiya.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.m.share.fehbvm.com/Article/details/gjfdqgehq.sHtML

[U68] PHP：PDO 连接
来源：http://wap.zdbjq.cn/Article/details/gqdalrejt.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://read.share.fehbvm.com/Article/details/gvkkwkdyw.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.fehbvm.com/Article/details/gitquwyrv.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://mobile.zdbjq.cn/Article/details/gbocqvdcs.sHtML

[U70] PHP：PDO 事务
来源：http://www.m.share.hesvh.cn/Article/details/ggiofugnj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://mobile.zdbjq.cn/Article/details/giirvqrol.sHtML

[U71] PHP：抛出异常
来源：http://3g.fehbvm.com/Article/details/gkudkermv.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gkyietrrd.sHtML

[U72] PHP：写错误日志
来源：http://mobile.hesvh.cn/Article/details/gxzreiaqs.sHtML

error_log("失败: " . $e->getMessage());
来源：http://read.share.hesvh.cn/Article/details/gxhqftmao.sHtML

[U73] PHP：读取 ini 配置
来源：http://www.share.hesvh.cn/Article/details/gamwjmjjr.sHtML

parse_ini_file("config.ini", true)
来源：http://baike.zdbjq.cn/Article/details/gjmxpbkyp.sHtML

[U74] PHP：读取环境变量
来源：http://3g.fehbvm.com/Article/details/ggqvfplcs.sHtML

getenv("APP_ENV") ?: "production"
来源：http://baike.hesvh.cn/Article/details/gjkucewjj.sHtML

[U75] PHP：依赖注入
来源：http://3g.hesvh.cn/Article/details/gadfpapmf.sHtML

composer require psr/container
来源：http://www.share.zdbjq.cn/Article/details/gdbbtscwj.sHtML

[U76] PHP：简单路由
来源：http://wap.fehbvm.com/Article/details/gskzlitkn.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://3g.zdbjq.cn/Article/details/gimcscstm.sHtML

[U77] PHP：模板渲染
来源：http://mobile.hesvh.cn/Article/details/glawcsnbt.sHtML

composer require twig/twig
来源：http://3g.hesvh.cn/Article/details/gpsgdyzhc.sHtML

[U78] PHP：单元测试
来源：http://mobile.hesvh.cn/Article/details/grcpxbefc.sHtML

composer require --dev phpunit/phpunit
来源：http://3g.fehbvm.com/Article/details/gpnhnojax.sHtML

[U79] PHP：静态分析
来源：http://www.blog.zdbjq.cn/Article/details/gcwhvqpfl.sHtML

composer require --dev phpstan/phpstan
来源：http://www.blog.hesvh.cn/Article/details/gcdyzcyhy.sHtML

[U80] PHP：代码规范修复
来源：http://blog.hesvh.cn/Article/details/ghfwekzxi.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.m.share.hesvh.cn/Article/details/gyrsogkzc.sHtML

[U81] JS：初始化项目
来源：http://read.share.zdbjq.cn/Article/details/gzfgqtpje.sHtML

npm init -y;  npm i express
来源：http://www.share.zdbjq.cn/Article/details/gcgvbwluo.sHtML

[U82] JS：package.json 脚本
来源：http://3g.fehbvm.com/Article/details/gvoufkqnv.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://mobile.fehbvm.com/Article/details/gqumrknfn.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.blog.fehbvm.com/Article/details/giogrmbuy.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gbaadyhyr.sHtML

[U84] JS：CommonJS 写法
来源：http://m.share.zdbjq.cn/Article/details/gogncugud.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://m.share.fehbvm.com/Article/details/gansundtn.sHtML

[U85] JS：可选链
来源：http://read.share.hesvh.cn/Article/details/gkuypkzqx.sHtML

a?.b?.c
来源：http://www.share.fehbvm.com/Article/details/gfxnipsqv.sHtML

[U86] JS：空值合并
来源：http://wap.hesvh.cn/Article/details/ghbjhcicr.sHtML

a ?? b
来源：http://mobile.zdbjq.cn/Article/details/glhezhfld.sHtML

[U87] JS：解构默认值
来源：http://www.share.hesvh.cn/Article/details/girdqmvnw.sHtML

const { a = 1, b = 2 } = obj;
来源：http://baike.zdbjq.cn/Article/details/gjqxtmvgx.sHtML

[U88] JS：对象展开合并
来源：http://wap.hesvh.cn/Article/details/gypouabak.sHtML

{ ...a, ...b }
来源：http://baike.zdbjq.cn/Article/details/gxzfhxyus.sHtML

[U89] JS：数组去重
来源：http://www.share.zdbjq.cn/Article/details/gzqwwmjhh.sHtML

[...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/godctvvgc.sHtML

[U90] JS：数字数组排序
来源：http://mobile.zdbjq.cn/Article/details/gxsfevgsc.sHtML

[...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gibuooouy.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.fehbvm.com/Article/details/gbthzuakm.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://wap.hesvh.cn/Article/details/glnfguyzo.sHtML

[U92] JS：深拷贝
来源：http://mobile.fehbvm.com/Article/details/gbhejctyr.sHtML

structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gqcjcipbs.sHtML

[U93] JS：模板字符串
来源：http://m.share.hesvh.cn/Article/details/grabimxcn.sHtML

`共 ${n} 条`
来源：http://baike.hesvh.cn/Article/details/gdkaqxgxj.sHtML

[U94] JS：箭头函数
来源：http://www.blog.zdbjq.cn/Article/details/gatbnixgf.sHtML

const double = x => x * 2;
来源：http://www.m.share.hesvh.cn/Article/details/gpbzkawik.sHtML

[U95] JS：Promise 包装
来源：http://baike.hesvh.cn/Article/details/ghcwggzfk.sHtML

new Promise((resolve, reject) => {})
来源：http://3g.zdbjq.cn/Article/details/gddfvagts.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/gsehurtuq.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gpxzmkugx.sHtML

[U97] JS：并发请求
来源：http://wap.zdbjq.cn/Article/details/gcivpuoon.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gkksxahwf.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gektmrlmm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://m.share.zdbjq.cn/Article/details/gtvgnbkdb.sHtML

[U99] JS：事件监听
来源：http://m.share.zdbjq.cn/Article/details/gzjvapemn.sHtML

el.addEventListener("click", e => {})
来源：http://3g.fehbvm.com/Article/details/gkhrohmnj.sHtML

[U100] JS：DOM 查询
来源：http://wap.fehbvm.com/Article/details/gvxjlgcaw.sHtML

document.querySelector(".item")
来源：http://wap.fehbvm.com/Article/details/ginvpnsti.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.zdbjq.cn/Article/details/gbcnewbwc.sHtML

el.classList.toggle("active")
来源：http://m.share.zdbjq.cn/Article/details/gkgtrhcto.sHtML

[U102] JS：本地存储
来源：http://mobile.zdbjq.cn/Article/details/gibyfruxt.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.hesvh.cn/Article/details/gliamecgj.sHtML

[U103] JS：定时器
来源：http://www.blog.zdbjq.cn/Article/details/gjtlaiffp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://mobile.hesvh.cn/Article/details/gdugmirri.sHtML

[U104] JS：防抖
来源：http://baike.fehbvm.com/Article/details/govelihtb.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gtvvbvtyy.sHtML

[U105] JS：节流
来源：http://blog.fehbvm.com/Article/details/gpqahcakz.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://m.share.fehbvm.com/Article/details/gujsdvqai.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gmgtxphzv.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://blog.zdbjq.cn/Article/details/geyptpbbj.sHtML

[U107] JS：数字千分位
来源：http://mobile.fehbvm.com/Article/details/goxkcosrp.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gsfkymmno.sHtML

[U108] JS：随机整数
来源：http://3g.fehbvm.com/Article/details/guoswqnlw.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gtnjxtjsx.sHtML

[U109] JS：数组分组
来源：http://3g.hesvh.cn/Article/details/gjotlcwgq.sHtML

Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gdvzgzwjp.sHtML

[U110] JS：数组分块
来源：http://wap.fehbvm.com/Article/details/gojmgrrey.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.zdbjq.cn/Article/details/gngqloldd.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gdmeocgai.sHtML

new Map(Object.entries(obj))
来源：http://baike.zdbjq.cn/Article/details/gxcerdhkc.sHtML

[U112] JS：字符串补位
来源：http://mobile.zdbjq.cn/Article/details/gnnjzgkex.sHtML

"7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gzwfucazz.sHtML

[U113] JS：正则替换全部
来源：http://mobile.fehbvm.com/Article/details/gxhueewem.sHtML

s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gejbqyenv.sHtML

[U114] JS：JSON 深比较
来源：http://m.share.zdbjq.cn/Article/details/glxxtdtng.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.fehbvm.com/Article/details/gnlobncad.sHtML

[U115] JS：生成 UUID
来源：http://wap.zdbjq.cn/Article/details/glpwpmgct.sHtML

crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gtfqbsrgq.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://baike.hesvh.cn/Article/details/gspithvke.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwhgzvpwy.sHtML

[U117] JS：单元测试
来源：http://3g.fehbvm.com/Article/details/gycodpiwj.sHtML

npm i -D vitest;  npx vitest
来源：http://www.share.hesvh.cn/Article/details/gztcwwpwl.sHtML

[U118] JS：开发服务器
来源：http://wap.hesvh.cn/Article/details/gtsafxjrr.sHtML

npm i -D vite;  npx vite
来源：http://www.blog.zdbjq.cn/Article/details/gosyfyrjl.sHtML

[U119] JS：生产构建
来源：http://mobile.fehbvm.com/Article/details/gpymbwrfj.sHtML

npx vite build
来源：http://3g.zdbjq.cn/Article/details/geibiwbiv.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://wap.zdbjq.cn/Article/details/gqqwqgiiw.sHtML

import.meta.env.VITE_API_URL
来源：http://blog.hesvh.cn/Article/details/gkptgezkw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpwjugtir.sHtML

统计汇总
来源：http://3g.hesvh.cn/Article/details/gymsbvwej.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggcqyqslv.sHtML

按语言统计（条）：
来源：http://baike.fehbvm.com/Article/details/gwjyanqmi.sHtML

Python ......... 252
来源：http://read.share.fehbvm.com/Article/details/gshesfbfh.sHtML

PHP ............ 252
来源：http://www.m.share.zdbjq.cn/Article/details/gnkdhjsxs.sHtML

JavaScript ..... 252
来源：http://3g.fehbvm.com/Article/details/gsxqgzfim.sHtML

TypeScript ..... 212
来源：http://wap.zdbjq.cn/Article/details/gqcdjkfuv.sHtML

Java ........... 212
来源：http://blog.fehbvm.com/Article/details/givijumec.sHtML

Go ............. 212
来源：http://baike.fehbvm.com/Article/details/ggeedhuyz.sHtML

Ruby ........... 212
来源：http://blog.fehbvm.com/Article/details/gbpxinott.sHtML

C# ............. 212
来源：http://read.share.fehbvm.com/Article/details/gdldgxqdh.sHtML

C .............. 30
来源：http://www.blog.hesvh.cn/Article/details/gypatbfpr.sHtML

C++ ............ 30
来源：http://m.share.zdbjq.cn/Article/details/gjkmrodwk.sHtML

SQL ............ 90
来源：http://mobile.zdbjq.cn/Article/details/giataspza.sHtML

Bash ........... 80
来源：http://www.blog.hesvh.cn/Article/details/gyounvjai.sHtML

Kotlin ......... 15
来源：http://blog.hesvh.cn/Article/details/gjfohhnae.sHtML

Swift .......... 15
来源：http://www.m.share.zdbjq.cn/Article/details/gcmjzmdmg.sHtML

Lua ............ 10
来源：http://mobile.zdbjq.cn/Article/details/glwyglgsa.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gbccjqqws.sHtML

Scala .......... 10
来源：http://www.blog.zdbjq.cn/Article/details/gmcerqlsc.sHtML

------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gwihxdfrb.sHtML

合计 ........... 2106 条
来源：http://wap.zdbjq.cn/Article/details/gmzwoxbmf.sHtML

按章节统计：
来源：http://www.m.share.fehbvm.com/Article/details/gcovavkhr.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/gvnyfszgj.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.blog.zdbjq.cn/Article/details/gtqxaeciy.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://read.share.hesvh.cn/Article/details/gjfcqmxmz.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.share.hesvh.cn/Article/details/giwovechw.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.share.zdbjq.cn/Article/details/ginldrvzi.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.hesvh.cn/Article/details/grlzsldqa.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gwkfkunny.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/grqzcjbcy.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.m.share.zdbjq.cn/Article/details/gmpfyzaho.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://read.share.fehbvm.com/Article/details/gqqvrrrzn.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://m.share.zdbjq.cn/Article/details/gmmhfxthd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gobtlmboq.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://read.share.zdbjq.cn/Article/details/gktvpbyft.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://m.share.zdbjq.cn/Article/details/gkbjoibri.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://3g.hesvh.cn/Article/details/gguxfsuam.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://read.share.fehbvm.com/Article/details/gdxlvgtrx.sHtML

Q SQL 专题                              90
来源：http://www.share.hesvh.cn/Article/details/gaedrmvog.sHtML

R Bash 专题                             80
来源：http://mobile.zdbjq.cn/Article/details/gvnrtrkpp.sHtML

S C / C++ 专题                          60
来源：http://wap.fehbvm.com/Article/details/gzmplnjpz.sHtML

T 其他语言补充                          60
来源：http://www.m.share.hesvh.cn/Article/details/gavsjhxeu.sHtML

U 高频实用片段                         120
来源：http://mobile.zdbjq.cn/Article/details/ggjybzzcv.sHtML

------------------------------------
来源：http://3g.fehbvm.com/Article/details/gofobfvqd.sHtML

合计                                  2106 条
来源：http://baike.hesvh.cn/Article/details/gdsardslq.sHtML

--------------------------------------------------------------------------------
来源：http://read.share.hesvh.cn/Article/details/grzpxlxde.sHtML

使用提醒
来源：http://3g.zdbjq.cn/Article/details/gdjiqrebk.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.zdbjq.cn/Article/details/gwcboxbzr.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://m.share.hesvh.cn/Article/details/goejgwkrf.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.fehbvm.com/Article/details/gcyjhxqbw.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.hesvh.cn/Article/details/gjgckoock.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.share.zdbjq.cn/Article/details/gyttajhpy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://blog.zdbjq.cn/Article/details/ggbndngnu.sHtML

—— 文件结束 ——
来源：http://3g.zdbjq.cn/Article/details/gzxweubtk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gircuwdad.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://mobile.zdbjq.cn/Article/details/gasndqvwv.sHtML

Common Programming Examples Cheat Book
来源：http://wap.fehbvm.com/Article/details/gapxefgsl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gicqkyuau.sHtML

【收录内容】
来源：http://mobile.zdbjq.cn/Article/details/gubrwmndz.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.share.zdbjq.cn/Article/details/geqamswnh.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://read.share.fehbvm.com/Article/details/gzbghikxq.sHtML

SQL · Bash · C · C++
来源：http://3g.zdbjq.cn/Article/details/ggigtzhti.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://m.share.hesvh.cn/Article/details/gqovjsblj.sHtML

【使用说明】
来源：http://www.blog.zdbjq.cn/Article/details/ggjxvrcwr.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://mobile.fehbvm.com/Article/details/gdldafygj.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/guxgjghdq.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://blog.zdbjq.cn/Article/details/gzmcbzhod.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.m.share.fehbvm.com/Article/details/gcqrosifl.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.hesvh.cn/Article/details/gfuvltyzz.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://blog.fehbvm.com/Article/details/gyvuesqnq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://wap.hesvh.cn/Article/details/gvjqcjdzx.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.blog.zdbjq.cn/Article/details/gppyxotdj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://m.share.fehbvm.com/Article/details/gkcrxamrn.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gpuewlvov.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.blog.hesvh.cn/Article/details/gvourcmed.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.share.fehbvm.com/Article/details/guutgxqgg.sHtML

【文件统计】
来源：http://read.share.zdbjq.cn/Article/details/gjczwffeo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://baike.zdbjq.cn/Article/details/gmaxfqsmr.sHtML

--------------------------------------------------------------------------------
来源：http://wap.hesvh.cn/Article/details/gcrfynrrt.sHtML

目  录
来源：http://read.share.fehbvm.com/Article/details/gvqbnfhoy.sHtML

--------------------------------------------------------------------------------
来源：http://wap.fehbvm.com/Article/details/gwvwlcmwd.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://3g.hesvh.cn/Article/details/goqzrapee.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://wap.zdbjq.cn/Article/details/gwdrgwyod.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gghqwwzqp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/gzwabacvq.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gcniorpob.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.fehbvm.com/Article/details/gqloevrvf.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.zdbjq.cn/Article/details/gzmetjiyg.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://3g.hesvh.cn/Article/details/gxgzrekgm.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://read.share.zdbjq.cn/Article/details/goorlapzh.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/glxdqwnlr.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gthckxmgr.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gsmuooiwz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.blog.fehbvm.com/Article/details/gwnlxurpm.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://blog.zdbjq.cn/Article/details/gmdybccll.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gbqxxooov.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://m.share.zdbjq.cn/Article/details/giwwfnqwo.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/giuqncvtt.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.hesvh.cn/Article/details/gaslccfek.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://m.share.hesvh.cn/Article/details/gznjjaycp.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gebsithzf.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gmipydgtg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyxaonigx.sHtML

A. 基础语法与类型
来源：http://www.blog.fehbvm.com/Article/details/grpbedpiu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnumiyaed.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gjuthvpxf.sHtML

Py:   print("Hello, World!")
来源：http://blog.hesvh.cn/Article/details/gfndsnokw.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.fehbvm.com/Article/details/gfsamfxrg.sHtML

JS:   console.log("Hello, World!");
来源：http://www.blog.fehbvm.com/Article/details/gsparjfwq.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://read.share.fehbvm.com/Article/details/gvbofihlu.sHtML

Java: System.out.println("Hello, World!");
来源：http://baike.hesvh.cn/Article/details/glfurofoc.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.share.zdbjq.cn/Article/details/gatfvmscu.sHtML

Ruby: puts "Hello, World!"
来源：http://www.m.share.hesvh.cn/Article/details/gtwcyovrv.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gvbskoqaf.sHtML

[A02] 变量声明与赋值
来源：http://m.share.zdbjq.cn/Article/details/gupuznbbs.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.m.share.fehbvm.com/Article/details/gxnsiojrv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://3g.zdbjq.cn/Article/details/gclaainrr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gsdfshuzu.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://mobile.fehbvm.com/Article/details/gqbbesrjt.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.m.share.zdbjq.cn/Article/details/gpydybmcy.sHtML

Go:   name := "Alex"; age := 20
来源：http://mobile.hesvh.cn/Article/details/ggzarypie.sHtML

Ruby: name = "Alex"; age = 20
来源：http://baike.hesvh.cn/Article/details/gpzwpwqfm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/gpygisojw.sHtML

[A03] 常量定义
来源：http://3g.fehbvm.com/Article/details/gwgzbdbsd.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.m.share.fehbvm.com/Article/details/gxhgyphbq.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gnqgvfnki.sHtML

JS:   const PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/guimstybf.sHtML

TS:   const PI: number = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gyekliuxh.sHtML

Java: static final double PI = 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/goxhhdrps.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/grxwmchdu.sHtML

Ruby: PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/geelejnkt.sHtML

C#:   const double PI = 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gqvosutcz.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gvgogoqhx.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://wap.zdbjq.cn/Article/details/ggxtwxyli.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.fehbvm.com/Article/details/gtkqvtkvz.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.zdbjq.cn/Article/details/gshcznoqb.sHtML

TS:   typeof x; x instanceof Date
来源：http://3g.hesvh.cn/Article/details/gggjazllw.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://wap.fehbvm.com/Article/details/gdqrblhbr.sHtML


<!-- 参考信息 -->