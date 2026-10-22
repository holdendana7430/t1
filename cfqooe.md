代发 wailian999

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2gwnmyald.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2pohhuycr.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2yuhqjkbc.html

list(zip(*m))
来源：http://www.52xcode.cn/Article/details/gt2mwcghahv.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2idpjvpxz.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2pmmdsndf.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2vbmhoesj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mslumxzx.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2gpxekbub.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2polkozfc.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2ketrwkmv.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt2lanfdcib.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2rykmhjjj.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2chkvslyl.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2zmfbuhxs.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2jnjrggtv.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2vblntkiz.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2wuezpveh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2wfteqvcs.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uvkzddvl.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt2zvkmvyml.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2wkzxxsop.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2puzbanox.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2psidzsji.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2isskwhsk.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2ayshazcq.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2playdswb.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2ztajheay.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2ytbpwxga.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2oqqolqav.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2azgkpxhp.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2rdkicmib.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2hzqfhhxg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2qseepfdl.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2gwbhkker.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2pbzznoqy.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2hymjvgiw.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2pzhkqhdf.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ursfkfol.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2czpvwfmd.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2ascpatxt.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2kmeasfvh.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2gdzjodia.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2sxkvexvn.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2oiietwmv.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt2iejnmktv.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2kjvfryvz.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2wssbiskp.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2mdtkgwgv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tpbzlmcb.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2pfpiwisg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2mesaerdb.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dbtuybnb.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2ggakttxa.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jvkbhkiz.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2deylijnp.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2seikopyl.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2bydnrqga.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2kjtmdlse.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzcveutt.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2kpldiwdo.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2djdpwewu.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2frdhbvjn.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bndcquss.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt2qlnwuyro.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2vjcvyccy.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2eaflaleg.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2jrtfvidb.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jxspgwqq.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2rylvhkay.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rwjcmxfd.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xxdrqpyv.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2gbodzmmu.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2osfwmncr.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2tluzfgqa.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lscvukoy.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2prgjzsdo.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2udwwrlgb.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2njoejnpa.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2lzrzdxcj.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2gzdswzyo.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oxucbxbl.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2sbuksptd.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2tqaszark.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2yemnvrrt.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2ggetrugw.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vgukzbdr.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2kyzbeusp.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2fpcrcmri.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2gmwszqww.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2nlnzaxpw.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ohzzozgd.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt2ftyomgde.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2wlqdfxzw.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2tdrhcdhd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2keapatcx.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2rgcpauxg.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2wljacquf.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2enhpnktg.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2zczeahor.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2sepkfbyh.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2dxwglxly.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2dazwsonn.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2hyuxhkaw.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2hcfdusac.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2pbknzlud.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mnhcwihh.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2gygbjqow.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2amfiwakm.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2jqsxumgs.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2ejllrbaa.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2upkkbiqx.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2hnrhtdml.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2lgwcjrvp.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2outmmyaj.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2mqjenfoz.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2rttcqyns.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2dpcksegy.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2riocosjd.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt2udwfltez.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2kubrdmgs.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2gpizvake.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2raclvvci.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2vyebleun.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2hsscoiwx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2irirores.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2bxdeqgtt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2tmcmvtgz.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2rdndzsxs.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2azparagi.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2jxgipqxg.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2zmiwfmxb.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2fpagwpoq.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2uhqwstzn.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2ywcrkqbs.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2ncpiieaf.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2qhokpffr.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2amtumfhx.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2vvsndbpu.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yegqwgtn.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hqindbyp.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2npwkrwmk.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2blbmwjcm.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ktooicgp.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt2usjssfqx.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2ltqcuebd.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2afusfszy.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2ldtsdato.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2pnzonsni.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2lzqmtolq.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2jsykaivk.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqvhkphp.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2cqifkdrg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mcgcewek.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qyxjnmqv.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.52xcode.cn/Article/details/gt2hmnseswq.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt2dzppdlul.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2ubdrweax.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2acjhihnn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2mgcrhlbx.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2gfxqwqmm.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2wftvrnox.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2uoheyyez.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2gzsxlprs.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2vakhlmop.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2gdxyvysv.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2fbhzjjvk.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ohudzbge.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ujtwewxu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2qyopnwzy.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2whyusdpg.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ffnusszh.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nawkozjk.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wqvwnniy.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2tehlqila.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2ppsiihni.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2jitbadtg.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zyuavyyn.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2vswpviia.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt2vudskoyk.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2aqlupxnc.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2dfeekboy.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2thnkekky.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bwfayzhn.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2lyoioccu.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2egjdizbb.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2xfngqpqv.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2clkqoufx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bpmhrcbk.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fapuhunu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2asdjeqqq.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2lxcczley.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2xxvhdnvl.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2wvzaeaos.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2tzugrelk.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2nrikmcnq.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2chkbaqfh.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2toazebcq.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2rmxkxzhk.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2taohtfkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ojuhfjcx.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2meveoybq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2raeelfqr.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2zrpwkgjl.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2echhaejf.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2sldbyfou.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2tcdkoxrs.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt2oadtbwwp.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2layoquds.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2ewdywygx.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2eqmkqefw.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2oreevrgr.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2zprgyhjq.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2cbmkautk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2dxahkgrt.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2ltopzxrk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ivsuqfyr.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2vuezvcix.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2ghyockjc.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2qqsbleus.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2lurpeswt.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ffykqpxb.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2vwybqmcz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2crnycjqz.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2nmclqdoz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2peudlhen.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2baiztinl.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2icmaohyj.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2ruuaycqb.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2ksecvgne.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fqbedfpf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2clgwuchv.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2tkokmjzn.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2dwtncabj.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rjqxhlsf.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qjmvcrxp.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2ziopslni.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2ukcehjwi.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2srwbbtny.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2rfuyivlt.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt2eheisitd.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2eshsovbv.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt2swvzcvxc.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2qbkxvrkv.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2npmlbpzd.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2mixxfvao.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2xhewmfxm.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2zawczxsk.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2omkavpzs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2rlwzjoee.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2pptgizid.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2jeorcmuj.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2apkmvowl.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2ujmxeaxf.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2dzszbhgy.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2eqhnqona.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdcyhgap.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2uyjttvlt.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2lmionvwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvzblieu.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2zljiqrfs.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2vvydmbww.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ampgugti.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt2itcdljgt.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt2rygpyukd.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2vezfmclo.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2npulbsbo.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2zhtzyggk.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt2jfijaroy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2gdnbpdzn.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt2oncmrypo.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt2izmtnmyy.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.ydjk.org.cn/Article/details/gt2bbqaxzva.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.52xcode.cn/Article/details/gt2yduzbbgc.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2wecxkafv.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2abhafftc.html

5. 标记为 "// 无" 表示该语言没有对应的一等语法，需用替代写法（示例给出替代方案）。
来源：http://www.ydjk.org.cn/Article/details/gt2dhwgqevc.html

6. 符号 "⏎" 表示代码在此处换行（主要用于 Python 等强制缩进、无法压成一行的结构）。
来源：http://www.52xcode.cn/Article/details/gt2uyujzwnl.html

【文件统计】
来源：http://www.52xcode.cn/Article/details/gt2kmqwbjuk.html

语言示例共 2106 条，分布见本文末尾的「统计汇总」。
来源：http://www.52xcode.cn/Article/details/gt2frhtcgcq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2aumdncwf.html

目  录
来源：http://www.52xcode.cn/Article/details/gt2jnegiroj.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2qsglxaow.html

A. 基础语法与类型              （第 1 节，26 个任务，208 条）
来源：http://www.52xcode.cn/Article/details/gt2qufwrkkz.html

B. 流程控制                    （第 2 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2zeqtnwtu.html

C. 函数与作用域                （第 3 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2lkgfkfkk.html

D. 数组 / 列表 / 集合          （第 4 节，26 个任务，208 条）
来源：http://www.ydjk.org.cn/Article/details/gt2uctsmbzb.html

E. 字符串处理                  （第 5 节，22 个任务，176 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hkwcjhcd.html

F. 文件与目录                  （第 6 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cmwrwibk.html

G. 面向对象                    （第 7 节，16 个任务，128 条）
来源：http://www.52xcode.cn/Article/details/gt2vfjfrdfq.html

H. 异常与错误处理              （第 8 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mcbmpcch.html

I. 正则表达式                  （第 9 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2veftaglf.html

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ozmajtku.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2olhyagwo.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2izbltboy.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2snoqszob.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qcpirqub.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ahhlhrtl.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ntbukmme.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2ldrvqlhw.html


<!-- 参考信息 -->