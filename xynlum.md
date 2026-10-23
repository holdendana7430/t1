代发 wailian999

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3acnaalsl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3smtlifzr.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3hvtejijh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3lnvufqhj.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgwzzqxj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3okrgcdnr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3eckglkzh.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3sxnnucry.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3nhutqaeg.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3djupmuof.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3zlxlskub.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3ntbrcpar.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3givqtzpu.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ikjknurl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3egrehjbu.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3mxjgspuh.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3npvzossa.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3ryujggpo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xrcclgcd.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3geoxlshr.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nrquyogx.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3hezxcaac.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3nlolivrq.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3nusrxbhu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt3hssrxhzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mejxekre.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3btvjxxwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obspehls.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt3yytdxpmf.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt3ncgwknbi.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3vmqkorpq.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fmyycujc.html

[U03] Py：加载 .env 配置
来源：http://www.52xcode.cn/Article/details/gt3ekbwimzx.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.52xcode.cn/Article/details/gt3owuayxop.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt3hzwjztdt.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.52xcode.cn/Article/details/gt3czrfdchk.html

[U05] Py：列表去重且保序
来源：http://www.52xcode.cn/Article/details/gt3qrhyyagz.html

list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3owpzxuez.html

[U06] Py：合并两个字典
来源：http://www.52xcode.cn/Article/details/gt3yyggbycp.html

{**a, **b}
来源：http://www.ydjk.org.cn/Article/details/gt3kiflytey.html

[U07] Py：反转字典键值
来源：http://www.52xcode.cn/Article/details/gt3nvmbvtvu.html

{v: k for k, v in d.items()}
来源：http://www.ydjk.org.cn/Article/details/gt3hxrugkra.html

[U08] Py：展平二维列表
来源：http://www.52xcode.cn/Article/details/gt3alpynthm.html

[y for x in nested for y in x]
来源：http://www.ydjk.org.cn/Article/details/gt3foeyihcl.html

[U09] Py：字典取最大值的键
来源：http://www.ydjk.org.cn/Article/details/gt3rdokkadj.html

max(d, key=d.get)
来源：http://www.52xcode.cn/Article/details/gt3sjsikhrk.html

[U10] Py：按值排序字典
来源：http://www.ydjk.org.cn/Article/details/gt3vovglxur.html

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://www.52xcode.cn/Article/details/gt3ampupylm.html

[U11] Py：生成器表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tnghckcr.html

(x * 2 for x in arr)
来源：http://www.52xcode.cn/Article/details/gt3svonjgvu.html

[U12] Py：取出现最多的 3 个元素
来源：http://www.52xcode.cn/Article/details/gt3mkohahrs.html

Counter(arr).most_common(3)
来源：http://www.ydjk.org.cn/Article/details/gt3llyaghpe.html

[U13] Py：固定长度队列
来源：http://www.52xcode.cn/Article/details/gt3dcaeorgh.html

deque(maxlen=10)
来源：http://www.52xcode.cn/Article/details/gt3gfwusjsb.html

[U14] Py：分组收集到列表
来源：http://www.52xcode.cn/Article/details/gt3goemotip.html

defaultdict(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mzngamvx.html

[U15] Py：高精度计时
来源：http://www.52xcode.cn/Article/details/gt3mjnrxnad.html

t = time.perf_counter()
来源：http://www.ydjk.org.cn/Article/details/gt3scgidvxu.html

[U16] Py：命令行参数解析
来源：http://www.ydjk.org.cn/Article/details/gt3gdepurko.html

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://www.52xcode.cn/Article/details/gt3jraoaita.html

[U17] Py：初始化日志
来源：http://www.ydjk.org.cn/Article/details/gt3gxtbolqe.html

logging.basicConfig(level=logging.INFO)
来源：http://www.52xcode.cn/Article/details/gt3xrmxoonc.html

[U18] Py：预编译正则
来源：http://www.52xcode.cn/Article/details/gt3tjozmvvw.html

pat = re.compile(r"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hwroifdf.html

[U19] Py：正则替换带回调
来源：http://www.52xcode.cn/Article/details/gt3ycdkmhrp.html

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://www.52xcode.cn/Article/details/gt3naudlggz.html

[U20] Py：缓存函数结果
来源：http://www.ydjk.org.cn/Article/details/gt3kbnawvgy.html

@functools.lru_cache(maxsize=None)
来源：http://www.ydjk.org.cn/Article/details/gt3ccqgsrar.html

[U21] Py：自定义上下文管理器
来源：http://www.52xcode.cn/Article/details/gt3zvbvzeqw.html

@contextlib.contextmanager
来源：http://www.52xcode.cn/Article/details/gt3slzopzyb.html

[U22] Py：矩阵转置
来源：http://www.ydjk.org.cn/Article/details/gt3sxcuiaxn.html

list(zip(*m))
来源：http://www.ydjk.org.cn/Article/details/gt3hjmlvogw.html

[U23] Py：分块读取大文件
来源：http://www.ydjk.org.cn/Article/details/gt3sffrrdqf.html

for chunk in iter(lambda: f.read(8192), b""):
来源：http://www.ydjk.org.cn/Article/details/gt3zbtqempw.html

[U24] Py：路径操作
来源：http://www.ydjk.org.cn/Article/details/gt3nsyqxunq.html

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tugqcggb.html

[U25] Py：CSV 按字典读
来源：http://www.ydjk.org.cn/Article/details/gt3qkebpaqg.html

csv.DictReader(f)
来源：http://www.52xcode.cn/Article/details/gt3yrpzdnxe.html

[U26] Py：并发下载
来源：http://www.ydjk.org.cn/Article/details/gt3zrwdzcgn.html

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://www.ydjk.org.cn/Article/details/gt3stylptnh.html

[U27] Py：异步 HTTP
来源：http://www.ydjk.org.cn/Article/details/gt3bcjkronh.html

aiohttp.ClientSession() 配合 async with
来源：http://www.52xcode.cn/Article/details/gt3wonanlnb.html

[U28] Py：类型别名
来源：http://www.ydjk.org.cn/Article/details/gt3mhldkreb.html

UserId = int
来源：http://www.ydjk.org.cn/Article/details/gt3usfvspca.html

[U29] Py：属性校验
来源：http://www.ydjk.org.cn/Article/details/gt3mdjjlsek.html

@property 与 @x.setter 配合
来源：http://www.ydjk.org.cn/Article/details/gt3slkvawxq.html

[U30] Py：数据类
来源：http://www.52xcode.cn/Article/details/gt3wtdgiget.html

@dataclass(slots=True)
来源：http://www.52xcode.cn/Article/details/gt3klgynouu.html

[U31] Py：单测
来源：http://www.ydjk.org.cn/Article/details/gt3lntrcuqf.html

python -m pytest -q
来源：http://www.52xcode.cn/Article/details/gt3rtnhbczi.html

[U32] Py：代码格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wyfrcleq.html

ruff format . && ruff check --fix .
来源：http://www.ydjk.org.cn/Article/details/gt3boejmcwh.html

[U33] Py：打包发布
来源：http://www.52xcode.cn/Article/details/gt3lenmzhiq.html

python -m build  （依赖 pyproject.toml）
来源：http://www.ydjk.org.cn/Article/details/gt3tcsvgnad.html

[U34] Py：判断编码
来源：http://www.52xcode.cn/Article/details/gt3lquegahr.html

chardet.detect(raw)
来源：http://www.52xcode.cn/Article/details/gt3oknwfbga.html

[U35] Py：发送邮件
来源：http://www.ydjk.org.cn/Article/details/gt3lffwcwmq.html

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://www.52xcode.cn/Article/details/gt3frsvuaiw.html

[U36] Py：定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3iaxodxql.html

schedule.every(10).minutes.do(job)
来源：http://www.ydjk.org.cn/Article/details/gt3oobmgkpl.html

[U37] Py：读写 Excel
来源：http://www.ydjk.org.cn/Article/details/gt3oqjhqqgl.html

pandas.read_excel / DataFrame.to_excel
来源：http://www.ydjk.org.cn/Article/details/gt3hytrvgfm.html

[U38] Py：获取脚本所在目录
来源：http://www.52xcode.cn/Article/details/gt3hvvzerds.html

Path(__file__).resolve().parent
来源：http://www.ydjk.org.cn/Article/details/gt3nrxeonrl.html

[U39] Py：判断是否在交互环境
来源：http://www.52xcode.cn/Article/details/gt3pignferc.html

sys.stdout.isatty()
来源：http://www.ydjk.org.cn/Article/details/gt3droubvuq.html

[U40] Py：打印到标准错误
来源：http://www.52xcode.cn/Article/details/gt3vdvqhnby.html

print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xkpnujnr.html

[U41] PHP：初始化 Composer 项目
来源：http://www.52xcode.cn/Article/details/gt3khzrznjw.html

composer init;  composer require guzzlehttp/guzzle
来源：http://www.ydjk.org.cn/Article/details/gt3pmldiojk.html

[U42] PHP：PSR-4 自动加载
来源：http://www.ydjk.org.cn/Article/details/gt3iywnzqax.html

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://www.ydjk.org.cn/Article/details/gt3oroukvsx.html

[U43] PHP：声明命名空间
来源：http://www.52xcode.cn/Article/details/gt3lauoozct.html

namespace App\Http;
来源：http://www.52xcode.cn/Article/details/gt3zipfgqnd.html

[U44] PHP：开启严格类型
来源：http://www.ydjk.org.cn/Article/details/gt3roysswbi.html

declare(strict_types=1);
来源：http://www.52xcode.cn/Article/details/gt3wojogsvd.html

[U45] PHP：类型声明与返回类型
来源：http://www.52xcode.cn/Article/details/gt3riydgqvx.html

function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3splwogjd.html

[U46] PHP：可空类型
来源：http://www.52xcode.cn/Article/details/gt3zjnsiaoz.html

?string $name = null
来源：http://www.52xcode.cn/Article/details/gt3gdrmfqmx.html

[U47] PHP：联合类型
来源：http://www.ydjk.org.cn/Article/details/gt3aruzpykk.html

int|string $id
来源：http://www.ydjk.org.cn/Article/details/gt3tpapttrh.html

[U48] PHP：纯枚举
来源：http://www.ydjk.org.cn/Article/details/gt3emomstfb.html

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://www.52xcode.cn/Article/details/gt3aqeewgqq.html

[U49] PHP：只读属性
来源：http://www.52xcode.cn/Article/details/gt3vqmywlff.html

public readonly string $name
来源：http://www.52xcode.cn/Article/details/gt3esyhzszy.html

[U50] PHP：构造器属性提升
来源：http://www.52xcode.cn/Article/details/gt3irfbbkqm.html

public function __construct(private int $id) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgxhulci.html

[U51] PHP：数组解构
来源：http://www.52xcode.cn/Article/details/gt3ghgcfdpa.html

[$a, $b] = $arr;
来源：http://www.52xcode.cn/Article/details/gt3milmdqjo.html

[U52] PHP：箭头函数
来源：http://www.52xcode.cn/Article/details/gt3wvqjpccl.html

$double = fn($x) => $x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yczfobym.html

[U53] PHP：空合并运算符
来源：http://www.ydjk.org.cn/Article/details/gt3knvxdxqz.html

$v = $a ?? $b ?? "default";
来源：http://www.ydjk.org.cn/Article/details/gt3iswvedih.html

[U54] PHP：空安全调用
来源：http://www.ydjk.org.cn/Article/details/gt3sumnvuhz.html

$obj?->method()
来源：http://www.ydjk.org.cn/Article/details/gt3tpukybpz.html

[U55] PHP：match 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tmruhzxo.html

$s = match($x) { 1 => "一", default => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3pldaowwa.html

[U56] PHP：命名参数
来源：http://www.52xcode.cn/Article/details/gt3nziwrkfn.html

f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tqswxwfr.html

[U57] PHP：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mofvqrhn.html

"值: {$a}"
来源：http://www.52xcode.cn/Article/details/gt3xmnwrpom.html

[U58] PHP：数组三件套
来源：http://www.52xcode.cn/Article/details/gt3wugfmdmi.html

array_map($f, $a);  array_filter($a, $f);  array_reduce($a, $f, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zsttwybu.html

[U59] PHP：自定义排序
来源：http://www.52xcode.cn/Article/details/gt3avhgkbvy.html

usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3uspwrekp.html

[U60] PHP：JSON 编解码
来源：http://www.ydjk.org.cn/Article/details/gt3yhosxnil.html

json_encode($d, JSON_UNESCAPED_UNICODE);  json_decode($s, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cmovwucx.html

[U61] PHP：正则
来源：http://www.ydjk.org.cn/Article/details/gt3oqexwiyp.html

preg_match('/(\d+)/', $s, $m);  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3asthxozz.html

[U62] PHP：日期对象
来源：http://www.ydjk.org.cn/Article/details/gt3wrwozprs.html

(new DateTimeImmutable())->format("Y-m-d");
来源：http://www.52xcode.cn/Article/details/gt3mrddjgdn.html

[U63] PHP：文件读写
来源：http://www.ydjk.org.cn/Article/details/gt3wklszous.html

file_get_contents($f);  file_put_contents($f, $data);
来源：http://www.ydjk.org.cn/Article/details/gt3yjdpfvtk.html

[U64] PHP：目录遍历
来源：http://www.52xcode.cn/Article/details/gt3smsrhuad.html

glob("dir/*.php");  scandir("dir");
来源：http://www.ydjk.org.cn/Article/details/gt3ocjshizo.html

[U65] PHP：会话
来源：http://www.ydjk.org.cn/Article/details/gt3dvzkvman.html

session_start();  $_SESSION["uid"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3nefiqgdk.html

[U66] PHP：设置 Cookie
来源：http://www.52xcode.cn/Article/details/gt3sybsdyie.html

setcookie("token", $v, ["httponly" => true, "samesite" => "Lax"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tlnpofrb.html

[U67] PHP：处理文件上传
来源：http://www.52xcode.cn/Article/details/gt3uqqowpma.html

$_FILES["file"]["tmp_name"] 与 move_uploaded_file()
来源：http://www.ydjk.org.cn/Article/details/gt3wxpuacaq.html

[U68] PHP：PDO 连接
来源：http://www.ydjk.org.cn/Article/details/gt3xsgmmvzh.html

$pdo = new PDO("mysql:host=localhost;dbname=app", "root", "");
来源：http://www.ydjk.org.cn/Article/details/gt3qdjcwiwa.html

[U69] PHP：PDO 预处理
来源：http://www.52xcode.cn/Article/details/gt3zpssxbfb.html

$stmt = $pdo->prepare("SELECT * FROM users WHERE id = ?");  $stmt->execute([$id]);
来源：http://www.ydjk.org.cn/Article/details/gt3lnelszjq.html

[U70] PHP：PDO 事务
来源：http://www.ydjk.org.cn/Article/details/gt3ftcfofiv.html

$pdo->beginTransaction();  $pdo->commit();  $pdo->rollBack();
来源：http://www.ydjk.org.cn/Article/details/gt3eplsywal.html

[U71] PHP：抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3geoqzyrq.html

throw new RuntimeException("失败", 500);
来源：http://www.52xcode.cn/Article/details/gt3hvjdscnz.html

[U72] PHP：写错误日志
来源：http://www.ydjk.org.cn/Article/details/gt3kdezoalb.html

error_log("失败: " . $e->getMessage());
来源：http://www.52xcode.cn/Article/details/gt3ridpopnv.html

[U73] PHP：读取 ini 配置
来源：http://www.52xcode.cn/Article/details/gt3oxnsdbps.html

parse_ini_file("config.ini", true)
来源：http://www.52xcode.cn/Article/details/gt3omiicmxu.html

[U74] PHP：读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wqbdanwe.html

getenv("APP_ENV") ?: "production"
来源：http://www.ydjk.org.cn/Article/details/gt3ypcymgrr.html

[U75] PHP：依赖注入
来源：http://www.ydjk.org.cn/Article/details/gt3snobthuw.html

composer require psr/container
来源：http://www.52xcode.cn/Article/details/gt3zouepwdg.html

[U76] PHP：简单路由
来源：http://www.52xcode.cn/Article/details/gt3xkoejmlb.html

$path = parse_url($_SERVER["REQUEST_URI"], PHP_URL_PATH);
来源：http://www.52xcode.cn/Article/details/gt3qwfbtbxl.html

[U77] PHP：模板渲染
来源：http://www.ydjk.org.cn/Article/details/gt3pfejfaid.html

composer require twig/twig
来源：http://www.ydjk.org.cn/Article/details/gt3qtdrvkgh.html

[U78] PHP：单元测试
来源：http://www.52xcode.cn/Article/details/gt3ppnrwsmq.html

composer require --dev phpunit/phpunit
来源：http://www.52xcode.cn/Article/details/gt3zbqajadl.html

[U79] PHP：静态分析
来源：http://www.52xcode.cn/Article/details/gt3dkhuxipi.html

composer require --dev phpstan/phpstan
来源：http://www.ydjk.org.cn/Article/details/gt3kqdptbay.html

[U80] PHP：代码规范修复
来源：http://www.52xcode.cn/Article/details/gt3ypttlqoj.html

composer require --dev friendsofphp/php-cs-fixer
来源：http://www.52xcode.cn/Article/details/gt3adlajnue.html

[U81] JS：初始化项目
来源：http://www.ydjk.org.cn/Article/details/gt3fdrjxqkc.html

npm init -y;  npm i express
来源：http://www.ydjk.org.cn/Article/details/gt3gtsbhnxy.html

[U82] JS：package.json 脚本
来源：http://www.52xcode.cn/Article/details/gt3zajtnrwc.html

"scripts": { "dev": "vite", "build": "vite build" }
来源：http://www.52xcode.cn/Article/details/gt3voodgnke.html

[U83] JS：ES Module 导入导出
来源：http://www.52xcode.cn/Article/details/gt3uhytiurs.html

export const a = 1;  import { a } from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rymvslso.html

[U84] JS：CommonJS 写法
来源：http://www.ydjk.org.cn/Article/details/gt3eiwvvnec.html

module.exports = { a };  const { a } = require("./m");
来源：http://www.ydjk.org.cn/Article/details/gt3hikvkmpd.html

[U85] JS：可选链
来源：http://www.ydjk.org.cn/Article/details/gt3aynxuwog.html

a?.b?.c
来源：http://www.ydjk.org.cn/Article/details/gt3tswnzujb.html

[U86] JS：空值合并
来源：http://www.ydjk.org.cn/Article/details/gt3ivercrkv.html

a ?? b
来源：http://www.52xcode.cn/Article/details/gt3kgntfzyu.html

[U87] JS：解构默认值
来源：http://www.52xcode.cn/Article/details/gt3jhtvoypm.html

const { a = 1, b = 2 } = obj;
来源：http://www.52xcode.cn/Article/details/gt3eqizknuz.html

[U88] JS：对象展开合并
来源：http://www.ydjk.org.cn/Article/details/gt3zsjccsve.html

{ ...a, ...b }
来源：http://www.52xcode.cn/Article/details/gt3kntpkhnd.html

[U89] JS：数组去重
来源：http://www.52xcode.cn/Article/details/gt3flqdzjpi.html

[...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qphnznbf.html

[U90] JS：数字数组排序
来源：http://www.ydjk.org.cn/Article/details/gt3gspczkzg.html

[...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fgxmwygl.html

[U91] JS：对象键值遍历
来源：http://www.52xcode.cn/Article/details/gt3kzjiqpvi.html

Object.entries(obj).forEach(([k, v]) => {});
来源：http://www.52xcode.cn/Article/details/gt3ydmgdjlq.html

[U92] JS：深拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yhnphvxy.html

structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3osimwsgf.html

[U93] JS：模板字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hvemalff.html

`共 ${n} 条`
来源：http://www.ydjk.org.cn/Article/details/gt3bdkxfejo.html

[U94] JS：箭头函数
来源：http://www.ydjk.org.cn/Article/details/gt3ixdwhdkd.html

const double = x => x * 2;
来源：http://www.52xcode.cn/Article/details/gt3yugpvztq.html

[U95] JS：Promise 包装
来源：http://www.52xcode.cn/Article/details/gt3obvpvviz.html

new Promise((resolve, reject) => {})
来源：http://www.ydjk.org.cn/Article/details/gt3qdfafqcq.html

[U96] JS：async/await 与异常
来源：http://www.52xcode.cn/Article/details/gt3sltbmjlm.html

try { const d = await f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngwrquss.html

[U97] JS：并发请求
来源：http://www.ydjk.org.cn/Article/details/gt3cdicefru.html

await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3asrqmfas.html

[U98] JS：fetch 带 JSON
来源：http://www.52xcode.cn/Article/details/gt3pyklwgfa.html

await fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify(d) })
来源：http://www.ydjk.org.cn/Article/details/gt3ntpnzkws.html

[U99] JS：事件监听
来源：http://www.ydjk.org.cn/Article/details/gt3xdcmbbxu.html

el.addEventListener("click", e => {})
来源：http://www.52xcode.cn/Article/details/gt3npgnwitj.html

[U100] JS：DOM 查询
来源：http://www.ydjk.org.cn/Article/details/gt3zlasdcto.html

document.querySelector(".item")
来源：http://www.52xcode.cn/Article/details/gt3sgvajqne.html

[U101] JS：classList 操作
来源：http://www.ydjk.org.cn/Article/details/gt3pjgzlfux.html

el.classList.toggle("active")
来源：http://www.ydjk.org.cn/Article/details/gt3vejwjqjy.html

[U102] JS：本地存储
来源：http://www.ydjk.org.cn/Article/details/gt3guknjvbr.html

localStorage.setItem("k", JSON.stringify(v))
来源：http://www.ydjk.org.cn/Article/details/gt3gvukmmgh.html

[U103] JS：定时器
来源：http://www.52xcode.cn/Article/details/gt3grhehrtn.html

setTimeout(fn, 1000);  setInterval(fn, 1000);
来源：http://www.52xcode.cn/Article/details/gt3ctyvcxmh.html

[U104] JS：防抖
来源：http://www.52xcode.cn/Article/details/gt3rrlkqibm.html

const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kwoekgun.html

[U105] JS：节流
来源：http://www.52xcode.cn/Article/details/gt3lgjbatei.html

const throttle = (fn, ms) => { let last = 0; return (...a) => { const n = Date.now(); if (n - last >= ms) { last = n; fn(...a); } }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ihijlipo.html

[U106] JS：日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mczoomxf.html

new Intl.DateTimeFormat("zh-CN", { dateStyle: "medium" }).format(new Date())
来源：http://www.ydjk.org.cn/Article/details/gt3litkvjfl.html

[U107] JS：数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ylxtzlln.html

new Intl.NumberFormat("en-US").format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qxmzsiza.html

[U108] JS：随机整数
来源：http://www.52xcode.cn/Article/details/gt3elsieojx.html

Math.floor(Math.random() * (max - min + 1)) + min
来源：http://www.ydjk.org.cn/Article/details/gt3ooxshgef.html

[U109] JS：数组分组
来源：http://www.ydjk.org.cn/Article/details/gt3dmspyjpx.html

Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wwaytzfs.html

[U110] JS：数组分块
来源：http://www.ydjk.org.cn/Article/details/gt3dvvqwhcc.html

arr.reduce((acc, x, i) => (i % size ? acc : [...acc, arr.slice(i, i + size)]), [])
来源：http://www.52xcode.cn/Article/details/gt3etzrixpq.html

[U111] JS：对象转 Map
来源：http://www.ydjk.org.cn/Article/details/gt3vwgmebsk.html

new Map(Object.entries(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ojoeehni.html

[U112] JS：字符串补位
来源：http://www.52xcode.cn/Article/details/gt3jsbfwadi.html

"7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qmjrlwbb.html

[U113] JS：正则替换全部
来源：http://www.52xcode.cn/Article/details/gt3yqutvogs.html

s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pvynwoio.html

[U114] JS：JSON 深比较
来源：http://www.52xcode.cn/Article/details/gt3gwmihjil.html

JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3tskhbdxq.html

[U115] JS：生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3nzdyyral.html

crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hedazoji.html

[U116] JS：类型检查（JSDoc）
来源：http://www.52xcode.cn/Article/details/gt3bnabbfql.html

/** @param {string} name */ function f(name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpekgqgk.html

[U117] JS：单元测试
来源：http://www.ydjk.org.cn/Article/details/gt3iqbzozdw.html

npm i -D vitest;  npx vitest
来源：http://www.ydjk.org.cn/Article/details/gt3wkeyqcac.html

[U118] JS：开发服务器
来源：http://www.52xcode.cn/Article/details/gt3wdikzrhm.html

npm i -D vite;  npx vite
来源：http://www.ydjk.org.cn/Article/details/gt3hxuqeqgx.html

[U119] JS：生产构建
来源：http://www.52xcode.cn/Article/details/gt3tjpmases.html

npx vite build
来源：http://www.ydjk.org.cn/Article/details/gt3fhwdnqov.html

[U120] JS：读取环境变量（Vite）
来源：http://www.52xcode.cn/Article/details/gt3dfighvtf.html

import.meta.env.VITE_API_URL
来源：http://www.ydjk.org.cn/Article/details/gt3zwhlvlrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvbxupbo.html

统计汇总
来源：http://www.52xcode.cn/Article/details/gt3pdgawwoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxmtqhwu.html

按语言统计（条）：
来源：http://www.ydjk.org.cn/Article/details/gt3ufqizyjz.html

Python ......... 252
来源：http://www.ydjk.org.cn/Article/details/gt3ompasvro.html

PHP ............ 252
来源：http://www.52xcode.cn/Article/details/gt3gttraura.html

JavaScript ..... 252
来源：http://www.52xcode.cn/Article/details/gt3fachxaki.html

TypeScript ..... 212
来源：http://www.52xcode.cn/Article/details/gt3hrqzbqxi.html

Java ........... 212
来源：http://www.52xcode.cn/Article/details/gt3indmppvt.html

Go ............. 212
来源：http://www.ydjk.org.cn/Article/details/gt3iyegtkge.html

Ruby ........... 212
来源：http://www.ydjk.org.cn/Article/details/gt3ckeojxva.html

C# ............. 212
来源：http://www.52xcode.cn/Article/details/gt3wdkkuxqd.html

C .............. 30
来源：http://www.52xcode.cn/Article/details/gt3pgetmnko.html

C++ ............ 30
来源：http://www.52xcode.cn/Article/details/gt3tfgtrmtc.html

SQL ............ 90
来源：http://www.52xcode.cn/Article/details/gt3nmjvbayp.html

Bash ........... 80
来源：http://www.52xcode.cn/Article/details/gt3oiulxqtk.html

Kotlin ......... 15
来源：http://www.52xcode.cn/Article/details/gt3ivirlpoe.html

Swift .......... 15
来源：http://www.ydjk.org.cn/Article/details/gt3ufmqppyp.html

Lua ............ 10
来源：http://www.52xcode.cn/Article/details/gt3bkapktmb.html

Perl ........... 10
来源：http://www.52xcode.cn/Article/details/gt3ihmaxjwj.html

Scala .......... 10
来源：http://www.52xcode.cn/Article/details/gt3wsiajnmm.html

------------------------------------
来源：http://www.ydjk.org.cn/Article/details/gt3vsnqgdmn.html

合计 ........... 2106 条
来源：http://www.52xcode.cn/Article/details/gt3gvwwoerz.html

按章节统计：
来源：http://www.ydjk.org.cn/Article/details/gt3byabnnbr.html

A 基础语法与类型       26 个任务 × 8 语言 =  208
来源：http://www.ydjk.org.cn/Article/details/gt3zcbzvizb.html

B 流程控制             16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3sshdvuac.html

C 函数与作用域         16 个任务 × 8 语言 =  128
来源：http://www.52xcode.cn/Article/details/gt3tedtmgfb.html

D 数组 / 列表 / 集合   26 个任务 × 8 语言 =  208
来源：http://www.52xcode.cn/Article/details/gt3gtprbpje.html

E 字符串处理           22 个任务 × 8 语言 =  176
来源：http://www.52xcode.cn/Article/details/gt3agryadcr.html

F 文件与目录           12 个任务 × 8 语言 =   96
来源：http://www.ydjk.org.cn/Article/details/gt3lmoufvlj.html

G 面向对象             16 个任务 × 8 语言 =  128
来源：http://www.ydjk.org.cn/Article/details/gt3radbcini.html

H 异常与错误处理       10 个任务 × 8 语言 =   80
来源：http://www.52xcode.cn/Article/details/gt3jaevvvnl.html


<!-- 参考信息 -->