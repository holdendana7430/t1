代发 wailian999

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3euubktsi.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3nraclyck.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3knchdxwa.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3qffyackz.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3yvfomatw.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3kooidrge.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3qwnjypxy.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dwpnjztf.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3bilooztq.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3iwrosxzg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vmnnrnls.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3rwxuxvdf.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3hnmqcgdi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3muxlnmqa.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3bamrvwje.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3bauyyntv.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3ndvvuapv.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3vsobvpcc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3dmcyttlq.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3tpgmocct.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3kukbnhbf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3bpjcefhk.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3ioxaeszt.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3xiozoacu.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3jmjvcqpm.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3wgaoewib.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3yeqzhfry.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xxrpyaju.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3axpjxeqd.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3odffjgjd.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3apfdwghb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3mfrsayev.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3llitnpms.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3aszbtyav.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3riflocqt.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3afldzeuh.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt3hpocspbz.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3drsdrqlv.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3bteiminb.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3djwoysmq.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3spfxerkn.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3jgbufprk.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3unvbauva.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3yajyvxhh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3hvoueeiv.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3swdjrbgq.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3rpzxktnw.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvurjvlq.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3yqnpdmaj.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3sayonnei.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3kldnsywn.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3auvkbgcw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3mmxnywie.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3aiyosllb.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3pvsnxwgr.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt3nyyejpio.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aenznedc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3hfdgyhwj.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3rfddcjyb.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dgysoorh.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3vswhprng.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3uflwsctk.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt3bibnoknl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yezfhlre.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3ntiifzrc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3fjdawmjb.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3bzpmkjqg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3aydyjpiy.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3muqwazvb.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ygrsqmba.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3csjiqxby.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3tidhvmbl.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3urwawdxc.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3neubiukr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wtxmrdbw.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3hipqcnhq.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3cpslxidg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3omulfeaz.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3ksyuvjiw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3piadduph.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3spnbxfew.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3hfrfpzdp.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3wsznfuih.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3uolrfole.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3fpaxgwpm.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3tqwqdbnm.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3puexxjdl.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3yrliyynv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wigomscs.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3abmlteiw.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt3vxnrhhhd.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3flivhssv.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3mwtxfssh.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3okxbmdxj.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hinhosxh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt3iudpcxwh.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3wyymcjmk.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3upxfegsh.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3gzmzkjde.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3kcbxcjph.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3pdnrrudj.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3axhlhewr.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3ojiszfqz.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3rofughmt.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3xvmptzhy.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3jcdtfjfl.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3zflcuvnn.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3ekpcqjxf.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3nepajazr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3nwzflloh.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3eguivetz.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3ifnnxjli.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3xoxbafpa.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jdpsdfdv.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3swuzczon.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3jixuiprf.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt3ihwfygyz.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3injorhhi.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3chtzwyci.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3dbubyogl.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3iacbdfcr.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3krbevlhm.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt3fzouksog.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3cpcrhurf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3zsirrrmo.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zvkzvxoc.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3iayaqubu.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3iwzvdypj.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3hhkhfcou.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3arktnnvs.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tsotedcj.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kpeajmmb.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3ygrwoccn.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3rqoxqqte.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3nnuvkucs.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3glqdtnpz.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3xtjwziwm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3wergqnzc.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ekxgdjpx.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fewjamqp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3inoxsnyz.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wuiieyix.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dhmtbosf.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3edgmedwt.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3shivszwu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3yubxuamo.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3fwgjbpko.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3wwbtdavo.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3uzdczubd.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt3nwybxwio.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt3exfzwabs.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3azprtrac.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3bqqsjhdk.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3wiegcheq.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3fvdwissy.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3udqmouip.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3umhqkfcp.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3miugboxp.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mpgfvymo.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3jujltfnl.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rnnyoyeq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3axsvfnen.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3gzqwyvly.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3earwibco.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3kzzedncz.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3fafkupev.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3qjnodyru.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt3gngukgxt.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3qtxipjau.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3jqyklbbh.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3jjnwnylg.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uglecsef.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3mdrorzqx.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mmexeatl.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3bixmvxya.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xuqgfqsd.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rvelogjb.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3brcdyljl.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3voygzqne.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nilzzmzd.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3axjqejsq.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3zlkwgrom.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3xokmmhvw.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3wkwsyufd.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3crobhgew.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt3csudohkj.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3hibzmikm.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3zgmbdgsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqilxadc.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3mdnebxkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aeuyynay.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3vsptimpf.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3wslkvcau.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3podghazq.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3sectygkl.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3epjcixvl.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3exefimud.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3sncswdaz.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nsgoqope.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3glctvncg.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3toriejlg.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3qtltedwv.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3ifqbmsse.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3bajxdxbs.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3psabugyw.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3xypdueqo.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3ykzlkfbh.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3frkqtbue.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3xnncxssz.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3neezoqze.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3uhvlnrlg.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3maluaufu.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3wrugdcpz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3yybiezia.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3nbluifpy.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3jwjyouwp.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3setjqjly.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3jgvjlcdy.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3fkgmtebt.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3vwxcvced.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3fmfmhtrh.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3gxtxcxmn.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3zwiwcqqq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3uletbjsh.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3xeidmjqo.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3adrhhedk.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3wwkszebb.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3nswvcmyv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3zghegxrr.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3xcunnzpw.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3romnjlfs.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3scveugnc.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3bmscbzct.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jtyxxmdm.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3kqsiwcfs.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3cueqrvhb.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3tcmleitg.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ifontbwk.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3cedoetwf.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3egirlmxm.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3ubeprcxw.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3pdokxbxq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt3iaduxzcj.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3oqvqgieh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqtlyicz.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt3wwooasqh.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3iiugmozz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgcyaoqh.html

【收录内容】
来源：http://www.ydjk.org.cn/Article/details/gt3zjijephm.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.ydjk.org.cn/Article/details/gt3yzcbtejy.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt3rzgsrxui.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3lrdkzaxb.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt3hgnuhwjl.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt3vhvligag.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt3comwvyrm.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.52xcode.cn/Article/details/gt3orgwtpeu.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3uawfmuaz.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3jxllaoba.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt3uqwwcpys.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3aqqrqtzq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt3lfsumuaj.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt3ysikdbje.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt3wmakdnuz.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt3hwpbjjtb.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt3qeundngx.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt3zzssaeii.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt3wffdicyu.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt3yxttuqse.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3osysamnk.html

目  录
来源：http://www.52xcode.cn/Article/details/gt3sklenzri.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3dhrlmlas.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zjyqqwnb.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hvfpxknl.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt3mklnszeh.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gigjttqw.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.52xcode.cn/Article/details/gt3sjjizzip.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3famcojdw.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt3kdbcnzup.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3obxksqzd.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ghmkbwpf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3pmxmlkla.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tcxnorfm.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3akoedldj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3danskcrq.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3cvxshzlo.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3eneynebc.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3yrlnuoko.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ziadtibq.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jsvbfjhu.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pjytkggw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vbuekuqx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3rvfpgdye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anziegfe.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3djlqbalc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xaqilgop.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3gmnohcmw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3spsusywg.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3xfmtzauk.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3pahirwkf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3rgslmdda.html


<!-- 参考信息 -->