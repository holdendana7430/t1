代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2aqflphay.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2oegcimun.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2xgqbrbjt.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mvzuzruh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2rpizizca.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2jfinpwzs.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2smgqeaev.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2tmdtazjr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2jcmszjht.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2uxzykfsb.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2fghwhhwj.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2uvcqepzx.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2qnjzvssh.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2exdcukgp.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2dbebrjst.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2gaykabnu.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2yqmvahrb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2cleustvm.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kjwieufb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2nyhbroli.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2yeyfsgye.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2wpgdwidz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2guwqkoiq.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2xdiifzyk.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rsqnfvxt.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2ibzwpzqd.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rzstgncb.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wueeugny.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2rjqotadc.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2rrjvlmuu.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2cdqgmstc.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2eohqpobr.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2bzlkxroh.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kuwrsvtv.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2povsvoet.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wbqphpur.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2awpuntnn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2elbjzyns.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2bnhvpwkt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2ffobrngu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2wudmukrh.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wxyblqkm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2cyhazphl.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2obxjaebz.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2hshlifen.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ndmrfwzj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ptctukpx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2wffidnjs.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2bssomfhg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2rohttzde.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2vienucyq.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2mfpjnpat.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2auuwfmmn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lniwgssd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2pxxuhust.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2yznwpvkg.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2sjureemt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2xienrzby.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ojlxcuou.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2munshlbp.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2hprhzxhs.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2khaiingy.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2rqqbywus.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ewhkbpld.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2uvzwlvzk.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gpfoweom.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hnexzbku.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2ifzxedmq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2yneloxdc.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2sqoewrky.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vpsnxaej.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2mpzgxmxj.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2jzdatlqc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2shbhogvl.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2lhfxckji.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2huhsezbq.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2vmqxblnq.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2hwfvplpm.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2avttfwxq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2zuitmwtv.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2swdtybil.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2tkbtmekf.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2prcibqbb.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2spwnrhuz.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2qyqbkwug.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zzecphbw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2rtxrwwww.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2sflalvcm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2yheymcpq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2godcnzms.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2ququlxib.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2yklulpzm.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2ynpscyby.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2qrxzxmoz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2kwhxtvsc.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2mtrrmsdq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2oqvedusi.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2avdscfmp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2cjszqoqj.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2bqcrpemk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2efpvvtwn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2geiuhsni.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2nulnsryt.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vzoffoqs.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2mxwazkei.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2xohdhjuh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2befyjdjs.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2avbvpcsi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2gkbehyel.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2nsojjxep.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xxsioagx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jmbuqtmd.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2srmtcqwt.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2jyoevtwc.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2gkaxnbmf.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqjxvnan.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2rjxyaabw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2apwnfycw.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2apxlscch.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2jksctltp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2pchxxkam.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ndxvhkdu.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2lmrnrdec.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2ojtdsttd.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2fcimlvrn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2tzdbdeuw.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2xleekurq.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2rrbaxtrb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2piokecza.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2yhsqybjw.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ihdlmcbn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rlnmaqaf.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ouktvwpf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2sktjczij.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lavdvtvf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2iguqatmy.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2qdsueszt.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ucvhejkb.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2tnhkmgmc.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2uksvkiht.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2iddwtnfr.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pzshsepd.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2uniqeoex.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2acvsytdh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2vvwnzhza.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qdaluvpy.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2sqvddgvz.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vzqxhntk.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2awqebgri.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2voenylxg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2kpiontob.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2osmlongb.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qfhldsqv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2nedsldpv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2pcbkjgax.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2uxnayxgd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2hiciqyws.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2fxrsxqda.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2idzgvped.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2xabzodac.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2znqvgixp.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2vtutjuxz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2vqrpsjia.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2hzxpyxog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssxszbru.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2jvkgjnqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwoxjyuw.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2kfmduara.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2drcowusz.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2bkhyecvj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2lkhtcbie.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2djoiuoau.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2fbwrszxn.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2oayijofs.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2wikpbzsg.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2yggxsepg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2hwfcaqqm.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2zddybism.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2mckjzwvo.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2lbpruxhx.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2puialisn.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hfwcdkle.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2thunqepm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2xnyzupzp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wbhrpipp.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vpcmardk.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2pjbawvlu.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2meufrvur.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2biiiyqsd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2itlsijjx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gvemolgo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ibmihpis.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2isswaagp.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2uaalqmch.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ohypohiz.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ijabtsgu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qsinedlc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2rnoojoxd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gvmzneyw.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2yonnzspl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2xazexhnd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2melxumlm.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2lnrwjvzc.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yfxbslkc.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2ubfuvqay.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2nirlcqkx.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ybaszobk.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2czmlmnba.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2wszxhsgh.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pciopekx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2mxjoiexo.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ovmpgicr.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2ttdagqrg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2egkefolc.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2syhytibe.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2ylagpjen.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2qptuttgc.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2mvvttcmh.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2jqujhwed.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2iennfseo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cnmyqwxt.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2agudhhuj.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2mrnqfygx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrajoltb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2uhjotmak.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2wlqjopsd.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2isopcvfb.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2ulspwdtz.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2qyuxvdjm.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2rxyfvlvc.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2zjgjsgrl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2dnzocuho.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2xqbwhyqd.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2hxszqqnn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2nysdddbn.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2gnjrgemv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2jpbyyawp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2zywmawub.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2xfefobtw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2jnvlocqv.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2pjzsadbq.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2oqetxbro.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2mrlrhcdq.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2ztzdhfni.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2szdreieg.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2lsbaptce.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vcfgpgmf.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zsomucve.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jkpstpmv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2znojgamu.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2zsruqjgy.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2nuovgmtt.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2giomjepl.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eegfdcrq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2knccpluh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2isdfuono.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bmlyvoyd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ennkcxvr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tfknblmk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tpfpeojd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2onifllpr.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qbwxnucw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vvgzjcfz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pbkuqlwa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2asgixssm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2tncmmtzz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2vhcwahqt.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mlnwajkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpxbcfht.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2sqgspgpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwhgmuqr.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tpcuclzg.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2acomhnfe.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2vhnlvymp.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kcjmsxht.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2nnbtvorg.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kogmstop.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2voayknex.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2cdhrmwqb.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2sgioazcj.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2bslmjexu.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2abmkriqg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2eznzgzwk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2apuddgae.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2yptowagg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2unkmzsed.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ayvevwot.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2jdwoatqh.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2eaokusgg.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2mweizghc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2tnlopamb.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wfajtnce.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2srycwavd.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2umngmecj.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2osflwuti.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hyxkhbqf.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rsgmjank.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dkpknrrp.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2gihmqlbu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2yygadfcp.html


<!-- 参考信息 -->