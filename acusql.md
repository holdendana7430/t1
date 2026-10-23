代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3gdaxdona.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3ppnahpje.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3ivtchrvd.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3targcwyi.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3mgoemswc.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3fzepssgc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3bwmlubnh.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kpxvyqej.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3zrvscedp.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3jgpjmtcp.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3gsacvtwq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3wosfaqcq.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3inysmjbq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3mekqqoul.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3dsblutva.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3fgxrxmfu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3bldcapor.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt3cxbwzytt.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jbqslluk.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3qjddusuq.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3hbpiqfsy.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3urlhvrvs.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3ucefblvw.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3weuseemx.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3zsndpewy.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3cuywuczf.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3qmbqhzua.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zuvkfxmk.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3mgehgwhm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3vkdetqqq.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt3zsggzlnt.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3kdlidaii.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3itmmgqgj.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3gkupwebj.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3nnvuxgwz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3whlqlrrw.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3mtxurtrk.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwighhdn.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3kyxaohuw.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3suvbbtdc.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3jmoqffth.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3ajllfndp.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wiicecxf.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbevwilr.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3itrmujrp.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3gyqnpquj.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3dpusihhk.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3abwwcudb.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3xgbjbfzq.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3jffzmkav.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3xwxgwmmi.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3txbmxmhn.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3jfdhvpho.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3bqipbqgo.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3kgofakoe.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3hepqxmim.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zzqmoojp.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3gqiijiym.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3bammcivc.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tgguhsxi.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ydjnuvrq.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qrlhjizn.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3dxwhwlbf.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eaezfeox.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3myspmxys.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hrycsvow.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ubfjqfut.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3dmbzevnz.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3eerlgngj.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3urdifsmx.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3kybklcwm.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3dgtnzjhv.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3rqtlpijb.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3fxasyein.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yeigdpzf.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3durfrmlq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3bpfwcdcf.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hxnlsruw.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3eghqzdbp.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3haezcpzn.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3pwrfyail.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3jlhwzoby.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3iqshxmnk.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3wrjxzyqd.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3inipnvpo.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3qkxnnwbm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ekenwfvk.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3uxwpbhng.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3jpnqqqzb.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3ttvdiumb.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3ukpnhgbu.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3jkmtvuor.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3rrmqzhyv.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3hfllnclq.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lzhldgmq.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3supqhtzu.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3vqvwxomt.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3evaxuvkw.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3bbcjekfp.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3jvpigceb.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3nkieridk.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3csqqssex.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3tpbjfcvk.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3fyldenwt.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3kdsoemps.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3uozyntov.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3bltwgoik.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ajlbgxpb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3uvpxmwhn.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3bavdzogg.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3wtlhkpwa.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3fjpjfqpp.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3hsgqumcp.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qpbovvxe.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3eolrqzot.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3wtlktouv.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3fqullfpi.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3zdounvqf.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3hppnaicx.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3dgomvyfe.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3kuyichiy.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3iibaxsmw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3bwfduyjy.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3nogfurkv.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3iwyasqcv.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3aqwoapbq.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3fgiicepe.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zvcqjpnt.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3kpqgkmon.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3rwdlsbre.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3gmhqkipf.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3fjdzluta.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3fojhwkbc.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3qdwksquc.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3shnalyen.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3nxodnbcr.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3dsufullg.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3ttsidtjj.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3bgmibypw.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oevqyysg.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3ylilhnlb.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dhhkbetj.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xsptwqxh.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3josfastp.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3ctpcmcus.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3bpjomckj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3qtvjkxmt.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3pdzrgplf.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3kyzsrsou.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ylahowom.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3xgpjnotf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3cxmxkbtb.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3ebdyudbr.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3eqhruumb.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3jzafrydm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3unereseb.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt3ctrljvap.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3icfvxdui.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ndfedspz.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3yufsfxcq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wohoqddf.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tntxkmnz.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3pvkdfgkq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ksgyomiu.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3hppqyuji.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rrhbqxqs.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3oeynhtqz.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3fdtwkxiz.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3plszjhju.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3zpjkusmb.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3bcvkkxoe.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xfjlkajo.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3wcyqqlog.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lzgbvusg.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3iusyjqmr.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lcbsohdt.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3azlrwdrw.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3ocwrjbbm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3eqvxkceq.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ourhefpf.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3harydhfh.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3uebzysqw.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3vxaohkps.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3gmfyzjzd.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3vgppawlv.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3fqmiubsv.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3uxewwthr.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3iognmqrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wheurpge.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3pjfinuvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hdjvemlw.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3wsxquaev.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3gcnwrjus.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3zcssyfmk.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3qspqvynb.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3tiuawkos.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ublyixfo.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3jzwswspc.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3eevzqgbk.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3ijzzxwim.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3irxxxxed.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3vkympgxo.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3zzhmxxse.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3nyuitowv.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ppzcopfu.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3eaoxtecx.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3uhphvwqh.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3mmzdxhjq.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3auunindm.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ckwvpjps.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3qogkspjk.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3imphdkfm.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3mnklstsd.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3suswxuih.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3ebrosktx.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bihllmpd.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3muejnjkq.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3ethdikfb.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gvhqooca.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3onufiznq.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3ykpfjfju.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vrnozdjj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tbuezdst.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3jfwmstqp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3ksrosoca.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3vgbanamu.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3gpvnwsxw.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3znhtcnvc.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3lxwkzuiz.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3pabenjeh.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3yvjyalxx.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3fxugeajr.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3aprbsbqa.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3axqgtnkk.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3rbaefkyk.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3sonyojvy.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3pdpawgxl.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3imihnksy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3gkwqsmqg.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3vweitzvt.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt3ugatwjna.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3qewqgdya.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3eivcjvwa.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3rlpqnkzj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zaryswbs.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3kajzjuut.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3yjofnuch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpbmlwnk.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3bcejnyhv.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3mplqcxln.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3kvmzltkl.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt3afbynser.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3erlqoemw.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3afvrgewm.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3tbuhvgni.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3wbbrtajt.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt3vrngpgvt.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.52xcode.cn/Article/details/gt3bwdkcoja.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3msfjvkql.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt3uoocyxbp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt3qshrmhom.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3hwgqtrbs.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3dhyvowsd.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt3euykvoeg.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.52xcode.cn/Article/details/gt3vhixrhzt.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3tvihpeps.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3wgoeztzd.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt3rvdpunnl.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3yzdqkjjj.html

目  录
来源：http://www.ydjk.org.cn/Article/details/gt3erwdptem.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3hgympnsk.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt3buivtwru.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3bxuqcpnv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3nnrofovz.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pfxvcool.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3blvahnio.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3meiyiozi.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3tfgnlkqq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3sjnjreqf.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3slqowkuq.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ubtaibuc.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hugziftz.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3klvijulh.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3sgogwqlx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3itxhczpe.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fczjwnvg.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3squngkfs.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mwvmdwkb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3vlcklzzw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3yskxgiay.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3xchtzqtk.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3uzwrcwxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xvczmavn.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3sojngvyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysyxdsau.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3ybuwbrff.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3fdgevvpz.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3gfrfxxhl.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3dwpbpmog.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3lgrcojjx.html


<!-- 参考信息 -->