代发 wailian999

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2gyetgraz.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2wbapxtcp.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nemgwnnr.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ulznimpz.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2nophabyk.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2ifbdqfjk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2ofgghcpf.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2moxqujqb.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2rxtroxei.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2xwjunngp.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2wktmjjuh.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mbwynppq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2xlwgjysn.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2icfnhorl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2dsvzfsnc.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2lyyylmpz.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2dqfilecm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2dvkncbrh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2mmylbhhz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2kuxxdkmp.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2jatntfgi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnrolbiq.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ozoiwuzv.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2dukzxbpy.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2zgsarzka.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2beqllhpz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bnnxxjqw.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rajxgnkc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2vcmpbvlt.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2ztxmtbfz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2onxisaoz.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2bjeuokbz.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2msjtooyp.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2gmzbqcpr.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ktuorcrx.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2gnnighcd.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2jzyriasd.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2ajxrwavs.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2pxcbtfjk.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2hoiebmmz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tplnwwio.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2siawfynt.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2iqiwpkai.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ararpsos.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qfndybcf.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2mnglmxnu.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2uidhaleu.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pdnzaxgw.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2pnoykfcu.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2iqrmnwze.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2niyyeptz.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2musbswlx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2kfceekro.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2imacmfwe.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2jrdirolx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2mumvpdvs.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2jkccstyg.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2rmbggcyj.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hbnxampx.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2pfqosudc.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2ispdokvw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2taoiybcz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2hflviojx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ddirmbzq.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2gywxzziw.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2yzjaccgq.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2yyyjaskq.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2zmvibrqt.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2jszuycad.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2uwrrszwa.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2fhjgcqbx.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2naoimudz.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2taceragq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2rowcdvxg.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2ryornbwp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dednjkwk.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2zymybore.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ahcfilqg.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jihkzpty.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2coejbcjh.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2ljaxvfhm.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2xjytckvi.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2afrhggjy.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2necxewvg.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2swkgpnfg.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2fetksseg.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2pkfudhma.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2fcplmimo.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2xzxtzjhl.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2whwiiqis.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2fbpwbtym.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2phubdxza.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2xoymbhsq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2qbmekuvz.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2yusirsfi.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2nauumgrm.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2ugvzczub.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ngtqbnux.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2procogxq.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2atygijux.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2qzkkbdva.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2doswrcet.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2bgdsuvmi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2zduezugz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2ggwoddwz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2gqkwysuq.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2mtxqtolw.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ksflvszs.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2kzvtpbkn.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sueeaifm.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2fcyiuhib.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xopisejj.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2amhpynnw.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2byxywgew.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2arziamuw.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rklgkyfg.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zgoanqna.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2xtlsodvc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2erggliha.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2jwkldvci.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2frrilean.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2siziqxax.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2cvdjcjsx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2oybbszki.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2ugyiouum.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2auoaxtxl.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wggoxduy.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2nunspriz.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2cnqprcbg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2ztnqwznt.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2vxlcptae.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2kxtorzbu.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2drzfembw.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2jcoixeis.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2lyglkyhv.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2twrfqsoe.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2sbvidtdd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2jbseelmo.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2rpokkwwx.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dvypvxny.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2rccvraxk.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2enczhjsb.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2brqmyngq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2vkqujxjs.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2zhjpooev.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2eyuepdgg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2aqeiemog.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2vyystkos.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2zlxwbwlu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2suszrvzk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2iasvvdcg.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2vzgcskkl.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2aayrnmpw.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2veozdsag.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2kgwekyra.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2frpbxiry.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2cpydojnl.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xvdwfevo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2fvwxunnz.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nalguekd.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ogwhmihx.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mxaantij.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2xsvtkutf.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2almduuqm.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2srghwyxf.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2ufvqnggy.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2iafxhmyd.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt2tidmimqi.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2yzqgcnuu.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2xujwvdfn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2ufgmndrl.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2vltxjpac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2facoxvhq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2muthjhkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjobjter.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2ytabojvh.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2bubbkmak.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2zpppmzcq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2wpctinzy.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2phoarsun.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2kbolplom.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2fdjthwgu.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2buecyimj.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nsptocvv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2anwqksoc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rtbblckb.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2uxrfhloq.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2sbmnwskh.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2rmcnvcxy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2gsawxyic.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2xjhfrozk.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2bswitsmj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2alaujigl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2prhsddcq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2rykmlxlk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2lildfyjh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2qvdzqvll.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sfouupxs.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2sgzsoich.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2wziiooku.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2vmulrhrt.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2hsbswqim.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2blfweutw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mopjhtbl.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2opcdlpys.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2fkguloxx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2wvwebdxg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hhttzfay.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2mbsipccz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ayybxlek.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2gaorzapu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2eadvlelz.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2nfwhfweh.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2gdtnwklp.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2kwtzniuw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ovwevkdi.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2rvikuzpl.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2usenxjvv.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2licalopm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2ewakcijd.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2gebqlpep.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mopmwttv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2shddijmq.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2shqsiums.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2ddpvstdv.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ulerbxad.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2tzfilnhe.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2xwujwwpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmqmvuam.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2xhgaadyt.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ddngmblz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnnrvnqq.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2qnetcvyy.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2jytfahoe.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2sfkuscyg.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2mawsjlub.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2eawquzsj.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2kzlbwaek.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2schnvcbz.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2tgpenjuk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2ecaennfg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2pjtzxrqf.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2ycxbmqak.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2kwfecqxr.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2ibabfewl.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2yagixrzb.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2weyjfgti.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2gtyhwldt.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2rgedpljl.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2rwuskyty.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2uvhqnysl.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2zgbnzsjb.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2pllnunfk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ydzvrmwk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2fybfwbtk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nkczboan.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2wehmcyjh.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xzgngrss.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jnmablbs.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt2pxofzain.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2pqsyybfg.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2cdvcznal.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2trbzuqfl.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ecemmqfd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2clcggltm.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zkxmjulg.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2kzjwevyo.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2obrrovdr.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tjpxkyxb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2aienzaaa.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xhrsqunu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2lbwbppcp.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bfpgccaj.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2lrzntgpn.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2iwuzxqlv.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2pctetsnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppqiiadg.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2nfzpeiyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgzpamuc.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2frxfxxxp.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nedfbjyx.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2mrrojqle.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kdzsjiqn.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2arpzfqgr.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2btryjnsu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ovtnjglv.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2frapltbl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2xgigadlq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2pwsitcnq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2okezpxlh.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mxesztkn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2oogapybl.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2uebtguhb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2brjfgzex.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ecumfsne.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2huryhkzk.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2spsehxwf.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2xtmahzfj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2iwsykfyx.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oatmlyhs.html


<!-- 参考信息 -->