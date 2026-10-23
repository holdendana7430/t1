代发 wailian999

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3kcwwfxot.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3wrfqntgg.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3mokqvxve.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3zrefatui.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3ytbamhdx.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3osedbziz.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3cewqdkdz.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3avzctavs.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3psusdbeb.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3lneqscds.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bnntzaat.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3iofjexdf.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3ldogxkue.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3iaaklybg.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3nwnvpcfs.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3txabulyr.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3rbqqmufv.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3njdjkdbr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3ocilhswd.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3otjjunyz.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3hzlhuetc.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3jnacchpf.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3lmzpisiv.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3mdgnjzpz.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3sjzkjjgj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3nwrttffl.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3esndiojw.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3syxtojxa.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3hxjjrkmi.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3yghjqzpa.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3djhlqjsc.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3qpifnaax.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3cmfjneos.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3ijmspcbh.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3eqopewsc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3izlmuehk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt3mgtbdcze.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3spqnglqr.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3scwhfwlu.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mphlwxuq.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3nxzdaepx.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cwuhnmdr.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3eoyomycx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3pcitbmsw.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3pubszvqi.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3wdfcjeky.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3bfndlkrl.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3wzfttmly.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tciunudb.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dvmsbpww.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3cswitrlu.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3owwdwjcz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3sibzhahg.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3qnjvzfxy.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3ljnpoabm.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3zewwpwxf.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3vfqjprng.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3udhpyorm.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3dkprbcho.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lhujkjor.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3idwiimxm.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gaameycl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt3ibsoqpjj.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3zqisqcgm.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3lytkknko.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3orukpblm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jldkbtch.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3vtbezfdv.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3mrtmpbjh.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wqikxgnd.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3geuumnan.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cewitptp.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3jppnvvxj.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3edwsqlja.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3fvfiomke.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3tworcpsu.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3kojrwidl.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3jdmdxncm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3udaltnbe.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3chlcngau.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt3wokrqvzj.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3bbsinglu.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3fkgbepib.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ugmwqmgq.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3agvyfcpl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3ehlfglgu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qlrthmmh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3giyhdvnq.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3bhklkzpp.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3ifqsnewk.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3wzyceice.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3gbeljjvo.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt3ksyljtzy.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt3uneorzzq.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3njvtxfzf.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3lwptmizu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3jpahgecg.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3irkezuki.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3fszaktfz.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3zuzxemal.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3njltqjvt.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3siwenxyw.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3ctgyqqgv.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3lzqcfkva.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3vtujoxuq.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ucmkfxdz.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3fryojcwr.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3vdztlpio.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3fkqbtohk.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3vevtefdp.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ppqxshre.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3fyhtuyrz.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3tibmlahf.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3jcvekann.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3vyfbhvdk.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3wwygjqhu.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3somqhpvd.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3rapuvhek.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qqltmmda.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3rahuvtnq.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3etwgtewz.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3faycthfi.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3bduapqcz.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nvsuhtds.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vwnbchsu.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3eofifbhy.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3hffyatws.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3nzpgjita.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3ozucfamy.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3axchljlb.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3mgcsmfvu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lfzuoctn.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3hhwdioki.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wwjyelfd.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3cxfbxehd.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3jqrgjgcw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3tbmqliyv.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3ateqtcqb.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3dsrdtbwb.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3iwocyzmn.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3ielpihls.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3vihkeifi.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ozmjligx.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt3oopbsyoi.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3jsradbip.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3sghiksqb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3hmenckxm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3alxrjecg.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3owllvuns.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3bhdwhifk.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3fblpjljo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3kzdorjbs.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3whqalfrr.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rvojijuu.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3betkqnql.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qyogtfhm.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ytvpsumd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hpzzucfy.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3llgvprds.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3scfoojja.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cecqtqws.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3zmxhdcfj.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3qrghweuo.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hoqaqogp.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3zlevwxtp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3npgeehts.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3nvszdczl.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bjgobmgp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3mxplankl.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3zevlmxbq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3moivrwtk.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymvludoh.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3eejvnedy.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3spypzkyl.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3ppwjkvhm.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3hcjhuzdm.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3knpajxrk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3vdksumrz.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3bxeoiarz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3mtqxomcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rivexblw.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3vnayizvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqecwrqd.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3czhevmog.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3veuyixaz.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3hczjtvfs.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3dytsiuqs.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3pueemfcn.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3ukzjgbxr.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3hivvdojn.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3syxnfqyw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3xcewstjv.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3sebtghev.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3qobofzti.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3kyqkkccv.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3vjnxtobp.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3xwbcjnys.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3jucgyyvh.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3xnpxmeda.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3gncuhttt.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3omqpjdtv.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3hakcsnpy.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3vvfktwve.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3zenlcqll.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3lzildydn.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3suigrezb.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3sagercqg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3futevoya.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3nrdvjflm.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3irnkttmq.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3iukttwnb.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3djqpdovt.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3awybavlq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3vainpxoq.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3wqkffjvc.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fxhbowoz.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3hybynhfm.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3dddkbxqk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3tfibjuki.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3yfkbcind.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3uimuebzs.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3lazfzmff.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3sfbcnwkr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3fahnhdcp.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3iwwcfeyc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3fhhrwiej.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3heolhfbh.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3nymwpbbj.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3ptxfbzmv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3mmlhiozj.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3dlvojtrb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3bksxwwld.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3pucnivky.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3edenargr.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3vhztlhna.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3ofggyxlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnephzyo.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3eqvyhewe.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt3mxmqqzpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zyqwfdxb.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3zpkawvgx.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3ojkqvide.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3dxzfktms.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3shyplvvv.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3hwppjcgk.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3rqkpwojn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3ymhuiadk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3hkcqzxpz.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3iqxnlvjg.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3wxpegpoh.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3wdlyxyhx.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3ztfgihid.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3hnpbtrdu.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ufcajzlf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt3mrxfewkm.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3kkyzmfjp.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3tbvxborg.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt3fooluwzu.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt3wfiuvzgy.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3dbjypqpv.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3vkwajxul.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3bkiulmtj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3lomghzma.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zaxjmcbx.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3uosezlza.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3avuzqoxp.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wcjkmsut.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ydjkixqq.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wxmwwixb.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jljmvmbu.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hsltqwzj.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3rbahpdis.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3rafdkryu.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jupbrsvb.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3twijkwhe.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ekcmkvus.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fnptjzbf.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3mljrimdl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3abdfibkd.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rlthaamz.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3fhdihtma.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3oekewrgq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3zsnzhnzf.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3pkcxvwzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unkfwbks.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3dwwkczlo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epstzmpf.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gtpajxxa.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3jyhfgmpt.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3ragozoxi.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ruvotihj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3prqysjzg.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3bphugbbs.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3wkhderyb.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3yipjvghc.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3zqzfyxrt.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3upbdruvo.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3eebjdulf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3iyfttsya.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zhxzdfhb.html


<!-- 参考信息 -->