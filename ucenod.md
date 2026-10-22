代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2yaxtxawz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttnzjnck.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2dpewzwtl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oklslvvx.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2kxbgctbb.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2qqmxrayt.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xxqnybhy.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2qkqqnvrr.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2wlqmuqqr.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2kgyulhos.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2ixbycnzk.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2oqwcjyyc.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt2vunloehw.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2rmrdaiuu.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt2jcuuaqsd.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt2lmstsjnl.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2uawqkgvl.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2wwcjjzfn.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2kwqycmff.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2umhhlosh.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2bdbdyuvr.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2wlsyammc.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2isesbobj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2wdhzcihu.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ibtordpi.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rrxjelic.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt2srjtdpyd.html

Counter(arr).most_common(3)
来源：http://www.52xcode.cn/Article/details/gt2txgircso.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2lriconlv.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt2vvbpenww.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt2pinfranj.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dzarpkgg.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2svpeknnt.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2usztalbs.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2gfgrbhjv.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2chnmvhxf.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2efxtjmep.html

logging.basicConfig(level=logging.INFO)
来源：http://www.ydjk.org.cn/Article/details/gt2vlswunlm.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2xsokntnr.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2evttcquk.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2tytfdtuy.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt2vsmfpjgj.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2xuzrpavk.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2gihcgnvk.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2xcfjzmbo.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt2diujprsz.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2gvqowuxn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2djqopkxw.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2peywxxuk.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2lhkbgpke.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2udgjhgvp.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2idaxaznk.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ragtyfee.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2fwkyxebn.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2wsphkdlx.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2jbcximpp.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2agdvzrle.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2kukejmto.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2ufqvzdbb.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2izkjwryc.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt2nkfiubfh.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2pysyiqfz.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt2ddhleiyx.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt2htrwxbwu.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2avulnfyq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt2zoyxutyc.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2laimcedq.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2xbxiqeyn.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2stvjpter.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2emhuwcvs.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2beunlxfm.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2bnexrasp.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2pjalrkgj.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2roaywmef.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt2crnxtszj.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2golsseot.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2rfotustg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2gduwcjsp.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2nwdvbfab.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt2svdrzmey.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2nsgcxdhb.html

sys.stdout.isatty()
来源：http://www.52xcode.cn/Article/details/gt2rhxbbhgb.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2lkfurjnz.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bzvyfinu.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt2jqohnupo.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt2ppacraqu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt2khziqxye.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt2hpfasdlb.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2xzazbxnh.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2gwwcnfey.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2efvaiqng.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2ndcwpgvt.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2lbehvweq.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sulxagrx.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2mvqfapbe.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2ychdaije.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2kmdavdxq.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2fankyqaz.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ebphwvgl.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnseggqj.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2jhdqgjde.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2kvkflrwg.html

[U50] PHP：构造器属性提升
来源：http://www.ydjk.org.cn/Article/details/gt2vrsdjgnp.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qsduuncl.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2fonsufvx.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2navutoon.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2ncjxlklx.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zwtxlkwf.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2hxwsjkgf.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2mewozrtr.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt2ochhtfwb.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2iyvgpuio.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2dwusjhux.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2muredbim.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2rgqschvs.html

f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ssxohcob.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2yxrrdkcb.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt2siypnaan.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2lzltojbl.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2dnjyqwtv.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2gnywrduc.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2eocqoknc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2lctfiuje.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.52xcode.cn/Article/details/gt2qdnqwrst.html

[U61] PHP：正则
来源：http://www.52xcode.cn/Article/details/gt2wndxwmwz.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hibydlql.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2avsoznoi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2bqtegogw.html

[U63] PHP：文件读写
来源：http://www.52xcode.cn/Article/details/gt2wcbqudrm.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2edzhijbm.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt2ylaunzop.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2jsjfxfyk.html

[U65] PHP：会话
来源：http://www.52xcode.cn/Article/details/gt2uhsjpmpm.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lotkbhkg.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt2dsnqcgjf.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qkcnglxw.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2jpzyhrnq.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2oogfzmgq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt2lkxtiqfm.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.52xcode.cn/Article/details/gt2umkfqqxy.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2mbgtrfya.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2dmfeffbd.html

[U70] PHP：PDO 事务
来源：http://www.52xcode.cn/Article/details/gt2fzdlnkai.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt2ndjzmqnc.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2sraskuhq.html

throw new RuntimeException("失败", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2pfcaeqkp.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2frfmuzgk.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2ucvcjtvf.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2snvarwan.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt2vceqlwvh.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yjqxxjcb.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2wgvmcxfq.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2tzhlpcfj.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt2cbyoxjkm.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2psvhyeic.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2ayuicrgn.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2pinremid.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2ncsjodpo.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2ctrzjaho.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2judgujfu.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2tmcpfdtq.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2akfmisfr.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2gsqzzofq.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2qooalkij.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2elcwmbip.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2lqoksrxo.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2xqhzmjeq.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2nspsjbby.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt2xisyxvms.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hywxaagi.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2oygkhapu.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2rqvyxxwc.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2tqzvmknj.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2vnwiokuw.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt2entdfhsa.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2trkkwmow.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt2eswkqxgf.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2rhgyavkn.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt2xutgavrc.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2bdwzsdcs.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2vhpiqybq.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dypxlwhl.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2mordkgma.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wfetdjxv.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2gdwurruu.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2slbunzwz.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2blzkzjkw.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2krefqeyc.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2mtnecdoy.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2qykqybae.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2dyfxfyxs.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2kovkduft.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2bwezsdso.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2cgfiphki.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2dgqyjawl.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxraoidh.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2jzmctmgg.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vcmicoew.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2pgobnczm.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2mxbvvmjt.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2aioifjml.html

el.addEventListener("click", e => {})
来源：http://www.ydjk.org.cn/Article/details/gt2fjlvusww.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2muycqaaz.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2qkkimtih.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt2bcllngaq.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2xpqgcnrs.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2invvgkju.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.52xcode.cn/Article/details/gt2oypgazvt.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt2muugarbw.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2njuknimg.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2lybwtkhn.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2fixzfqqi.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2cgsavjzs.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ujqvtybw.html

[U106] JS：日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2goslywjw.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2bgnqardt.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rrrmmteq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2icgsoakn.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2iweuzwkh.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.52xcode.cn/Article/details/gt2krwuezzs.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2gremjclu.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cszwgixk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2uystxauh.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2gtjzkemf.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fxyxfszt.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2dsshbdlq.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2obrombvq.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nfdioczs.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2axwnpgbw.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2clwsfdqs.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2vlluiuph.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wvornvxp.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2qwvcqbrd.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2dqcsldge.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2zhihdrkc.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt2xpxhxppv.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2phhvjydg.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt2mgyqdcxz.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2avuthwny.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2uomnfjjz.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2jdtesuut.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2jiefywye.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2znwrxjbs.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2xbqlkyqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plgnfiqg.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2qqahzdjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eiunabkc.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2mzspeedr.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2rhfutxwh.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2fajjvinf.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2bwiabbpg.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2mpsuzkir.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2ufysltis.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2otagjoez.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2mnwwgqyi.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2zogjrtyy.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt2kwnptsle.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2tmochggk.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2zjzerese.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt2fsbxhuon.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2ggxpboit.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2livotvyl.html

Lua ............ 10
来源：http://www.ydjk.org.cn/Article/details/gt2ennbswjg.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt2jcmaqyyi.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ktixbwdc.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2tvjusado.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2pfcxnuhf.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2bvvkuwvf.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2adpbflrx.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2gbtkrmrr.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2sqfiimel.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2zogqilbh.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2dkfaqbqu.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lksmeiks.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2isgdvdhw.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2vlvxmlgj.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2lheswrrq.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2rlunffbw.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nsdtaywo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2hvnmnany.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2nddoedve.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2zwumunew.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.52xcode.cn/Article/details/gt2ogjwmujm.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2yjfpbhzv.html

Q SQL 专题                              90
来源：http://www.ydjk.org.cn/Article/details/gt2iizuihki.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt2bgpcdait.html

S C / C++ 专题                          60
来源：http://www.52xcode.cn/Article/details/gt2sofwbcfd.html

T 其他语言补充                          60
来源：http://www.ydjk.org.cn/Article/details/gt2pojiqiky.html

U 高频实用片段                         120
来源：http://www.ydjk.org.cn/Article/details/gt2kxwkuyhy.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2sblmhnla.html

合计                                  2106 条
来源：http://www.52xcode.cn/Article/details/gt2adxhvsvs.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt2xastpjca.html

使用提醒
来源：http://www.ydjk.org.cn/Article/details/gt2iclbmcbt.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2xwhvnklv.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt2xkglpjpv.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.ydjk.org.cn/Article/details/gt2aocxvvws.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.ydjk.org.cn/Article/details/gt2xlhkugmp.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt2vxuphbjx.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.52xcode.cn/Article/details/gt2tcamatdg.html

—— 文件结束 ——
来源：http://www.ydjk.org.cn/Article/details/gt2ncecxxjj.html


<!-- 参考信息 -->