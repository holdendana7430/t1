代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gdwcfxhgz.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gzbiljnri.sHtML

[U46] PHP：可空类型
来源：http://baike.hesvh.cn/Article/details/ghhvtyiuq.sHtML

?string $name = null
来源：http://www.share.zdbjq.cn/Article/details/gzbfwiirx.sHtML

[U47] PHP：联合类型
来源：http://www.m.share.fehbvm.com/Article/details/ggqrzosyt.sHtML

int|string $id
来源：http://www.m.share.hesvh.cn/Article/details/ggxnbxibp.sHtML

[U48] PHP：纯枚举
来源：http://read.share.zdbjq.cn/Article/details/gqgohqnoq.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsmsftant.sHtML

[U49] PHP：只读属性
来源：http://blog.zdbjq.cn/Article/details/gtruyqwez.sHtML

public readonly string $name
来源：http://3g.hesvh.cn/Article/details/gxxyjgihn.sHtML

[U50] PHP：构造器属性提升
来源：http://mobile.zdbjq.cn/Article/details/gzixtdhig.sHtML

public function __construct(private int $id) {}
来源：http://www.share.hesvh.cn/Article/details/gnoevtvsx.sHtML

[U51] PHP：数组解构
来源：http://baike.hesvh.cn/Article/details/gniaociwr.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gguhdjtxo.sHtML

[U52] PHP：箭头函数
来源：http://mobile.fehbvm.com/Article/details/gblabxvvj.sHtML

$double = fn($x) => $x * 2;
来源：http://3g.hesvh.cn/Article/details/goubtqqfs.sHtML

[U53] PHP：空合并运算符
来源：http://read.share.fehbvm.com/Article/details/gtbpfisqo.sHtML

$v = $a ?? $b ?? "default";
来源：http://blog.zdbjq.cn/Article/details/gsmybakua.sHtML

[U54] PHP：空安全调用
来源：http://mobile.hesvh.cn/Article/details/ggublvclm.sHtML

$obj?->method()
来源：http://m.share.fehbvm.com/Article/details/ggluewvxg.sHtML

[U55] PHP：match 表达式
来源：http://mobile.zdbjq.cn/Article/details/gcjmntfjd.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gmjsvsgly.sHtML

[U56] PHP：命名参数
来源：http://baike.zdbjq.cn/Article/details/glnjnheoh.sHtML

f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gobauondg.sHtML

[U57] PHP：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/glqvsxwnr.sHtML

"值: {$a}"
来源：http://baike.fehbvm.com/Article/details/gxdemmxys.sHtML

[U58] PHP：数组三件套
来源：http://www.blog.fehbvm.com/Article/details/gfghcjpua.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://baike.fehbvm.com/Article/details/gpbpjzwpg.sHtML

[U59] PHP：自定义排序
来源：http://wap.zdbjq.cn/Article/details/gnfchihoj.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/goweltuek.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.zdbjq.cn/Article/details/gevlahurz.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://3g.zdbjq.cn/Article/details/gdwjebwdy.sHtML

[U61] PHP：正则
来源：http://wap.zdbjq.cn/Article/details/gpwefdaaj.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/glyycobiw.sHtML

[U62] PHP：日期对象
来源：http://blog.hesvh.cn/Article/details/ggkqzxcla.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://baike.hesvh.cn/Article/details/gozzvmmgf.sHtML

[U63] PHP：文件读写
来源：http://www.blog.fehbvm.com/Article/details/gztzsgiac.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://mobile.zdbjq.cn/Article/details/gwwrrrzzn.sHtML

[U64] PHP：目录遍历
来源：http://m.share.zdbjq.cn/Article/details/gcunydyvl.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://www.m.share.hesvh.cn/Article/details/gslbpqyff.sHtML

[U65] PHP：会话
来源：http://www.share.fehbvm.com/Article/details/glqdlfrrl.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://m.share.hesvh.cn/Article/details/ghuagcojs.sHtML

[U66] PHP：设置 Cookie
来源：http://wap.hesvh.cn/Article/details/guwjumcja.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://mobile.fehbvm.com/Article/details/gdyvpynik.sHtML

[U67] PHP：处理文件上传
来源：http://m.share.fehbvm.com/Article/details/gsrdxjdhj.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://baike.hesvh.cn/Article/details/gyzmctutp.sHtML

[U68] PHP：PDO 连接
来源：http://www.share.zdbjq.cn/Article/details/gnxgzteem.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.share.zdbjq.cn/Article/details/glmastikz.sHtML

[U69] PHP：PDO 预处理
来源：http://mobile.zdbjq.cn/Article/details/gizyisclk.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://wap.hesvh.cn/Article/details/glxgwkvba.sHtML

[U70] PHP：PDO 事务
来源：http://m.share.fehbvm.com/Article/details/gnuojprme.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/ghbtdcjpu.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.fehbvm.com/Article/details/glpikcjid.sHtML

throw new RuntimeException("失败", 500);
来源：http://mobile.fehbvm.com/Article/details/gnolcjbgl.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gddoqwums.sHtML

error_log("失败: " . $e->getMessage());
来源：http://m.share.fehbvm.com/Article/details/gcosajyvf.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.zdbjq.cn/Article/details/gdnuuvuzt.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gxweljyww.sHtML

[U74] PHP：读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gtkprtjfn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://read.share.hesvh.cn/Article/details/gmkrgsowh.sHtML

[U75] PHP：依赖注入
来源：http://www.blog.fehbvm.com/Article/details/ghatuvzxh.sHtML

composer require psr/container
来源：http://wap.hesvh.cn/Article/details/gfltxfmuj.sHtML

[U76] PHP：简单路由
来源：http://m.share.hesvh.cn/Article/details/gzweufvil.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.fehbvm.com/Article/details/giefssvgm.sHtML

[U77] PHP：模板渲染
来源：http://3g.fehbvm.com/Article/details/gwquobury.sHtML

composer require twig/twig
来源：http://m.share.hesvh.cn/Article/details/gratccvnn.sHtML

[U78] PHP：单元测试
来源：http://read.share.hesvh.cn/Article/details/gqyibolac.sHtML

composer require --dev phpunit/phpunit
来源：http://www.share.fehbvm.com/Article/details/gitlsgpzc.sHtML

[U79] PHP：静态分析
来源：http://www.share.zdbjq.cn/Article/details/ggzatypej.sHtML

composer require --dev phpstan/phpstan
来源：http://blog.hesvh.cn/Article/details/gtmrfdpnp.sHtML

[U80] PHP：代码规范修复
来源：http://blog.fehbvm.com/Article/details/gmabtiplb.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://m.share.zdbjq.cn/Article/details/gbfyptago.sHtML

[U81] JS：初始化项目
来源：http://baike.hesvh.cn/Article/details/gulhpmdjv.sHtML

npm init -y;  npm i express
来源：http://www.blog.fehbvm.com/Article/details/gdewkcnmi.sHtML

[U82] JS：package.json 脚本
来源：http://wap.hesvh.cn/Article/details/graoxings.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.zdbjq.cn/Article/details/gzwpqsksw.sHtML

[U83] JS：ES Module 导入导出
来源：http://read.share.hesvh.cn/Article/details/gxifuyezg.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gyufkomxb.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gqqzifwtp.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.zdbjq.cn/Article/details/gknfsyksh.sHtML

[U85] JS：可选链
来源：http://wap.zdbjq.cn/Article/details/gudqgauko.sHtML

a?.b?.c
来源：http://blog.hesvh.cn/Article/details/ggnvuywzl.sHtML

[U86] JS：空值合并
来源：http://wap.zdbjq.cn/Article/details/gxpzdicvz.sHtML

a ?? b
来源：http://blog.fehbvm.com/Article/details/gqwshqbea.sHtML

[U87] JS：解构默认值
来源：http://3g.zdbjq.cn/Article/details/gpepcajkv.sHtML

const { a = 1, b = 2 } = obj;
来源：http://blog.hesvh.cn/Article/details/glrzischf.sHtML

[U88] JS：对象展开合并
来源：http://www.m.share.fehbvm.com/Article/details/grofbodkg.sHtML

{ ...a, ...b }
来源：http://3g.zdbjq.cn/Article/details/gbehqkuai.sHtML

[U89] JS：数组去重
来源：http://m.share.zdbjq.cn/Article/details/gaqcipimx.sHtML

[...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gmujbtkpy.sHtML

[U90] JS：数字数组排序
来源：http://blog.hesvh.cn/Article/details/gkbsovqik.sHtML

[...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/geqwsvgaf.sHtML

[U91] JS：对象键值遍历
来源：http://www.blog.hesvh.cn/Article/details/gqfetmzho.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/gidcwfnnk.sHtML

[U92] JS：深拷贝
来源：http://wap.hesvh.cn/Article/details/gtokszrqm.sHtML

structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gkbhskolv.sHtML

[U93] JS：模板字符串
来源：http://mobile.hesvh.cn/Article/details/gdykpuedb.sHtML

`共 ${n} 条`
来源：http://www.m.share.zdbjq.cn/Article/details/gexcruxwy.sHtML

[U94] JS：箭头函数
来源：http://www.m.share.hesvh.cn/Article/details/gkdnoiddn.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gaxjakoej.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/ggfywxkwo.sHtML

new Promise((resolve, reject) => {})
来源：http://m.share.zdbjq.cn/Article/details/gqqeuuwwb.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.fehbvm.com/Article/details/guefshkra.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gabgzhynz.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gotsumkax.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gaayvjtvt.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gcimqiikh.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.fehbvm.com/Article/details/gctqknsfn.sHtML

[U99] JS：事件监听
来源：http://blog.hesvh.cn/Article/details/ggfrcblqk.sHtML

el.addEventListener("click", e => {})
来源：http://www.blog.fehbvm.com/Article/details/gbhbemzdr.sHtML

[U100] JS：DOM 查询
来源：http://www.blog.zdbjq.cn/Article/details/gjeipbaew.sHtML

document.querySelector(".item")
来源：http://www.m.share.hesvh.cn/Article/details/gisfuldfk.sHtML

[U101] JS：classList 操作
来源：http://www.m.share.fehbvm.com/Article/details/gdwufqzpg.sHtML

el.classList.toggle("active")
来源：http://read.share.zdbjq.cn/Article/details/gnqwtfuxd.sHtML

[U102] JS：本地存储
来源：http://m.share.zdbjq.cn/Article/details/gynwbxwtu.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gnkhlrcgr.sHtML

[U103] JS：定时器
来源：http://www.share.zdbjq.cn/Article/details/gxnpdkllh.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.m.share.fehbvm.com/Article/details/grkmicwul.sHtML

[U104] JS：防抖
来源：http://blog.fehbvm.com/Article/details/gzsxbxmtk.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/ghywaflzu.sHtML

[U105] JS：节流
来源：http://blog.zdbjq.cn/Article/details/gfuuygjuv.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://baike.zdbjq.cn/Article/details/gfiwhaqha.sHtML

[U106] JS：日期格式化
来源：http://baike.zdbjq.cn/Article/details/guqwtbusu.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://mobile.fehbvm.com/Article/details/grhkdjvuu.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gqnqukjir.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://wap.hesvh.cn/Article/details/gsvjxaqxc.sHtML

[U108] JS：随机整数
来源：http://mobile.fehbvm.com/Article/details/gqrlbebvb.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.m.share.hesvh.cn/Article/details/gfmiayjxy.sHtML

[U109] JS：数组分组
来源：http://blog.hesvh.cn/Article/details/gvncwnkqg.sHtML

Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gmrsdqxay.sHtML

[U110] JS：数组分块
来源：http://mobile.hesvh.cn/Article/details/gzcuqdsgg.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://baike.fehbvm.com/Article/details/gurphjjvi.sHtML

[U111] JS：对象转 Map
来源：http://wap.zdbjq.cn/Article/details/ggyicuiox.sHtML

new Map(Object.entries(obj))
来源：http://read.share.fehbvm.com/Article/details/gsdqdfurs.sHtML

[U112] JS：字符串补位
来源：http://mobile.hesvh.cn/Article/details/gptbkxzqs.sHtML

"7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gldeqodsw.sHtML

[U113] JS：正则替换全部
来源：http://3g.zdbjq.cn/Article/details/gpfekpvcw.sHtML

s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gjkklyape.sHtML

[U114] JS：JSON 深比较
来源：http://read.share.zdbjq.cn/Article/details/gppkyqkbp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gmuwezjmx.sHtML

[U115] JS：生成 UUID
来源：http://www.m.share.hesvh.cn/Article/details/gunruvmxv.sHtML

crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gckjuultb.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://wap.fehbvm.com/Article/details/grcjqouwl.sHtML

/** @param {string} name */ function f(name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnefqllmf.sHtML

[U117] JS：单元测试
来源：http://www.blog.zdbjq.cn/Article/details/gmrlcxidj.sHtML

npm i -D vitest;  npx vitest
来源：http://m.share.fehbvm.com/Article/details/grsjhbatz.sHtML

[U118] JS：开发服务器
来源：http://www.share.fehbvm.com/Article/details/gzyastwai.sHtML

npm i -D vite;  npx vite
来源：http://baike.fehbvm.com/Article/details/gxmtvzphu.sHtML

[U119] JS：生产构建
来源：http://m.share.hesvh.cn/Article/details/gdubzbmwh.sHtML

npx vite build
来源：http://baike.fehbvm.com/Article/details/glvtnqjkw.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://blog.zdbjq.cn/Article/details/goqylfovq.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gtdgsjtcr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxfrmdsdw.sHtML

统计汇总
来源：http://www.m.share.zdbjq.cn/Article/details/gvvsknoxk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqrtmzcvl.sHtML

按语言统计（条）：
来源：http://www.m.share.zdbjq.cn/Article/details/glniqtfps.sHtML

Python ......... 252
来源：http://www.share.hesvh.cn/Article/details/gdeipeoav.sHtML

PHP ............ 252
来源：http://mobile.hesvh.cn/Article/details/gqptolqvj.sHtML

JavaScript ..... 252
来源：http://3g.hesvh.cn/Article/details/gczdbavdj.sHtML

TypeScript ..... 212
来源：http://www.share.hesvh.cn/Article/details/gyyszfgtr.sHtML

Java ........... 212
来源：http://mobile.zdbjq.cn/Article/details/grwimyzqe.sHtML

Go ............. 212
来源：http://read.share.zdbjq.cn/Article/details/geirmeinz.sHtML

Ruby ........... 212
来源：http://baike.fehbvm.com/Article/details/gslkoxhfx.sHtML

C# ............. 212
来源：http://mobile.hesvh.cn/Article/details/gpxkomegd.sHtML

C .............. 30
来源：http://read.share.hesvh.cn/Article/details/gmnxauqdm.sHtML

C++ ............ 30
来源：http://baike.hesvh.cn/Article/details/gqouygugy.sHtML

SQL ............ 90
来源：http://blog.fehbvm.com/Article/details/ghuikvrqn.sHtML

Bash ........... 80
来源：http://m.share.hesvh.cn/Article/details/ggtehlmli.sHtML

Kotlin ......... 15
来源：http://www.share.hesvh.cn/Article/details/gohwflodr.sHtML

Swift .......... 15
来源：http://3g.hesvh.cn/Article/details/gbjulntta.sHtML

Lua ............ 10
来源：http://baike.hesvh.cn/Article/details/gcciwirpb.sHtML

Perl ........... 10
来源：http://3g.fehbvm.com/Article/details/gjdoaqzpx.sHtML

Scala .......... 10
来源：http://blog.fehbvm.com/Article/details/gpkpqalqi.sHtML

------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gjxogmnbc.sHtML

合计 ........... 2106 条
来源：http://read.share.hesvh.cn/Article/details/gqssxspxs.sHtML

按章节统计：
来源：http://baike.zdbjq.cn/Article/details/gpxhjkids.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.hesvh.cn/Article/details/ghdhmywsu.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://baike.zdbjq.cn/Article/details/gvyquyhua.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://wap.zdbjq.cn/Article/details/gcvrgggyw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://mobile.fehbvm.com/Article/details/galeotzxb.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.fehbvm.com/Article/details/gozvcohcj.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://wap.zdbjq.cn/Article/details/gbrwmzszi.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://wap.hesvh.cn/Article/details/gmlasmpxq.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.blog.fehbvm.com/Article/details/gvicpikhf.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://3g.hesvh.cn/Article/details/gdevcvyrl.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://3g.fehbvm.com/Article/details/gfkmsrwni.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.share.fehbvm.com/Article/details/gyoknwirq.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/ghxodughz.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gxgpesaex.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.zdbjq.cn/Article/details/gswzkyaah.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://wap.hesvh.cn/Article/details/gniqryvpz.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.fehbvm.com/Article/details/gqofmxwtj.sHtML

Q SQL 专题                              90
来源：http://baike.fehbvm.com/Article/details/gbiwvyegn.sHtML

R Bash 专题                             80
来源：http://baike.fehbvm.com/Article/details/gmyihycly.sHtML

S C / C++ 专题                          60
来源：http://3g.hesvh.cn/Article/details/gzzpklmqq.sHtML

T 其他语言补充                          60
来源：http://www.m.share.zdbjq.cn/Article/details/gjjdvuecf.sHtML

U 高频实用片段                         120
来源：http://blog.hesvh.cn/Article/details/gpxdcutlb.sHtML

------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gcygvxnab.sHtML

合计                                  2106 条
来源：http://read.share.hesvh.cn/Article/details/gscuemdrx.sHtML

--------------------------------------------------------------------------------
来源：http://3g.fehbvm.com/Article/details/gentiyvnf.sHtML

使用提醒
来源：http://3g.hesvh.cn/Article/details/gmrrthcti.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/gpuvxdiny.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://blog.fehbvm.com/Article/details/gmikphhkr.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://wap.fehbvm.com/Article/details/gppshbykd.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://read.share.fehbvm.com/Article/details/gijcprsnp.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://baike.zdbjq.cn/Article/details/gkansybvi.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.hesvh.cn/Article/details/goqfjeyxy.sHtML

—— 文件结束 ——
来源：http://m.share.fehbvm.com/Article/details/gvsfjhlfe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfgfuoslb.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://read.share.fehbvm.com/Article/details/ghmnlsvkx.sHtML

Common Programming Examples Cheat Book
来源：http://www.share.fehbvm.com/Article/details/gltmturxj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxxemgpho.sHtML

【收录内容】
来源：http://www.share.zdbjq.cn/Article/details/gryodeibv.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.blog.fehbvm.com/Article/details/gionclrmx.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://baike.hesvh.cn/Article/details/giplzcviq.sHtML

SQL · Bash · C · C++
来源：http://mobile.hesvh.cn/Article/details/gsunlwkrk.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://blog.fehbvm.com/Article/details/gslljqsra.sHtML

【使用说明】
来源：http://baike.hesvh.cn/Article/details/gzkuepgsn.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://wap.hesvh.cn/Article/details/glytgqfqz.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.share.zdbjq.cn/Article/details/gbwmizfsi.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://3g.hesvh.cn/Article/details/gnuxchpdv.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://mobile.fehbvm.com/Article/details/geyjfldqw.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.m.share.fehbvm.com/Article/details/genqobtxv.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://read.share.hesvh.cn/Article/details/gjyajxaww.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://mobile.zdbjq.cn/Article/details/gzigrccta.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://mobile.zdbjq.cn/Article/details/ggbygvnnn.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://3g.zdbjq.cn/Article/details/gjaannsbc.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://mobile.fehbvm.com/Article/details/gxdjemzai.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://blog.hesvh.cn/Article/details/gyaaddmtc.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://blog.fehbvm.com/Article/details/gsbpqlarp.sHtML

【文件统计】
来源：http://m.share.zdbjq.cn/Article/details/ghhmtfnot.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://blog.hesvh.cn/Article/details/gwonocnsc.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/giahkrrzv.sHtML

目  录
来源：http://3g.zdbjq.cn/Article/details/gmiwmgkut.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.hesvh.cn/Article/details/grnzhytmc.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.blog.zdbjq.cn/Article/details/gsfxuscjj.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/gukohgxpw.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://blog.zdbjq.cn/Article/details/gneoreaba.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://baike.hesvh.cn/Article/details/ggidqxczb.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gxomnmdgn.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://baike.zdbjq.cn/Article/details/gifouqnln.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://read.share.zdbjq.cn/Article/details/gfazymazs.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.fehbvm.com/Article/details/gbjcuezzk.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gzfqzedai.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://read.share.fehbvm.com/Article/details/gjtuiqqqh.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/giazriuol.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://wap.zdbjq.cn/Article/details/gdrsclkfz.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/girtrtrce.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gleymywqg.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://m.share.zdbjq.cn/Article/details/grzrbfwbd.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gptveizas.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.hesvh.cn/Article/details/gfeodqkqf.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://blog.zdbjq.cn/Article/details/grkforfli.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://baike.hesvh.cn/Article/details/gykezljzi.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gspukfuas.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://wap.fehbvm.com/Article/details/gwghgecoy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcuiyfzfz.sHtML

A. 基础语法与类型
来源：http://baike.fehbvm.com/Article/details/glkdjajki.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxcylgyil.sHtML

[A01] Hello World
来源：http://read.share.zdbjq.cn/Article/details/gdaevakdd.sHtML

Py:   print("Hello, World!")
来源：http://read.share.zdbjq.cn/Article/details/gtgcmktil.sHtML

PHP:  echo "Hello, World!";
来源：http://wap.zdbjq.cn/Article/details/gvklvehjy.sHtML

JS:   console.log("Hello, World!");
来源：http://baike.zdbjq.cn/Article/details/gjtpgcnra.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.blog.fehbvm.com/Article/details/gwfdjjbbb.sHtML

Java: System.out.println("Hello, World!");
来源：http://3g.fehbvm.com/Article/details/gwrqbxvic.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://m.share.zdbjq.cn/Article/details/gqavuhwrn.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gjfrpbpjq.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://baike.fehbvm.com/Article/details/gpqxteprp.sHtML

[A02] 变量声明与赋值
来源：http://www.share.fehbvm.com/Article/details/gekqqekra.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://wap.zdbjq.cn/Article/details/gnsvwdyhd.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://m.share.hesvh.cn/Article/details/gxvhsnzpz.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://baike.hesvh.cn/Article/details/gjuczguaf.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://blog.zdbjq.cn/Article/details/gjstdufuh.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.blog.zdbjq.cn/Article/details/gmmcafdzz.sHtML

Go:   name := "Alex"; age := 20
来源：http://3g.hesvh.cn/Article/details/gvlluonwb.sHtML

Ruby: name = "Alex"; age = 20
来源：http://wap.hesvh.cn/Article/details/gfipbfytm.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.fehbvm.com/Article/details/gmrxjmeor.sHtML

[A03] 常量定义
来源：http://baike.zdbjq.cn/Article/details/gspeqdmrn.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://mobile.fehbvm.com/Article/details/gvswpcpks.sHtML

PHP:  const PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/ggybqgdji.sHtML

JS:   const PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/greeskvfp.sHtML

TS:   const PI: number = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gevabimtb.sHtML

Java: static final double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gvmjtlwoa.sHtML

Go:   const PI = 3.14159
来源：http://read.share.zdbjq.cn/Article/details/gyxolwwam.sHtML

Ruby: PI = 3.14159
来源：http://m.share.fehbvm.com/Article/details/gqgtttyjl.sHtML

C#:   const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/giibhutok.sHtML

[A04] 判断变量类型
来源：http://baike.fehbvm.com/Article/details/gegnfaycd.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.fehbvm.com/Article/details/gyxzbngrq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.fehbvm.com/Article/details/gqtpxhvsu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gvackatns.sHtML

TS:   typeof x; x instanceof Date
来源：http://www.m.share.fehbvm.com/Article/details/gloruoxjy.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://read.share.fehbvm.com/Article/details/geybtzyxi.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://read.share.zdbjq.cn/Article/details/gqvulxetb.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://m.share.zdbjq.cn/Article/details/gwezbqdzg.sHtML

C#:   x.GetType().Name; x is int
来源：http://read.share.fehbvm.com/Article/details/ghkcdujxz.sHtML

[A05] 整数除法与取模
来源：http://www.share.fehbvm.com/Article/details/givdkokgt.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.zdbjq.cn/Article/details/ggldzcxvo.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.fehbvm.com/Article/details/gfpmmthtd.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/ghlilhskf.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gpuvyvdlc.sHtML


<!-- 参考信息 -->