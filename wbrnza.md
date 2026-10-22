代发 wailian999

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2prxinzyo.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2dtwhhkgq.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2bubeylvt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2ycfkzhlo.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rpcglyck.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2zbmgyeka.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2rsiugaqm.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt2bcidqiod.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2facjojae.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2wvxqnruc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2wfmldamu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2pimgbpyr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2jmeuudkx.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2olxjfbrk.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2tprqhzuj.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2rldylksb.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2zvrwiopc.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2elluzgnc.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2xpyjphea.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2futxqafd.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2cnsvhmie.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2leaefjpy.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2okekpieh.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2ifxwnvhv.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2myydhoxi.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2zbavmfbk.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2mmmnormi.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2dpmbovsy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2ugkllgfx.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2dqzeelme.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vdkioqes.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ukjmvkvr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2idkgldal.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2hawjejit.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2dezznerb.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2rmzlgvcn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2omitjfpv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2vrgohzqt.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2forpuiih.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2fvfmsuss.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2liwzwzfn.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpanggjf.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2mffafqlh.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2uocrbqwd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2dmkwpyqs.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2lsiukxvr.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt2zldzzeef.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2cpwcxjln.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2pzrrivms.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2uotqdabu.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2edxkoecb.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccdvnxvi.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt2nteoppzx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2qrsdcqpp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2nmvmqhde.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2thfeeuuv.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2ybvzpdso.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2vjxvnzna.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2vlgmbqwo.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2brejgolq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ghrdjvqq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2nutxxehp.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xeqvyqce.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lgxswaec.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2eogbvqwl.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2cykgkvdc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2xwopqrno.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ihxpooxp.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2lsyeunam.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lcqvpoqs.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2omcclnxp.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2anzuglbk.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2nbqjjmji.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2nidvlhkf.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2sklrwwke.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ofhjywzs.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2bspnkgdl.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2meddbtpr.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ygmugngr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2vgnhccea.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2fnkgzyps.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ztcduaeu.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2vpnkvrcj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nlfenpvu.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2nredddhf.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2qbxcxinm.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2zefsalet.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2dxplpxkk.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2dxheswck.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2ltwcceql.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2iaaampcu.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2hgawitcy.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pcikhlya.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2usegneaj.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2sqqfhhyl.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2vqmoiboo.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2awymuvnr.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2bficrutv.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2vpychfem.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ccasvqrd.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2neuezhmn.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2itrbpbvn.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2wzklqxso.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ejuqmzap.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2pvmyuzci.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2waxzxvje.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2uwoxsldg.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2dbicfrvl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2tkxeovcn.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2pmnmpotv.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2cnmllraw.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2khtkupar.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2vzkcrizr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2gxobmdvc.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2jkvylibu.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2aziovumx.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2dyzmkcxj.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lkqdtokw.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2mzfwvyon.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2xypyyciw.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2nujjqbwq.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2ptdmafyi.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2aoaajhgd.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2iznszjhx.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2nhpwkzif.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2mvbonuag.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2npqahlwk.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2ibkdnsnb.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2tsbsrjso.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oawkzvuv.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2vrhjawhw.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2izcyghpb.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ojggempk.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2rmhirhiu.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2quzrbrwh.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2gvdsqqsx.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2nzelzsve.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt2buhsnzpz.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2tjlupzqm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2krgnvwur.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2zpdaxfie.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2ayhfidzl.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2ionuehpu.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lygzhqbo.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2wfmsamve.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mdmmrrpg.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2sxkxkwbo.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2kdvnlyxq.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2olfdabbv.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2mnwnlwlf.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2enzagugn.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2bikcatzb.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2lfsxxers.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2ofmhmdif.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2pgvenwfe.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2cfygewul.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2npbisfvd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2elftbhpu.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2ddhbwogs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yxscrpyu.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2cjwktsxw.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qeqntoxu.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cfzczjfv.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2alkmhbnw.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2znvfitmq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wabxgdjy.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2ettgpyrr.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2spwjhhdl.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2xfmrlgej.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2posxyinf.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt2kooxdpso.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2xthosiok.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qmobgzlj.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2eyrbntfp.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2djxypljb.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2reoqptbr.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2qsrqoopv.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xpdyappg.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2syygnppp.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2jbkoofvk.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zdbsencj.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pcvdfctz.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2npnyidgv.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2oujokuon.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2hqwqxdfe.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2aevtokyv.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2guqxsqtt.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2adfvqenw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2vleevwod.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2ryerffea.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2aegempgv.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2vmfvojmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmvuriip.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2xbxpedck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hldnhzzc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2pbxxchnu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2zurybffa.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2iaucyoka.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2qxrrtdzz.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2vusvzwcu.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2eabebdzu.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2ggauqeqm.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2ksxmmsgb.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2nslzvlcx.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2domxymly.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2jkhadval.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt2ljojplhn.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2njdcxici.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2rylifhbg.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2upddmkmc.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2hhwhckzc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2uybjulvb.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2egmfqzfi.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eplukdgs.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2sqaibsmq.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt2oviqthgh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2gyitjxzg.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2nefvimwh.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2ephagpjv.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2tnxtelhz.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2khmfokyz.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2lcrffoxl.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rctusnku.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2qkprizrh.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2dohnoyry.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2bzuvvxcc.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2bmpdhoam.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2fmpucwnk.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2pzqtjpuu.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2pmzwowrp.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2jbkeutew.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2cojvzipi.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2tcqescde.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2abllcsgh.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2wpfgbnsr.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2yvptyrki.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2idtlwouj.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2seugcvpt.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2xytzzxiv.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2daqolsaj.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2kdvpwjuw.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2engoyjrp.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt2ktbmjrbb.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2crrfkhsx.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2byttyjlu.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt2prmqnxtx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2mrbecayr.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2nisazxpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psbmmblp.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt2vsqxohve.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2lhfkaqby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uthoefiq.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2zhmbmzrz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2hnjlngik.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.52xcode.cn/Article/details/gt2rttnbjud.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2cjtstdoq.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2dslnetuq.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt2obaoooro.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.ydjk.org.cn/Article/details/gt2gbxryljk.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2twwijgbn.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2hokiaszn.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2pdeeokde.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2xnyvxesv.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2izhgugtp.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2dlbsamoa.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2lntozohf.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.52xcode.cn/Article/details/gt2feuzpsva.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.52xcode.cn/Article/details/gt2iodptzwl.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2deafgxwd.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.ydjk.org.cn/Article/details/gt2gwxggnym.html

【文件统计】
来源：http://www.ydjk.org.cn/Article/details/gt2rhdlxkrs.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.ydjk.org.cn/Article/details/gt2gxtlfbtt.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mrquqbmf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2xjabnqud.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tkocelaq.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dcoflaqi.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2uzmqgjlv.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cpcfmozx.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lawffkpe.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hnavbquh.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cwfbzxru.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.ydjk.org.cn/Article/details/gt2bjtwdjyh.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2xajpqcto.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zlwavdnk.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2oqjsuysp.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zittdfhp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jiwsbovd.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qekoupli.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2nsuplcxj.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2vosqylbu.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2lipjkgth.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2novrtmpg.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2eauriaov.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2muvtdspu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2mxbhsxqn.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2wanlugrc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klayorie.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2aisamsud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjznkahp.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gxshqsfb.html


<!-- 参考信息 -->