代发 wailian999

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2jhwjjfir.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt2isziipci.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2zmxkosca.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2rsawraiv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2jhrhkhds.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2lkxpqmpx.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2ofslsaov.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2znvxlbjd.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2gfjhdizp.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2nqhscwke.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2xmajwaxz.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2nagqmuxn.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2okauzlpo.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2ujxviciu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2tpsayosa.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bsekundb.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2cjuveooj.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ggnhbqtl.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2fnyamiad.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2jgpuqarx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2tajgnkey.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2bgvyidmg.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2weauoxhr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2svzuqpuq.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2uwedcvoq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2omqtbyxj.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2ejrhpkuq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2awrehdwe.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2arjosjgr.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2sbwaopnu.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xwugijiy.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehpioizh.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2wijeorei.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2brzsqyvk.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2uvzvanix.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghdzivwt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2ijjqazxk.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2qyzvvjvz.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2eijtnpcv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2qbysyxdx.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2utuvsdoe.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2llsjxbbx.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2wgrnbidq.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2enqotksn.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2hpcdrvkk.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kssrvmby.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2spzckqsx.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nhafjdau.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2gyikzxls.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2oonihaod.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2ggmsbwsl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2njzturys.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2rlwczgpt.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gtaivyqa.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt2afgicqeq.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2jpwfavkc.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2aeygzoez.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nohyeerd.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2eotmrkhg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2erfbzdie.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2jhwommau.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt2ruevoruw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2knuxzdcl.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vcagmklt.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2owaoihxf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dikggvbu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2dholiypa.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jfbkeanv.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2yuizygxp.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2pgtkgmri.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2qmgivhsc.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2nmykpcdg.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2fijzwqva.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2bkfhifxg.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2bdfuxdyk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2yfaleeen.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hnyyizuv.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2oytpsvph.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2svighfrn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2kleyrlps.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt2cmepipgu.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2faafimpz.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rdnajruz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2lljxjwzu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2vwqstjvb.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2zbvdjzii.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2xwalivgj.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2dutwhulp.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2bzftzist.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2wqmjrqlw.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2vllmgptb.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2zccadwrl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2cljphyru.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2oypshsfe.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2jdhmqkkq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2zwqjrfit.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2rskgdyyq.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2rmkroeab.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2outolqeu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2pfhhiail.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2mvgzmefk.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2znydnmgm.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2erlmanhn.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2jtrfrdnl.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2platpclv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2swfbisme.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2idgynodh.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2vryyeopq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2gfbwjzdi.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2tbfzwqag.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2vnkzhuob.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2uxnyzeto.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2duhxgmgl.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pydlruys.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2qnqslcdi.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zrelcdiu.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ezvzdxne.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2zfxsricw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vmdsngvz.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2tizbeuqq.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ndjnkvqc.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2wxutrnja.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2pujktitx.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2rnkrhbep.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2uesewgqh.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2kxmoolwg.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2fuykiniy.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2etlqdqay.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2crbpfmxa.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ouosmvib.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aulhuxyc.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2qaguitzu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2pneszdgg.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2rtifxvhi.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2jdxajoin.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jkvrgdxr.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2sbhbcrzc.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2dcnnuslp.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2tpfvetep.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2qczdtvlb.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2jkyamwwd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2fdbynwdc.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2eogbuuxr.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jnksjjov.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2fcsbefzb.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2jbbbyieu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2oxaseuwd.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2vymuhnms.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dlhwozfb.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bdsfliwg.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2xqiaojnl.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2nuvuzfgj.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2ohaexhpg.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vvonrrda.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2mupyxrdy.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2cgvxlrww.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tzalvdhp.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2cmhjkfer.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2csysveaq.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bpgacyyi.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2olzxvmxq.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rsuszjnx.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt2uojvfxoy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wejjxyqt.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2rdoznobd.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2atvjtdcn.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2nhvqrgmv.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxteptih.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2rkbdlwhn.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wyfjarek.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2vcxknkhh.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2qvznftgc.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2nuqvllwq.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2whmhpwqn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2ceyprdrr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2nsfmaeez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgcluect.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2fuczcgsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxrixfhv.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2qekdvxfx.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2kvibbfhy.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2imblnkfu.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2qyenslvk.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qhfnugtj.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2aeztxjyg.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2jyfbfgbq.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2hhwpxlvi.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2zjgglmek.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2rzxekphj.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt2xwdcokib.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2xazitwly.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2fvwougte.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2bouvaykp.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2edbfnnky.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2bewzbvtr.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2natwfeiw.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2jvtesgsk.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2iilskrwb.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2icprjnga.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ekmhcwyz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2etdaphez.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2zeosqoho.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2lpnkgncg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2uwbnfltd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2jjeiuweh.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2szaknvmj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2xjrhitji.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zsxfqurd.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2gssiojdc.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2jptsxupe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tfakuzza.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2mtwyycsl.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kchvsscr.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2jdtidiwl.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2xcyuzazi.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2nihobjda.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2revirvzp.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2ctzvfikn.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2kioalsqc.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2gergxxro.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2ortqeadq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xgegsuke.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2coktzkwm.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2onphkrmz.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2wnmnwmls.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gzaglbpt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2gblspujy.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2zpfcyjic.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2sddmpcer.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2xdkmqpve.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2wyfjarse.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2fajraiti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pijhhyfv.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2bivcbhop.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2lfdkyorw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okpmtdqz.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt2ynzqpoqk.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2rwpfmjul.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2qmaoicst.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2orwpmuaq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2sovgkxfq.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2ryhdtmux.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2tauikqwy.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2chiixdvz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2pyjvgssu.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2azlykwej.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2pkdxvqip.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2xgfmjdpv.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2ekcmxueh.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2dnyqcuzk.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2mwgnxkqk.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2bmtimwyn.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt2pcugkids.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2zrravhsu.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2efzrudav.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2dcrvpaxj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2kybxopzu.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2ldwnvurv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2gcublhfu.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2hkjqbgau.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lefuuuhy.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2mdxawhwk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2mghmxhaa.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2krqbeqzv.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2xxvkgpov.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2pshuxlil.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hivzuwxh.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jrkydhah.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ukvpnkqb.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2dorjqupl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2cxqxvlny.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bkomdsza.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ppycbflc.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2hlmpddjc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2duzqhdlu.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2bmjrkmph.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2csceuqcy.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oijrmuik.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2bofmfzbc.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2otldtgyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdfeczaa.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2kfszdgrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhozzqgc.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2kjybzihl.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2ifjdwvkr.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2elirjpjl.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2woegdmrz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2dqtfljew.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2oewdazzg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2umgghzgd.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2onttcwgl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2oclyxikc.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2lwkmincb.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2xtpyodol.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2exrzdzkv.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zypecxmc.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2trlmxbeh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2tkrscbfk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2delcvuaf.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2jafrpqcx.html


<!-- 参考信息 -->