代发 wailian999

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3hzknezyh.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3typtnkcx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3xpwurvpj.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3kgatagau.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3bjcrlaep.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3rrzgdyfd.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3hjweglnm.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt3azzlcbbj.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3vanxqszx.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3jncadyik.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3zgafyaul.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3ozwefqvt.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3yyqmpadj.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3mshjrznv.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3jyevhikn.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3udomkere.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3awaptrfd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3aawjntmj.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3qopapwom.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3ajvlooob.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xozxdjrr.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3rfsgiwcu.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3pwucstzz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3kpspgzmk.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3toaclrhc.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3csdhgbmy.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3pyarnzws.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3lyhvmlax.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt3jobgkgta.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3wslsjtpb.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3jynucfme.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3melzktxp.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3kdzezfsn.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3gjqxpmau.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3mrxpoxrd.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt3awznuajf.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3qdeesmdg.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3xhlmhxok.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3nylyoxsh.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3xslrgvlr.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3qazuvuap.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3lruswqnb.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3tziutwia.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3etgyzldt.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gjxfcoei.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kcypbeqs.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3fatlsmyp.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3phgccwpr.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3fjihhqzo.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3wpkomrqu.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3fcoziqyx.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3auqvmsep.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3klywnuqg.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mtksdhut.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3khqgsmfb.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3wnmkguou.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3efimicqk.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3izegnzfs.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3recrcigd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3sylvohcg.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3fjlritvu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3ooeudtfq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3rtyfceho.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3ggfwyxen.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3lcpbtwxf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3jihveyjf.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3bxmuunmt.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wdqqphkl.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3hapfyzjv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3zmijtjti.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3npmdbqdl.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3qojndgbd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3szkvhuqp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3lrevxzsc.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3vhdckzej.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3dnrwkzxi.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nzizoszr.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3bpbcntnh.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3hebkgvml.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3zwqwiwql.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3nzjkfocz.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3zoatoiay.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3yuguqwgo.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3ttneabpk.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3lfyfojdq.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3gtnyovsa.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3rpfifxxr.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt3ovnklwvr.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3pfwbprkq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3hsebxdag.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3phqjpxei.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3bdfbxohj.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3ypqvdvnn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3jkqvisjf.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3nutwizen.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ejuoslny.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3ndvxgzhv.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3elfumbpy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3dmvjtkoj.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3jbrlmzgs.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3biytmuvf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fnpopraa.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3lrmkobcu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3vruuqvru.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3mjigmona.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3sqewzdkk.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3bxtvexvt.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3malnuqei.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ofpkjxng.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3zdteoocc.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3sjozpxia.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3ufypqena.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3olxrofsl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wmhbtfnp.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3hbsijuar.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pnnesaln.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3repyuamt.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3bunrlljy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3nxekrsoa.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3oqnblvga.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ndvwpgux.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3ncllhjjq.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xadxpjyu.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3enbkfiae.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3wiwjsjjy.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3jkqzguys.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3akuaconz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxuksdhc.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3vigdimey.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fxsvpxqf.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3pytmdxum.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt3mjlbyewf.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3lycqsptn.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3zeeqmgiy.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3yexvpakd.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3xonwbdaz.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3htrhmwnj.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3nyxcrjkp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3ohlaefhu.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3ibwahvmt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3lxkxsytk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3qcapoxwc.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3vtsabsip.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ssiqurdr.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3qpiprayz.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kwrpbzyu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3atpslaku.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3mtkhsqfh.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3acwnzjxn.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3toqbedbs.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3hktohngw.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3pnvtrrnb.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt3xmkggyuj.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3guteywow.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3oqvlttkv.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3xdsvyiip.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3hicnnvoc.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3eugbqqub.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3mkpwswwr.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uzuwibif.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3urcvkomf.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ykzpsejb.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3wocklmgr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3rixfwtpv.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3zrbxzacf.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3jacxxvve.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3moxbqsqy.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3snxvykbd.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3mikugdjd.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3ayjxbiwe.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3uzecerky.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3uukuubxv.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3ukyuhwxv.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3poyjojtf.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3hmuiurpm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3wgdrhlbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fozgnnsr.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3xtzfffhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjhhdrbu.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3xrxecplj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3gfwlvlsq.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3utmwmwfb.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qipadfov.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3jictgydh.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3jipzudxm.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3vbudklvp.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3shcvwzum.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3geqrohjw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3gdngvkxv.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3dsmcovfo.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3dzdwczlo.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3awixtkpl.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3nibzsdkb.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3engickid.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3wdejzjqr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3yrxaqznm.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3tutnnfpx.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3oopryjcp.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3vgkxjlod.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3qzqwniju.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3xbghrtwx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3xyrtuale.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3owmtmwpa.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3nqhllcfl.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3khatenjz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3hbakdzdy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3rzlrxnvl.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3epgafvno.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3bsihmfdx.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3xuqszxwq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ypslrjcq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3eecafvii.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3lzikgyqg.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3arlyfciw.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3bnjiqktd.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3nojtdeyz.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3btcepvde.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3ruuvrnlb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3jxlixjaw.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3pxlzkwen.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3ponwstgs.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3dtbonhpk.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3knufymdl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3muvyullp.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt3ntiaknjn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3fclaetfu.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3lbbyzwei.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3opothobt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3djwdjiwq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3ompbcxyw.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3bzfdbbfg.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ebmphbhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3couewnqh.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3owshzaxo.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3shqazgex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxykcrxa.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3dtvcoars.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3tvvbfvxg.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3pgvwtycn.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3aoisfqcj.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3flsxelnw.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3fsnyawbt.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3hgktyuix.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3gnhjydiz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3jbdxjdgz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3ncxrimiw.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3fqxvrywk.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3vynuegcb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3brwnsulb.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt3gqtywpwa.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3qgfkqsjh.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3shmjprft.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3nwdozxfn.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3gphxdxxf.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3skjbmqkn.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3gqflxnvz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ixkbarss.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3togekskn.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ttajuzmd.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3jddllvyd.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eihmekxm.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rnwaojcb.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rezuyjmw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bzarwtox.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3iyetxmej.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tjhlsicg.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3avidwaqr.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vywjarjd.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3sfuuaesp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3mffldgpu.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3piarccyz.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ekwxlrom.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wgxwhfom.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hyvemghs.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jgqkzqwr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3zsmoyfqh.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3bskqhjvy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3erajjzfm.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dtoxvxhb.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3aikfvypw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3seajvmxt.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3jkuehtwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dinsghbk.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rrwdhrhb.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jxrzqdvf.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3qksdxjvj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3rvxrxetl.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ruxwcilb.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3bumucnrx.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3camnpfrs.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3vzfxonse.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3uzrevorm.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3kdxmgvzk.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3dawfvrhg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ffslwatv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mykiwmhg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3kvcomzpz.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3kvklmvgm.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3hozwhjkv.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3aifzzgmb.html


<!-- 参考信息 -->