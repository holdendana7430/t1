代发 wailian999

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3poqsfhei.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3rigxxfzj.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3bfrdwoqb.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ultdgbqu.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3ffvkprwe.html

max(d, key=d.get)
来源：http://www.ydjk.org.cn/Article/details/gt3rcqetdbv.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3qsavqklt.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3fadagrad.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3dqjrjvbc.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3urzkfwzq.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3yhmlnijn.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lrnzhwwd.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt3vpxsroed.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3whasyhlt.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3dekioern.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ygpjyepe.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt3lfuydtbc.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3kixqlntd.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3uawjpldd.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3fbgtvbsr.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3xloqamif.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt3qrqgdksp.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3fmbeuers.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wywanhla.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3mhootsbq.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3vffyfpqm.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3dnkeplil.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3wvnhugpm.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt3obrxnrxw.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt3hnkstitv.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3cbrxdztu.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3azntjlbe.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3ltnvtivj.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3pvpzrmvi.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt3zwfmpdjp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3sydxuggx.html

[U25] Py：CSV 按字典读
来源：http://www.52xcode.cn/Article/details/gt3otnwwbil.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt3hypqjjzd.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3htcfxuge.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3ixmrkyxq.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3zgzobxdq.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3wijvxrug.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3iktnjlon.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3yacnlwud.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3quzpzrfj.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt3pisguskh.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3mluzsexu.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tyudxwgw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt3uumoygxn.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3rkxkpamd.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3lvhvohtn.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt3hmfhripw.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3nwkodywi.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt3btrxrbls.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3csbuecri.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3bacyiwqz.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3bcsampii.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3xyxmanjp.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3abhewfif.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3erkdeidr.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt3tipignzf.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3zpzalogy.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt3lsuqnrks.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt3pvtxwmfj.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3qjijlvxq.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt3esmhpolj.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3zuztsmtt.html

print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jsqhjsvf.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3guomdyin.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3cmfzsdvp.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3dykjgeif.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3hfngdghy.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3jwsirmvt.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3csoxfnod.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3voelwocm.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3cqpqhcuf.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3guygkxkv.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hypildrw.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3ytywtpad.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3xtimxtib.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3oletowxe.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3fjffmadi.html

[U48] PHP：纯枚举
来源：http://www.52xcode.cn/Article/details/gt3ueaylqzq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3swjjkxmh.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3btgswqgh.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3yyqkctoe.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt3tdwnekig.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwkqmvfr.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt3hrfcprhl.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3cuymngyp.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3cmhrmjzl.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt3kqewcjav.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3ukxqbkhr.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt3rgypukdw.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3eddyzmjo.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3wupaccgl.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3ndsycdtg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3tmahzdgw.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3vkspxbpl.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hdiuttwz.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3pvvkpadz.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt3zyhghxun.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3mxudluoe.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt3awtgxqja.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt3affixmmx.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pkxeuntn.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3aahmdmsf.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt3wftbfbbn.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt3zzemwdic.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cchdujwn.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3iudxwpde.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3gntkkenu.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt3lrkejwea.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3vogvucsq.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3oijzdkzi.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3njwcxadi.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt3kjeppkqg.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hghrxydl.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3kgnhxjus.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt3uxehhvhe.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3sbesigzr.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3bexxeeoj.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3dnjzuuzu.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt3fmhkxlyv.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt3ushadxts.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3epkwhtzk.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt3hmdpxiif.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3pozsxiua.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qvyzntma.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3zgmtawfi.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3sspjvcud.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ggdkfjww.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3guhaqphu.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3yobbpcat.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ldacqkby.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3tlizleno.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3kifluyje.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3zsztzabo.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3kdgmmpjf.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3iqqjtzgi.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3crrohqgv.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3rjmywhat.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ovywyxai.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3qsdqnejk.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3qykmrrse.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3svscuoow.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt3dobicvzj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3kbxdalho.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3lseishxk.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ydtrgfvq.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3pxfqiadl.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt3tixfymwf.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3smcpvzih.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tbssjntx.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3babzehkt.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3xogtccmu.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3fqqobnbd.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3zwthqjdr.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ewmmeqpt.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt3uduoxxny.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mvctarkv.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3dasqmetn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3crhinkrn.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3taqynuda.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3qcftlvle.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3eknlcemp.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3qhkgiskj.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3etpmhxyi.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gvuudxjo.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3rufjkqdw.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tzlgsidg.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qyikthgp.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3drbbvkqp.html

`共 ${n} 条`
来源：http://www.52xcode.cn/Article/details/gt3uudtxgsq.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3cmbbpmbz.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3zzhvulum.html

[U95] JS：Promise 包装
来源：http://www.ydjk.org.cn/Article/details/gt3syntaxnp.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3syopfolf.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt3ejzwdnbj.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3djuyipfg.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt3anjjlgix.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pvcthdld.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3nqemlwbt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3zhxvxghe.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3fpddkkze.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt3tbgrunln.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt3xetsgnvx.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3kevdaqdl.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt3azbfropp.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3xngajwhr.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3snfvtduf.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3icwvrhcl.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3azyjtaxx.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3jeznzofl.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3rausdizq.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3fvufsnye.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3wuedmzho.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3svdmvbua.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vvdcmnwu.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3obwcrvjq.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fnzlhnnx.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kjcxytuv.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3nidlorww.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt3qqwarrwb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3ltdmtyzd.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tthyvmiq.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3dzgxdbtx.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3tteibmte.html

[U111] JS：对象转 Map
来源：http://www.52xcode.cn/Article/details/gt3twzstgdj.html

new Map(Object.entries(obj))
来源：http://www.52xcode.cn/Article/details/gt3ukewdkte.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3fsaxaigm.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3atqhsvlk.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3acnqnuva.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3icjbeqwp.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3zttyktfy.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fqwunksu.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3rrxcyrqo.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3sukyfsuu.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3tbevlfwh.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3onawqmtg.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3liubvjcn.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3tqrbjgcu.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3igmpgsda.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3rcogmerw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3lszkmdsm.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3iazhvdkn.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3mfykaxsi.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt3emohtcvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fedidnsq.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3ddnnrxxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kjuklskm.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt3feqvcowj.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt3xgbtdnqo.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3uqfhnpkv.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt3firniiqm.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3jxfzrekt.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3hnbhgblz.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3fzwyinta.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3lmmxzpxk.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3uoiijvlq.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3vgacelgc.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3scgseyse.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3dyxihacy.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3wwheynmp.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3fufcwzxq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3niqxvinz.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt3tnvolmry.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vwafmqsp.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt3vesollhq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ygpqmpyr.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3ldosumgn.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3oscnmxxn.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3bceeatoj.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3wemjzkpq.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3gzjbxhah.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3tllofrvm.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3yqjofzvd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3gzdptjrv.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3sxjnzzbv.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3zyzmoxje.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tnmyhfjz.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3fxwutibx.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3hmrgdxuo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3gzqrdlht.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3vhnndmmq.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3ohrgxzvj.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt3yofxaljh.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3xjvifhlq.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt3djnujimd.html

R Bash 专题                             80
来源：http://www.ydjk.org.cn/Article/details/gt3rivapikb.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt3rqgrbgsd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt3ussoyrhf.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt3nxfwihyg.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3tocoksiw.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt3fwckeonz.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3qdzzipqt.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3klgmlura.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3ycpfvygt.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.52xcode.cn/Article/details/gt3xqseqiwl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt3zryhprhd.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3cbxsrbeg.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.52xcode.cn/Article/details/gt3njqdxnjd.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3jjuxloau.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3rnncleyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3soiyyyuw.html

程序语言常见例子速查手册（2024 版）
来源：http://www.52xcode.cn/Article/details/gt3tgitsaox.html

Common Programming Examples Cheat Book
来源：http://www.52xcode.cn/Article/details/gt3cshignab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjkpzmwn.html

【收录内容】
来源：http://www.52xcode.cn/Article/details/gt3zzkmkaya.html

覆盖 12 种语言 / 语法与常见 API：
来源：http://www.52xcode.cn/Article/details/gt3eoxeimqq.html

Python · PHP · JavaScript · TypeScript · Java · Go · Ruby · C#
来源：http://www.ydjk.org.cn/Article/details/gt3kgkpfogc.html

SQL · Bash · C · C++
来源：http://www.ydjk.org.cn/Article/details/gt3yjjuyzxm.html

按「任务」分组：每个任务下按语言各给出一条最小可用示例。
来源：http://www.ydjk.org.cn/Article/details/gt3unwygvuq.html

【使用说明】
来源：http://www.ydjk.org.cn/Article/details/gt3nuzyaijz.html

1. 每个任务形如 "[编号] 任务名"，下面每行以语言标记开头：
来源：http://www.52xcode.cn/Article/details/gt3uvxfffqn.html

Py:    Python        PHP:   PHP           JS:    JavaScript
来源：http://www.ydjk.org.cn/Article/details/gt3nmlnqmzs.html

TS:    TypeScript    Java:  Java          Go:    Go
来源：http://www.ydjk.org.cn/Article/details/gt3nqkvfexy.html

Ruby:  Ruby          C#:    C#            SQL:   SQL
来源：http://www.ydjk.org.cn/Article/details/gt3yofbicza.html

Bash:  Shell         C:     C             C++:   C++
来源：http://www.ydjk.org.cn/Article/details/gt3lpxhzdkz.html

2. 示例只展示核心写法，刻意省略 import / require / include / using 等样板代码。
来源：http://www.52xcode.cn/Article/details/gt3qkjkpryi.html


<!-- 参考信息 -->