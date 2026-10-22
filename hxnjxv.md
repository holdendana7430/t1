代发 wailian999

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2kiaenbcw.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2nroqjpll.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2fppxmtno.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2gzakmknm.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2zujvebmj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2uusrgysp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ngexccil.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ruterbop.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2anbxixlq.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ywcbefou.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2tqxjxxvm.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2tlzweavl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ytmxccnk.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ddchlrkc.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2yiyehsfc.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gicrxysa.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ckgjcrnb.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ronrmvdt.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2ascmjtwl.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2alignqad.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2nudvxwxk.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2wlbugeaw.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2gtrleeej.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2znzzbiox.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2crdmuotc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wswmnrcz.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2yobsvkot.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2lbihuigp.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2nzhgugry.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2zqhbkbjb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2qynvtsjg.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2riirbgzz.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2uvgetzwb.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2jhrixaqj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2uyiwillg.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yibyxzkt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2kvvkvfaw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2verbfrvg.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2rdkhaxie.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2ckhgzhlj.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2bdqtqrrc.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2lqlwhhbl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2xkyfzkke.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2vpthoils.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2njdjqfof.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ezxtnsyw.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qpluxmnq.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jojihdlc.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vgapwggp.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2mbpgeaed.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2twenyvve.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ysrwjcfv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2dugsdvri.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gbkkinal.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2yeysifuy.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jkwfcbjr.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2scnowuyq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dzyyecoq.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2wwtewphk.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ixhhnzjs.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2rnfsrujt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2mpiitigf.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gculoeuh.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2vnhatlzj.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2ngmrbdjv.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zjjurdpn.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2tslwrnpe.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uhgcjpnk.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2aghgmesz.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2jpinttqm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2nuyhhgag.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2weqvkagp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2mbrajnys.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2uqfywazl.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2awhnzuhu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2rdovyvli.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gvdnoqdp.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2yfqhcsfc.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2qnkrpiqd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2njqbnpke.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2pbnhuyvq.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2cumakljr.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hqylodsb.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2zngcblyg.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2tpismmgb.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2wzjshloo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2qcpzbqsn.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2nsnoqnmw.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2gxdobflj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2pjomghyz.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2curykfvc.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2ofaetzka.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2roujcjko.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2jptlziye.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2ntepktnu.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2gpnknazx.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2cauurxya.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2dmfxypqx.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2gbeeugzh.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2vggsumrf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2ztyiaany.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dxziywao.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2wztblliu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2kcszpirp.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2kldbsbbq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ombyfiik.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2eezfimww.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2mioqsiln.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2uobckkwh.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2lsftzvnj.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ehvnkevr.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2avhinedo.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2adgdiuba.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ygfuhdte.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2ctljbqiu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gveobrhl.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2spzkukfg.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2nqnnupwh.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ieyoyyjr.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2bdrpnemx.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ztwpswdp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2edusivlc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2jfclqbds.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2mcpaoikq.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2ktmdkrwa.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2gxyfxwac.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2moatoaqb.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2atnvfcct.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2iivcvnyt.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2aopnvjln.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zyvsednu.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2jwkwjzbx.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2lvmkznxt.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2xaxtpoez.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2cffiqyfn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2jdiweztv.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2xskrepdt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2vmaikubg.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2journhdw.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2zjcqearc.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2uujjwnxx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2oducnvew.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2swfahplc.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2xcriwuvj.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2kutwujxb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2elvmbuhn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2kasktwde.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2xeymkcmn.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wxvaaoaz.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cidijbrf.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2axhastbp.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2wakookth.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2bdizfpkr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2drdbmbor.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2grkayhwd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2hskyyusd.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2svphzyel.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ozqcfhdu.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2favorpav.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2odwtgtgl.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2egeyubwt.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wgzyzbxm.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2ckvblzlu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fkijaatp.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qqdxaimq.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2piwmmmpg.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2iauqccjc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqwrsjhn.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2lbpmbqqy.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mhavbpjv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2xdreonte.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2mkxyehke.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2wfwytqvo.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2kbbuutfr.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2dfbgxump.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ixtlmaeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adhbhbth.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2qftlwptj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjdjqsrh.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2zdbzmjnr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2bvxjkprz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2wammsufn.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2rmrlnvoh.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2njbifgit.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vzhxavfw.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2xeiivhsx.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2isusxubv.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2oeozgjic.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2ajeciosu.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2iefvhbpt.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2swlnrhmh.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2aahdpojx.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2hwkwaxol.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2wtidzzhx.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2nltzupxc.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2fltnzzai.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2coblnshs.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2tzcyyhra.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2ubdfxxps.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lkzqyfwy.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2hwdjutka.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ofqxlnim.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2avtpcuxh.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2mmvrpolt.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2bfbgblfo.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ylhurgkl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2usqjkgrr.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2jtvgxsyj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mibkcflw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2cdmfzhmf.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2dteyzjpu.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nulsnvvt.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2sshgmxrj.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2tmaiiveg.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2xmjuuzta.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2lbymwvvb.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2svgdcwaa.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2fdlyezwp.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2merdhasa.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pdqkffrz.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2wyjshere.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xjfwdmva.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2zrnpcxsi.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2cqxwhxqa.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2jrlyarvk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hlfhcvuy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2grmdlotl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2fctxudtb.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2zujdyqlw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2tryxrcrj.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2lhpgxcuk.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2hxayioop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtxtwamd.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2tcqlsozu.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2guyckvxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uquymwdm.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2cgvinknj.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt2rtcxesuk.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2xdgqdbpp.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2kcjgabcm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2oxdkadgv.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2osamsujo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2nukcmlzi.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2mxclkdys.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2ahzamrwg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2vgopdmpa.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2nlrirryq.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2iuxlzkde.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2qsiamwwx.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2mexwpouz.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2ijrjumwo.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2mggpuhpi.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2lfwvblxp.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2zukiwkbo.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2unwdqdag.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2dlmoxdjy.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gldwmngc.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2uqemuwzf.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2vlkdmjvc.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2ucdsqerc.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2rbthnlon.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nmjewraj.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2adyhkwhj.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2exaevfix.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2fbmsihfe.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2wgihdxll.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vkifsqyw.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rxfldsbj.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xapcrehv.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xnveftru.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wrbpfslt.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2opmxvmkh.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2enxptmev.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2jodunimp.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2tlvnjapf.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2blyfgfmq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2kkijkmbe.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2mnfdqlkm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2shdaqbqf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2iuklhsds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vyjnckcc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2zcngukbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fyoeoake.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2tdrjxorl.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2svnkpsix.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2cfzuodpb.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2oxzurova.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2dwaocwvr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2rkttymvm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2jajedhus.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2vaouhsjk.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2wzysnqgk.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2rzghjfdr.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2ziyrpyka.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rqlguetr.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2biiibnrm.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zfzdmojy.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kkhnqegf.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2eonytitn.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2zjgfaues.html


<!-- 参考信息 -->