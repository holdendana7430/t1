代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2svqnrhmg.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2xilpqpqd.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2ltvsbiqz.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ilegncrp.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2yxwahjuk.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2oidtbaiu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2ueszchwq.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2wfvfbtlh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2khiiruiy.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2iyyybhmp.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2pounpspg.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2qlmvijza.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2qcrbdosz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2umxgmlnm.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2zjmxxzav.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2dzvbahoj.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2focwwnbz.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2azszdinv.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2xvzufoei.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2jsfeverg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2guarztom.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2rothogvx.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2enysokqw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2ungsmywf.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2uiwwoydx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2ciesbbvu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lhzhldpk.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2wfzaifvi.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2pejxpwrf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2bcbgotfq.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2hqgeusnx.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2jhqmnpzr.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qanuxhja.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bxuczkuh.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2aaqljikg.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bdelywaw.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gloetzai.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2iaoyaqvp.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fchzlzap.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2blafcnca.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2czogzdob.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ugaxcswk.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2tqxczyth.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aatqdwfw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2xxfwejpj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ydnlrrze.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2ohnaltcj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2xnlawkzr.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2khlmwyga.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2capkwboq.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uhsglrhc.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2fgujogzb.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2bpyerkcr.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2refrjuwm.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2pirauaod.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jlrjxteg.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2watvfbqp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2gywbiwlv.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2cdawctwe.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2kafrtsig.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2jncmynsm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2zclsqjlm.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2mejnpbec.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2dwmzwsug.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yprasngc.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ovfkjrds.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2cyjsagwj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2szlbftbr.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2bxrkbwul.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2jnhyhpzb.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zbmvvlyr.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2wckgrodx.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2spcbbslb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2dimdsuwy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2vuwtpgbf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2akabaqza.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2sbofcfyl.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2lqrxpzak.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ppisrrbe.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2llyaeuri.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2ulqkhwlt.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2maszkafa.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2omzwtfdx.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2drkeesgi.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2yydvowgk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2cgwgyzuk.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2wauopbir.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2pnvyalts.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2bnrofzil.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lkjixdnj.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2bjcsyiwm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2jgzgrjoc.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2fmiylpbf.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2hmkuurbe.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2banbdlxu.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2bluyohut.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2cdfipqfd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2ujjqwgfk.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2hpobgiyw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2yzendznp.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2uxagejco.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jbridmcy.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2tzyrubgr.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yanufoin.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pkdsxaob.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2xuhdmqen.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2irwvrjsx.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ozswbpvi.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ojmnteor.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2lwrpmibt.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2irkyfmez.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2errmptuc.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2zatdklmc.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mvqraauw.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2xbduhboo.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2czdllgjg.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2wbbgimay.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2numzcslo.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wcmdkymf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2tctkkcke.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2qojasnnt.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2jmjbujep.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2kpmytgqc.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2vvnjyrpu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2tgwepbvs.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ycyipudx.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2viqfgqvi.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2wytmyhpg.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2pueplhuy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2taggzhyl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2ghltgwwy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nvadzwtw.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2oyylofhf.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2iekkoaae.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yettfwqp.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2fqacwmya.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gcffkizd.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wyshlotj.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2wtqomlkb.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2iqxnckyz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ynjjuwrm.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2baydwfjn.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2ruoecdbw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2zfboeibx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2uvzdhysr.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2pacravhh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2lxuwkrsv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cinyiqeo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2awajbtpi.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yfpuscbc.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2yomjavgi.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2azlffebi.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jxcklray.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2lxjxypkd.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2qwyzxsga.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2fwvsbttx.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2nivkjfvq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2ffqfkygq.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ophrulen.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2fmhphjjd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2sreezxwe.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2bsywjpur.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2vcetzpjk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2ljyidjzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmfdkcyd.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qyunhcqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypipufzz.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2owufopid.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2aeebufkx.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2tmsbtkjj.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2lywyxkma.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lsrnellj.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vcuopkwm.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2feeiqoct.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2bffeuhlh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zbcjeaov.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2bvtnwmrr.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2aahumsme.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2rufxbkjg.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2qgrjufdr.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ggyothue.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2doxlfxij.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ciggyhrw.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2njrrgdwz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2tcdmtctz.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2unwhwylf.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2gwwnfgrr.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2jvbohzch.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gdtcsxuf.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2lacohutx.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cabjeove.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2ylaedgup.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2fwqfmcxa.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2iyalafhi.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2hsdeuldd.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2tafhbpno.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lmnotkhl.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2hkpcpkfd.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vjwemezr.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2opigcrdv.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ybwijkah.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2gyufqxyj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2boziqssx.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yqcgmgcv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2hagschjn.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2eeirtqzv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2quihmifl.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2bbktkkop.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2arrlcosu.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zrglbafx.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2hobybiro.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2lwbrxoxn.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2bzmaygvv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2apvpncxd.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2tqkrnvui.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2xjzelman.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2nmxiryqh.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2sermlaha.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2iioryafg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2aqxxwjwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ighblafc.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2qynzyhsg.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2geihwauz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfhjumwm.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ttojrovj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2xyjzzxye.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2dzjrumre.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2eyovmacu.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2nzvggowg.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2pbelretr.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2fqvctnoj.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2usrwmltl.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2wcaorrly.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2yvfpheha.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2nyeevuzr.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2jvryfmtv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2chsahniz.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2qaikqqsb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2jspmuacx.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2lalpvipi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2bevjfrac.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2nzzhmnvr.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2ofokzdis.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2decrikms.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2pwkhtcqa.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2xeuwwjfz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2izqgqzaz.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jrykugaf.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ynexhtbb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pahviqvg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cuwrypbv.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tumuduld.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2omrkxdit.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2yedeswnt.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2suaiqzav.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mjmcfoit.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2cjxgujgi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pgjkblav.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wurvycgt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2upborrvv.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xljyonre.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2yklqqcbl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2hkkzekfz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kadlvjiw.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jbbhithw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tfevcjqt.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mrfsswgi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2deajpkxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbwdwhea.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2vvmnymig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnscczhv.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2gtkmfjwp.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2cloyvpny.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2xqidlkgn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ptcxuwvf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2phxyuyda.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kphuigdk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ciqxbafp.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2kdsttysj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kivsdave.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2dfbabzyz.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2bmgcpkte.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2flttkoxk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ontqfumd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2aomgtoyi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bxrosteq.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2zxrziulm.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2ijpsvzqt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fzqdqern.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2dpvxkmya.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2vpdjvkqt.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pqrsfnrx.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gynfjyll.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zmmtptxt.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vxdxzrnc.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2ldjpnaxx.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2delygugq.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gseobkuv.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2kotwqfqn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2acrvlgei.html


<!-- 参考信息 -->