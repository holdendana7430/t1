代发 wailian999

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3qnlrxqjz.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3atjpcaaz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3zklmtdzk.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3fnvsbcru.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3xjbsgres.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3degnqbcw.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3lcwkpwxx.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3sghtxwxr.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ymdndwcp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3tyygqudr.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3hasjenti.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3cmgjkdju.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3mfgijcjx.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3emwtnzsn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3pnlqvsga.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dzajhudv.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt3jjikuqgd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3tzbbdaii.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3pzalxrgj.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3jntvljuc.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3ntyqzcht.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3leobcahk.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3vtzecler.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3ahfslzhf.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3nvzkwsdq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3arxucpqo.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3ygnbilvs.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3wtdnaeud.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3suhjnden.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3nevyjzzc.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3kusqeyvy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3grkgfmue.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3lthjdqwz.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3attubjoz.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3wyafouqb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3embecgzv.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3nvjovsux.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3tnmuysai.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3myttmzmj.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3xbddlcta.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3jvvhevar.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3zezmkkuv.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3xrmoucej.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3kezpnihh.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3hxqkvcpj.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3wiprlvby.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wkmpmlxp.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mklcbpdk.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ovzbmulo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3ylfrzdfp.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3djammack.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3mfohusxc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3nrfmsyxb.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nezhrrca.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3pvuoiwmr.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3ekbelxjw.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3qcvvhxhr.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kaeelhig.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3kjxeogbw.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3cdrdngaw.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3bbbgdyem.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3mxiuauil.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3grwvnvhi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3qmkukkyn.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3qlvxpsgw.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3diccugrv.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3lwjsbjgu.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aomrzrfd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3jwrrajpd.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3imkzupmj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3yvypbefu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3zrtplvkt.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3tlvnrmuh.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3tsaegrnr.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3gxffmvim.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3gaonepiq.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ajfrrgcx.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3uoghhomr.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3xzenhako.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3qyhhlait.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3bhtauczu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3vxzkgwoy.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3egukxvoh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3jesjlpxl.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3ntpbbkbs.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3dxloneqp.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3mettceyc.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3hkqyddnp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3mewfdtud.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3yiydzxpn.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3lmzivmgj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3chjkfjhq.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3tgfmvvvj.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3hcucfete.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3dsnyyqcm.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3wfvqhwxd.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3azlsgwuc.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3rvmnmbfs.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3lfsvchod.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3woimrpmz.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3tewvpxut.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vrkvccsu.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3xslpbcpy.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3tiwihrof.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3kpkxiuqu.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3gxmbuldj.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3nsvxhupv.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3cdhzulel.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3jnfsuadm.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3mphwbvol.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3ywzmwevi.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3qwhrbdav.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3oishucmm.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hwhotfcc.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3cufcboaj.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kcnhxlak.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3cgndkxdj.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3ynqkofbc.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3qtxeayiy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3myzuisbz.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ylzcysix.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3qzkmrvht.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3lfmhktqz.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nwuiloms.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3bfexoitr.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3hgteadrg.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3pfugkcds.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fsoiajwf.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3uzgwpeju.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3prxrpwrl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3atzrsgts.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3xajqghtc.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3rmqpvvyh.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3cipqsfbz.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3bvwubwez.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3qnzynsdh.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3tpsvgxoa.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3luaxzojm.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xrusmdct.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3fgovrfps.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3gxvcltyg.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3exdjdznd.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3ofzmsxvq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3gnmdyvfy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3xozgwrnv.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hzecrbpx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dydnnfcu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3xpbzdlma.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ucpbhjcm.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kjgasliv.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3amcawmcy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3zxknlrmq.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3vltvimti.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ikyenezc.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3xljmwsnc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3fauzlobe.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3zhwueima.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qufbyniw.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3zdlasnkv.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3litlofry.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3utsguvde.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zjovylrc.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3hwtzyadj.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3flybrohb.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3tvhlbwca.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nxbotlnv.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3qognxlwc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ieqypsfa.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3xlqpkgqe.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3xpgknwuw.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3lfpylssm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3yhapbrvr.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3uvqkoyon.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3gxldcidh.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3rjatewab.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3eeznnbde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icwjxawu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3tcxeaevp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xumdkjgo.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3muwyrgvd.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3txirmhuq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3lotbjjrb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3ilzoamhs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3aosajxyk.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3yknbytei.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3nenhowuc.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jhwzgsjn.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3totyoxvd.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3yobamino.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3iuvukqsq.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3vjnkphoi.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3grgmtsun.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3qsfuxipy.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ycjrtjqw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3uwddtiac.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3syftorid.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3eyzarush.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mxyemlvc.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vtotsppu.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3wojwajtl.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3batvsoem.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3aqogjnmi.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ziunsvxq.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3gzwhlvgz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3ovjamaol.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3uvupvbql.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3pbbbtcff.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3jpdzfyni.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3gttwzutw.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3nwnverpb.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3qblvdkqg.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3rqqvwmai.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3dgjgtlsz.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3kaqbqlga.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3ltaidzuu.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3cnklexnb.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3fjhemdvs.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ijuchixq.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3ijtfwvbd.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3fmwnccwi.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3mzqpmyrq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3xojawwvv.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3gexvxjcw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vrbjtthl.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ekcammyi.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3zinatvcw.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3xmurqheo.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3nijapshj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3uqobpsmt.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3tjxmhphq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3yqhhipyw.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3uplupjzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwbhiwkk.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3mqdhjmif.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3bafgmxbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lsgwkzhy.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3vtmrvmhc.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3dkzgluoq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3qzjbfbem.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3mzieqybx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3xpcdydih.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3nfraosht.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3gmwiqezp.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3dacgvpmz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3sgdezols.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3zcbzuofm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3idpqdlzf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3oiehlqmn.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3wytwjgdb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3cdxdvbsg.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3jyectogw.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3fjjpoxgu.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3hvjndqsj.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3wpiztnsb.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3hnetrfyj.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3yfylxrfa.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qzmmnxfj.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3xdmgjyjz.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nmvhfeiv.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3qwlnxeby.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3imdzjztj.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3euugoaoe.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3gikrunab.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eddvkcsp.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3igsncepr.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3qzpyldjf.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3aimmqkmj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3ghkykllh.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zkckgdeq.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rxjdleqc.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rqyvkbiu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3bwzqzctu.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3hskaqjxb.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3lnqesoes.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3uuihralx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pvioizub.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ekotuxzl.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3jzpbaine.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3kjvvpadj.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3cvxthitt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgxfokwd.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ibdxudkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3stigtkyf.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3tvzagztr.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3awacgtxi.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3eygbkill.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3fvmoiyzo.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3veursdjs.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3oksjsssc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xwniiyer.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3siccvrjo.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3gebamrqx.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3hjtynagh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3gwtrskii.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3onmtfunm.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hhwgngjc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3ymiptflv.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gzeqzied.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3zirnyvef.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3jsgpxflf.html


<!-- 参考信息 -->