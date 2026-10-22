代发 wailian999

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2qtcscqeh.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt2immejoji.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2sdhjorwn.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2ydjmmrtg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pyxqnbxd.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2uxcnesqa.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2mnvizvfy.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2booszmhx.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2pozuxqoi.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2nbzcossz.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2vartdxbn.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt2uegjrtgr.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2kofofbqt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2genpatrq.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2dwmonrcv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2cbqqxpcj.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2bmjwyqdu.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2okedphbs.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2fxmnslyk.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tivcmxrs.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2taglbzzv.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2nkntvpom.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2dnmyumnc.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2fpkkpibu.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2lvcqcsou.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2plqwjevy.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2fgxypvkk.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2mlvsankx.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2onxienmx.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2forlfsnf.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2vubmsvlj.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cwxofoby.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt2rfurfohw.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2mpqrcysi.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2gfzbbvpg.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2xtfnllek.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2fadpjpnh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2dvkqzfio.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2pnlhihcc.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2fjfwwugp.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2grtwdwgz.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt2qnqcubvk.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2bntjqqsr.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2pfdwawpr.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2fmoijjyu.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2roxaolwx.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rdrogbms.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2lzuzsxyy.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2hllxprcs.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2dzprtygd.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt2yqosrgou.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2lfnkamqh.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2dcdgacac.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2ibrtftpr.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2gyjgvkpl.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2zhkilmko.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rufcompc.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2whxzcyip.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2cfwjbkmo.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2labzlxzz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2hcgxydpg.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2njblvzqn.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2zscebgug.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cyzwajuh.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2vafkdkjf.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2xniltdts.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2fchpavua.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2vyvxqmug.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2jiwsdvua.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2woyfpdel.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2qagmbvjb.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ciqsteik.html

[U45] PHP：类型声明与返回类型
来源：http://www.ydjk.org.cn/Article/details/gt2uhhxcgpr.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zyzdtyen.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2vyfqvyqy.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2rowinlfs.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2wxqgksvt.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2bmhualre.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2whrxxdth.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt2xserxsvq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2dxezuxka.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2cmeznulz.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2xgvvxsjv.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2jytckdlx.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2amsazdit.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2gsverrlo.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2tqaaxvjv.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2fmnoazgw.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2syjbagay.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2jrozsjdh.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2dvmhlfia.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2mjnhotbq.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2asxoujhw.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kjjjlveo.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2fvbneaer.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ihgjdptd.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2litrjxto.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2tibpcwxd.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt2fbeplcdc.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2lxilxxdu.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2pqczjeqw.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mpkvozyc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2koarfadx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2loxbemsm.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2jifjcswg.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2majqpbzn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2dwdeinmg.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2ndkbcoif.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2dwdmbbyk.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2dgsmzqyc.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qdsuikft.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt2aeozfghi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2cjpnwjqs.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hatwrtij.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2wumltnpj.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2seibkrfr.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2aygobnat.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2jtsjgend.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2ccyhwjwu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2dyrjadmj.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ixepbgla.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2jgpndrdu.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2lvmkioqv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2tqtpuiic.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2eljgsfye.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2hqmjvfqa.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2atjrzrvk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2nwghmqou.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2pvdynmdp.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2hnuvustc.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pickuidz.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2xyngqjew.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2osocydtf.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2jocrqtzy.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt2kezxaroo.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2hzpsjcgy.html

[U77] PHP：模板渲染
来源：http://www.52xcode.cn/Article/details/gt2nntjjvyc.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt2zkuzhnqc.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2oaxwjjqw.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt2nrqhmpgx.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2emekjtjo.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt2ssfpwxns.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2fdgocvln.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ozljpeye.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2zcyidqvr.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2bdlxoldh.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2jlpmnhof.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2ojycbved.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2drfbhboe.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2uhyjfgkn.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2sapsicib.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2yjxppbrp.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2rkfnrfux.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2bicaxtgo.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2lxcglfsd.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2ogrsymnu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2eegisilz.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ffywamog.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2htohqsvl.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2byihaate.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2fjtwrmrx.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yrtlzwjw.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2wrvouhqg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2eyeuiqbz.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fmoldnzl.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2crmepqoy.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2wkdidafk.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mpzftzeh.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2juajtrdo.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2agkolzqn.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2kpdtajmm.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2lgspkxae.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt2harobcig.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2vlbndeha.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt2pychclkz.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kvvyjhex.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2oellkypm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tghhlikp.html

[U98] JS：fetch 带 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hkdrnusl.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2kvvvarvv.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2xmouobgs.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2duvbxaha.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2buqqijbi.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2gdnkhgrq.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2ohaofyav.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt2uopuqghm.html

[U102] JS：本地存储
来源：http://www.52xcode.cn/Article/details/gt2jcywikop.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2isfjwttf.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2vscqoihy.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2irsxnkcg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2pkuvtmhs.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2dxwatjwy.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2olkzycwm.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt2fotwsxpn.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lwanwnyq.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2ejgxcexx.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ocymbxhh.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2asemiidl.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2civghzjy.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2lbldwzdj.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2nezogoro.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2sduaxuxz.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2fxzmksga.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2dnmrhxif.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt2xlblnoir.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt2ppgmipgv.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt2epwezrwz.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pmhsvqdy.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2cysufpry.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gdcppevj.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2kbmzdrqu.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2eujypmwt.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2eizqfrpy.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mdapuody.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2gkfnkpwb.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2fkvtylwz.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2iqchjbxp.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2rwxepkqt.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2qxyckzxb.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2rcrmsqgw.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2bxicjpvb.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2gglphxpw.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt2xyfdqcyz.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2bwxidppg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtplkjiu.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt2tzvlhykf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpersglp.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2cxfcprrq.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt2nqziucbg.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt2qwcnedin.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2umhktqlc.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2lkzbnwzc.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qkkjfvbc.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt2djzkxhlm.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2qyrruxeq.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2qrexfxzq.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2kweuqgwe.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2pnojeunn.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2kgytziil.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2xzklluvu.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qoyvwgfx.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2zuhtinnw.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2urcvkzbm.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2czkgtxer.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2sfawdjjw.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2eysduibq.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2iwyctgsj.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2ssmqyoxn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2pcfbhhgj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2hryvxcop.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2niorwdlg.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2lvmungwe.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt2knoycjzl.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2brchuyke.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2yktvupes.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2ddkkpuaw.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fpcnjduu.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2tipsqphz.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qnzuaenn.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2kouolzhe.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ixedoyas.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2aofxutgs.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt2titatzla.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2qzuqfmbp.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2fxycmpru.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt2avhjyswm.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2krllqfgf.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt2ndhguqla.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt2yhvjabqg.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2dtcjpudj.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2yoaazilx.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2gfsipevm.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2rgjwdopq.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2ngeojvur.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2pzkijnno.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt2rhzznifr.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt2jjykmpus.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2nbixpczq.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt2cyvnegbj.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt2rzracjjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubhjknzr.html

程序语言常见例子速查手册（2024 版）
来源：http://www.ydjk.org.cn/Article/details/gt2clgorurr.html

Common Programming Examples Cheat Book
来源：http://www.ydjk.org.cn/Article/details/gt2ckejigpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncxilhsf.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt2hckehcpz.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt2veeyondr.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt2ofcoibfr.html

SQL · Bash · C · C++
来源：http://www.52xcode.cn/Article/details/gt2pyzstyfm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.52xcode.cn/Article/details/gt2bokbqtpc.html

【使用说明】
来源：http://www.52xcode.cn/Article/details/gt2fadpbxzn.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt2abywgarl.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt2rsujxtui.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.52xcode.cn/Article/details/gt2mapwvcqo.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt2cfjjispm.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.52xcode.cn/Article/details/gt2egvdriuh.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.ydjk.org.cn/Article/details/gt2irmjyciq.html

需要完整可运行文件时，请自行补齐当前语言的导入语句。
来源：http://www.52xcode.cn/Article/details/gt2yjwzwpjp.html

3. 语法基准：Python 3.10+ / PHP 8.1+ / ES2020+ / TypeScript 5 / Java 17 /
来源：http://www.ydjk.org.cn/Article/details/gt2jzapnfwj.html

Go 1.21+ / Ruby 3.x / C# 10+ / C17 / C++17。
来源：http://www.ydjk.org.cn/Article/details/gt2yumpjalg.html

4. 检索建议：用编辑器或浏览器 Ctrl+F 搜关键词，如 "排序" "读取文件" "正则"。
来源：http://www.ydjk.org.cn/Article/details/gt2uzeplini.html


<!-- 参考信息 -->