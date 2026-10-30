代发 wailian999

[U45] PHP：类型声明与返回类型
来源：http://read.share.fehbvm.com/Article/details/gkemqhaso.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gxgjgtdwc.sHtML

[U46] PHP：可空类型
来源：http://3g.hesvh.cn/Article/details/gymbcievm.sHtML

?string $name = null
来源：http://wap.hesvh.cn/Article/details/gaiugoxnx.sHtML

[U47] PHP：联合类型
来源：http://wap.hesvh.cn/Article/details/guadipscj.sHtML

int|string $id
来源：http://mobile.zdbjq.cn/Article/details/geytfpkbg.sHtML

[U48] PHP：纯枚举
来源：http://www.share.fehbvm.com/Article/details/gmhfaozbj.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://baike.zdbjq.cn/Article/details/glkquwzqw.sHtML

[U49] PHP：只读属性
来源：http://blog.hesvh.cn/Article/details/gcvnefllp.sHtML

public readonly string $name
来源：http://blog.fehbvm.com/Article/details/ggrxwmwar.sHtML

[U50] PHP：构造器属性提升
来源：http://3g.hesvh.cn/Article/details/gmfiyrkiy.sHtML

public function __construct(private int $id) {}
来源：http://read.share.hesvh.cn/Article/details/gkgblrfox.sHtML

[U51] PHP：数组解构
来源：http://baike.zdbjq.cn/Article/details/gyelzdyav.sHtML

[$a, $b] = $arr;
来源：http://blog.zdbjq.cn/Article/details/gvufaoteb.sHtML

[U52] PHP：箭头函数
来源：http://read.share.fehbvm.com/Article/details/gmintoabg.sHtML

$double = fn($x) => $x * 2;
来源：http://baike.zdbjq.cn/Article/details/gbjnmzvns.sHtML

[U53] PHP：空合并运算符
来源：http://3g.zdbjq.cn/Article/details/gepigcksb.sHtML

$v = $a ?? $b ?? "default";
来源：http://3g.fehbvm.com/Article/details/ggnyrjidx.sHtML

[U54] PHP：空安全调用
来源：http://wap.fehbvm.com/Article/details/gupxbxqty.sHtML

$obj?->method()
来源：http://www.blog.fehbvm.com/Article/details/gabijcfdm.sHtML

[U55] PHP：match 表达式
来源：http://m.share.zdbjq.cn/Article/details/gvalipsti.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gcixejktz.sHtML

[U56] PHP：命名参数
来源：http://wap.zdbjq.cn/Article/details/goauiohus.sHtML

f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gtxqjkxib.sHtML

[U57] PHP：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/grkwlasmq.sHtML

"值: {$a}"
来源：http://www.m.share.zdbjq.cn/Article/details/girklgfkq.sHtML

[U58] PHP：数组三件套
来源：http://read.share.hesvh.cn/Article/details/gtuklofui.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://wap.fehbvm.com/Article/details/gpvxkcqjw.sHtML

[U59] PHP：自定义排序
来源：http://baike.hesvh.cn/Article/details/gcbjxptil.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/garaakgma.sHtML

[U60] PHP：JSON 编解码
来源：http://blog.hesvh.cn/Article/details/gkcymctzj.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.hesvh.cn/Article/details/gwqajibem.sHtML

[U61] PHP：正则
来源：http://3g.fehbvm.com/Article/details/ggylgifog.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gejwoovnj.sHtML

[U62] PHP：日期对象
来源：http://m.share.zdbjq.cn/Article/details/gypczjqme.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.share.zdbjq.cn/Article/details/gaupdjgnr.sHtML

[U63] PHP：文件读写
来源：http://blog.fehbvm.com/Article/details/glzgkxbbq.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.blog.fehbvm.com/Article/details/gdvgxbdra.sHtML

[U64] PHP：目录遍历
来源：http://www.blog.zdbjq.cn/Article/details/gllsuodlr.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://baike.fehbvm.com/Article/details/gewnkempe.sHtML

[U65] PHP：会话
来源：http://baike.zdbjq.cn/Article/details/gofnbdqvp.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gydnylron.sHtML

[U66] PHP：设置 Cookie
来源：http://www.blog.zdbjq.cn/Article/details/gsgzkbjvm.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://3g.hesvh.cn/Article/details/gjqpgswmg.sHtML

[U67] PHP：处理文件上传
来源：http://wap.fehbvm.com/Article/details/goapypcde.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://3g.fehbvm.com/Article/details/gxgaawzja.sHtML

[U68] PHP：PDO 连接
来源：http://www.blog.fehbvm.com/Article/details/getaiizfu.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://3g.zdbjq.cn/Article/details/gvbnjwlpm.sHtML

[U69] PHP：PDO 预处理
来源：http://3g.zdbjq.cn/Article/details/gvggtrllp.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://m.share.hesvh.cn/Article/details/giahddmas.sHtML

[U70] PHP：PDO 事务
来源：http://3g.zdbjq.cn/Article/details/goxshprrj.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.share.zdbjq.cn/Article/details/gkkcyyfqv.sHtML

[U71] PHP：抛出异常
来源：http://m.share.hesvh.cn/Article/details/glztcogbh.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.blog.hesvh.cn/Article/details/gnusztwkj.sHtML

[U72] PHP：写错误日志
来源：http://wap.hesvh.cn/Article/details/gllbcuwxi.sHtML

error_log("失败: " . $e->getMessage());
来源：http://blog.fehbvm.com/Article/details/gpdiniqsm.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/grqnblnmx.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.hesvh.cn/Article/details/gbpezufge.sHtML

[U74] PHP：读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gxbnjotgn.sHtML

getenv("APP_ENV") ?: "production"
来源：http://www.share.hesvh.cn/Article/details/gihcqbgic.sHtML

[U75] PHP：依赖注入
来源：http://m.share.fehbvm.com/Article/details/gmbeflnrr.sHtML

composer require psr/container
来源：http://www.blog.fehbvm.com/Article/details/gbmiusisx.sHtML

[U76] PHP：简单路由
来源：http://www.share.hesvh.cn/Article/details/gcaaoeris.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.zdbjq.cn/Article/details/gzahbjflj.sHtML

[U77] PHP：模板渲染
来源：http://www.blog.hesvh.cn/Article/details/gmzbwweba.sHtML

composer require twig/twig
来源：http://baike.zdbjq.cn/Article/details/gtvgaqifr.sHtML

[U78] PHP：单元测试
来源：http://m.share.fehbvm.com/Article/details/glszivujs.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/gabtyplcl.sHtML

[U79] PHP：静态分析
来源：http://3g.zdbjq.cn/Article/details/gukuelumy.sHtML

composer require --dev phpstan/phpstan
来源：http://www.share.hesvh.cn/Article/details/gdbiavjow.sHtML

[U80] PHP：代码规范修复
来源：http://www.share.hesvh.cn/Article/details/greruesvk.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.share.hesvh.cn/Article/details/gpkujgnus.sHtML

[U81] JS：初始化项目
来源：http://blog.fehbvm.com/Article/details/gztyzulte.sHtML

npm init -y;  npm i express
来源：http://mobile.fehbvm.com/Article/details/gnycdindz.sHtML

[U82] JS：package.json 脚本
来源：http://read.share.fehbvm.com/Article/details/gdjpbwawz.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://read.share.fehbvm.com/Article/details/giqfrroeg.sHtML

[U83] JS：ES Module 导入导出
来源：http://www.m.share.hesvh.cn/Article/details/giehsfxno.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gsqldragi.sHtML

[U84] JS：CommonJS 写法
来源：http://wap.zdbjq.cn/Article/details/gispyhgbh.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://mobile.fehbvm.com/Article/details/gecixgqoj.sHtML

[U85] JS：可选链
来源：http://www.m.share.hesvh.cn/Article/details/gwtlowxdf.sHtML

a?.b?.c
来源：http://3g.zdbjq.cn/Article/details/gbursivwl.sHtML

[U86] JS：空值合并
来源：http://www.blog.hesvh.cn/Article/details/gzayasjwq.sHtML

a ?? b
来源：http://wap.fehbvm.com/Article/details/gsruyomww.sHtML

[U87] JS：解构默认值
来源：http://3g.hesvh.cn/Article/details/gahczxwcd.sHtML

const { a = 1, b = 2 } = obj;
来源：http://wap.zdbjq.cn/Article/details/geexmojzj.sHtML

[U88] JS：对象展开合并
来源：http://www.share.fehbvm.com/Article/details/gqrubmplc.sHtML

{ ...a, ...b }
来源：http://www.m.share.zdbjq.cn/Article/details/gtwanvgvk.sHtML

[U89] JS：数组去重
来源：http://3g.zdbjq.cn/Article/details/glmfbfqgp.sHtML

[...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gwjpmfhlz.sHtML

[U90] JS：数字数组排序
来源：http://m.share.fehbvm.com/Article/details/gyzprrksr.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gnbokmotd.sHtML

[U91] JS：对象键值遍历
来源：http://www.share.zdbjq.cn/Article/details/gkvtfrluk.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://baike.zdbjq.cn/Article/details/gsqsxvcnk.sHtML

[U92] JS：深拷贝
来源：http://baike.hesvh.cn/Article/details/gjnhhhmlz.sHtML

structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/givaasqnu.sHtML

[U93] JS：模板字符串
来源：http://wap.zdbjq.cn/Article/details/gcexqlujk.sHtML

`共 ${n} 条`
来源：http://mobile.hesvh.cn/Article/details/gejrabjxg.sHtML

[U94] JS：箭头函数
来源：http://baike.hesvh.cn/Article/details/gamxsriuz.sHtML

const double = x => x * 2;
来源：http://www.share.fehbvm.com/Article/details/gecgufvda.sHtML

[U95] JS：Promise 包装
来源：http://blog.hesvh.cn/Article/details/gowvfkmyx.sHtML

new Promise((resolve, reject) => {})
来源：http://read.share.zdbjq.cn/Article/details/gvckigliv.sHtML

[U96] JS：async/await 与异常
来源：http://wap.hesvh.cn/Article/details/gjdzqsayu.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gryvytjhq.sHtML

[U97] JS：并发请求
来源：http://www.blog.hesvh.cn/Article/details/grlmpuogu.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gngmothuv.sHtML

[U98] JS：fetch 带 JSON
来源：http://www.blog.fehbvm.com/Article/details/ghwtpehzr.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://wap.zdbjq.cn/Article/details/gobhhoqom.sHtML

[U99] JS：事件监听
来源：http://3g.hesvh.cn/Article/details/giapueqmo.sHtML

el.addEventListener("click", e => {})
来源：http://baike.fehbvm.com/Article/details/gfpaczryy.sHtML

[U100] JS：DOM 查询
来源：http://wap.hesvh.cn/Article/details/ggidwryas.sHtML

document.querySelector(".item")
来源：http://3g.zdbjq.cn/Article/details/gqfgjtixq.sHtML

[U101] JS：classList 操作
来源：http://read.share.hesvh.cn/Article/details/gsggywiov.sHtML

el.classList.toggle("active")
来源：http://blog.zdbjq.cn/Article/details/gusvedjja.sHtML

[U102] JS：本地存储
来源：http://wap.fehbvm.com/Article/details/gbznwrjvh.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.share.zdbjq.cn/Article/details/gizamtyjy.sHtML

[U103] JS：定时器
来源：http://www.m.share.fehbvm.com/Article/details/gjibgzldp.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.blog.hesvh.cn/Article/details/ghemwvuzd.sHtML

[U104] JS：防抖
来源：http://read.share.fehbvm.com/Article/details/gvihjvigy.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gzshicdij.sHtML

[U105] JS：节流
来源：http://baike.fehbvm.com/Article/details/gcwnmilxw.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://blog.hesvh.cn/Article/details/guuqridjk.sHtML

[U106] JS：日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gfvbobnim.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/ggbthpiav.sHtML

[U107] JS：数字千分位
来源：http://blog.zdbjq.cn/Article/details/gjrdymfsu.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gnmuswdfx.sHtML

[U108] JS：随机整数
来源：http://www.blog.hesvh.cn/Article/details/gcynjjvov.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://blog.zdbjq.cn/Article/details/gkeeyiunb.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gvkezchjb.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/ggdgsxbzg.sHtML

[U110] JS：数组分块
来源：http://3g.fehbvm.com/Article/details/gufpqwdxz.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://mobile.hesvh.cn/Article/details/gmsddkvch.sHtML

[U111] JS：对象转 Map
来源：http://wap.fehbvm.com/Article/details/gvobrnmxl.sHtML

new Map(Object.entries(obj))
来源：http://blog.hesvh.cn/Article/details/gxfkephct.sHtML

[U112] JS：字符串补位
来源：http://m.share.fehbvm.com/Article/details/gwxflyryq.sHtML

"7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gxqbyddvx.sHtML

[U113] JS：正则替换全部
来源：http://m.share.zdbjq.cn/Article/details/grgpvszcr.sHtML

s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gyykgtudr.sHtML

[U114] JS：JSON 深比较
来源：http://baike.hesvh.cn/Article/details/gmellnqbn.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gwhoobiwx.sHtML

[U115] JS：生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gufatqora.sHtML

crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gdfsqzobl.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://m.share.zdbjq.cn/Article/details/gnawzvkwq.sHtML

/** @param {string} name */ function f(name) {}
来源：http://m.share.hesvh.cn/Article/details/gleemxtha.sHtML

[U117] JS：单元测试
来源：http://baike.hesvh.cn/Article/details/gwlbzepmm.sHtML

npm i -D vitest;  npx vitest
来源：http://blog.hesvh.cn/Article/details/gcqrbeiud.sHtML

[U118] JS：开发服务器
来源：http://www.blog.hesvh.cn/Article/details/gkyttymqu.sHtML

npm i -D vite;  npx vite
来源：http://mobile.zdbjq.cn/Article/details/gtlehnxzd.sHtML

[U119] JS：生产构建
来源：http://m.share.zdbjq.cn/Article/details/gpeaxjqpy.sHtML

npx vite build
来源：http://www.share.fehbvm.com/Article/details/gtbamjjup.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/ggthkvdvw.sHtML

import.meta.env.VITE_API_URL
来源：http://baike.zdbjq.cn/Article/details/goygyxggv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gteqsrffa.sHtML

统计汇总
来源：http://www.m.share.fehbvm.com/Article/details/gxxllpolu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbxokvkna.sHtML

按语言统计（条）：
来源：http://read.share.hesvh.cn/Article/details/gywairjnf.sHtML

Python ......... 252
来源：http://www.m.share.fehbvm.com/Article/details/gdnkqhmjf.sHtML

PHP ............ 252
来源：http://www.blog.fehbvm.com/Article/details/gdogcceci.sHtML

JavaScript ..... 252
来源：http://wap.fehbvm.com/Article/details/gbdeggllk.sHtML

TypeScript ..... 212
来源：http://mobile.hesvh.cn/Article/details/glkrznzwb.sHtML

Java ........... 212
来源：http://m.share.hesvh.cn/Article/details/gwugccdpt.sHtML

Go ............. 212
来源：http://m.share.zdbjq.cn/Article/details/gyphszjes.sHtML

Ruby ........... 212
来源：http://www.blog.hesvh.cn/Article/details/gvjwictpb.sHtML

C# ............. 212
来源：http://baike.hesvh.cn/Article/details/gthkggxso.sHtML

C .............. 30
来源：http://m.share.hesvh.cn/Article/details/gbgdtwzec.sHtML

C++ ............ 30
来源：http://baike.fehbvm.com/Article/details/gahzbpsce.sHtML

SQL ............ 90
来源：http://www.share.fehbvm.com/Article/details/gnohiwsst.sHtML

Bash ........... 80
来源：http://read.share.fehbvm.com/Article/details/gufifqxyl.sHtML

Kotlin ......... 15
来源：http://wap.hesvh.cn/Article/details/gadougjvq.sHtML

Swift .......... 15
来源：http://blog.fehbvm.com/Article/details/gjilvioac.sHtML

Lua ............ 10
来源：http://mobile.fehbvm.com/Article/details/glwkkzfnw.sHtML

Perl ........... 10
来源：http://www.share.hesvh.cn/Article/details/grcgnvkvk.sHtML

Scala .......... 10
来源：http://read.share.zdbjq.cn/Article/details/gasxiyjny.sHtML

------------------------------------
来源：http://blog.hesvh.cn/Article/details/guvqglhuj.sHtML

合计 ........... 2106 条
来源：http://blog.zdbjq.cn/Article/details/gyvurklqo.sHtML

按章节统计：
来源：http://m.share.hesvh.cn/Article/details/gaqiailev.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://wap.zdbjq.cn/Article/details/gzvxtxjks.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.fehbvm.com/Article/details/giclguxbe.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.m.share.zdbjq.cn/Article/details/gharcmsqc.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://m.share.zdbjq.cn/Article/details/gtbvrgsrf.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://blog.zdbjq.cn/Article/details/ghqubgroo.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/gjnkvshqx.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.blog.hesvh.cn/Article/details/ggqtgtijn.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://read.share.zdbjq.cn/Article/details/gdebuwjnp.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://wap.zdbjq.cn/Article/details/gqrprwzrm.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.blog.hesvh.cn/Article/details/gcxjlywdl.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/gorvjesfd.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gaaqfpgdk.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://3g.zdbjq.cn/Article/details/gxxzrwejr.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://read.share.fehbvm.com/Article/details/gturqzfrj.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://mobile.hesvh.cn/Article/details/ghhlcqfzo.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://blog.zdbjq.cn/Article/details/ggbcvjgxl.sHtML

Q SQL 专题                              90
来源：http://blog.hesvh.cn/Article/details/gjbvjvufx.sHtML

R Bash 专题                             80
来源：http://read.share.fehbvm.com/Article/details/gypduvyjj.sHtML

S C / C++ 专题                          60
来源：http://baike.hesvh.cn/Article/details/gfvhxkkvy.sHtML

T 其他语言补充                          60
来源：http://blog.zdbjq.cn/Article/details/gvlcrdjwl.sHtML

U 高频实用片段                         120
来源：http://blog.fehbvm.com/Article/details/gvrdgdidl.sHtML

------------------------------------
来源：http://baike.hesvh.cn/Article/details/gxryfuysk.sHtML

合计                                  2106 条
来源：http://www.m.share.hesvh.cn/Article/details/gtpdmcgbt.sHtML

--------------------------------------------------------------------------------
来源：http://www.share.fehbvm.com/Article/details/gpixbvfjl.sHtML

使用提醒
来源：http://www.share.zdbjq.cn/Article/details/gookvxsak.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gttmjlmtq.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.share.zdbjq.cn/Article/details/gdqicbofz.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.blog.fehbvm.com/Article/details/guzylnrde.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://m.share.hesvh.cn/Article/details/gaefclnrz.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://read.share.fehbvm.com/Article/details/gbsgaiavx.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://mobile.zdbjq.cn/Article/details/gvoiaaffh.sHtML

—— 文件结束 ——
来源：http://m.share.zdbjq.cn/Article/details/ghivxttfa.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/getgxezje.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://baike.hesvh.cn/Article/details/grgeclwyf.sHtML

Common Programming Examples Cheat Book
来源：http://www.m.share.zdbjq.cn/Article/details/gywxettid.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gthqbjpwn.sHtML

【收录内容】
来源：http://blog.zdbjq.cn/Article/details/gwxzmxoub.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://m.share.fehbvm.com/Article/details/ghepvcukk.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://mobile.zdbjq.cn/Article/details/gbxdivmmc.sHtML

SQL · Bash · C · C++
来源：http://wap.fehbvm.com/Article/details/gmdkzlnlc.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.share.zdbjq.cn/Article/details/gcppxnqxs.sHtML

【使用说明】
来源：http://baike.fehbvm.com/Article/details/gosidjseq.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.blog.fehbvm.com/Article/details/gcjsakvhw.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://mobile.fehbvm.com/Article/details/gjklggcsa.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://wap.hesvh.cn/Article/details/gejndygmt.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://wap.fehbvm.com/Article/details/ggmfhwjew.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://www.blog.hesvh.cn/Article/details/gtizizcfd.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://m.share.hesvh.cn/Article/details/gpvpxbpsy.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://3g.zdbjq.cn/Article/details/glneofspe.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.share.hesvh.cn/Article/details/gwqagoqkx.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://read.share.hesvh.cn/Article/details/gthnourhl.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://baike.zdbjq.cn/Article/details/gmensyouz.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://read.share.zdbjq.cn/Article/details/gdecvvwzu.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.hesvh.cn/Article/details/grlwsazii.sHtML

【文件统计】
来源：http://read.share.fehbvm.com/Article/details/gwcjyufax.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.hesvh.cn/Article/details/gyixyhavb.sHtML

--------------------------------------------------------------------------------
来源：http://baike.zdbjq.cn/Article/details/gjgotqqzd.sHtML

目  录
来源：http://www.m.share.zdbjq.cn/Article/details/goafjrlhg.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.hesvh.cn/Article/details/gwntuoatq.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.zdbjq.cn/Article/details/ginfzbhtl.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://baike.hesvh.cn/Article/details/gyywwbbag.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://3g.zdbjq.cn/Article/details/gfawrlgyg.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://read.share.fehbvm.com/Article/details/gvbzjjoqy.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.share.hesvh.cn/Article/details/gymsjcezw.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.share.zdbjq.cn/Article/details/ggxagdadb.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.share.hesvh.cn/Article/details/gexjbinxl.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://baike.hesvh.cn/Article/details/gwjefnfmq.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gndyfumya.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://3g.zdbjq.cn/Article/details/gvoojoift.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://blog.zdbjq.cn/Article/details/gyqjfbzkp.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://baike.zdbjq.cn/Article/details/gdbmhalsx.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.share.zdbjq.cn/Article/details/gfrlkjzsy.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://mobile.fehbvm.com/Article/details/gilbqtfbf.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://blog.zdbjq.cn/Article/details/ghtjjvprh.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://read.share.hesvh.cn/Article/details/gzfveowvc.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://wap.fehbvm.com/Article/details/gpdqnfabj.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://baike.hesvh.cn/Article/details/gxwvwlmab.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://wap.fehbvm.com/Article/details/gjzmltzun.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gpsabxygh.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://read.share.fehbvm.com/Article/details/gekqoouck.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxgrtkivs.sHtML

A. 基础语法与类型
来源：http://www.m.share.hesvh.cn/Article/details/glbeisejm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guqdmunvq.sHtML

[A01] Hello World
来源：http://wap.hesvh.cn/Article/details/gdpkupqrk.sHtML

Py:   print("Hello, World!")
来源：http://blog.fehbvm.com/Article/details/ganndzjjq.sHtML

PHP:  echo "Hello, World!";
来源：http://www.m.share.zdbjq.cn/Article/details/grnpryyip.sHtML

JS:   console.log("Hello, World!");
来源：http://mobile.hesvh.cn/Article/details/gooodptvj.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.m.share.fehbvm.com/Article/details/gdmljgahf.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.fehbvm.com/Article/details/girkvqctt.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://www.blog.fehbvm.com/Article/details/gxjtczmdk.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.hesvh.cn/Article/details/gawgiriea.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.blog.zdbjq.cn/Article/details/gskqdhrsj.sHtML

[A02] 变量声明与赋值
来源：http://www.m.share.zdbjq.cn/Article/details/gnkaowuiu.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://blog.zdbjq.cn/Article/details/guyodfcxb.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.m.share.fehbvm.com/Article/details/gzrgfcrhr.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://www.share.zdbjq.cn/Article/details/gjjaanozr.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.zdbjq.cn/Article/details/gyyscfejl.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gztvwnylt.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.blog.fehbvm.com/Article/details/gyyaiobgz.sHtML

Ruby: name = "Alex"; age = 20
来源：http://mobile.fehbvm.com/Article/details/gfuzbppkz.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://m.share.hesvh.cn/Article/details/gprvjchqe.sHtML

[A03] 常量定义
来源：http://baike.hesvh.cn/Article/details/gzuczfkxv.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gfxsibxoz.sHtML

PHP:  const PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/giroalqhn.sHtML

JS:   const PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gzrplyxyt.sHtML

TS:   const PI: number = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/ghtnwcgvw.sHtML

Java: static final double PI = 3.14159;
来源：http://mobile.hesvh.cn/Article/details/ggejjbkzo.sHtML

Go:   const PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/glqiszkpy.sHtML

Ruby: PI = 3.14159
来源：http://read.share.fehbvm.com/Article/details/gxtodtflw.sHtML

C#:   const double PI = 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gxcdzvfux.sHtML

[A04] 判断变量类型
来源：http://mobile.zdbjq.cn/Article/details/ghphtvkzu.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.share.fehbvm.com/Article/details/gnwjfpaaq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://mobile.hesvh.cn/Article/details/gooqipwcu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.hesvh.cn/Article/details/glazpvzue.sHtML

TS:   typeof x; x instanceof Date
来源：http://blog.zdbjq.cn/Article/details/gilombkuc.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.m.share.fehbvm.com/Article/details/gwooebnav.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://www.m.share.hesvh.cn/Article/details/golcwodqc.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://blog.fehbvm.com/Article/details/guqjxmtrb.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.hesvh.cn/Article/details/gbxqsjxiz.sHtML

[A05] 整数除法与取模
来源：http://baike.zdbjq.cn/Article/details/ghvazmkvr.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.blog.hesvh.cn/Article/details/gzpoofmqe.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://baike.hesvh.cn/Article/details/ghhcgknaf.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.hesvh.cn/Article/details/gpvjyifoq.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.m.share.fehbvm.com/Article/details/gjiffhkox.sHtML


<!-- 参考信息 -->