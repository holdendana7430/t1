代发 wailian999

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2mhldrwxu.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2voznhnqo.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2cjgvapjh.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2arwnefwz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2anhhqlse.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2zfxsiqol.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2dzkhpakd.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2napavejr.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2pnggfhnm.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2mjyorslg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2pyqpkqag.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2eobjxzyv.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2ceoxhwiv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwwlezpl.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2uycxbugk.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ejafityw.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2icfjjkim.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2oxszsrcy.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bnuycggc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2wfkgzvpp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2hrppcacx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2bekgnqjo.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2hphywqbb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzwksaln.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2jebnwqdp.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2geienndu.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2wlnozqes.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2qobxkdxr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2svirmlxg.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2ftybiyby.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2slcvodly.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2wnnkrios.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yjwavlrn.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2xgmyfael.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2ayrkvltq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pjgoaiep.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2dlkstvpp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2rtezebbg.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2bmlahlvk.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lunzixtz.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2clszplyz.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2auhewfyb.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2gjssmpoi.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2ddpivhpa.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2hbnlsqep.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2dximepxe.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2bkajiwsr.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2hmdarhue.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2mfualxmt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2qaugpmlb.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2znehrmql.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2cxfadgny.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2qfnsibfi.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xlsyvspa.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2agkyloyl.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sovbkgij.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2yjrlhvll.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2kmltqagw.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2jzgvuxrr.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2rnvkokxd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2pkpliwaq.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2cciqsndr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2hjzedras.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2bkmbpyia.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ppcwtqee.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xwcssgfw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2yjgudasj.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ekcgzuzi.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2gfbgkgui.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2adirocjq.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mflyklkj.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2lfywvgjw.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ilklguvc.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2hfticqxb.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2lmzioxpb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2nxlyvpsb.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2aoxrmxbg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2ezvjckjb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ljdugapp.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2ofsbpbca.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2wirrqevg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2wfsezjrf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2pixpoeqm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2cnfgebwc.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2jnbryjod.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2zlblojqt.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2ciyainhv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2lozfcovt.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2wzbhknez.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cdeaudmf.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2dgnzdajv.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2vqeecgok.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2emlnweag.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2mjdpfrmv.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2qvieuhbi.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2nwthowsw.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pwodumco.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ccrejlvg.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2ktgnxzgg.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2tqjydjau.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2qvtasogi.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2vfyytjaz.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2hazmcvpb.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gaqyfymh.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yyooprgg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2cjlrnqps.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2rkcwfonm.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2swnjbwvh.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jjbullpf.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2fvviudqv.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2thimceck.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2syrlsiez.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2vbbtskfq.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2advuxxvp.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dsnjxehk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2daapxrwa.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2liavpbpv.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xuutakcj.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2vccepfsf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2oxzkjkpx.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2juyvugil.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2hznmykxd.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2tnvnnjkr.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2qothyloj.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2otqmnoix.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2kxalhiyf.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2rhknatia.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2ziwqbfnk.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2plmlcbcl.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt2atljifzl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2bfqmzaqe.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2hnqryurf.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2leenyggj.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2nursruvq.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bfzbzpop.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2guomrmrf.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2uwrumyht.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2sxscyqoq.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2qcfpbydm.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2wrbwlhjy.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2biznrmfl.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bmhpkflj.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2xyocrair.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2sxrmtqmm.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qtxfabcx.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2slzicyev.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2ojjpperz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mdtwcnzk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2jlnkwelu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mchmddyt.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2wcauwtca.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qeyraxrd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2teyzdbef.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vzysxtat.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2sawnjrqh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnvihsee.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ofgqgvek.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2jaenhmgb.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2pkaryyti.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2dcjstkyk.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2oqhripvm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2rhizkesb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2nuekpmcg.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2nimjezoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uliawfss.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2nsrailao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckdifbyl.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2mpjycsxu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2qlhhmbtn.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2tucvdnhy.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2klfzpdhv.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uvymbwxg.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2eewubths.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2byykgkmc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2bvviludd.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2deckuppv.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2ahhrzzdx.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2knakojgp.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2kfhrtvhy.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2zkhoflic.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2itekcuxw.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2bmzbvrzb.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2bjepvhhx.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2itdsbfmq.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2eweljhpb.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wasdaeen.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2lrovcboh.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2vfnigyci.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2xqkmcsjg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jizubyxb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2kebmderp.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2ddteygjx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2kikuwywo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ifaqpfsu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2cinonpxa.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ckjznhda.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2sxkzmlep.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2inxttnzm.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gubpkepb.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kldoeyfr.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2edfogeat.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2jrupkrym.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2iuychiti.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2denuowfv.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2dglzaobe.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2ugahwjxd.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2gudtokuy.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2uyirkvnl.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2yamhemuc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2vcmorhzc.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2xybomodp.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2lrzhngeo.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2csvcazpj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2whjrezkw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2ccoflzqy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2ydnthnrk.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2miqcscko.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2frtgxgvc.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2swijmuqo.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2bfrmtzkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zadvohro.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2bsposshw.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt2xuppkbwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uogimtua.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2ydrcaxnr.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2efspukas.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2uxjoblqf.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2cbagaine.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2knopewui.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2nipckgrb.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2zqtzlfpi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2jabmgyko.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2mutszwpz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2usmwpwoj.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2jrfmxtaa.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2mujvgsbn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2umadyizu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2fcsorbss.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2yukqnqxv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2fndiuevo.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2jcgmfttn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2vvdhffsa.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2mjuyszkc.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2tjopvtvj.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2qsdqcaar.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2tkzwkdml.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2yxjhgucg.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2istpjxtv.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ixcicwze.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2febaqbxg.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ehzljzqx.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2fcijkmkz.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2zsxfrcxi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qsmhwpqm.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2setuayoq.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2yndsjnnz.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wlkgzgfi.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gsixthim.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pmzwndic.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dvwtdcwx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2ovrypyxx.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uepylztw.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cmflnezt.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2timuerls.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gcgzxfpv.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2ybheqpft.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2woeolvso.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fipayofu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rawlacgs.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2ehjcyxcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dyqvosyg.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2lzuecuxq.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2ujtajzmr.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2bbsamoac.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2gftkohbp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2cjsvlfqm.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2edtofwog.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2rhrdfuse.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2dfiidoae.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ibacwqxa.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2qjpuhfvv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2hmunfxpq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2fmhbdhkv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2zyutacyr.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2msjllaln.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2dkscdnoj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2kbgxiyjz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2jfmdqtoq.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2lfmhwfqe.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2tnquxrut.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2dolqclai.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xeyivszg.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nflhopja.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2akjlpwgx.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2kpecfmuu.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2sfbqjqrd.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2dzgcghiu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hlmdauya.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2zcqjylsn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2rkfsqgyr.html


<!-- 参考信息 -->