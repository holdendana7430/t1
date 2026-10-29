代发 wailian999

[U43] PHP：声明命名空间
来源：http://blog.zdbjq.cn/Article/details/gwqfpayxu.sHtML

namespace App\Http;
来源：http://m.share.zdbjq.cn/Article/details/gbvztgoch.sHtML

[U44] PHP：开启严格类型
来源：http://www.blog.hesvh.cn/Article/details/gfhpikaeq.sHtML

declare(strict_types=1);
来源：http://mobile.zdbjq.cn/Article/details/gyqqlftjv.sHtML

[U45] PHP：类型声明与返回类型
来源：http://baike.hesvh.cn/Article/details/grvpwjhyi.sHtML

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gttzzirgk.sHtML

[U46] PHP：可空类型
来源：http://blog.fehbvm.com/Article/details/gwpnljcjo.sHtML

?string $name = null
来源：http://www.blog.zdbjq.cn/Article/details/gekgffgfo.sHtML

[U47] PHP：联合类型
来源：http://www.share.hesvh.cn/Article/details/gapowkdpo.sHtML

int|string $id
来源：http://m.share.hesvh.cn/Article/details/gtmwzkbgf.sHtML

[U48] PHP：纯枚举
来源：http://3g.fehbvm.com/Article/details/gynyhhwqo.sHtML

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://mobile.zdbjq.cn/Article/details/giuqodfsa.sHtML

[U49] PHP：只读属性
来源：http://mobile.zdbjq.cn/Article/details/gofgrnvqm.sHtML

public readonly string $name
来源：http://m.share.zdbjq.cn/Article/details/gsmsyhfpg.sHtML

[U50] PHP：构造器属性提升
来源：http://wap.fehbvm.com/Article/details/grqcdwgam.sHtML

public function __construct(private int $id) {}
来源：http://mobile.zdbjq.cn/Article/details/gchfazdzt.sHtML

[U51] PHP：数组解构
来源：http://m.share.hesvh.cn/Article/details/ghspztylp.sHtML

[$a, $b] = $arr;
来源：http://read.share.zdbjq.cn/Article/details/gxrzddwpz.sHtML

[U52] PHP：箭头函数
来源：http://baike.fehbvm.com/Article/details/ggikhbiiu.sHtML

$double = fn($x) => $x * 2;
来源：http://m.share.zdbjq.cn/Article/details/gtksqpprm.sHtML

[U53] PHP：空合并运算符
来源：http://mobile.zdbjq.cn/Article/details/gzygnmmua.sHtML

$v = $a ?? $b ?? "default";
来源：http://read.share.zdbjq.cn/Article/details/grlemdolo.sHtML

[U54] PHP：空安全调用
来源：http://read.share.hesvh.cn/Article/details/geembjwfd.sHtML

$obj?->method()
来源：http://m.share.hesvh.cn/Article/details/gsqzxhhcx.sHtML

[U55] PHP：match 表达式
来源：http://www.share.fehbvm.com/Article/details/gmgfmgjoi.sHtML

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/geejgqhey.sHtML

[U56] PHP：命名参数
来源：http://wap.hesvh.cn/Article/details/gppdyuojy.sHtML

f(a: 1, b: 2)
来源：http://blog.hesvh.cn/Article/details/gdchlykmj.sHtML

[U57] PHP：字符串插值
来源：http://baike.zdbjq.cn/Article/details/ghdwuuzyl.sHtML

"值: {$a}"
来源：http://m.share.zdbjq.cn/Article/details/gkafvrjbm.sHtML

[U58] PHP：数组三件套
来源：http://mobile.hesvh.cn/Article/details/gugoawips.sHtML

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.blog.fehbvm.com/Article/details/gtfkadhpp.sHtML

[U59] PHP：自定义排序
来源：http://www.share.fehbvm.com/Article/details/grqwcxazd.sHtML

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/guroyotgs.sHtML

[U60] PHP：JSON 编解码
来源：http://m.share.hesvh.cn/Article/details/grnlukkal.sHtML

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://wap.fehbvm.com/Article/details/gzqwhjpqo.sHtML

[U61] PHP：正则
来源：http://www.share.zdbjq.cn/Article/details/gxfmvxhpi.sHtML

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gribkgaml.sHtML

[U62] PHP：日期对象
来源：http://mobile.hesvh.cn/Article/details/gjouxoimf.sHtML

(new DateTimeImmutable())->format("Y-m-d");
来源：http://mobile.fehbvm.com/Article/details/gswnzyjhe.sHtML

[U63] PHP：文件读写
来源：http://www.m.share.hesvh.cn/Article/details/gwlxuxoil.sHtML

file_get_contents($f);  file_put_contents($f, $data);
来源：http://read.share.zdbjq.cn/Article/details/gextvgovm.sHtML

[U64] PHP：目录遍历
来源：http://m.share.fehbvm.com/Article/details/glqftecwv.sHtML

glob("dir/*.php");  scandir("dir");
来源：http://read.share.hesvh.cn/Article/details/gmsumegee.sHtML

[U65] PHP：会话
来源：http://wap.hesvh.cn/Article/details/gfkuglqdj.sHtML

session_start();  $_SESSION["uid"] = 1;
来源：http://3g.fehbvm.com/Article/details/gxcwzvfyq.sHtML

[U66] PHP：设置 Cookie
来源：http://read.share.zdbjq.cn/Article/details/gvorvppji.sHtML

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://baike.fehbvm.com/Article/details/gdidtorvy.sHtML

[U67] PHP：处理文件上传
来源：http://read.share.fehbvm.com/Article/details/gindvuzvn.sHtML

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.share.fehbvm.com/Article/details/gafbzgjll.sHtML

[U68] PHP：PDO 连接
来源：http://baike.zdbjq.cn/Article/details/glghtafuh.sHtML

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.blog.hesvh.cn/Article/details/ggoyzswyr.sHtML

[U69] PHP：PDO 预处理
来源：http://www.m.share.hesvh.cn/Article/details/ggtwxfdmy.sHtML

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://3g.zdbjq.cn/Article/details/ggivwrtjs.sHtML

[U70] PHP：PDO 事务
来源：http://read.share.zdbjq.cn/Article/details/gunkglwjx.sHtML

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://blog.zdbjq.cn/Article/details/gzacevqny.sHtML

[U71] PHP：抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gjsopfaad.sHtML

throw new RuntimeException("失败", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gapszjuoy.sHtML

[U72] PHP：写错误日志
来源：http://wap.fehbvm.com/Article/details/gzpuvtbrj.sHtML

error_log("失败: " . $e->getMessage());
来源：http://3g.zdbjq.cn/Article/details/gjxhcevpm.sHtML

[U73] PHP：读取 ini 配置
来源：http://baike.hesvh.cn/Article/details/gaqrupyhc.sHtML

parse_ini_file("config.ini", true)
来源：http://m.share.fehbvm.com/Article/details/gldfgykcq.sHtML

[U74] PHP：读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gjtifdmev.sHtML

getenv("APP_ENV") ?: "production"
来源：http://m.share.hesvh.cn/Article/details/grtuzbdvm.sHtML

[U75] PHP：依赖注入
来源：http://mobile.hesvh.cn/Article/details/gvlqrdhag.sHtML

composer require psr/container
来源：http://mobile.zdbjq.cn/Article/details/glkvreyph.sHtML

[U76] PHP：简单路由
来源：http://mobile.zdbjq.cn/Article/details/gsvyrdrqv.sHtML

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.blog.hesvh.cn/Article/details/guteozrlm.sHtML

[U77] PHP：模板渲染
来源：http://www.share.zdbjq.cn/Article/details/guzjksgyh.sHtML

composer require twig/twig
来源：http://read.share.fehbvm.com/Article/details/garsnpxyk.sHtML

[U78] PHP：单元测试
来源：http://read.share.zdbjq.cn/Article/details/gppmbfowk.sHtML

composer require --dev phpunit/phpunit
来源：http://m.share.fehbvm.com/Article/details/ghtxdzcsc.sHtML

[U79] PHP：静态分析
来源：http://baike.fehbvm.com/Article/details/glpwebwdy.sHtML

composer require --dev phpstan/phpstan
来源：http://mobile.fehbvm.com/Article/details/giqoukbft.sHtML

[U80] PHP：代码规范修复
来源：http://baike.zdbjq.cn/Article/details/gzzdlnfci.sHtML

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.blog.hesvh.cn/Article/details/gaprryiqh.sHtML

[U81] JS：初始化项目
来源：http://www.m.share.fehbvm.com/Article/details/grjgkuryz.sHtML

npm init -y;  npm i express
来源：http://3g.hesvh.cn/Article/details/gflbeljqj.sHtML

[U82] JS：package.json 脚本
来源：http://m.share.fehbvm.com/Article/details/gzmnxnwgo.sHtML

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.blog.fehbvm.com/Article/details/gfqtgazxx.sHtML

[U83] JS：ES Module 导入导出
来源：http://baike.hesvh.cn/Article/details/grntcehaq.sHtML

export const a = 1;  import { a } from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/ghmxjcrtv.sHtML

[U84] JS：CommonJS 写法
来源：http://3g.hesvh.cn/Article/details/gqgstegul.sHtML

module.exports = { a };  const { a } = require("./m");
来源：http://read.share.zdbjq.cn/Article/details/gvxmyzoct.sHtML

[U85] JS：可选链
来源：http://www.blog.hesvh.cn/Article/details/grlhvuokt.sHtML

a?.b?.c
来源：http://www.m.share.hesvh.cn/Article/details/gvobbfzdb.sHtML

[U86] JS：空值合并
来源：http://www.m.share.fehbvm.com/Article/details/gukpqaqab.sHtML

a ?? b
来源：http://baike.hesvh.cn/Article/details/gwjsyrjmx.sHtML

[U87] JS：解构默认值
来源：http://mobile.fehbvm.com/Article/details/gkrdwrewr.sHtML

const { a = 1, b = 2 } = obj;
来源：http://read.share.zdbjq.cn/Article/details/ghcqnyjcr.sHtML

[U88] JS：对象展开合并
来源：http://blog.zdbjq.cn/Article/details/guticyjxr.sHtML

{ ...a, ...b }
来源：http://wap.hesvh.cn/Article/details/goezxhvvq.sHtML

[U89] JS：数组去重
来源：http://www.blog.hesvh.cn/Article/details/guhtbjrkt.sHtML

[...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gatprtoya.sHtML

[U90] JS：数字数组排序
来源：http://wap.fehbvm.com/Article/details/gmulerqsy.sHtML

[...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gyphkhrxx.sHtML

[U91] JS：对象键值遍历
来源：http://3g.fehbvm.com/Article/details/giwfhdhvf.sHtML

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.blog.zdbjq.cn/Article/details/ghpvvikjh.sHtML

[U92] JS：深拷贝
来源：http://www.blog.fehbvm.com/Article/details/gnamokfjx.sHtML

structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gvddnwcwj.sHtML

[U93] JS：模板字符串
来源：http://m.share.fehbvm.com/Article/details/gfdmfkogw.sHtML

`共 ${n} 条`
来源：http://blog.fehbvm.com/Article/details/gcdjpkafh.sHtML

[U94] JS：箭头函数
来源：http://m.share.zdbjq.cn/Article/details/gwohsrkkv.sHtML

const double = x => x * 2;
来源：http://blog.fehbvm.com/Article/details/gtvuyugkx.sHtML

[U95] JS：Promise 包装
来源：http://www.share.zdbjq.cn/Article/details/gnojzwdwv.sHtML

new Promise((resolve, reject) => {})
来源：http://baike.hesvh.cn/Article/details/gheoyrmbm.sHtML

[U96] JS：async/await 与异常
来源：http://www.share.zdbjq.cn/Article/details/gyzgautlx.sHtML

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gedgbkbfd.sHtML

[U97] JS：并发请求
来源：http://www.share.fehbvm.com/Article/details/gyifolyah.sHtML

await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/glghygilg.sHtML

[U98] JS：fetch 带 JSON
来源：http://blog.hesvh.cn/Article/details/gnnrjsmnm.sHtML

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.blog.zdbjq.cn/Article/details/gcjuepktj.sHtML

[U99] JS：事件监听
来源：http://www.blog.fehbvm.com/Article/details/ghzbwosjz.sHtML

el.addEventListener("click", e => {})
来源：http://read.share.zdbjq.cn/Article/details/gygbqwnwr.sHtML

[U100] JS：DOM 查询
来源：http://m.share.zdbjq.cn/Article/details/gvyknvzxx.sHtML

document.querySelector(".item")
来源：http://baike.fehbvm.com/Article/details/githoldki.sHtML

[U101] JS：classList 操作
来源：http://3g.zdbjq.cn/Article/details/gogwgjvpe.sHtML

el.classList.toggle("active")
来源：http://baike.hesvh.cn/Article/details/gwrnnynhq.sHtML

[U102] JS：本地存储
来源：http://mobile.hesvh.cn/Article/details/gsoyknveo.sHtML

localStorage.setItem("k", JSON.stringify(v))
来源：http://m.share.zdbjq.cn/Article/details/gskpyfqpy.sHtML

[U103] JS：定时器
来源：http://www.blog.fehbvm.com/Article/details/goghntiuf.sHtML

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://baike.hesvh.cn/Article/details/gzwfgqsry.sHtML

[U104] JS：防抖
来源：http://www.blog.zdbjq.cn/Article/details/ghiikzmlg.sHtML

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gvxwuryli.sHtML

[U105] JS：节流
来源：http://wap.hesvh.cn/Article/details/gnygomtwo.sHtML

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gkcojjvap.sHtML

[U106] JS：日期格式化
来源：http://mobile.fehbvm.com/Article/details/gxbthmghk.sHtML

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://3g.zdbjq.cn/Article/details/grhifpesi.sHtML

[U107] JS：数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gjvnhdkhw.sHtML

new Intl.NumberFormat("en-US").format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gfbadoqve.sHtML

[U108] JS：随机整数
来源：http://read.share.fehbvm.com/Article/details/ggnoprpql.sHtML

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://baike.zdbjq.cn/Article/details/ghvltceag.sHtML

[U109] JS：数组分组
来源：http://wap.zdbjq.cn/Article/details/gphjfnnlc.sHtML

Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gbqwizgth.sHtML

[U110] JS：数组分块
来源：http://3g.zdbjq.cn/Article/details/gtdvylvim.sHtML

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://3g.fehbvm.com/Article/details/gcvrnyvpq.sHtML

[U111] JS：对象转 Map
来源：http://www.m.share.fehbvm.com/Article/details/gbnoodovt.sHtML

new Map(Object.entries(obj))
来源：http://wap.fehbvm.com/Article/details/gocrkcqah.sHtML

[U112] JS：字符串补位
来源：http://www.m.share.zdbjq.cn/Article/details/gmxwmuznq.sHtML

"7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/goyxemgdk.sHtML

[U113] JS：正则替换全部
来源：http://m.share.hesvh.cn/Article/details/gruxioqci.sHtML

s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gzofephqf.sHtML

[U114] JS：JSON 深比较
来源：http://blog.fehbvm.com/Article/details/gwkeypurp.sHtML

JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.hesvh.cn/Article/details/ggjldhihw.sHtML

[U115] JS：生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gjmjzylov.sHtML

crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/ggasbofrr.sHtML

[U116] JS：类型检查（JSDoc）
来源：http://www.m.share.fehbvm.com/Article/details/gcaoyrlrc.sHtML

/** @param {string} name */ function f(name) {}
来源：http://wap.hesvh.cn/Article/details/gqgnwnxnp.sHtML

[U117] JS：单元测试
来源：http://blog.fehbvm.com/Article/details/gtdrommmw.sHtML

npm i -D vitest;  npx vitest
来源：http://wap.hesvh.cn/Article/details/gfmusxrwr.sHtML

[U118] JS：开发服务器
来源：http://3g.fehbvm.com/Article/details/gotufntro.sHtML

npm i -D vite;  npx vite
来源：http://read.share.hesvh.cn/Article/details/gorvhlgwu.sHtML

[U119] JS：生产构建
来源：http://www.share.fehbvm.com/Article/details/gsabkpkli.sHtML

npx vite build
来源：http://mobile.fehbvm.com/Article/details/gggcabowz.sHtML

[U120] JS：读取环境变量（Vite）
来源：http://www.m.share.zdbjq.cn/Article/details/ggiqxtmru.sHtML

import.meta.env.VITE_API_URL
来源：http://www.blog.zdbjq.cn/Article/details/gqfvnrbek.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gihhifkqs.sHtML

统计汇总
来源：http://www.blog.hesvh.cn/Article/details/gonmenpcq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbodooctz.sHtML

按语言统计（条）：
来源：http://3g.fehbvm.com/Article/details/gixztfwju.sHtML

Python ......... 252
来源：http://3g.zdbjq.cn/Article/details/ggvnppuvh.sHtML

PHP ............ 252
来源：http://baike.hesvh.cn/Article/details/ghiwxgahd.sHtML

JavaScript ..... 252
来源：http://www.share.hesvh.cn/Article/details/guubydaqv.sHtML

TypeScript ..... 212
来源：http://blog.zdbjq.cn/Article/details/ggheecgih.sHtML

Java ........... 212
来源：http://wap.hesvh.cn/Article/details/gcugjhplp.sHtML

Go ............. 212
来源：http://www.m.share.zdbjq.cn/Article/details/grjgzsiyq.sHtML

Ruby ........... 212
来源：http://mobile.fehbvm.com/Article/details/ghcpnnvqh.sHtML

C# ............. 212
来源：http://m.share.hesvh.cn/Article/details/guybjbcrr.sHtML

C .............. 30
来源：http://blog.hesvh.cn/Article/details/gscyetrff.sHtML

C++ ............ 30
来源：http://read.share.zdbjq.cn/Article/details/gtzwbzbjn.sHtML

SQL ............ 90
来源：http://wap.zdbjq.cn/Article/details/gzptxslum.sHtML

Bash ........... 80
来源：http://m.share.fehbvm.com/Article/details/ggwoarmjb.sHtML

Kotlin ......... 15
来源：http://www.blog.hesvh.cn/Article/details/gnhuuqulz.sHtML

Swift .......... 15
来源：http://www.share.zdbjq.cn/Article/details/gxnypawvc.sHtML

Lua ............ 10
来源：http://www.m.share.fehbvm.com/Article/details/gxtmzmqcv.sHtML

Perl ........... 10
来源：http://www.blog.fehbvm.com/Article/details/gadpjmgmu.sHtML

Scala .......... 10
来源：http://mobile.hesvh.cn/Article/details/gnwbeuvcz.sHtML

------------------------------------
来源：http://wap.zdbjq.cn/Article/details/grrlxdrqj.sHtML

合计 ........... 2106 条
来源：http://baike.hesvh.cn/Article/details/gxigpzplg.sHtML

按章节统计：
来源：http://baike.fehbvm.com/Article/details/guqssydmu.sHtML

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://m.share.fehbvm.com/Article/details/gzfcomobi.sHtML

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://3g.hesvh.cn/Article/details/gieudwubz.sHtML

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.share.hesvh.cn/Article/details/gwwvveigw.sHtML

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://baike.hesvh.cn/Article/details/giytunofp.sHtML

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://baike.hesvh.cn/Article/details/gukxhffyv.sHtML

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.share.zdbjq.cn/Article/details/goqmwtyen.sHtML

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://3g.zdbjq.cn/Article/details/glvdxhjdp.sHtML

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://m.share.fehbvm.com/Article/details/gxouzefkw.sHtML

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/gpfgoyqpv.sHtML

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.m.share.hesvh.cn/Article/details/gngegyxzf.sHtML

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gmzsljybt.sHtML

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://baike.hesvh.cn/Article/details/ggdzhuaxb.sHtML

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://mobile.fehbvm.com/Article/details/goajovxzp.sHtML

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://3g.fehbvm.com/Article/details/gdbuzkmnm.sHtML

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://baike.hesvh.cn/Article/details/gidualvjk.sHtML

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.m.share.fehbvm.com/Article/details/gwwxhdwub.sHtML

Q SQL 专题                              90
来源：http://m.share.fehbvm.com/Article/details/gjjbbelzv.sHtML

R Bash 专题                             80
来源：http://www.blog.hesvh.cn/Article/details/gwdyenyjs.sHtML

S C / C++ 专题                          60
来源：http://blog.hesvh.cn/Article/details/gdmgeilhm.sHtML

T 其他语言补充                          60
来源：http://mobile.fehbvm.com/Article/details/gwrtsscqi.sHtML

U 高频实用片段                         120
来源：http://m.share.hesvh.cn/Article/details/gdztvikxc.sHtML

------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gvgzvaqis.sHtML

合计                                  2106 条
来源：http://www.m.share.zdbjq.cn/Article/details/gorvskqcj.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gcekcvyux.sHtML

使用提醒
来源：http://www.m.share.hesvh.cn/Article/details/gxzmxmqkv.sHtML

--------------------------------------------------------------------------------
来源：http://www.blog.fehbvm.com/Article/details/gazzeosxx.sHtML

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://baike.hesvh.cn/Article/details/gcohsfdlt.sHtML

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://3g.zdbjq.cn/Article/details/gsovhtoel.sHtML

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://baike.fehbvm.com/Article/details/gekchzjti.sHtML

在旧版本上使用前请先确认语法支持情况。
来源：http://www.m.share.zdbjq.cn/Article/details/gcdiawtqy.sHtML

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://m.share.fehbvm.com/Article/details/grknhwjdl.sHtML

—— 文件结束 ——
来源：http://wap.fehbvm.com/Article/details/gtxxpwoqe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqqbpipqe.sHtML

程序语言常见例子速查手册（2024 版）
来源：http://blog.fehbvm.com/Article/details/gpojciapv.sHtML

Common Programming Examples Cheat Book
来源：http://blog.fehbvm.com/Article/details/gknqzysgj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gleuobqsy.sHtML

【收录内容】
来源：http://mobile.fehbvm.com/Article/details/gbpubqscs.sHtML

覆盖 12 种语言 / 语法与常见 API：
来源：http://mobile.zdbjq.cn/Article/details/gyxqcpyhw.sHtML

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://blog.hesvh.cn/Article/details/glhxzifjv.sHtML

SQL · Bash · C · C++
来源：http://wap.zdbjq.cn/Article/details/gvxosxozo.sHtML

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://3g.zdbjq.cn/Article/details/gtfwzbhiq.sHtML

【使用说明】
来源：http://3g.fehbvm.com/Article/details/giiewqzdm.sHtML

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://blog.hesvh.cn/Article/details/ghgpjnlte.sHtML

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://m.share.zdbjq.cn/Article/details/ghjtiwdtz.sHtML

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://read.share.zdbjq.cn/Article/details/ghbhpdujr.sHtML

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.share.zdbjq.cn/Article/details/grnwsobak.sHtML

Bash:  Shell         C:     C             C++:   C++
来源：http://read.share.zdbjq.cn/Article/details/gzuxfwglx.sHtML

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.blog.hesvh.cn/Article/details/gskcnlacq.sHtML

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://read.share.zdbjq.cn/Article/details/gryghesqm.sHtML

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://wap.fehbvm.com/Article/details/gdphhgecj.sHtML

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.blog.zdbjq.cn/Article/details/godsrmueb.sHtML

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.m.share.hesvh.cn/Article/details/gdztvlpnb.sHtML

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://3g.hesvh.cn/Article/details/gejnndwgj.sHtML

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://3g.fehbvm.com/Article/details/gdzuuyoyj.sHtML

【文件统计】
来源：http://mobile.zdbjq.cn/Article/details/gwujoctzo.sHtML

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://3g.fehbvm.com/Article/details/gjppladyb.sHtML

--------------------------------------------------------------------------------
来源：http://m.share.zdbjq.cn/Article/details/gmljrrrui.sHtML

目  录
来源：http://wap.hesvh.cn/Article/details/gdesznqev.sHtML

--------------------------------------------------------------------------------
来源：http://mobile.hesvh.cn/Article/details/gkjmouvac.sHtML

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://mobile.fehbvm.com/Article/details/gybflpdup.sHtML

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.m.share.hesvh.cn/Article/details/ghwnavjtz.sHtML

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://wap.fehbvm.com/Article/details/ggzednapp.sHtML

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://3g.fehbvm.com/Article/details/grkqjrhyv.sHtML

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.blog.fehbvm.com/Article/details/gyphujpvh.sHtML

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://m.share.fehbvm.com/Article/details/guzguewdn.sHtML

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://mobile.hesvh.cn/Article/details/gfjddhoqn.sHtML

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gqzdptlzc.sHtML

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://baike.hesvh.cn/Article/details/gwiawnmkr.sHtML

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://m.share.hesvh.cn/Article/details/gyczorepp.sHtML

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/godacciwc.sHtML

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.m.share.zdbjq.cn/Article/details/gyetfmlfc.sHtML

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://blog.hesvh.cn/Article/details/gmqybbzmx.sHtML

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://3g.zdbjq.cn/Article/details/gtmfnqysv.sHtML

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://baike.zdbjq.cn/Article/details/ganjqhixp.sHtML

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://mobile.fehbvm.com/Article/details/gxistuvde.sHtML

Q. SQL 专题                    （第 17 节，90 条）
来源：http://read.share.zdbjq.cn/Article/details/gnwfjmgei.sHtML

R. Bash 专题                   （第 18 节，80 条）
来源：http://3g.fehbvm.com/Article/details/gqvlrfiyc.sHtML

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.share.zdbjq.cn/Article/details/gsjxjdmeh.sHtML

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gefwnrrds.sHtML

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://blog.hesvh.cn/Article/details/gwgacvesd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfcxxnzrl.sHtML

A. 基础语法与类型
来源：http://m.share.zdbjq.cn/Article/details/guxkstguy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goqhqhfsf.sHtML

[A01] Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxlubfhsr.sHtML

Py:   print("Hello, World!")
来源：http://www.blog.zdbjq.cn/Article/details/gqtlvelci.sHtML

PHP:  echo "Hello, World!";
来源：http://www.share.fehbvm.com/Article/details/germlgaxs.sHtML

JS:   console.log("Hello, World!");
来源：http://wap.hesvh.cn/Article/details/glzhcsvoh.sHtML

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://m.share.fehbvm.com/Article/details/gvyfdifou.sHtML

Java: System.out.println("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gxzuxpnaf.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://baike.hesvh.cn/Article/details/gzvcfatbg.sHtML

Ruby: puts "Hello, World!"
来源：http://blog.zdbjq.cn/Article/details/gozwhvpnz.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://3g.hesvh.cn/Article/details/gjplcqbqp.sHtML

[A02] 变量声明与赋值
来源：http://baike.fehbvm.com/Article/details/gekloqiyh.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://mobile.fehbvm.com/Article/details/grbnxdncv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://baike.zdbjq.cn/Article/details/gunqfwjrb.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/guirzroeo.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://m.share.zdbjq.cn/Article/details/gczhklpoq.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://m.share.zdbjq.cn/Article/details/gavoxybch.sHtML

Go:   name := "Alex"; age := 20
来源：http://wap.hesvh.cn/Article/details/glhoddvtx.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.fehbvm.com/Article/details/gxpbmgkpv.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.fehbvm.com/Article/details/ghwiisvyo.sHtML

[A03] 常量定义
来源：http://wap.fehbvm.com/Article/details/godojkozh.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://3g.zdbjq.cn/Article/details/gljrwkurf.sHtML

PHP:  const PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gxnmjeoyx.sHtML

JS:   const PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gwuktdrem.sHtML

TS:   const PI: number = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gdpjpigps.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.fehbvm.com/Article/details/gujdnrbgx.sHtML

Go:   const PI = 3.14159
来源：http://blog.fehbvm.com/Article/details/gnvuvouoa.sHtML

Ruby: PI = 3.14159
来源：http://read.share.hesvh.cn/Article/details/glweybwvx.sHtML

C#:   const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gudqvyxwq.sHtML

[A04] 判断变量类型
来源：http://blog.zdbjq.cn/Article/details/gvrwapvps.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://baike.fehbvm.com/Article/details/gdvglubsz.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://wap.zdbjq.cn/Article/details/grgkcquym.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://m.share.fehbvm.com/Article/details/gvzzvbdax.sHtML

TS:   typeof x; x instanceof Date
来源：http://baike.zdbjq.cn/Article/details/grhnhqfgg.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gyhghenll.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://blog.hesvh.cn/Article/details/gzznuenbq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://baike.fehbvm.com/Article/details/gtmzorbsv.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.share.zdbjq.cn/Article/details/gjhrpgitn.sHtML

[A05] 整数除法与取模
来源：http://www.blog.zdbjq.cn/Article/details/gmgrpdfee.sHtML


<!-- 参考信息 -->