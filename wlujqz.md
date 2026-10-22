代发 wailian999

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2gzobhaqb.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xsnbyrbv.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bfileggd.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2imctxghb.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2lpveonfk.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rdgwpccj.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2loljymxd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2kltdelyq.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sgitiooh.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2prmbzfog.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmjfktqp.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2hvlptgeq.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2odxttvtz.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hkknscig.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ndcdhdlv.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2dtucbebr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2owthzdju.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2wbrvzmin.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2xqrvreev.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2qphphvkg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ejjymrge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzsrborh.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2opizmtvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vpzgnrhw.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2jtdepsrl.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2igjzikqj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2jhtqqlpr.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dhrxntux.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2mvbmbnwj.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2kofpbgqq.html

[U04] Py：变量调试打印
来源：http://www.ydjk.org.cn/Article/details/gt2peazovjb.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt2vipduyja.html

[U05] Py：列表去重且保序
来源：http://www.ydjk.org.cn/Article/details/gt2qvpvhsrl.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qlskpela.html

[U06] Py：合并两个字典
来源：http://www.ydjk.org.cn/Article/details/gt2sxihnnzp.html

{**a, **b}
来源：http://www.52xcode.cn/Article/details/gt2gpcefrfq.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt2tiqmnvfc.html

{v: k for k, v in d.items()}
来源：http://www.52xcode.cn/Article/details/gt2nbxignct.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt2dqamdcey.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt2qwkratnj.html

[U09] Py：字典取最大值的键
来源：http://www.52xcode.cn/Article/details/gt2vvxncrtf.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt2citqqpzy.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt2cnoxnnhh.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.ydjk.org.cn/Article/details/gt2gflmgoap.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tthnfxnd.html

(x * 2 for x in arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tvsuwgdi.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.ydjk.org.cn/Article/details/gt2rcdihmtr.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt2srnljlrq.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt2wuoauzrk.html

deque(maxlen=10)
来源：http://www.ydjk.org.cn/Article/details/gt2trrxctsq.html

[U14] Py：分组收集到列表
来源：http://www.ydjk.org.cn/Article/details/gt2bzbtgzzf.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt2parhxken.html

[U15] Py：高精度计时
来源：http://www.ydjk.org.cn/Article/details/gt2srzstzds.html

t = time.perf_counter()
来源：http://www.52xcode.cn/Article/details/gt2dwgymzxz.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt2jsqpteqg.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt2jkwwznqf.html

[U17] Py：初始化日志
来源：http://www.52xcode.cn/Article/details/gt2xgbislrt.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt2etvjkcrk.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt2pvtnunfb.html

pat = re.compile(r"\d+")
来源：http://www.52xcode.cn/Article/details/gt2knjmmryi.html

[U19] Py：正则替换带回调
来源：http://www.ydjk.org.cn/Article/details/gt2rcarpcne.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt2zgfmdlpg.html

[U20] Py：缓存函数结果
来源：http://www.52xcode.cn/Article/details/gt2izvmtjco.html

@functools.lru_cache(maxsize=None)
来源：http://www.52xcode.cn/Article/details/gt2wuzihrbn.html

[U21] Py：自定义上下文管理器
来源：http://www.ydjk.org.cn/Article/details/gt2xyiother.html

@contextlib.contextmanager
来源：http://www.ydjk.org.cn/Article/details/gt2chxadkdg.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt2icjxjxaz.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt2nalqodse.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt2wnxesdez.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt2yvrgpnhb.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt2sklssgdq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zvtecbeq.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt2ujwsqoot.html

csv.DictReader(f)
来源：http://www.ydjk.org.cn/Article/details/gt2zspriyxz.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt2agwoqxov.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.52xcode.cn/Article/details/gt2lzzchuzf.html

[U27] Py：异步 HTTP
来源：http://www.52xcode.cn/Article/details/gt2rpxtlwdk.html

aiohttp.ClientSession() 配合 async with
来源：http://www.ydjk.org.cn/Article/details/gt2zrkzmcqw.html

[U28] Py：类型别名
来源：http://www.52xcode.cn/Article/details/gt2hxfosyna.html

UserId = int
来源：http://www.52xcode.cn/Article/details/gt2hbpclsjm.html

[U29] Py：属性校验
来源：http://www.52xcode.cn/Article/details/gt2lrbmulpe.html

@property 与 @x.setter 配合
来源：http://www.52xcode.cn/Article/details/gt2nvoyfquc.html

[U30] Py：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2hngfouft.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt2ghfkklsj.html

[U31] Py：单测
来源：http://www.52xcode.cn/Article/details/gt2spcrlcdk.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt2zgikxusg.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hecyorjv.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt2vclndyrm.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt2vyifkmio.html

python -m build  （依赖 pyproject.toml）
来源：http://www.52xcode.cn/Article/details/gt2nwirkvyx.html

[U34] Py：判断编码
来源：http://www.ydjk.org.cn/Article/details/gt2unmdqslc.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt2akwvhavw.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt2pyvjyzmn.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt2woheiorc.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ripzyrjn.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt2esxyovvf.html

[U37] Py：读写 Excel
来源：http://www.52xcode.cn/Article/details/gt2wxgqaozg.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.52xcode.cn/Article/details/gt2qhowwfpu.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt2osqidzub.html

Path(__file__).resolve().parent
来源：http://www.52xcode.cn/Article/details/gt2cttvxkrz.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt2jrokphyr.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt2uiwssrxr.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt2vfcrjqnq.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2yfoayyub.html

[U41] PHP：初始化 Composer 项目
来源：http://www.ydjk.org.cn/Article/details/gt2mojorcpm.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.52xcode.cn/Article/details/gt2qwsnucvb.html

[U42] PHP：PSR-4 自动加载
来源：http://www.52xcode.cn/Article/details/gt2vpsdszoz.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt2qnlfmwjd.html

[U43] PHP：声明命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2equkfehm.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt2tmritohh.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt2nlddczqr.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt2wfkprhoc.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt2gdyjssql.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjknqcac.html

[U46] PHP：可空类型
来源：http://www.ydjk.org.cn/Article/details/gt2oxcibgrq.html

?string $name = null
来源：http://www.ydjk.org.cn/Article/details/gt2ytglxpkn.html

[U47] PHP：联合类型
来源：http://www.52xcode.cn/Article/details/gt2dhociovh.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt2puhfyjsc.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt2osnrnuxc.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vopvrwuc.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt2qyenvitw.html

public readonly string $name
来源：http://www.ydjk.org.cn/Article/details/gt2owwelpwt.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt2ulpezhtf.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwfdsbru.html

[U51] PHP：数组解构
来源：http://www.ydjk.org.cn/Article/details/gt2bezmombw.html

[$a, $b] = $arr;
来源：http://www.ydjk.org.cn/Article/details/gt2tpkpmcgl.html

[U52] PHP：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2cliiysif.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt2zsbctpaa.html

[U53] PHP：空合并运算符
来源：http://www.52xcode.cn/Article/details/gt2cqsvkhqq.html

$v = $a ?? $b ?? "default";
来源：http://www.52xcode.cn/Article/details/gt2itucimeo.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt2noxrkztn.html

$obj?->method()
来源：http://www.52xcode.cn/Article/details/gt2zvcdtszt.html

[U55] PHP：match 表达式
来源：http://www.52xcode.cn/Article/details/gt2fonrfwbg.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2pbcsnnml.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt2vembnrbz.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2disohdfz.html

[U57] PHP：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ybxwhcmj.html

"值: {$a}"
来源：http://www.ydjk.org.cn/Article/details/gt2donbbsxb.html

[U58] PHP：数组三件套
来源：http://www.ydjk.org.cn/Article/details/gt2qoknjlpw.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.52xcode.cn/Article/details/gt2gnxfroba.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt2wipkslsj.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2noqzlhoc.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt2deswjkdx.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jbzzxbvk.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt2nosgnrwp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pafigaoz.html

[U62] PHP：日期对象
来源：http://www.52xcode.cn/Article/details/gt2ahpnucnc.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt2cboqktsk.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt2ajyfmibu.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt2wehebebl.html

[U64] PHP：目录遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gexevygb.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt2wekcxegh.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt2dttndytt.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hikkmupu.html

[U66] PHP：设置 Cookie
来源：http://www.ydjk.org.cn/Article/details/gt2wwxrcynx.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.52xcode.cn/Article/details/gt2ydfqmoji.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt2uyyueemv.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.52xcode.cn/Article/details/gt2rfjixebj.html

[U68] PHP：PDO 连接
来源：http://www.52xcode.cn/Article/details/gt2dexxysrd.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt2vprqtfkq.html

[U69] PHP：PDO 预处理
来源：http://www.ydjk.org.cn/Article/details/gt2ojvxsyhp.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.52xcode.cn/Article/details/gt2byoeonjq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt2oxvgxjks.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.52xcode.cn/Article/details/gt2mhnuekun.html

[U71] PHP：抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jcjbydne.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt2smpnhnsz.html

[U72] PHP：写错误日志
来源：http://www.52xcode.cn/Article/details/gt2vpsmzrcp.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt2dwmqjfdh.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt2tuecnhea.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt2ptwunmeu.html

[U74] PHP：读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hgpcrisv.html

getenv("APP_ENV") ?: "production"
来源：http://www.52xcode.cn/Article/details/gt2dolylwzy.html

[U75] PHP：依赖注入
来源：http://www.52xcode.cn/Article/details/gt2rbwmvcur.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt2ietyzodl.html

[U76] PHP：简单路由
来源：http://www.ydjk.org.cn/Article/details/gt2jdhdilej.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.ydjk.org.cn/Article/details/gt2mbpgrzea.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt2xosrpkzu.html

composer require twig/twig
来源：http://www.52xcode.cn/Article/details/gt2waizcooi.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt2wdfuunba.html

composer require --dev phpunit/phpunit
来源：http://www.ydjk.org.cn/Article/details/gt2skuscowl.html

[U79] PHP：静态分析
来源：http://www.ydjk.org.cn/Article/details/gt2khfrblhg.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt2mbcnvtsd.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt2iyimisbf.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.ydjk.org.cn/Article/details/gt2ygdujhkg.html

[U81] JS：初始化项目
来源：http://www.52xcode.cn/Article/details/gt2hvmvievp.html

npm init -y;  npm i express
来源：http://www.52xcode.cn/Article/details/gt2okthvwvt.html

[U82] JS：package.json 脚本
来源：http://www.ydjk.org.cn/Article/details/gt2nyruncdy.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt2orrugcws.html

[U83] JS：ES Module 导入导出
来源：http://www.ydjk.org.cn/Article/details/gt2qbjrtxnx.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nltvgxtu.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt2ufoabuml.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt2reoeqwmd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt2yluhcufo.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt2czzfadnc.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt2utrffapk.html

a ?? b
来源：http://www.ydjk.org.cn/Article/details/gt2cdnckxqq.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt2oaidzdgn.html

const { a = 1, b = 2 } = obj;
来源：http://www.ydjk.org.cn/Article/details/gt2ekecgvlw.html

[U88] JS：对象展开合并
来源：http://www.52xcode.cn/Article/details/gt2qazmfvoz.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt2wvzrmipy.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt2ysebelun.html

[...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2mzllzqvo.html

[U90] JS：数字数组排序
来源：http://www.52xcode.cn/Article/details/gt2vucpzmzm.html

[...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2uyfrdddx.html

[U91] JS：对象键值遍历
来源：http://www.ydjk.org.cn/Article/details/gt2khvnkwdm.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt2tviituxc.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2dbgbihig.html

structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xxvkdkhz.html

[U93] JS：模板字符串
来源：http://www.52xcode.cn/Article/details/gt2tjgcleby.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt2qhoubceg.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt2qakatoad.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt2bdyrglut.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt2lhnmaskk.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt2giznzrct.html

[U96] JS：async/await 与异常
来源：http://www.ydjk.org.cn/Article/details/gt2ydivjcap.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzvihnsg.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt2phahgypy.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2plbfdohl.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt2ovikylzt.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt2gpjueoin.html

[U99] JS：事件监听
来源：http://www.52xcode.cn/Article/details/gt2oeuxxrri.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt2iigfxfiu.html

[U100] JS：DOM 查询
来源：http://www.52xcode.cn/Article/details/gt2zaswcqxt.html

document.querySelector(".item")
来源：http://www.ydjk.org.cn/Article/details/gt2diaokxzp.html

[U101] JS：classList 操作
来源：http://www.52xcode.cn/Article/details/gt2ujsdknyy.html

el.classList.toggle("active")
来源：http://www.52xcode.cn/Article/details/gt2tjnaasev.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt2dkutyiah.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt2pmlxcfef.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt2ekcqxuhd.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt2opuleruk.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt2mjgnnubt.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yxoqvnfc.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt2ysipwvyh.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ypbkfase.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dkokylez.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt2fbjdcuuv.html

[U107] JS：数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tiupesjq.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ehfkxces.html

[U108] JS：随机整数
来源：http://www.ydjk.org.cn/Article/details/gt2knoeisin.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt2rulxrwcz.html

[U109] JS：数组分组
来源：http://www.52xcode.cn/Article/details/gt2jkewuszw.html

Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cqblvsvk.html

[U110] JS：数组分块
来源：http://www.52xcode.cn/Article/details/gt2hkyadzql.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.ydjk.org.cn/Article/details/gt2itihvnmx.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt2xgdonack.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2himxbnix.html

[U112] JS：字符串补位
来源：http://www.ydjk.org.cn/Article/details/gt2swmbzgkn.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vtysokvj.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt2grghlpwp.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2prunuphe.html

[U114] JS：JSON 深比较
来源：http://www.ydjk.org.cn/Article/details/gt2svsqiatt.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2josxioxg.html

[U115] JS：生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2arkrzcdc.html

crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2wbwjjnoq.html

[U116] JS：类型检查（JSDoc）
来源：http://www.ydjk.org.cn/Article/details/gt2hwbyhkqm.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2evewcdgc.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt2pyqbbhov.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt2imbeacqf.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt2bjuyyoof.html

npm i -D vite;  npx vite
来源：http://www.52xcode.cn/Article/details/gt2xloucjtw.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt2ylwvzaqj.html

npx vite build
来源：http://www.52xcode.cn/Article/details/gt2slhxkeyu.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt2yigimjgf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt2ljtgdckp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crmnjicv.html

统计汇总
来源：http://www.ydjk.org.cn/Article/details/gt2agdxdpea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwialkdb.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt2qhadavqz.html

Python ......... 252
来源：http://www.52xcode.cn/Article/details/gt2jwiepbdk.html

PHP ............ 252
来源：http://www.ydjk.org.cn/Article/details/gt2wxebigby.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt2mpwgqdxr.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt2xypczriq.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt2fpfjpakr.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt2hfnachjg.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt2qagjelnh.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt2kpnmsukr.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt2qgswxpxc.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt2demahysa.html

SQL ............ 90
来源：http://www.ydjk.org.cn/Article/details/gt2eefvbjnx.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt2ylpilsdi.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt2qdqnobiq.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt2mzyumfut.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt2gcxmofcl.html

Perl ........... 10
来源：http://www.ydjk.org.cn/Article/details/gt2tuuzzqiz.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt2wujdmjxc.html

------------------------------------
来源：http://www.52xcode.cn/Article/details/gt2nafkbwzf.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt2wdlyayfa.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt2qmltzlyt.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt2rnqmqhny.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt2fehvahtg.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2jemrarko.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt2dyoljzxv.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.ydjk.org.cn/Article/details/gt2skrsgevf.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.52xcode.cn/Article/details/gt2lkligvvu.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt2kyturnnf.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2uzhzdgwf.html

I 正则表达式            8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2tlzgxxdm.html

J 日期与时间           10 个任务 × 8 语言 =   80
来源：http://www.ydjk.org.cn/Article/details/gt2mxxhrtku.html

K JSON 与序列化         8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2qsddfbgo.html

L 网络请求              8 个任务 × 8 语言 =   64
来源：http://www.52xcode.cn/Article/details/gt2fvrllggs.html


<!-- 参考信息 -->