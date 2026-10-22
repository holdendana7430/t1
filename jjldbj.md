代发 wailian999

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2bworsjyy.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2phmbtxqt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cydmqgwi.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2svtxrvyl.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2etfrrxks.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2kutgqxnt.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2wujkkgfu.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2dobbduku.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2milfdzch.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2ywedaosv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2rfozgguk.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kyoiixxt.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2djdrqsyl.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2ittjpsup.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2fvyriqvf.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2zvfgadoh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2mlspurkf.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2fwcnkiue.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2wweeexsd.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2dtvzybgg.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2viinxbah.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2afrolcit.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2fzlrbhmp.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2wecocchc.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2hdzguwpf.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2vvctywnh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2rqgsdcqf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2tkbpwhmg.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2peezulry.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2rivxbvie.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2qogkahui.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2frdjzwgm.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2cqkzdhaj.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2jwgxeipn.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2whunnkms.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zyxxvcto.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2hkqovptz.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2asehukjw.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2egafjayn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2ivmdfzpb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lvlwoarj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gbqvxdsz.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fkwvuiov.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tnsitkvi.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2crnovzwd.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2olpblxkq.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2zotxtgoz.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2egnyaigu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2zlobyayw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fdmmfmyk.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2eeqizfxc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vzeajptw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2prikegxt.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oakzblom.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2naqevixw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2tkljhddq.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2ulqxbvab.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2hkmocwmn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2citptyzm.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2aadpyixz.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2rjcxhkkc.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2osyhtkyi.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2nfbwomfg.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2yeklogdy.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2iwhtanlp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2kmqnifdc.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2kalfoodd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2homjztwg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2njqfeabp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2vvxmwwmd.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2xskswdrj.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2kwjjsctd.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hoiikxgo.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2monlnoho.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2hyqdevpx.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2dwwgxeii.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2eokjiocm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2zviatrvo.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2crojxklv.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2nfrnaczv.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2vnwywxli.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2iterwzcg.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2xpnchbtn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2bacmsepl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2readygyx.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2pbqlgrci.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2jqwkwrjj.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2egpeycjr.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2mqtgqbsr.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2gpvfusux.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2tkqittzo.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2rcdpglnm.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2dvsqdnsz.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2iwzoeego.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2kdfzjkzt.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2htvsujwl.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ecewhima.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2bwoytusi.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2bopbzcoa.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2cyiymfey.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2kqwatvok.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2hafsxmpp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2gofcebyj.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2wafenisq.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lcwxeqnz.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2lxkwpzgw.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2exppviht.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2lippuwjw.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2rthewbna.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jktxsdph.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2wtnlnefp.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gxuniwjc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2wskclmth.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2xsjmzrvw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rzripwoo.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2obobycgg.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2kstqusqm.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2tcqfbdbq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2dhnflslz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gfkxnnrx.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2hbilmgnj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2nusrpdkb.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2onmrpwve.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vcrruoba.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2zvrytgwl.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ekdisdug.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2gbygvrsq.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2xcgcgutj.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2wpoviifc.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ntmtsitt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2vghkcfdk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2benmbxmi.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2dtupuhmn.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2dwikciws.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2lzhkgjvv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2mrnsondn.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2hdmkrnpt.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2znjvgzwr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2nfapqtdj.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2njftkhxo.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2zxjopndr.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2bbsegtde.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lqkchfcg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2uaaeehfu.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zrnjuryv.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2blqpheaz.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2twchyaom.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2hljumigp.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2xmaypxec.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2tdxkkldi.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2kjfbzcon.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2woyvgkfl.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2wqcbokjp.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wzfsbwom.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2wjelfteb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gfvbpljs.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2ymxftigv.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hcczfkkl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2qbobewib.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qhddmvbl.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ljzbbwxu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qoxsdulh.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2ucskeaoj.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygjrnptg.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2oxeetpye.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2rtrxfsgy.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2daxyxybm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2pbheovdz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2rbfnonfq.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ljtdfmcq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2rzxqqszi.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2pejnbduz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2psyzfeei.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2tjnnyzbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvtimwoo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ahvnpcnr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2spepqyyl.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2qacetbjb.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2ekmmenrz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2lyibhhwo.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ahhmoaay.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2troojwel.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2sciqjpws.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2efqhzcfw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2pjqgigav.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2snlzjjla.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2iylprqsh.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2azgatnpg.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2qscywjpv.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2maxcoivx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2cptuqupo.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2poxvyexn.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2pzagtrmw.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ewhyyylc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2spssrnos.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2zhchwqgv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2vjakejnm.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zrmntuhg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2aztdauqy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2xxyetqml.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2afumhnhg.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ninhdhbr.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2pobiecky.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2gmgjjyvo.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2gekctuqy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2ptopnlzq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2zpbatuuz.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hbggqysm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2caettcmy.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2teblstgz.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2iwyxkwuf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fzngouma.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2zncpnyob.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2mzzvqewx.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2zawrukur.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2pymteywb.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2ajmkslzo.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kbjwwwov.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2zkymorpj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zfwoshtt.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2fzdotugz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2akiccqrs.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2qoqxxhrb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2zkuqumdb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2ovyqhyxn.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2zyynerct.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2oyzegszb.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2mkdujuwx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apjnoaah.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2uswqjojc.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2jyitetwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbpgjkqc.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2unhxltwr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2xwlwproz.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2qtyzcqsh.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2xaojicfd.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2beczchwo.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2jlxeutgi.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2xrxxjeua.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2gampxzik.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2tnhlxnyq.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2kultdfrr.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2emmpdnfg.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2izdhlxqj.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2gkfpbvoa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2rrgodoth.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2nabjcjem.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2xowmpsap.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2kucifacw.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2lqzkhvqt.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2vwtikpln.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2gpfeoiac.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vqkzlacg.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2iapnydju.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hskfukzq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2cusglgox.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2nygdvscn.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jkizxzbh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2muxlpraj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xcoyhpng.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ssvpftcs.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2ibljfkfx.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2stjmjelq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2arlrdiom.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xujrljmu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tmglqlqq.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cvbwbdre.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kzeorham.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2txchjnkh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kpnhzvrv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2jcmcctjz.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2upstaioe.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2woopkrlm.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2fylhmllz.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2dopvpltb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2goglxkmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqdtatkc.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2clfykwzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kynfecic.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ijcbawja.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2qdgsgxpx.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2pvlktsdo.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ojsuuxpy.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2ubwjksll.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qfhhwzpy.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2kdmtadsb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2zcbiduqv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2sycvxpyd.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2srsicuhj.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2vmmgutco.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2obwzcsyb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rdfowsbx.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2aerzkskm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mcxwzhwj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2tsrdbjrt.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2lxbdxasn.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lsmlhylr.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2frmovxnn.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2aquqmfpu.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mlhutivm.html


<!-- 参考信息 -->