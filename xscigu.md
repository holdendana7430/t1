代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2eaepnusj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2lvejttov.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2ptrnvyib.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2egfnkwkc.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2aimyrkfz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2obgjtfxl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2eoeigcbe.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2tfsymelr.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2bpzcubff.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2yeqjfcme.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ayncsqqg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2yldfqksi.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2jmrkipza.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2xbdtaoif.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qduzdbfj.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebjgnlqf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2nnzlypsw.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2kytzutdq.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dcgsvysp.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2pniyseyk.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2ghjwwoea.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2vslkguev.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2aczxqfmo.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2sxygwbqq.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2rafibjvb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ytbigzmz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2boftuwbg.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2auoohtyz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lcwcsete.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2cnulbxfa.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2yeevlnwg.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ydweharl.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2wbmahgam.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cfulelml.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2ksrasbpr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2rkanqoof.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2mddcdevg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ydhumiqu.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2rjnbpngy.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2tntpjzvl.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2geajukxv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2binssipg.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2elimrbab.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2yvsafyqj.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2drusfcwe.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bbeopzux.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2jnhbaqhu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cjsxlpym.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2zafbaaxb.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2trlgzmjv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2hygsyrlv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2dnrejlmn.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2vongvlad.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2vykdxhup.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2pdbhqovz.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ocfxokqq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hbbrcxlc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2npxhyzju.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2buupgkzn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2cahddqsk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2ugqfhplz.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2yyuhwfvc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ebyksxtx.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ozzajozr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2ygpzqdbm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2rtmtswgj.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2zmkjnolx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2eubgrtji.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2zcsbtxer.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2jlfzgaqy.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2oijbesza.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qwrkjeds.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2qeewicea.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vtdjtmxj.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2urohysnh.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2anjzwekg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2eeeedpgl.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zpbrhpbz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2avrktjhs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ljpbitoo.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2nahxfflv.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ukgqkbvo.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2qhualksr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2cgcqrwfr.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2yrlvzfos.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qcssaree.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2lwfqnyid.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2pwogmubq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2mctubash.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2rhbbjzfq.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2mbzanpsi.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2wauqaapv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2dtcupwhr.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vrfgfaac.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2zeabrxei.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ihjpbdlh.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2xdjbtoct.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2igzvifsu.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2dabdysha.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tgcrwvlo.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2xqnxowrz.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2thzqrrxn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kevzftuz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2behfakvd.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2cararpng.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2agemdewi.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2qyesaekf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2elzsflxf.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2mqvvounm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2coctcnef.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2qltcwibq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2tkunmnuf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2cyinalpg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2acutvpep.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2wyiongfs.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2oqygrulg.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2crgkxdxv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2akwbdcrp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2supjfdaq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2hneinlkm.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2yotaplfc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2pwjtcsju.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ymnfcumr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2csrnzfqw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2mbmtyhrb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ortzoujs.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zyuoyezc.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ggbebvop.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2stygcgwi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jpbpjqtu.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2obbdzohy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vphaxzio.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2yqjbtigm.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lrkdfsks.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2xlhzpaek.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2tvpdjgca.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2tudfsurn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2kqpspvya.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2kllkemkx.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eaziachg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2wovrxrgm.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2urskxfci.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2habnkzpz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bcmlpeeg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qqmwopjw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2leqojzbv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2wwgfvmhf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2exhxizqv.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2dadnwaiu.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xakcnscs.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2omixokbq.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2ryrghobr.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2brfpuknk.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2udlhzuvf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2jebgnqhx.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2wmvecgvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rpkpvguv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2feekurjz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cufssrrk.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2lstqgjfg.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2jvqvvzlz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2acrnnjxf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2moxqsoxu.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2tiivazhx.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bzjcvxri.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qgbuafpz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ofcmjmfd.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wlvvfvwr.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ejlljqfb.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2yolyhvdy.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2getpapse.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ifjxuvpt.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2meppdqij.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2lxshxoag.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2dsylpjht.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2ctzyhgxe.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ijepfqlk.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hntakwem.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2sfpglazb.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2kxmcwinl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2czrjkyie.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2mrsxbibm.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fbvkunru.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ajnjqprs.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2javkupwp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2piihdkme.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2azpplguu.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ydwewyop.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lbtsjsoi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vjfcsnbv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2akmwayty.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dnnveebq.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hijeaibu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2wwnzbxee.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2brpqwxgb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bgneqzeb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2kjgszxpi.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2bayxzcmu.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2qeqdmsif.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2zzgpsjyn.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2iszklxax.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2nmeatocv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2bmkavxkv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mbgyncpr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2kkmgvxut.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gnxpmsys.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2gbehckqp.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2opklhfxo.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2dxguvwdh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2hxkrbszf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2iaftvmab.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2yrlxedns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkzowzln.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2mvfugtzg.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2vbfgwzhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ijeqqkfc.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2heoblyrx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2aufqdmrc.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2jldhhbyh.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2jebpnqai.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2qdfeqflj.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2bgugidie.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2nrrbebrl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2unywiebb.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2bkafkxzl.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2ahepfmpu.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2kjdailud.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2zczzcpbl.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ibilrbnz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2lqcierqy.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2usqtiwda.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2siswqbip.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2sisulhjx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2huaexpre.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2zjfiufbg.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2dmonxebi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ngqkmoog.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2gunkuizz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xwysvzjd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wzoumqxs.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ceqwiqnw.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2guqnljdu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2adoaohdo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2szywfalu.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2axilviks.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ityykvbr.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2vxvxsrfr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2iobylscq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2fokupblf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2nctqoway.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fprgsxmh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2iywekdrs.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2fwnkxwxj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2guicrljg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2lqavrccx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2omxujdzi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2loshdoua.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2wgivmbnk.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2nmeofjef.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2vjtfvlqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kspemhyu.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2rzjdatzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2updpspim.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2gyegayjm.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2xuuxpjig.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2imjvkgog.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2tmgrnupf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2nbnrtymd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qwgqmmqz.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2gfnceanu.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2cpdzkxcd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ixukpkml.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ssopkhym.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2rhvfiekh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hzpcvtey.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ldvowoew.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2gjbzfzlb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2msylgwds.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2bwzddyem.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2exknlgyv.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2borusgzm.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ewcxqbqb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2nhsnagsj.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2emwerppn.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2urnoypkp.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qnbmdnhl.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hlkpuwbd.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qubdhrhr.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2berkvkku.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xqcnxzft.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vkpzjkyt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2xeebvtmp.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2qzpkybws.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2esyeinob.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2scdgacso.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2sylmuava.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2vscqmint.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2gohnyrtm.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2vorduorx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2fbjdqekt.html


<!-- 参考信息 -->