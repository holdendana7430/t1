代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3yhgoppsu.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3owivkqav.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3mbpgjtux.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3htbktrnn.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3mmnizxjs.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jecykqsa.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3xyhztpqh.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3gqarfywz.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3pgseqwbv.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3rgvcobse.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3sqcxjyle.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxajchce.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3jvttyhja.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3bnhsjztt.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3vlmumgjm.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3szsommnv.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3ihtjyvxw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3cyssaicm.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3jfbhclxr.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3yjzqtgfd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3szssexpx.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3alqvgzfl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3dhdvnekf.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3yyxwchtb.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3dnjsopnv.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3pkqixfbf.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3sooouawx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lmhyztho.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mvzjprpf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3htzwnwsq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3nmsyvcog.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3gtoqgnol.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3qwqgwmft.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3unvpbrke.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3sovyxdne.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jrkkuubw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3mtjymhvi.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3elzckerq.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3skmxkehw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3oybelyjx.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3mfstrcpc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3sxhrlnin.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rwelqgcx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3brzxaulp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3xswklwts.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dcitnezc.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3szwtnzxb.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3onlnylqz.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3siwqfcrr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3stoixpnq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3gqmwwclf.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3dwveuavx.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3fvaztkbo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3efslcsnt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3suoovknl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3wiwpnthl.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3rzrgeogw.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3wyzexeqx.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kpeilqqi.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3mbcrsrxa.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3sosdhsau.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3lrgntcdf.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3crmdsqiu.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3dxfttseq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3rrlmzofz.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3mstabenr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3fqievggu.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3ssuucdpw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3stohdyti.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3wawfyclg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bvorbbzl.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3xjjmderg.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3tnpekwuy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3yzshczqq.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3htddlebf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3txelxwcc.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3hmhjztzw.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3bvsbhlcm.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3sznabkuc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3xguzyemc.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3gxpkeivn.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3glhsfpve.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3cspudwte.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3mgzgxaly.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3qqmjccup.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3ezphlmfi.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3igqqfuuz.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3jkqkqeok.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jgaxobcv.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3joogqsov.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3icmpxeka.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3giswtrhz.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3jcwcybfe.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hmzmwivp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3uvbeflcs.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ymqzwqjp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fnwjnyxg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3pwzvwkie.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3tpwjnvrz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kfegbqkh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3amfaznsm.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3wiozlapk.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3qptkytoc.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3vdvgceoo.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3emnzwneo.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3iggmpsdc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ovbydoyt.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckhkuewi.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3qhwkqijc.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vtpjacmr.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ojvvhlcf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3rtizuneu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3waxeokfq.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3orwgivbg.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3lhatprvl.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3zedwkgtj.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3lecpzmid.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3rbxvscwz.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3qzlrytdf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3kdrvlcbn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3clekdyxz.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3aprmkwct.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3cazjgdxr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3mohltkni.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3edmwvlte.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3lkzvpaij.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3muygotqz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3llvxbiuu.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3pcmgtozd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3gvumryal.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3fssjvtkc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3drkhpkoj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3hsucdimp.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3timerfpl.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3cbgyzcwj.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3tsvdcowf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3fnxenfym.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3bneojifa.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3hjyuvcrg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3prehztiz.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3lrrcvncn.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yohdxktp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3fwhezbpt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gnelxvsl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3nqrktlee.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jukoqivh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3jiuimejy.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jifqrtiz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tzmuxvph.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3obetnlti.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3anjuzglq.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3kbbalmez.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3tupulgmk.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3gznabvdt.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3hkajxnvy.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3zofjcjld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kwkkmdij.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3gddiczgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dwlmufah.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ssyaunpt.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3fmkbyqda.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3hngvjqhq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3icovfppd.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3hedzebpg.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3rfmbfazp.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3qkjodtle.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3fzfabpcx.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vyyxiosb.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3ciqhczli.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3ynpfezxp.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3udungwas.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3mbivrqow.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3swyshqvl.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3drakscgw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3yebazkul.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3andcogbu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vdgwwaxu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xfipjprr.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3zfjrfxuh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3atwwrbsk.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bsuhkyfo.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3cshlzbll.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wmtyhfrv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3fqkfumsg.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ixewfgvi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3xeunlgnm.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3axsxrgue.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3njqsdvuh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3axzzccgb.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3yewikuns.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fpabzabx.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3zaqduzwy.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3pndgkdzl.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nbrrllvn.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3hrguqqzr.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3wldldvzp.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3mocrjnrb.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3qealwqvt.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3qoisiblo.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3oovtvacn.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3drxkdnoh.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3utuxwvid.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3oowvjkkx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3xqcwnnjp.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3hjotdwgw.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fssjirxo.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3olrpcosk.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3nwkmkoci.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3dguxtbsl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3rchngtfr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3orbgjezg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3kwnljzmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sofppnzd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3fqyisudk.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3mpkkgvdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ievghzjp.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3lzqwosob.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3hfaliiuk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3snxckhfp.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3wiovbbmj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3proerokr.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3izszxvmm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3pskrknep.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3bomcdsnk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3gvresxxe.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3yuxzajkf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3jlhwfmtd.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3yvvvpeeb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3jkhmhwui.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3pgkaytsb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3joirnnpz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3htdftqwv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3zskwixcc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3jkcvcfke.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3tzsrbekf.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3tpxdqicb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3yngkmncx.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3xssiyzcr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3tzhtvyol.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lopbtqps.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tuxkslou.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3ccnvgtqk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3llgisrev.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3swjbwtwe.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3fmqxyzup.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3jmngebjj.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3xkxgzird.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3vwstwgre.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3qaxdrmer.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3iajglbbg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3arotmrsr.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mhtvquix.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3egvuejps.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ekxibcqu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3xohgqmrr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3lzeeywtc.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bbomiflq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3qxblggwu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3kespcimi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3mhbqtqes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdvhrkkf.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3oooaupil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hntazmvg.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3beujrbfz.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3iqsaqgfm.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3eeatcdnt.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qsdbbjsl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3avrpxdss.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3kchkzenh.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qqxxjvrw.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3coixhdri.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ssmyymjw.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3oxhotbad.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3qllgseuv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ptfirwst.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3akxiaqbf.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vtpllegd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gamllrtf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3sctyvkfr.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3zcumchvn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lhviltoc.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3tgabjkhb.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3tisahubl.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hvyxmvtk.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3epurkxbe.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dxgwwsnr.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qrghhkdv.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3ancaooha.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ugxkvskb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3oyirbgvk.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3uxqgnbse.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3ytdtoqhw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3oyhvutmm.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3rigxihkl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3kgzfkeiu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3pqtfhmkj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3blhdmbnc.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3fjczxwih.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3xugndhwb.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3btlvtqsm.html


<!-- 参考信息 -->