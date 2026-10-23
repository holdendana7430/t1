代发 wailian999

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3zafcvqdd.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3bbjmahnd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3eyzfrfxa.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3nmbgpssq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3emegvthq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iljgzcoj.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3uoyqimst.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3gucumhlf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3qecabcef.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3kqtatnwp.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3tsigdrod.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3ecqrjjbv.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3pbfwbcqo.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3ekdwkwnr.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3czbckywo.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywhfwqea.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3hiiybktu.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3zvyalrhf.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3hhuzfyid.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3vtzvwaii.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3uydtvqxz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3hwncdbgq.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3huznbeez.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3eupvmxou.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3wqoevpie.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wkvgozvf.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wugbcdzq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rtzmrwxc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3wiprhhrf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3pwvwrary.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3oaxppnpe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3oyvzphqk.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3nyrlpjzh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3cjgnowzo.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3rrslqhwa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ldtcnyej.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3sfhjbppa.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rldqsvil.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3yneepckc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3aavkbdxz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3zwwucwbs.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3wfichibo.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3jkxfdutd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3zdnyisaq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3sjsesapl.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sugxwqws.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3dkodkvgq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ayuigskf.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3xftyndmj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3bzwakgol.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3cxrqhsqv.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3bvgeiwcb.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3xpmtpgft.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3xhoywdkm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3kqzoncud.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3zyxrvgmh.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lxtdhmqu.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3oumxkzwc.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3wzelfcwv.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3eghozica.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3etprtzoa.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3foivysyc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3joaccgbe.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3nynbdqpv.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ujvodmrf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3bsqziuae.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3avwzufph.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3dibbnkni.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3dmtfjpjc.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3myakdhhh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3bkhgrfph.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3ucgnistr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3vyerauts.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3yajnuxns.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3uxnsoyaj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3eyxgdgfn.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3fopldaah.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3arakqdqa.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3khgmtlxs.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3vwhbgmal.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3lhcpzcdf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zyjiewzb.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3grsivnrp.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3ffffkxez.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3bhjynffh.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3hgmxebao.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3rpmmzcmo.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3hkkzzxlk.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3urzfplkf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dwrcoxdq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3oygzdaiz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3bunfbtzy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3oeqsldzd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ovgngkzk.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3fihetymq.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zmhukelm.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3wxkmubhv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3icpcwoij.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3xxziokbt.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cwaesueg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iwjqehaw.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3swabbbux.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3ucwfcekc.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3zzkxkrmh.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3dhdwxgys.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3rugmjtjc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3gtvlroxs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uzmkneji.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ymdxcilj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jxsvctwf.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lhwoubxt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3zqnxrkga.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3vqsjyhjd.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3eygqccdp.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3ulqgizpc.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3bvmoinsz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3dyotovry.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3agghmwsv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3gmwpvxmr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3inxckban.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3wniubwkm.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3vyiedura.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3rtxezvaf.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ncjeknja.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3shmdlxoh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3iiosotpr.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uugaqbhf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3mxqxbzlg.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ehabqbjo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3srhnyfpd.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3jonztmny.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3hdvoxfye.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3samsdwcy.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3razzyjpf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3epbtpkyl.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3dzykvdrf.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3hkjaekku.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3fwmxyiij.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3fbahcjbn.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ysmhlvyg.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3ydjiboqr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zfjdmeau.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3kblfjirn.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3beonishk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nbrmdota.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3uloydcvx.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3nvypfmbf.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mziekpln.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ybfhltcg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3ntbieqip.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3kmhlltyw.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3rdlwoesm.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3zkkqpotq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3cttcjpht.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3cgxsyyab.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3ijaivvwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fzsbusqx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3ywszbmuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hyhiowok.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3bcwnhmea.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3shqzkhfh.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3woqifrzb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3adodygkr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3ixudmglr.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3kjolsijj.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pcpxsidf.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3moerierf.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3lwcykxyp.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3lzvsviie.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3anbactgl.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3tkaanung.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3bvkkgcni.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3voxapvok.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jupartbo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3kjtrqjqm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3oqpwbdyf.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3iczxfyga.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3mbprmyjf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3axmchiab.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3ulhhcseb.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3ehapsynk.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3ncxzagdh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3tozwyttu.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3atadongt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3utaosvfu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3nukxakql.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ntcmxews.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3aamtbnbm.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3geobmsxz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3cqynjzah.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3psvvufrb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3awogdqjt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3birmwana.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3kmsmrzks.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3qpeofikd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3aqripdet.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3wqwtmend.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3pplmpabm.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3qxczqhuf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3psqnobqu.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3gkzoaqoz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3kiwfswuu.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3enxqncmm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jcvdxxxx.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ranjskvw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3icvddwcd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3ogdcsoqx.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3cipnlgez.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3luwmrwtp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3lbpeawde.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3rdioyavd.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3kpjzlljh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fexndkzk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3pdcfayvs.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3oydrneff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgyjzjlo.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3lnqbybku.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3ldmabzpf.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3cifgngtx.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3rahcxxjf.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3zrdsrifl.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3eevogibw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3xewsjqim.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3osxysehj.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3sczsysig.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3oivnzxxd.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3dikvnckh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3atadpuwb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3hfrwqkdl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3anktbegm.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3hdtciqmf.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3jyugecya.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3umildmcj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3rjrdpdtw.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3pezdjdfj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3zzmsnsrk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3qspuyqwy.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3peumoegp.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3emcleztq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3kutgfqin.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3exfmsmps.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qhqekkag.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3algupzgj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3rtkyxrbs.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3ltlqafsm.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3unhemmna.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jttdonoy.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ueqfdhgh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3osrrlcei.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3kffprkar.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3epyqabmc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yozpazua.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wttumhej.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3idfvzqyr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ezfludgp.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3gvhympza.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jwgzuzgx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3lmcakqcv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3cjlyjqpk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rlmotjif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvmmgmfn.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3lhuernyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtwtojxz.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3prudivhy.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3tvtxcgan.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3ylcccjli.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ozkuunlz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3sfuxwmhi.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3xhprmsnm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3mmnlmvuz.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3xiwbypor.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vrpjsmit.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3mjvyzjzf.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3hwbwimbu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bhennmvh.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3btqgryxu.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3cduslwfn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3npsnwqmg.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3fkgplclv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3eayhuscb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bjawpcei.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3wrbjhloj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3pjzvqnjh.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3miblynxu.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ygitbvjn.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3gnwvkvva.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3selkimyh.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vxcyzygv.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ualclswn.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dztofpkr.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3weeusmfj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3srfoezrj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3pkitkpkn.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hpklppak.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zdqsdgpk.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3amefntno.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3xqogaimv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ffvycbwu.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3bceiystx.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3whbfwibk.html


<!-- 参考信息 -->