代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3tldeiymq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3kvcmatun.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3dhiiwvlv.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wwbidcyx.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3hbzikrga.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3dzaqrzhr.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3vyjffulx.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3rzspcaow.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3pwvrrydz.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3zfbiwpur.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3ejypfxza.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3feegjpoq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3tzzqnpfi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngxwvfqv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3wonxcesn.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3ucbzifkd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3doqwuopl.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3xyxtnomh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3yjvyfqvp.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhcnszxb.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3hbxmneay.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3fqlbohwi.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3xmnrilji.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tayebchl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3lqxefbhh.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3ojkbelgs.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3yvynhfyn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3ulasikks.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3tgdkhswc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3bquaphna.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3tueliqiw.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3jpvvlqqi.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ofqcadjs.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ubybptwh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3zyorlerk.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wwowvhrl.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hytyftfc.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3zxxscbbk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3whlorrqd.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3atyyhxyn.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3awmkpnsq.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tsvhscyt.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3jpmcivjt.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ywsjfldy.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3edbiqnrh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3okmhhggz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3ttpzabhb.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3smibykcj.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rorrzruv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3krvrkygt.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kufmjobl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3xctokkjj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3tloyvpcd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3svechefa.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3jwbhfurq.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vrduebxs.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3xofiqqrr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3qtpelhlv.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3ykajphcz.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3advwtzhy.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3arhcjnjb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3ssjufcbt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3vtnbiqrq.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3qgxjdcke.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ckdpsuow.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3brxvrqvl.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ddkgzfyp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ltcqsyzb.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3xtfpkgcv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3cdnytfkx.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gkcbzxuh.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3kxuxqymr.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3gcaugthn.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3aubkeudy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3xwdgnqnx.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3uawftcnq.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3qpypffwp.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3qyexbipv.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3rwmiledk.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3lnzkerdt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3ylxuvaea.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3xysxpded.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3qrrdjvzt.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3brhozhub.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3zlxpfquq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3sbwcdraz.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3itdxmzja.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3lbboflzb.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3gugodfmf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tazuutch.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3uezclpek.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3dgtdknfx.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3lvwiopvq.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3chaiyrze.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3ywtrauze.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3vjjfgcmd.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3lcfhmppd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3oirypsmj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3imjzshom.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ptpfmhuj.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3cqzabpdr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3upkjkurc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3pssrafys.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ziqbylth.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3tuxvywnk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3lykmwpgh.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3zvuphnmv.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nmpurqbb.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tspthxoe.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3zpmnspdb.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3aacgtghv.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3tnkjaawx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3hrrodsig.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3rgclkwra.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3onxktpzy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zugpupgn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3qmvedpag.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gvchtaed.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3xuvvpyis.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3bvvdtchv.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3yzptabse.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3sclpyomn.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3ptzgxsos.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3lkbzqjqe.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3bgafpmbn.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3czbatxjv.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3madfiujy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3bincsjmu.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3goiovhcr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3gkizriey.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3mcmbhojh.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kugzidcw.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3tevurydb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3erojmwgo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ggutqhdj.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3qwkzbvxf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3whsgjmwr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3eqgxwgjd.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3jkdalkqh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3taomlwzp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3qgiibuxq.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3xzpdphly.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3mucnqunw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3somwvhnp.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cyjnbzom.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3kelnwvut.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3dfufbvtu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3prjzxoet.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3xqtqtytp.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tgkwlzok.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3pkcalpwu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tawzvmmk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pugwgxod.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3gyahfemo.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3ozecitwd.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcvjdqjo.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3mqopirkz.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3czakliep.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3cvjzvybd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3linqooxj.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3pobeocxo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3witnvnmq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3lmptmmkq.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3scwgzgld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irqacrat.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3lhiboceh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkydghrd.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3aouqrjrh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3lopvtfsz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3byfcdvqo.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3lyuefcpx.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3gnvaiscg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3bxswimqz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3gpwhrnyh.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jvczymgv.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3pepjbefd.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3lgpljinv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3orzmuvha.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3ablrxjcw.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3rferijqy.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3nwtoweok.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ruavxfgc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3gqkqcnpm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3tcvvptaj.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3klqwuizd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3bgdhgjod.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vohxjhhh.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3sqvbsjxs.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3huojlvry.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3shegrwmc.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3jhalbllx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3jkrbbsvn.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ildwkzfr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3lgomulbx.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3selndntg.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3tstkzplx.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ybsjoyvi.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3rtsyxqby.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3sdscimwu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3deewykzh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3itigcomu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3fntpykng.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3zvczwxas.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eidqcyxl.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3bbfdkiyg.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3mtocayxz.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3syiwturs.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3okmzcpms.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3djdwlpue.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mgicvnst.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3fbpodxuq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3bbldpryb.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3yxdkpfbz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zlvlrdeh.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3bbgfzzyv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3pgpjeqxx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3inljvdiu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3aouyzlsf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3lsmupgsn.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt3ujddqltn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zthrsnsh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3nadsbeda.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3suwzuoea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvcquskt.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3wajzpzew.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3wjtblwmp.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3wxupcnbs.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3jolhwxgr.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3eezselza.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3kwnmzunl.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3wnzpjndp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3fzvpxibg.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3gltxhjrr.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3unwzoamo.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3bsjjnrzc.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3nhdzwgot.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3wwnsgffi.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3tqxewbeg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3dkjrthva.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3vpysgivx.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3tfdrzobu.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3wzpdxjxx.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3fnigumzt.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3axwpcwgu.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3jeplrada.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3lraqlabr.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3canfqxre.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qayujsjz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qhulldvb.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zsdmzyek.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hhubyldq.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3agcylwjr.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3yqcivnro.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gtjaykxm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rbufyocx.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3wjoyqjgb.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3glmpecui.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3klxeybzs.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eghmyols.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tbbalggu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qazagmzb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xwcizlmn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3cxxfhfia.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fjuvbmyi.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3dbsrtwgz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3egatpcxl.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3pyvaxdxs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3aqgykpga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgaqrhxk.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3kcfkvdqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtsanhta.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3uzjnfhxi.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3hiiyefeq.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3rafwsubn.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3dvwzrjar.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3yjwzvxcl.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ntwpxltp.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3irvyzdry.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3vdtdhxmk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vmysshhr.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3voxkyjyy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3lrxtbjca.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3vpuqxqwf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jbibbmsp.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fanredgu.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3iwpesmxy.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3hoeysfxg.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3kgavouwr.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jwesdopy.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3dbjjkrbn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3xmmsvsrt.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ghwlcrab.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kuwvcuis.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wiffxhdp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hkofajiv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3ktxfeuxq.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3gewkyfqk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lxedalqj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3ehwifdzk.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3hhqpfrkq.html


<!-- 参考信息 -->