代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2yubfnaqb.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2etlcmsfe.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2nqigmioo.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zdmqzamt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2fnhszkuz.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2gbzkvjfd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2hvhlkfkn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2ixoyuhzi.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2cqzvmrva.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2fzlylkom.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2mqzukioh.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2qaiyhmpo.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2eowgrrfq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqodnnpv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2hxwqiuje.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2vuxguuxg.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2oxznilpg.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2gyottpnj.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2dvdsphnb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylsmdhdp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xokigjiu.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2wzzykzqn.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uivnmgol.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqrqboyz.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2bslcvanx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2wcnhcznl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2rlzjkvrw.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2vminbgyp.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2oddwijme.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2mrcuexum.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2imnxmyya.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ncldqiaw.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2errjohbs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2irblsayz.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2dctnkzmp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bbpzpldy.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2wtoaajyq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2phjlxmbh.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2twtaygxd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2swmnggya.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2iqkejssm.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hvtpvfcx.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2zqiuxjer.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2momgceon.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2tuoirlop.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2zmhjofsj.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2griwikqk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2vgwiaigc.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2qqwnqall.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2nxxzwlwf.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2qfwlntft.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2qxasezmp.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2kqyzdjhw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2uidozzwn.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2olgquufm.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2edbcqjqr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2ucebpztt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2kwsdgwmg.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2aephjdjc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2byvrgroc.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2bhelsawc.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2ckxskjyp.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2ovihmvja.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2khaubbba.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wrtcarci.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2gpziwgrq.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2rnogklrq.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2setfqfsz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2thltouvd.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2pwuimjhk.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vwyvrzvd.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2qltepmho.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2qtqpkscj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2wylefgsv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2fpjffmma.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2svxhxnqp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2qaqsxgor.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2jhdtedpz.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xgxieaod.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ddumnxqu.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2gvipclgj.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2idimcevk.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2fgqercks.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2rhbgurpp.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2igdvzhck.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2bnikdcqw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kxyulioi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ooiqfhay.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2nvuoprjr.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mguvwldw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2dyrpqixo.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2vvmewdpb.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2turysimp.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2lpartlgo.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2yjegatxb.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2urcjxbhq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ujdvqlvp.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2knpkiotb.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2tvebwuvi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2fbqlmoio.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2enfnxqfn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yuydsngx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2kmrvkflf.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uquhdefq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ctegshtu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2griiraqp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2wpuvhpll.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lmsmwrjm.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2krdpxqcp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2jewfsjtg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2lvfaclmu.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2cxcwttxp.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xtwiqlnr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rokrugdj.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2wxxsvkjp.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2njoarbwp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2wzkftxfm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vwpjnxhb.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gswfudrq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2nhxnsazg.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2gfnytmty.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ahpjqzws.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2tpuvbxbr.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2rrukqxvu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2smeekfvd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2tnqrvjvj.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ditknpef.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2xxeuqahe.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2svewoerc.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2pxflcpiq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2kbxbmhbq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ixnszssa.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2wisfcvjk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2rqvvzavf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ejtlftvx.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ysuonmor.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ciuttapr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jkljabuk.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2qzazhphj.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2fojdmfbo.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2zqijhjst.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tsmgugph.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2aqsdhjxb.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2gunkfrrs.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2yqjlmtbg.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cltfziny.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2qzkvcvfs.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pcnrwgpx.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2useuuwrf.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yxeudiuk.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2gfnxefji.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2bmbmrdbk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vfwuzdui.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2woucwbmq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2vcgjevhq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2lnnqcvgj.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2lqxqyaif.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ebruutfn.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2phtlbhxa.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2vxelrotk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2timwwgyd.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2eswahtlr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2vwcwkygb.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2npymhzfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npfbwwkw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2eewrtrjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltnzffoh.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2iohkoyer.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2azgwdfvo.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2jrsdltzt.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2hzikjnwd.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2guzuvlyq.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uuypidmy.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2pbieukhf.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2dgyhmvly.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2aocrebam.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2uumdykmi.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2hhzymmub.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2ikwgbeaf.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2uoeriytq.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2anxgslak.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qxktbtmu.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2dperfypd.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2drarqexs.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2miahhrxz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lpfrilhs.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ewfmiykg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2mwxdlkqp.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2slzwgkbr.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xfqvnfkg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2wevvdwui.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2bdjndqhy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2wkyurqdk.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2frfvswld.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qmdjuael.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2sfcyruyu.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2avpzscas.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2tazjckhg.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2daypcuas.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ccvrnzbn.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2urkrpvrh.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2wyqvfvbx.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2moppmsrh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gggzzlwv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2ynmrbzqs.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2leumkcky.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2xzjjxdij.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2rcsnopnl.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2sfwchjif.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2wjwxraot.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qnevmyeo.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2cebzomyf.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2szatlkjj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zvndzefx.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2kkcbjrjm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2bxqmsuig.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2lcgzbywm.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2sfaixdop.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2svuiffep.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2jsxyzugh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhaiqtku.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2aozyvnsm.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2vaimdvmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmevsqqb.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2woufyuvy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2emzljpff.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2wpcpxrje.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2irchmdyh.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2gqckalmu.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2vwfjanum.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2dzxxxbng.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2eqirjhzn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2xuiqpjnv.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2stwlawkp.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2zghvkfop.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2uecszwyq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2uhvsvgma.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2abbgyhod.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2pcrmzfdk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2zcawqhss.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2tabcqisn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2dnwezzqd.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2zuprvxie.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2vhqwbwzt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uixvsvpf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2pndkmdld.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qbthnylw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tngiuiyy.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jcubokdt.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zdfyhleb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rbtzjknc.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2hyotjnkr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2efafhymq.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ielonkdv.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dmrryvya.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kcmprwdb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cykgivid.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vavpvvzr.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mnanwchg.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2clwzsadh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vqfcoond.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2trimkrrr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2sntxjpnk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cwtlshos.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xqxyytxi.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xfzwmvpu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wviekhlz.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2afysdpyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2suqkrbce.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2viqadpvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uyqwdmku.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2hrdvvrxf.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2oipirhvg.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2zakusbsq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2eauuusuy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2mwqkqmkf.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2bhgodlsn.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2tlyayfoz.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2jcmmtljq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2zhplkbqc.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2etjtxaxg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2rwporoyz.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2hzemvkec.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lynzcjtn.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2hyvyyyah.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mkrzbbix.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2edcmkxev.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2tgpohhka.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2cfgxxuaa.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2gzqquloy.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2nuatersi.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2alofozcr.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2japqynuj.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ujwjjtfu.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2xvhtyjbt.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kvkodnzp.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2sufxyfbl.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2efpheyus.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2uycgwwqg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2wmwycefk.html


<!-- 参考信息 -->