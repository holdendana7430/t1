代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2zuowzqgy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2jmygvltu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2frbnpioe.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ocfzdpqm.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2tqsotlvb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2yumgnufi.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2gpeybrme.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2zjytqfrf.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tyqjxrbn.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2mjsdwzbs.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2pifyujce.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2mxqhsxia.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2tczyzuzb.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vztreksu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2ckrjmwaw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2rwtuqbki.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2lsdjzogu.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2afeodshm.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2gtcmraim.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dinwjaxg.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2bedaienj.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rfbzpqff.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hluufrvg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzwtrvlg.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2lsswmycb.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2wdjfbxha.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2bgxmmaes.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2vaxppagk.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2vmzozbhq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2eejiapfp.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2gzdibdfp.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2eeyenfht.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tljguwcm.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tiquhegi.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2xnxgjviw.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zbcdhjou.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mgxewlxp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2wdxekhtl.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ldqdgfax.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ygejzxqt.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2egwnrahy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2iottjafv.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2weocsjmm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uuxfhmlj.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2uytslywf.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zfrhvwbl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2unryqajl.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2qtsrcvum.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2hfzcchcu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ygtstfaf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iwgfhnjj.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2gufzpteh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2wtgkhtaf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vrjyftic.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wsusvauc.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2rysocalu.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2gvvrwkpd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2glzuvhxo.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2iosumqia.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2vmxwagag.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2hdbtnvtu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2noskhazi.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2pisgyoju.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2jwozzylp.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zygerqhn.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2tcorxqqz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2yqfrtcuq.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ussjwgux.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2ukheonpt.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2tpezlnky.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mpoxrgbf.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2rbuduizn.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2kfsjylyo.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2msvsewjz.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2byvxcbya.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2xeafbwmv.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2jzgsdhrh.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2zdaycjlu.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ouxbkkkw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ctyvyvhm.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2margmtaj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2wuxqwmqo.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2pxcpkjpr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2cweypbit.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2dinormiv.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2zhgmqrdo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2xxazxnen.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2vkhvpcbr.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2statjukp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nxyrnxnz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ihdvmxkn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2ohesbvlq.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2hftayjdz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2tavvokae.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2lqichiot.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ihzbpmxv.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2gjcpmdhe.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2yjvlplii.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2xzluqatn.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ymfsjhbh.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qprqavzi.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vilvbotu.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2djmzlawy.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xlrxryvp.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2onnvqlez.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2pgmeativ.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2wpweweic.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qafgegtm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mcwdbarh.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2oifemzic.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2bkoejhbv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2xftkhtnh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2fplubmxj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2wdvyxrol.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2scpdxnpq.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxqmliac.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2ftcydhvl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2sgsdzszm.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ndjsvjyk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2gkxzscew.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2grgptaol.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2pozowcry.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2qcdgsqyp.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2nsedntoq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ckuplydi.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2tafdndhg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2qudwsovb.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2thhesbrs.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2pzjpqyjv.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2ojebzoot.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2vgljmyox.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2cawwlvbm.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ncogkihv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sugevuwd.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bzaczibr.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qatlddld.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2objsjkym.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2jocggbup.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2qrmmkqpx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2lptkzchh.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2nfsadjnl.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ikmqhnlf.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2svvtomgq.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2zxmirzqr.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2koumnjft.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2oeworatn.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2xsvkdwim.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qefuhssd.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2wcfjnfor.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cfnmkzio.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2ckhbsnqz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ieqghuwx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2oypzmmop.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2emdrfbak.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2zicntfsh.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2iqnpigrf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lrivzmbk.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2gnyafcqj.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ykcafamk.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2jecvpbhn.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2enpkzsxq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2qzowhlon.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2bjljkyor.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2twpzumsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkbvwchd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2acwpqynl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwmgrhqh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2vteawazy.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2iuwwrsvn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2xnynoknu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ryqlosnn.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uwbofhvs.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2brkczchd.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2opjhsovd.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bcvbhfpo.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2voktsvpq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2gtlxjyuq.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2gddrcztm.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2pntqxeaw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2qihuflzm.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2oqfrpyrk.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wuxxxitp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2hslhobrw.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rfngreuc.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2jguvwoiv.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xunbkexj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2jkmerlss.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2thrukzht.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2yvzbrgmm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ndtbwqpl.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fuxvhjdc.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2fsfydgag.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2rltvjgaf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2paqiqhpd.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ioigphwk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ltyhbyam.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2cyezhnwa.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zgernqzo.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tynemzwi.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vrimjrnj.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kbnflhii.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ifxhbyit.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2rqzfavhq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2csolrtdf.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2raqmnbxy.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2mmdyulwm.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2eajynpkg.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2ymgidmtt.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2kxqbezqi.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2rnfcdmhl.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2bgqogaxl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fbacexum.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2pmlotigj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gokmpakh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2zhbcnuoa.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2mgalngon.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2nghrafac.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2ipfjlapm.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2efwoctgg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2izmkkacx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxnobkgn.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2mzwddhvp.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2twijqzsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otughxnl.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2jribsmee.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2evvghzjq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2mtpwcbsr.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2shugyybl.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2rwdguswk.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2ajwmawaw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2clqvfsws.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2zgqpynqq.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2xsqcjsnr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2elqduvrf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2lhaspygo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2ndlijpiq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2aajupwju.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2flqebegb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2xhlnmsrg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2ummcogci.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2czruwcya.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2qmsctcmp.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2jdljfiwh.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2widimuur.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iavxtvcd.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2moquyzzh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2fjwtqalh.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kbevnbny.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2bxcaqwec.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nofrxjlc.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pqoupben.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2yjdysppa.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2xutfwcxv.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hpuohwwt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fgopbwzk.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2oxmhsvfm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mxubjwli.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nrnvywaf.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dkxiszxc.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bsvgdcjj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xpsjnsra.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tunyzoar.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xzaenpbz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mhoiiwga.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2czijucie.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2gibraxxd.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2dytdplyg.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fxgulndz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slfgxgnb.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2nwyxjbei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jgowdqqf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zrrahevl.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2dfkvawvk.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2wwmmrkob.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2jcxyxkoa.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ewsrqjgd.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tnpjgxch.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wslnwuuv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2ysrmouty.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2pmmkxemf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ignffjpv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2sydhybak.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2ycxavmnd.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2layyctcy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2dcfhmavy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lnfqmawg.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2fwyedesk.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2lzohdatt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ylokjawi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2yixfbxwr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2uircjqhc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pxybkjdq.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bzlftszd.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2amrtsxob.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zdscztmz.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xkdmmwan.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ugmrvyhb.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pgihynvb.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2mxefirdd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2lmburvhc.html


<!-- 参考信息 -->