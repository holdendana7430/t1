代发 wailian999

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3vymtyjpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhhqipcz.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3kaansnxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eucoyige.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3vvgabfkj.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3meiesjvn.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3xrstlver.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt3nxatguur.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3dvmeabnv.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt3kfwstqqq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt3uwixhkpp.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt3qtbvrlbc.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt3ulismaio.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kfbgmdes.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3bxpksbfk.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3iktezgbb.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt3mdybwvep.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt3tzzsnmys.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt3poirfqhw.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3ewkdxofo.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3novntmcn.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3eujzvgii.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3nffrosjj.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt3nmvnmfvp.html

[U11] Py：生成器表达式
来源：http://www.52xcode.cn/Article/details/gt3ufmtgtsw.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yneaicde.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3cgigorqf.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eshuigma.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3cqxnvbpy.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt3hkofgxon.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt3zqheubyv.html

defaultdict(list)
来源：http://www.52xcode.cn/Article/details/gt3wihixcyp.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3stdltyjg.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt3wlryzioz.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt3skhqcbmb.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3cafofqbs.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt3klosfmvy.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3sjbwwmmz.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3ncwqzxbn.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xqjdtagf.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt3dwcdadwk.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.ydjk.org.cn/Article/details/gt3ozfbndvk.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt3conclvjp.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt3dmowohtb.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3gnspvvmz.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3kukqiwej.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt3jhuddpdj.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3wcnhbjrp.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt3xlaptskn.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt3owhpcskb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3nvbpushl.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jyphyqjv.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3ztzfbofb.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3iotosyeh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt3jqreygdt.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt3hzyyrlvu.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt3fncyylyr.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt3tfjwcdjy.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt3hippicyo.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt3flngbqks.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt3usgduolb.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3ghzvzyds.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3feccattm.html

@dataclass(slots=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zilinhoj.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3scueopeq.html

python -m pytest -q
来源：http://www.ydjk.org.cn/Article/details/gt3fcxdizes.html

[U32] Py：代码格式化
来源：http://www.52xcode.cn/Article/details/gt3thlpppgi.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3vcorvuiv.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt3gaawujiv.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3wfgfqfbl.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt3vfyberew.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt3rhfdckbt.html

[U35] Py：发送邮件
来源：http://www.52xcode.cn/Article/details/gt3pkdfvmhx.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3ebyligal.html

[U36] Py：定时任务
来源：http://www.52xcode.cn/Article/details/gt3ctdvmfgu.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3rbalxbbp.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3vdfuaoon.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt3wptuzrqv.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3wrzatgmx.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3esazcbyh.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt3rfjghqne.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3pouzsiiu.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt3sqipcbav.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qmmxahlg.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3aceizlek.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt3wcgwlgbc.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3syeyepre.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.52xcode.cn/Article/details/gt3gluozipw.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3fgvoisak.html

namespace App\Http;
来源：http://www.ydjk.org.cn/Article/details/gt3pfywrtge.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt3hydbvytj.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt3dgqikzru.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3rowarnih.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wujbvzor.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt3qvswqxfk.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt3mbqjigex.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3plgdjzol.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt3qagdhkoc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hxxxbqwm.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt3okiclnxi.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3mlnpkyhr.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt3nvruuysv.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3yvxqyvgs.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3meukmylh.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3rjxobzip.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt3hinqxyfq.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3bjrdrfah.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3mzviamdl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt3vdpuapen.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3eqejvlbo.html

[U54] PHP：空安全调用
来源：http://www.52xcode.cn/Article/details/gt3forhjuli.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3fkkblfnz.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt3zqmhreye.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3iymjicsm.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3wgefeohd.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vuacabkj.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3tpvlsbkj.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3qrnnicbk.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3kpwmffor.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lhzubpqo.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3xdnqoqql.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ypvbicvl.html

[U60] PHP：JSON 编解码
来源：http://www.52xcode.cn/Article/details/gt3ioxapfgg.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eabpcvlt.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3sljjhmvq.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kifsqmob.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3rzjyoylx.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt3aqblkvij.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3mnamnddx.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.52xcode.cn/Article/details/gt3rioplimj.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3fonefmap.html

glob("dir/*.php");  scandir("dir");
来源：http://www.52xcode.cn/Article/details/gt3kubiplrd.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3rpddldqz.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lsyndyri.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt3nswhdwjx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3otyiukus.html

[U67] PHP：处理文件上传
来源：http://www.ydjk.org.cn/Article/details/gt3zbzqhcmc.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt3jbsisibo.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt3cmokeklo.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3ozocbtqp.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3tzvthymv.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt3llbiabdx.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3znoqceqh.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt3kyxnssaq.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3flbweizz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3esiijmuh.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3rxbjzvne.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt3jpubsicl.html

[U73] PHP：读取 ini 配置
来源：http://www.ydjk.org.cn/Article/details/gt3dmpywajl.html

parse_ini_file("config.ini", true)
来源：http://www.ydjk.org.cn/Article/details/gt3onqlxnvx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cdgvxadc.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3gnigltlc.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt3csdltmve.html

composer require psr/container
来源：http://www.ydjk.org.cn/Article/details/gt3npnynuhy.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt3fcpkctme.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3nejwsfph.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3hrxgsbed.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3tybcvosb.html

[U78] PHP：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3edlrjqrh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt3gkihrwot.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt3bicsijgy.html

composer require --dev phpstan/phpstan
来源：http://www.52xcode.cn/Article/details/gt3vlkjfaqg.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3hkemufvr.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt3dszdglvb.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt3igoencpm.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt3ftuhluye.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt3bogxarsf.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3iytqixyh.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt3hbphcmbb.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nddmbgqm.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt3dhgnydsa.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt3zvstqevj.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3wklkglsv.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt3bhgbgsqm.html

[U86] JS：空值合并
来源：http://www.52xcode.cn/Article/details/gt3mprrvksi.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3izjgktms.html

[U87] JS：解构默认值
来源：http://www.ydjk.org.cn/Article/details/gt3reorxlik.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt3asulmktu.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3voxtkgpp.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt3utsxadwr.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt3nksmdsjc.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3eqgrygaf.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt3rwownibx.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pvbnotwf.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qsmswdfc.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt3unphouee.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt3wpkjpfwu.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jtjglowq.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt3obyhboxk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3vwhsxwts.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3vmfwbvel.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3rypvlnqw.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3fbehbbuz.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt3tntubgjs.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3ctblinjv.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tcicfqmk.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3alnstnqm.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hidoimnh.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3hukxdimx.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3unszyqxu.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt3opqueqmp.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3reuhhpwl.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3iziraapk.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt3soxwvykt.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3kuqakfdx.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3ocncxvfb.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3ycmvymeg.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3djayftih.html

[U103] JS：定时器
来源：http://www.ydjk.org.cn/Article/details/gt3jyckvjko.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.ydjk.org.cn/Article/details/gt3drldjdyz.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt3xchcziiu.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tqfxbxlx.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3nifzjqix.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.52xcode.cn/Article/details/gt3dgjdipsf.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bezhszch.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt3yzvnntdg.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mypsyupi.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kgaonrve.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt3swwemfbn.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3huiduypb.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3yqcdtwzr.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3qtrmiwsr.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt3gudltbyc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3jtlcizll.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3cpwagbxx.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ywbgfrmz.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt3ukdgyhex.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rbmjkxqw.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt3mttyjeod.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ctorvhwo.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt3zibioeiw.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xgghlklx.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3louvqsyf.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3wzdaqije.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt3bgihpgkp.html

/** @param {string} name */ function f(name) {}
来源：http://www.52xcode.cn/Article/details/gt3nivschyu.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt3aojfbxwx.html

npm i -D vitest;  npx vitest
来源：http://www.52xcode.cn/Article/details/gt3fgcwnmra.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt3izqpubnj.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt3qhgrpfzy.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt3kkwqshds.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3ofbdfude.html

[U120] JS：读取环境变量（Vite）
来源：http://www.ydjk.org.cn/Article/details/gt3sctckhqp.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3wmhafrmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tkfcsdqd.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt3gfdxbyxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrroosrb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3idbfemih.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3szgjmxvu.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt3zxqgcdcs.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3calbbiuw.html

TypeScript ..... 212
来源：http://www.ydjk.org.cn/Article/details/gt3sspgspsp.html

Java ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3xmcvxjrk.html

Go ............. 212
来源：http://www.52xcode.cn/Article/details/gt3slpjfzin.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt3nzrnhrny.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3wvzequmr.html

C .............. 30
来源：http://www.ydjk.org.cn/Article/details/gt3kcxggrou.html

C++ ............ 30
来源：http://www.ydjk.org.cn/Article/details/gt3rnexwsyr.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt3cbemyilr.html

Bash ........... 80
来源：http://www.ydjk.org.cn/Article/details/gt3rbxrccxb.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3fbkftgam.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt3hqszbuwc.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3hxoawwna.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3vexptorx.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3olebubox.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3ulowxbdt.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3aftuinfp.html

按章节统计：
来源：http://www.52xcode.cn/Article/details/gt3kycfxxyh.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3quejcpnz.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3zygqivfk.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3okzeekts.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3ebrdgjyx.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt3javsvwrd.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt3iniebimf.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3fwpyirma.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3czcyeaga.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3fcqykidr.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt3hacgufxe.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt3tshnmukh.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3tbstxhhx.html

M 命令行 / 进程         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3unvmojlc.html

N 数据结构与算法       12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3pjyemcqo.html

O 并发与异步            6 个任务 × 8 语言 =   48
来源：http://www.ydjk.org.cn/Article/details/gt3lzdzgrzq.html

P 常用工具函数          8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt3algbygrd.html

Q SQL 专题                              90
来源：http://www.52xcode.cn/Article/details/gt3omhrqygc.html

R Bash 专题                             80
来源：http://www.52xcode.cn/Article/details/gt3tmkyzylo.html

S C / C++ 专题                          60
来源：http://www.ydjk.org.cn/Article/details/gt3epgxwidl.html

T 其他语言补充                          60
来源：http://www.52xcode.cn/Article/details/gt3verwdrtt.html

U 高频实用片段                         120
来源：http://www.52xcode.cn/Article/details/gt3xfdekhmq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3rfptyrai.html

合计                                  2106 条
来源：http://www.ydjk.org.cn/Article/details/gt3lhysjzzk.html

--------------------------------------------------------------------------------
来源：http://www.52xcode.cn/Article/details/gt3gewwciik.html

使用提醒
来源：http://www.52xcode.cn/Article/details/gt3romsvlai.html

--------------------------------------------------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3jkodcnxy.html

1. 示例追求"最小可用"，正式项目中请补齐导入、错误处理与边界判断。
来源：http://www.ydjk.org.cn/Article/details/gt3qazckvkl.html

2. 涉及文件、网络、数据库的示例，注意资源释放与异常捕获。
来源：http://www.52xcode.cn/Article/details/gt3hbebrkrw.html

3. 语言版本差异较大（如 Python 3.10 的 match、Java 17 的 record/switch 箭头），
来源：http://www.52xcode.cn/Article/details/gt3mucdcptq.html

在旧版本上使用前请先确认语法支持情况。
来源：http://www.ydjk.org.cn/Article/details/gt3rqduzfwk.html

4. 标注"手写"的条目是因为该语言缺少对应内置能力，实际项目中可引入成熟库。
来源：http://www.ydjk.org.cn/Article/details/gt3ihrodhne.html

—— 文件结束 ——
来源：http://www.52xcode.cn/Article/details/gt3swetvxat.html


<!-- 参考信息 -->