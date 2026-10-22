代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2xmeyahgh.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2appnvsth.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2whmuyqmc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qiwwqgfc.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2qdynfuma.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2ecwzsoht.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2elzbmycn.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2tnntqreu.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2zrrljogt.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcxxjqli.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2kbtsoizg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2pspaffcf.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2ymokxsiy.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2jnxdkxxb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2pggpvyxw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2ffjilghm.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2cmyalcmm.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2gcfrpomi.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2efvhutre.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fojqkkvr.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2brlixvnc.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2feiixtbc.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2aqdjiqij.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ibbbpdbw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2bwfcmshj.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2dnxbdgmz.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2qigfwlkh.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2iunqtfcq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2scoaxwox.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2zspntgft.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2xfdmxmbs.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bsyishfv.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2utezwymi.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2zjqarauu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2gztkctmr.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2zafinifu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2xkygxhjl.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ccotzvuj.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2tcvxgbrc.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cesgnbot.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2rqlbotdz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hkvyhdxg.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2hneeeusn.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2mgspmzet.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2mjpxeorv.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2iycndyls.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2zulydetd.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2kbmirjzj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2gvfcfjkk.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kptiiutg.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2efkkdgud.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2dzyyrbqr.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2lwrimyde.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2cgzlehhq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2tcsldxeb.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2qjkhqzhb.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2molmlkzb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2inkegwej.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2stesvwjl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2gvwdpyrk.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2sdbjgzps.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2oxllnopn.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2unkqlceb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2nuaqaubf.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2qxqxzhvm.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2eccqfhdw.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ahegchpv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2prxleilu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2athozdhj.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2wvhxegga.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2uuoygaos.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2kewulsuk.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2wjgnrohb.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2cmspmhga.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2cdbgrfdc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2bxovjhqq.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2bfcfdihe.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2cgznyvpx.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2eqzbqlcw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2sjbodiod.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2lagoirar.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2thzcinvl.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2fgeppwew.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2xdujcufs.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2glahjvxp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2azycalai.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2fpcqgfwm.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2zwmdqjes.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2hqdgzawq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2uwbmnmhi.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2fwmwmura.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nreajfzy.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2imlkijgd.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2pxgfywyr.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2cdympqbr.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rysupyha.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2bozbetlx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vjtzplam.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2zshkqdch.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qcalgske.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hzxwedep.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2uqznzvdb.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2zaqttvgm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bqfwmmto.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2sbuqrpmn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ibtkkaeu.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2gdrelrvj.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2xtxrkfsa.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2qyazqyaf.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2nlyrllku.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2tokbjche.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dflsywkt.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2vtjnniaj.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gmqakscv.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2wwquvnsf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2ecoaajya.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2vqrdkrth.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ttcfesvc.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2cnlxakok.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2wyhxciiz.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ksjdptfy.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2hegmukgz.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2twyozpqv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2wbgyexpn.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2copkuqjh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2zpwdsicf.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2dhqsexfd.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bbqjviej.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2ssxivuog.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2omdttnsh.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qxaezmcz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2bhjsnhjt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2chfuhexs.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vdvnnlry.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2nwzmakzz.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2cygeoaxa.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2sggkuvof.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2hhhsxwil.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2jsffrnyw.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2thudwrkh.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2wnnatokn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ynfozsog.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2qllzhkmm.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fphswqye.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2yjbbiwju.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ktllmnug.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2xtweokme.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uzlbihbm.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2clegthtu.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jrxgceyy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2oqiwzxsy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2kamtzezt.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vjcqyyqt.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2jjtlyfju.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2aisoeops.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2wufwujib.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2lyzsvvyn.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2qpnkubdj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2dcvhxdbu.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2rgxureur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmqxruso.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2mbxzbayz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lqliemfb.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2odotxzvi.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2lcdnsmzy.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2zktybgus.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2lpamclmq.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qdlmkqca.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2zupfcwwi.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2adtfnmwl.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2zabbxshn.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2tppiuckf.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ootjffns.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2sqirktrh.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zvreuszo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2rornkggq.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2wqgosgns.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2ivyvzelp.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2iydtenhx.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ftdepcuu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2wejkfqte.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tkbpfzhi.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2qjqhfsun.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2gfhulskx.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gznuiwuv.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2zenzxzsp.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ighsfwll.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2aqknpwhy.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2ydrhpqmy.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2pheebgtk.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ihorozqk.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mvlpabdt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2hbmkaqnk.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zxkqxmbv.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rrviqeye.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qxadkbmm.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2vwykixch.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2tfrberdv.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2nemwwyrf.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2waxgmdcc.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2aopyvqrj.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2yrkjjnfr.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2mjezdkdr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2wqpwiaar.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2tbakehbj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jbrsndna.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2sivvjjew.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2jtbkujiq.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2okksdukq.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vlxczitv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2nkctbrby.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2nkuzbrbm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2khxzwxxw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2forpnrgq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2xftwblru.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2hktyrsin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2naugmluj.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2rtocvmlw.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2nceicily.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdlosvkw.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2eilcnzhc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2ospeaega.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2ryirmnca.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2atzbzojb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2yohxcces.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2eituvgpt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2ntlsapjx.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2whslbpqa.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2eclrkyzn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2ukvdemhf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2fxquzxgl.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2doenyuie.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2rsdwlqas.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2kztjldmz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2lhucdwuk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2oymfaccy.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2qawosctg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2iyjgywgu.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2idihdezo.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2xwvnroky.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yogmxkkb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2waxnbwwl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2uzthkgiw.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ffmhdnuk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tubsaolv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kcokqdzi.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2bozhzhxo.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vuwdgtau.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2uxhxcoyr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ugyuadjq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ffnlluxi.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xhbbyxwg.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nyxlkjbf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cqamzaqu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uvlsgzed.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pwuxtjzn.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2amkhbbmf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2rfqewihr.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2paovebkh.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gjivbwsl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2nvkgfeyj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2aqvqevnv.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mtmhxzwx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2keykpmkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqssflkx.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2vjmtsbig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtlqhnvl.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wmhzzxnc.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2gfwlhiyy.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2bcvqbuin.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2iqeeldea.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2lvtluigh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2jzfksgty.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ihcxpskg.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2zbwiqhex.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xkqhjomn.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2dimfatxn.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ouyyvnnu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mbuzxwnn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nocpxrra.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zpzocbtl.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2jsbgxuay.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2yicwmtfr.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2zyhyprcj.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mvphqref.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2nltwsycr.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ibklklbo.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hjgslkiz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lbinxtdx.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kmcvolnu.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rjgjtsxd.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2qarullqb.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jghrftsp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2edjysrrs.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2vwgoffcs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2fgtragal.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kcxfydti.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2wmyjjfut.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ovvfzmxo.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2grushnlo.html


<!-- 参考信息 -->