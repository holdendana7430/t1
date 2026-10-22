代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2ukevpsvq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tszalpyf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hjgikdms.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2jowmxddq.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2yijbkfma.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2lwuzigtf.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sziyrxaz.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zcjevvmm.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nvozaoyc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2elbbfmiv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2rsodzrtv.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2gjnmwelh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2sdnmkovm.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2emaepxlt.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fwrxlytc.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2ujetaokt.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2cgwvmzzv.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2xmqwqsrv.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tnwgrnmx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2afhkwgea.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2tpmnpknb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnignrbu.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2mohznqsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjrfufud.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2jfdvwdso.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt2anritllj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2gqaalgqq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.52xcode.cn/Article/details/gt2mamuzhqc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt2yzlgzacq.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2zjstcsrl.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2wczuruat.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2liemcrmj.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2fllosrbt.html

list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sfbxkidz.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2pviuucrf.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2zchozivh.html

[U07] Py：反转字典键值
来源：http://www.ydjk.org.cn/Article/details/gt2pakzlmjg.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt2fovwlvpp.html

[U08] Py：展平二维列表
来源：http://www.ydjk.org.cn/Article/details/gt2aahhkubr.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2mziwbver.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2xbaxmcwg.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2thzazsgh.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2inpvihvq.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt2pfwzczzg.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2fktbrtkm.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt2sybpjnyp.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rbcojcxq.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gavcjkba.html

[U13] Py：固定长度队列
来源：http://www.ydjk.org.cn/Article/details/gt2eqmtsifk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2tazoolla.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2hlyrmsov.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2upojtjqy.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt2qatxtoxo.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt2zamktjge.html

[U16] Py：命令行参数解析
来源：http://www.52xcode.cn/Article/details/gt2edbupygm.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.ydjk.org.cn/Article/details/gt2ltkarhup.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt2karunqdz.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2hnezapoj.html

[U18] Py：预编译正则
来源：http://www.ydjk.org.cn/Article/details/gt2ewcnvior.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zpmhottm.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt2vqvmemxs.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2ujbyowvo.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt2mbynapqe.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2nrdnfahy.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt2jfyejpyt.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2ljwuswnm.html

[U22] Py：矩阵转置
来源：http://www.52xcode.cn/Article/details/gt2ffcmpaff.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2qbvzqgka.html

[U23] Py：分块读取大文件
来源：http://www.52xcode.cn/Article/details/gt2hjevkpjb.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.52xcode.cn/Article/details/gt2cpnetzio.html

[U24] Py：路径操作
来源：http://www.52xcode.cn/Article/details/gt2zzbwvgvd.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dtzkjsun.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2oqfceufn.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt2yixodubh.html

[U26] Py：并发下载
来源：http://www.52xcode.cn/Article/details/gt2jmmogpsu.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2hjcukuty.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt2nuheqcwg.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt2prhqsixh.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt2crzholnn.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2mmodzcei.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2kzyeount.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2rszlytyh.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2yqqphmvu.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2wvnhtqlw.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2hmejjhja.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2uubmgzbq.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2csnsxmng.html

ruff format . && ruff check --fix .
来源：http://www.52xcode.cn/Article/details/gt2jkvkiepc.html

[U33] Py：打包发布
来源：http://www.ydjk.org.cn/Article/details/gt2kdpifbhu.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2fbhrvisi.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2wqebbtau.html

chardet.detect(raw)
来源：http://www.ydjk.org.cn/Article/details/gt2xrjejzzu.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2wxexgatw.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.ydjk.org.cn/Article/details/gt2xmtugblb.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qxrvsibu.html

schedule.every(10).minutes.do(job)
来源：http://www.52xcode.cn/Article/details/gt2dmqucnjj.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt2mswpzwlt.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt2klmicmpe.html

[U38] Py：获取脚本所在目录
来源：http://www.ydjk.org.cn/Article/details/gt2hfgvwhjp.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2nqivfunh.html

[U39] Py：判断是否在交互环境
来源：http://www.ydjk.org.cn/Article/details/gt2fnsaghnq.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2liidnkty.html

[U40] Py：打印到标准错误
来源：http://www.ydjk.org.cn/Article/details/gt2ozwyhrai.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jpqdonul.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2ayiehptp.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2lgndxymu.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2gyjznwaa.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2vtjbhlra.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt2aqridiqp.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2wxowykrh.html

[U44] PHP：开启严格类型
来源：http://www.52xcode.cn/Article/details/gt2rcqlxipq.html

declare(strict_types=1);
来源：http://www.ydjk.org.cn/Article/details/gt2bpkfbopj.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2jauuqqfl.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2abspzstv.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt2facvaypg.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt2xbnbhjcd.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt2rwqomned.html

int|string $id
来源：http://www.52xcode.cn/Article/details/gt2cksezaoj.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ojilwvaq.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvoguesk.html

[U49] PHP：只读属性
来源：http://www.ydjk.org.cn/Article/details/gt2xceifigx.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt2oewthhlq.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2iguybdyw.html

public function __construct(private int $id) {}
来源：http://www.52xcode.cn/Article/details/gt2mwlskhff.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2zkmswvun.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt2fluvyjbd.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2mynctdze.html

$double = fn($x) => $x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2uvcmrnwl.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2fezosilq.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt2gwatzqzl.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2xkijmswy.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt2twxukdqj.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ywjcgesc.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2aawsfidh.html

[U56] PHP：命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2veflgycc.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dbtxyiya.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2obvoqndb.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2loujvrsc.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2ajylglgs.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2qfoqotms.html

[U59] PHP：自定义排序
来源：http://www.ydjk.org.cn/Article/details/gt2rufedppj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2yygvzyzc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2mgvummkm.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uuhwquvv.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2gzysozlh.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2vheznndm.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt2tdmkobzi.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.ydjk.org.cn/Article/details/gt2rzakclec.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2fpwngefn.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2iwsjipnm.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fjjxodyv.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2orgekkog.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2denflamn.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2esdmfujb.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2qlnqpdsi.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2nfmfcqwi.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2bowmiuzt.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt2fbsrvdiz.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2ucbwuctt.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2ifdpmcwr.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt2fpjfidgu.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt2omscbgzt.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2iljfwpbn.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2ledtokdv.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ltwqzvsz.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2djfpulmp.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt2mzwbhmlf.html

error_log("失败: " . $e->getMessage());
来源：http://www.ydjk.org.cn/Article/details/gt2cghdmpib.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2gsxbfjdl.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2bnhqxnnx.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dfsycftk.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt2ryssdfvj.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt2xsiynlcq.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2vpadepgf.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2xgoozmgb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt2ytwxutka.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2bzzmqbfq.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2bjhimezf.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2eefkwfrh.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2tdhmkutf.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt2omxwuugw.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2bnxaexfg.html

[U80] PHP：代码规范修复
来源：http://www.ydjk.org.cn/Article/details/gt2ielxpkgg.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2zgvwlzks.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2eodimpdp.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt2efsmjsaa.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt2zriprpuk.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.ydjk.org.cn/Article/details/gt2ocidyilz.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2cqwfmzws.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kospggsg.html

[U84] JS：CommonJS 写法
来源：http://www.52xcode.cn/Article/details/gt2nhhflbqi.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.52xcode.cn/Article/details/gt2aiyksyhn.html

[U85] JS：可选链
来源：http://www.52xcode.cn/Article/details/gt2jzwkzvcc.html

a?.b?.c
来源：http://www.52xcode.cn/Article/details/gt2ouskfcrz.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2njlcmyux.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt2wqoqynmv.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2oosomgms.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt2szeoxlkp.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2xsifjgvf.html

{ ...a, ...b }
来源：http://www.ydjk.org.cn/Article/details/gt2rgngicsk.html

[U89] JS：数组去重
来源：http://www.ydjk.org.cn/Article/details/gt2uwejhnse.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gonyivzt.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt2filovclm.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bdgjepbp.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt2ixvafubv.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.ydjk.org.cn/Article/details/gt2ruvrungp.html

[U92] JS：深拷贝
来源：http://www.52xcode.cn/Article/details/gt2cdzxoovo.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gjlbiemi.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2cngsqxvk.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2itihloha.html

[U94] JS：箭头函数
来源：http://www.52xcode.cn/Article/details/gt2xcrzzmnh.html

const double = x => x * 2;
来源：http://www.ydjk.org.cn/Article/details/gt2zzcxwqnh.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2xmsgzhlm.html

new Promise((resolve, reject) => {})
来源：http://www.52xcode.cn/Article/details/gt2xbhhdbwl.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2hpuiijyg.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gxokpsom.html

[U97] JS：并发请求
来源：http://www.52xcode.cn/Article/details/gt2lqymreij.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dztxiobq.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ggpsqvrk.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2fyvccbhw.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2xkkdnfhz.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2irqybdiv.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt2mtsxzhqn.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt2jyehtuoc.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2mfcspzmv.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2tscirfer.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2ienztkcy.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2hktwetfr.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2tjifpjkh.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2irgwcmdr.html

[U104] JS：防抖
来源：http://www.ydjk.org.cn/Article/details/gt2azuwlyov.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2gllgeokr.html

[U105] JS：节流
来源：http://www.ydjk.org.cn/Article/details/gt2lsbhfhgu.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2htdqkfpx.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2vptzxjwb.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.52xcode.cn/Article/details/gt2aehrzajr.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gnjuupth.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zdxpalsw.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt2spyfrxtq.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2jvuasotf.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt2uqytjuyx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rgrdzaku.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2yecqudom.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2pjbyxtsq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2fqejxhft.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ulojesxw.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2sepbbuay.html

"7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uugbtggj.html

[U113] JS：正则替换全部
来源：http://www.ydjk.org.cn/Article/details/gt2neunmaqd.html

s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gxgpjlhw.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2cyxvgbxk.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uosdzzxh.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xmdxzckv.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bvaxhwbm.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt2usxutxuc.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvkupvan.html

[U117] JS：单元测试
来源：http://www.52xcode.cn/Article/details/gt2ovjmoeeq.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2kbfiwoth.html

[U118] JS：开发服务器
来源：http://www.ydjk.org.cn/Article/details/gt2mnvlaiqr.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2ovsakywf.html

[U119] JS：生产构建
来源：http://www.ydjk.org.cn/Article/details/gt2ohdkgjdk.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt2rfzertjc.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2xbulfgfj.html

import.meta.env.VITE_API_URL
来源：http://www.52xcode.cn/Article/details/gt2yiyuycyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzlglfvh.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2qwrpqgxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkoeclax.html

按语言统计（条）：
来源：http://www.52xcode.cn/Article/details/gt2bffqsziu.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2atfvacco.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2axrpmuyh.html

JavaScript ..... 252
来源：http://www.ydjk.org.cn/Article/details/gt2bnsduhej.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2gktebkzr.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2tcloptds.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2brxzbtlb.html

Ruby ........... 212
来源：http://www.52xcode.cn/Article/details/gt2lrotheqo.html

C# ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2wprmupey.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2rzneaflf.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2skzojmfs.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2tbezbhdu.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2phtgrvik.html

Kotlin ......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2jazehbcs.html

Swift .......... 15
来源：http://www.52xcode.cn/Article/details/gt2vgjvjodr.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2dvmroqmn.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2zrmeqgao.html

Scala .......... 10
来源：http://www.ydjk.org.cn/Article/details/gt2ocxiljvq.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2hcittjbj.html

合计 ........... 2106 条
来源：http://www.ydjk.org.cn/Article/details/gt2rqistkaq.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2nxwglolg.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2wgjijdft.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2ckklexkn.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2vkjlbxey.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2exqipbvb.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2yxhaufzi.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt2elqxrrop.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2rjgynzto.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2zjkdkgnc.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2aghvlnuy.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt2gmlgbhdt.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.ydjk.org.cn/Article/details/gt2zlgyresq.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2ukcliani.html


<!-- 参考信息 -->