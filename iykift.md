代发 wailian999

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2idxefjgg.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2ikwwfmvm.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2zntzxuye.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2qahzaobw.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt2sjfdtepg.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2zzloeqrf.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ufcsllxk.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2oekuhfix.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2qetcntdv.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2wwpzlbxs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2mvzmcevd.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2mdhvfpzi.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2ayiaxoem.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2nlyldush.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2mwlwyufn.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mfgkfflq.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2jpspdjas.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2wtlimbil.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2fdioyvhr.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2xmkyaank.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2ichdvrrv.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2fyclbmbh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2cvmohpri.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2mdntakzm.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2edjrfqta.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsseouzi.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2phpxagij.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2dekoaksa.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2cvvkuucu.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2qcoezgpw.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pchoryzc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cysqaxxf.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2tyfsnkex.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2lzyxojiy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2bcyregsp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wezoygyo.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2jnzveeyk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2xjtnjuwx.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2awuzvqbh.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ljqnonsv.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2rneomunq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2nkrsjhkr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ekulrwcm.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2angcrkad.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2yxycctpg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ntnbishd.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cpuuppeb.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2prozzlph.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2meysyhuw.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2qompzcbb.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2legasona.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ijnhvcoc.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2qcyfjlvj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2affvmcvm.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2ljgvspry.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2grqvizax.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2elvurowj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ixfitghf.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2qjknbylz.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2mjejmqaz.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2gmkzkaof.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2eqlzpjqt.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2kfwjltsv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2gevirpmu.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2tcbjzbdd.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kidixkmw.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2ydvaqids.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2lewhxddf.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2gkqyqdiq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2oagqbdba.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2vhwvjopp.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2dxgxkjsp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2altwkjpl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2mzmjbbef.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2gevxkoit.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2iqmulagc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jpownmqf.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2erjzxwxa.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2vzhllhtd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2iclsbfhz.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2aiabfgmo.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2bfvpecme.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2unsahhqn.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2bxspyhsz.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2mjoqzimb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2pthtkfwv.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2pohotlth.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2igpwypea.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2wzqlscfu.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2oikfwahw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2oojtwspc.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2qodadmyj.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2whlahfeb.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2vvsyjqrc.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2hqqrgmzp.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2cjnjeaqb.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt2zeuntkyo.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2djhofcqw.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2qaziycdc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2qbqivwgf.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2fsslszgf.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vgvxcoxm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2lajrazjg.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2fhtmkntj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2pddweryq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2jdlxnwcm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2zsncnjxk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2zpvkioey.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2wuwzzrbj.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ccyhzafm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ghurnsje.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2rgrouxtj.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2filhndzv.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2aqkpjcfx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2lklplzcy.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2axoagwqa.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ipdkkdsu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ivltrhqr.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2bbqoddee.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2chwmeatn.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2lbofaryi.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2sruflgnw.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2qykbtoqq.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2znnhtlyt.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2podwzvfd.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2eaauwycc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2cfrlacim.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ltwpngcw.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2xkohantw.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bpkuzmfa.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2alsikoyo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2zxbswxay.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2ithrlnqd.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2kypochfi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2emeblspe.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2yrgqngpo.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2amasyoyt.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2emvptmlp.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2zabrwloe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2kmjwnltp.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2xdbgdmpq.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2rqodepys.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2rsuxdvpp.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2etssmczu.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2euvyiqsa.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2hsdmpvis.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2isjxkszd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2jkyoanuc.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jnxfvpwp.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dnoqmvoc.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2lsgakmyn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2acmlzelm.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2shmzuxid.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ghziords.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2iveysfkd.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2llpkjzyk.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2wzfwjirn.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2hbipiunr.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2zdrchczb.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uwnroxrl.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2kumdznuy.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2algxykdh.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2pxtfaqou.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2juixmczk.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2jvrxpedm.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2paivginn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2anlzmffi.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgjyaltf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xeqphjgp.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2xsruvcwo.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2ejpwhhbd.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2lpdpmdhm.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2jvqeoizl.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2nrrvgaeb.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2rzjgupdc.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2bshxcjol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vpsqytpv.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2svhiunrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yigwpsyz.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2vpgsoypu.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2yrxfdsuk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2cgahzfwt.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2xtrackit.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2uzhfloyb.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lktixnzf.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2otjweozq.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oqksthuu.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2aixumfzw.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2jribvrvh.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2rjpuebhv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2soezojvt.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2fiykfgax.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2bhlzvjis.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2nowxtehk.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2feutdxcg.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2rdhtywiw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2ttrbfynm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ynovseda.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2oqixortd.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2qqrjpjug.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2arpmbzsb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kqgzdayw.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2fxkzwswo.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2iguevraw.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2evaymzcb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2mwlhcsci.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2thobkvum.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2peemtvum.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gtbtnsor.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2mogigyeq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mozhqvtt.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2syiaznvz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2isgpklrd.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2bsqplaqs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2znqmyqfa.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tdwaygfx.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2tzunmoyq.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2vzryldmn.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2vapioaos.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2rqebtwst.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2kdzvxxnj.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2zctrmwus.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2kxgjhudm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2jxtcjeun.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt2lwtjjisj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kmgesbuq.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2fnovkbwm.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2txvzumuq.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2zvafqbel.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2fwmswjbz.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2zyrijmgq.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2bvdkwzxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpdzwyxl.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2vtvzydex.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2redneybc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htinsypb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2zglnippg.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2ushjjxzy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2kiwnbflv.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2evqjjfpx.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2ffptmnia.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2umnikytw.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2mzxsglta.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt2npbzbphz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2bhhlyitn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt2eyoaadji.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2mrcyqnpf.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2adytyspb.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2wsyphjtq.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2eiudmbro.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2hmvgkxuk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2vdqhaytl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2ipsitjfx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2szqtsgkx.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2moliaupy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2hkpqsafs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2wbrmwvna.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt2kesyjwgh.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2hhmspcsy.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uimumvvk.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kewtbmog.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vyeantel.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pewjsrhu.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jtkhcgpm.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xftgomkf.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2proyviap.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2alszqfqd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kogbbsbm.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2cpwpumwh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2gqlkwsam.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bieykzyk.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2uveobbid.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2wiwjetnd.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ciewfirt.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ljynqaob.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2cmzelznv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2virnsdzk.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2xwlkhnug.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jaoqwryp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2pmkmupfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avwztxua.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2pjskpmjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snnoxmuh.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ahusazap.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2dnsgdjcg.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2umqcoxib.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2ezfqgzrq.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2jvrnpldd.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2clgamelk.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2banyqasy.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2zcvaxoff.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2oubxvurb.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2pxnpvmvo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2fibjvpgm.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2sngyqwen.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2wsxcbgaw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2pkvcjnjd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wxxvsqqd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2mefufuiw.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2luanbviz.html


<!-- 参考信息 -->