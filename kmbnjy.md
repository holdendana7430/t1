代发 wailian999

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2iagwepgg.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ticufspq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2gkhewhfn.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2epjqceyh.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nrxxzaqi.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2gwdivtqa.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2yxpvxykg.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2cmosdahf.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2cwaqtham.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sdlwjrnu.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2bqdkrujs.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2temzeesm.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2xswbdnmi.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bypgnall.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2veocfbhj.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdytupuu.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2qaxoiiuc.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2arikdgez.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2tkezehjx.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fuimgzfw.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2rtbwfzsk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2dpumovba.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2xsfggkrg.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2nkpbijaz.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2doukcbyb.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2bdzetavz.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2fdnjtljv.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2kjuapmvs.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2ideauklz.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2cboiglzs.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2yexaputx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uinkscla.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2wpobzsxu.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2gjilbzdy.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2qinurgrt.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2emcghvml.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2ygwskjme.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2yvgsxhmc.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2vceyacod.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2peqyqtzb.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2tgdxmeae.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2bbcovtbz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2thxcmvzw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2rasqtlts.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2xhwznuox.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2lwmjaysn.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nkjwwhye.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2jrhuggqg.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2nhxwrplw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2svssdtml.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2qrchpwit.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kxwqbubo.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2plxfjpft.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2xohhsykj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2dlbrcwjp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2wevjwknu.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2umahkdpx.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2eokjsype.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2ylvwescm.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2tbnhmcub.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bsfdjckx.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2rieenuww.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2ubnmtnbc.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2iwrfutme.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2dwlgpowu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2dirtskus.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2liaxqgvi.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2zlnjqizg.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2mndhxdbp.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ubfpzbxr.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2nyzlsoie.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2rhvmxdcl.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2mbcffkpo.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2yblrmelc.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2drrpjipd.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2wlqpovbf.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2cnzycpcg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2qbteonjc.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2rjbylpkn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2tuvsvqiw.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2bzzmdzfo.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2bqdwjhza.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2gwhskfft.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2tgzkqxjh.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ywvoavwz.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2yzklztfx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2suyexndi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2kjpcnizl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2dqpfbdog.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2oalgitmk.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2upgxyvll.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2aajivtzz.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ffrhigel.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2yhxmudyk.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2zpccblbj.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2pylzsxgx.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qqxmzsrg.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tswgnvbm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ziavobws.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mlgubrcc.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2yivvpenp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2kjnavwqn.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2mklcmrwu.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2pjxmftlh.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wfexpewy.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2kgocixxp.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2sxbcjqes.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2myrdymqb.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2haisndlj.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2auuwnxpg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2roapgufs.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwaanrqc.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2qoaehqkr.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vmhmcxvj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jkhyjazj.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2ocsgegto.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2aixgrdge.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2yxfkvkys.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2awiixwww.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2dpbxcznq.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2styefgle.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2rgeukqev.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2zikdjgkf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2utkbfhbl.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2rfmfxbqs.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2sixxnvhf.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2nmkawzxn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2qhhnqbbf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2fbcivmol.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2yuswhxpz.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zfvzzpab.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2qekdjunl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2buxgrwuo.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vcprqikk.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2wstrrgyx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vgctjjdm.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2lltbwopo.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kkqgsnlb.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2czozynln.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2umkwfhbe.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2obdqeacn.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2htucsnhh.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2dxuroceu.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wkfgpnwg.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2krlzpbxr.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qlnjceul.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2mbikbtib.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ctgppmsg.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2iummxspy.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2koljijiy.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2agutpygw.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptxazmhh.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2tnihszqe.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xfeppkro.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ljllucid.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2wkqiwrcl.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2rwkgythb.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ckyqbsus.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2aquiacef.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2fkfkkuda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlcbaffd.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2xnkvncuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mcbdcpzc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2iutoggwr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2lbunalxp.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2adlllhjq.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2aczkmdly.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2jwghulee.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2pqcasxqw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jnofnvov.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2munbakbr.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2xhihhiyo.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ftxrqhnk.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2sydynkcd.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2fzqiyvyo.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2addwfzbe.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2jrgdawvj.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2fcjubxeh.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2fcdalzvj.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lyyrekxu.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2pmguiufn.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2kstrplzm.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2qnrrhchx.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ownketiv.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lmmphjsx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ixairnho.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2roaasvly.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2bdjsgeby.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2hczwfbzj.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2mlkujlyu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2qipiijge.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2xxqwlxhz.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2uuwnudph.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2nczdfknb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qjuizxsc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dsrameps.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nwxxxmky.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2juojdghy.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2ldhmlidt.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sorfpbll.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2vqbmxyge.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2zmpmppxp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2kwasocby.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pngpgprg.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2mihcgrpo.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zrhtrtmh.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2ysnthbde.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2luqqgksy.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2vebfzufi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2noldkiui.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2jlhigefw.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2frpphhdy.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2eceuezvr.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2dzmnqdlf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2zaxqkilq.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2rqrcqffw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugzkdvcv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2rbinchyi.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2zmezzyrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2woqqfqpf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ldfwfpbh.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2lfqhtkse.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2trxdlhbi.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2awgshxho.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2mtqhwyrh.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2yreocaas.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2cudemnyu.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2yjddoqap.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2dgkwzhfh.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2qjkawtui.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2hamcinqy.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2bfricywa.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2bwepggvx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2rtrituan.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2anzcliko.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2hqhxfvtw.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2rscjgojb.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2lhjxhamm.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2blpeywjk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2zmishskt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qqrtxiwb.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2cnazgnar.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2iopjnmnx.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2knyzhszx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2auqdfpoc.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ykreiidv.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2skafdifb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dryqbhka.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qxxiwmei.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ykjfqbhs.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ubryipvm.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2eawehkrn.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fwcmbgtf.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2owcxrude.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2awmmrslf.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2fjsceiuz.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ezamfoau.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2ykswkjwy.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fkjndwrb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2jlgjgpgy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qwagkbgp.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oulqtlmi.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wvzrvgxw.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sbkiwwae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2egrphfan.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2mbrxmuph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtvpyckc.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uglgaqep.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2yoqxuhzo.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2pyuhmlcm.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kcqbpcmq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2vuivllek.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xezyicla.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2qtavndcf.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2rtkltjrl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wfqagdcs.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2cdhsrhfa.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2qjtusbfx.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qgsxurtc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zvcizzex.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qdqcvykd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2uqbpfhea.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2kevplmsh.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2iqdqpyvc.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mrgsyxpa.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2nnajznyx.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2cvfiktky.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2skqijktg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zrbedpub.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nxpjcgdd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rmelqgpo.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2agkasywy.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sdrxwhgv.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2butncmed.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2xnimndla.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2snjrbtap.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2aomhpzch.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2sfatbqek.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2gphnzcpu.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2yzisulbb.html


<!-- 参考信息 -->